# Comparing `tmp/casambi_bt-0.1.0-py3-none-any.whl.zip` & `tmp/casambi_bt-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26963 bytes, number of entries: 17
+Zip file size: 27043 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      229 b- defN 23-Apr-07 15:31 CasambiBt/__init__.py
 -rw-r--r--  2.0 unx      828 b- defN 23-Feb-21 11:39 CasambiBt/_cache.py
 -rw-r--r--  2.0 unx    15729 b- defN 23-Apr-07 15:24 CasambiBt/_casambi.py
--rw-r--r--  2.0 unx    17483 b- defN 23-Apr-07 16:35 CasambiBt/_client.py
+-rw-r--r--  2.0 unx    17487 b- defN 23-Apr-07 18:55 CasambiBt/_client.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Feb-21 11:37 CasambiBt/_constants.py
 -rw-r--r--  2.0 unx     1144 b- defN 23-Feb-21 11:54 CasambiBt/_discover.py
 -rw-r--r--  2.0 unx     3831 b- defN 23-Apr-07 15:24 CasambiBt/_encryption.py
 -rw-r--r--  2.0 unx     2389 b- defN 23-Apr-07 15:30 CasambiBt/_keystore.py
 -rw-r--r--  2.0 unx    11573 b- defN 23-Apr-07 15:24 CasambiBt/_network.py
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-07 12:56 CasambiBt/_operation.py
+-rw-r--r--  2.0 unx      824 b- defN 23-Apr-07 17:08 CasambiBt/_operation.py
 -rw-r--r--  2.0 unx    13496 b- defN 23-Apr-07 15:31 CasambiBt/_unit.py
 -rw-r--r--  2.0 unx     1551 b- defN 23-Apr-07 15:46 CasambiBt/errors.py
--rw-r--r--  2.0 unx    11341 b- defN 23-Apr-07 16:43 casambi_bt-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2076 b- defN 23-Apr-07 16:43 casambi_bt-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 16:43 casambi_bt-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-07 16:43 casambi_bt-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1339 b- defN 23-Apr-07 16:43 casambi_bt-0.1.0.dist-info/RECORD
-17 files, 83988 bytes uncompressed, 24795 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    11341 b- defN 23-Apr-07 19:08 casambi_bt-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2076 b- defN 23-Apr-07 19:08 casambi_bt-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 19:08 casambi_bt-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-07 19:08 casambi_bt-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1339 b- defN 23-Apr-07 19:08 casambi_bt-0.1.1.dist-info/RECORD
+17 files, 84133 bytes uncompressed, 24875 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: CasambiBt/_unit.py
 Comment: 
 
 Filename: CasambiBt/errors.py
 Comment: 
 
-Filename: casambi_bt-0.1.0.dist-info/LICENSE
+Filename: casambi_bt-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: casambi_bt-0.1.0.dist-info/METADATA
+Filename: casambi_bt-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: casambi_bt-0.1.0.dist-info/WHEEL
+Filename: casambi_bt-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: casambi_bt-0.1.0.dist-info/top_level.txt
+Filename: casambi_bt-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: casambi_bt-0.1.0.dist-info/RECORD
+Filename: casambi_bt-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CasambiBt/_client.py

```diff
@@ -129,15 +129,15 @@
 
         self._logger.info(f"Connected to {self.address}")
         self._connectionState = ConnectionState.CONNECTED
 
     def _on_disconnect(self, client: BleakClient) -> None:
         if self._connectionState != ConnectionState.NONE:
             self._logger.info(f"Received disconnect callback from {self.address}")
-        if self._connectionState == ConnectionState.CONNECTED:
+        if self._connectionState == ConnectionState.AUTHENTICATED:
             self._disconnectedCallback()
         self._connectionState = ConnectionState.NONE
 
     async def exchangeKey(self, keystore: KeyStore) -> None:
         self._checkState(ConnectionState.CONNECTED)
 
         self._logger.info("Starting key exchange...")
```

## CasambiBt/_operation.py

```diff
@@ -20,11 +20,15 @@
 
     def prepareOperation(self, op: OpCode, target: int, payload: bytes) -> bytes:
         if len(payload) > 63:
             raise ValueError("Payload too long")
 
         flags = (self.lifetime & 15) << 11 | len(payload)
 
-        packet = struct.pack(">hbhhh", flags, op, self.origin, target, 0)
+        # Ensure that origin can't overflow.
+        # TODO: Check that signed is actually correct here.
+        packet = struct.pack(
+            ">hbhhh", flags, op, self.origin & (2**15 - 1), target, 0
+        )
         self.origin += 1
 
         return packet + payload
```

## Comparing `casambi_bt-0.1.0.dist-info/LICENSE` & `casambi_bt-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `casambi_bt-0.1.0.dist-info/METADATA` & `casambi_bt-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casambi-bt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A minimal, unofficial implementation of a bluetooth client for casambi devices
 Home-page: https://github.com/lkempf/casambi-bt
 Author: lkempf
 Author-email: pypi@lukas-kempf.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

## Comparing `casambi_bt-0.1.0.dist-info/RECORD` & `casambi_bt-0.1.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CasambiBt/__init__.py,sha256=CEMX1TML7iQINB4fqWPfKg42WMVIOeQwnX8Z5FFfuHw,229
 CasambiBt/_cache.py,sha256=s299WWpOh89kLPV24O7dAu3cBZ4uKJYAUZV10s4hVHc,828
 CasambiBt/_casambi.py,sha256=rjqY3A5rZGfgyfCFatyd_rPsHw8XyScZ9RzOw-S6ksE,15729
-CasambiBt/_client.py,sha256=y4pqM3Ug18JhRoHeKI6x6K2Emrpgox8I8pT00pFPrag,17483
+CasambiBt/_client.py,sha256=ngmsOEMMgNpry5dn28Mrp2Maq1cYpcTnDIsp1Y9RnPU,17487
 CasambiBt/_constants.py,sha256=r3Egb7xCM5Gq8csnVss4gOlXVvnj0uUS4nqKzbBy1FM,194
 CasambiBt/_discover.py,sha256=v11ucqWHsPOZXjMCrJIaldEsY3BmY3ekVmMnlcuQB4U,1144
 CasambiBt/_encryption.py,sha256=CLcoOOrggQqhJbnr_emBnEnkizpWDvb_0yFnitq4_FM,3831
 CasambiBt/_keystore.py,sha256=OMGf7zjc3U658cnmQ141lTZFROPLnJ3Bwbg51X30SsI,2389
 CasambiBt/_network.py,sha256=TSQWd7HiGHJqRHMo-Pfodz_s5OIcp3g6P7WFqCijCo0,11573
-CasambiBt/_operation.py,sha256=Cq98wKY2R4xohKf9tIo2ssbANplGmjLALMxW4_C8sI4,683
+CasambiBt/_operation.py,sha256=9Wr9c_kHiDc46G5un4KG0HWo5lGdWxiERO1XyxYKaIA,824
 CasambiBt/_unit.py,sha256=JB22f3pQh5GIEVksCrcmeFgYjuyjSsYwhG3leQ28R5Q,13496
 CasambiBt/errors.py,sha256=6Kz9JgpIs4FTOYqtHKQc-Cj3ybzRWYaDulqPw0DXL7Y,1551
-casambi_bt-0.1.0.dist-info/LICENSE,sha256=TAIIitFxpxEDi6Iju7foW4TDQmWvC-IhLVLhl67jKmQ,11341
-casambi_bt-0.1.0.dist-info/METADATA,sha256=FbaW9HoyDVyDujZBgkNBfSDhC6pf25YGas7K1ttihwA,2076
-casambi_bt-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-casambi_bt-0.1.0.dist-info/top_level.txt,sha256=uNbqLjtecFosoFzpGAC89-5icikWODKI8rOjbi8v_sA,10
-casambi_bt-0.1.0.dist-info/RECORD,,
+casambi_bt-0.1.1.dist-info/LICENSE,sha256=TAIIitFxpxEDi6Iju7foW4TDQmWvC-IhLVLhl67jKmQ,11341
+casambi_bt-0.1.1.dist-info/METADATA,sha256=VJGlap5HTsOVJXpOUQQawrNop2t1bxwUbkNdIHAnTxk,2076
+casambi_bt-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+casambi_bt-0.1.1.dist-info/top_level.txt,sha256=uNbqLjtecFosoFzpGAC89-5icikWODKI8rOjbi8v_sA,10
+casambi_bt-0.1.1.dist-info/RECORD,,
```

