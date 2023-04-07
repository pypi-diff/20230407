# Comparing `tmp/opvious-0.9.3.tar.gz` & `tmp/opvious-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opvious-0.9.3.tar", max compression
+gzip compressed data, was "opvious-0.9.4.tar", max compression
```

## Comparing `opvious-0.9.3.tar` & `opvious-0.9.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10756 2023-04-07 18:18:57.258050 opvious-0.9.3/LICENSE
--rw-r--r--   0        0        0     3181 2023-04-07 18:18:57.258050 opvious-0.9.3/README.md
--rw-r--r--   0        0        0     1982 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/__init__.py
--rw-r--r--   0        0        0    23218 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/client.py
--rw-r--r--   0        0        0     1062 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/common.py
--rw-r--r--   0        0        0    15835 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/data.py
--rw-r--r--   0        0        0     1966 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/executors/__init__.py
--rw-r--r--   0        0        0     1880 2023-04-07 18:19:47.474284 opvious-0.9.3/opvious/executors/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3521 2023-04-07 18:19:47.486284 opvious-0.9.3/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
--rw-r--r--   0        0        0     9497 2023-04-07 18:19:47.478284 opvious-0.9.3/opvious/executors/__pycache__/common.cpython-310.pyc
--rw-r--r--   0        0        0     2762 2023-04-07 18:19:47.566285 opvious-0.9.3/opvious/executors/__pycache__/urllib.cpython-310.pyc
--rw-r--r--   0        0        0     4068 2023-04-07 18:18:57.258050 opvious-0.9.3/opvious/executors/aiohttp.py
--rw-r--r--   0        0        0     8799 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/common.py
--rw-r--r--   0        0        0     2412 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/pyodide.py
--rw-r--r--   0        0        0     2685 2023-04-07 18:18:57.262050 opvious-0.9.3/opvious/executors/urllib.py
--rw-r--r--   0        0        0      788 2023-04-07 18:18:57.262050 opvious-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 opvious-0.9.3/setup.py
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 opvious-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    10756 2023-04-07 19:33:27.317574 opvious-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3181 2023-04-07 19:33:27.317574 opvious-0.9.4/README.md
+-rw-r--r--   0        0        0     2177 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/__init__.py
+-rw-r--r--   0        0        0    23786 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/client.py
+-rw-r--r--   0        0        0     1062 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/common.py
+-rw-r--r--   0        0        0    15835 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/data.py
+-rw-r--r--   0        0        0     2354 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/executors/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-07 19:34:25.591104 opvious-0.9.4/opvious/executors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3521 2023-04-07 19:34:25.599104 opvious-0.9.4/opvious/executors/__pycache__/aiohttp.cpython-310.pyc
+-rw-r--r--   0        0        0     9683 2023-04-07 19:34:25.595104 opvious-0.9.4/opvious/executors/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0        0        0     2762 2023-04-07 19:34:25.779109 opvious-0.9.4/opvious/executors/__pycache__/urllib.cpython-310.pyc
+-rw-r--r--   0        0        0     4068 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/executors/aiohttp.py
+-rw-r--r--   0        0        0     8942 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/executors/common.py
+-rw-r--r--   0        0        0     2412 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/executors/pyodide.py
+-rw-r--r--   0        0        0     2685 2023-04-07 19:33:27.317574 opvious-0.9.4/opvious/executors/urllib.py
+-rw-r--r--   0        0        0      788 2023-04-07 19:33:27.317574 opvious-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4125 1970-01-01 00:00:00.000000 opvious-0.9.4/setup.py
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 opvious-0.9.4/PKG-INFO
```

### Comparing `opvious-0.9.3/LICENSE` & `opvious-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/README.md` & `opvious-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/opvious/__init__.py` & `opvious-0.9.4/opvious/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,22 @@
   under the License.
 """
 
 import logging
 
 from .client import Client
 from .common import __version__
-from .executors import ApiError, Executor
+from .executors import (
+    ApiError,
+    Executor,
+    aiohttp_executor,
+    default_executor,
+    pyodide_executor,
+    urllib_executor,
+)
 from .data import (
     Attempt,
     AttemptRequest,
     CancelledOutcome,
     ConstraintRelaxation,
     DimensionArgument,
     FailedOutcome,
@@ -48,15 +55,14 @@
     TensorArgument,
     UnboundedOutcome,
     Value,
 )
 
 
 __all__ = [
-    "__version__",
     "ApiError",
     "Attempt",
     "AttemptRequest",
     "CancelledOutcome",
     "Client",
     "ConstraintRelaxation",
     "DimensionArgument",
@@ -77,11 +83,16 @@
     "SolveResponse",
     "SparseTensorArgument",
     "Summary",
     "Tensor",
     "TensorArgument",
     "UnboundedOutcome",
     "Value",
+    "__version__",
+    "aiohttp_executor",
+    "default_executor",
+    "pyodide_executor",
+    "urllib_executor",
 ]
 
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `opvious-0.9.3/opvious/client.py` & `opvious-0.9.4/opvious/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,34 +91,51 @@
             f"executor_class={self._executor.__class__.__name__}",
             f"api_url={json.dumps(self._api_url)}",
         ]
         return f"<opvious.Client {' '.join(fields)}>"
 
     @classmethod
     def from_token(cls, token: str, domain: Optional[str] = None) -> "Client":
-        """Creates a client from an API token."""
+        """
+        Creates a client from an API token. You can use an empty token to
+        create an unauthenticated client with limited functionality.
+        """
+        token = token.strip()
         api_url = f"https://api.{domain or _DEFAULT_DOMAIN}"
         return Client(
             executor=default_executor(
                 api_url=api_url,
                 authorization=token if " " in token else f"Bearer {token}",
             ),
             api_url=api_url,
             hub_url=f"https://hub.{domain}",
         )
 
     @classmethod
-    def from_environment(cls, env=os.environ) -> "Client":
-        """Creates a client from environment variables. OPVIOUS_TOKEN should
-        contain a valid API token. OPVIOUS_DOMAIN can optionally be set to use
-        a custom domain.
+    def from_environment(
+        cls, env=os.environ, require_authenticated=False
+    ) -> "Client":
         """
-        return Client.from_token(
-            token=env[_TOKEN_EVAR], domain=env.get(_DOMAIN_EVAR)
-        )
+        Creates a client from environment variables. If present, OPVIOUS_TOKEN
+        should contain a valid API token. OPVIOUS_DOMAIN can optionally be set
+        to use a custom domain.
+        """
+        token = env.get(_TOKEN_EVAR, "")
+        if not token and require_authenticated:
+            raise Exception(
+                f"Missing or empty {_TOKEN_EVAR} environment variable"
+            )
+        return Client.from_token(token=token, domain=env.get(_DOMAIN_EVAR))
+
+    @property
+    def authenticated(self):
+        """
+        Returns true if the client was created with a non-empty API token.
+        """
+        return self._executor.authenticated
 
     async def inspect(
         self,
         sources: Optional[list[str]] = None,
         formulation_name: Optional[str] = None,
         tag_name: Optional[str] = None,
         parameters: Optional[Mapping[Label, TensorArgument]] = None,
```

### Comparing `opvious-0.9.3/opvious/common.py` & `opvious-0.9.4/opvious/common.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/opvious/data.py` & `opvious-0.9.4/opvious/data.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/opvious/executors/__pycache__/__init__.cpython-310.pyc` & `opvious-0.9.4/opvious/executors/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 18:18:57 2023 UTC, .py size: 1966 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,118 +1,147 @@
-00000000: 6f0d 0d0a 0000 0000 915e 3064 ae07 0000  o........^0d....
+00000000: 6f0d 0d0a 0000 0000 0770 3064 3209 0000  o........p0d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
+00000020: 0007 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
-00000060: 6d0a 5a0a 0100 6700 6406 a201 5a0b 6407  m.Z...g.d...Z.d.
-00000070: 6408 8400 5a0c 0902 640e 6409 650d 640a  d...Z...d.d.e.d.
-00000080: 6503 650d 1900 640b 6506 6606 640c 640d  e.e...d.e.f.d.d.
-00000090: 8405 5a0e 6402 5300 290f 6100 0300 000a  ..Z.d.S.).a.....
-000000a0: 4c69 6365 6e73 6564 2074 6f20 7468 6520  Licensed to the 
-000000b0: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-000000c0: 466f 756e 6461 7469 6f6e 2028 4153 4629  Foundation (ASF)
-000000d0: 2075 6e64 6572 206f 6e65 0a6f 7220 6d6f   under one.or mo
-000000e0: 7265 2063 6f6e 7472 6962 7574 6f72 206c  re contributor l
-000000f0: 6963 656e 7365 2061 6772 6565 6d65 6e74  icense agreement
-00000100: 732e 2020 5365 6520 7468 6520 4e4f 5449  s.  See the NOTI
-00000110: 4345 2066 696c 650a 6469 7374 7269 6275  CE file.distribu
-00000120: 7465 6420 7769 7468 2074 6869 7320 776f  ted with this wo
-00000130: 726b 2066 6f72 2061 6464 6974 696f 6e61  rk for additiona
-00000140: 6c20 696e 666f 726d 6174 696f 6e0a 7265  l information.re
-00000150: 6761 7264 696e 6720 636f 7079 7269 6768  garding copyrigh
-00000160: 7420 6f77 6e65 7273 6869 702e 2020 5468  t ownership.  Th
-00000170: 6520 4153 4620 6c69 6365 6e73 6573 2074  e ASF licenses t
-00000180: 6869 7320 6669 6c65 0a74 6f20 796f 7520  his file.to you 
-00000190: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
-000001a0: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
-000001b0: 6e20 322e 3020 2874 6865 0a22 4c69 6365  n 2.0 (the."Lice
-000001c0: 6e73 6522 293b 2079 6f75 206d 6179 206e  nse"); you may n
-000001d0: 6f74 2075 7365 2074 6869 7320 6669 6c65  ot use this file
-000001e0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
-000001f0: 6961 6e63 650a 7769 7468 2074 6865 204c  iance.with the L
-00000200: 6963 656e 7365 2e20 2059 6f75 206d 6179  icense.  You may
-00000210: 206f 6274 6169 6e20 6120 636f 7079 206f   obtain a copy o
-00000220: 6620 7468 6520 4c69 6365 6e73 6520 6174  f the License at
-00000230: 0a0a 2020 6874 7470 3a2f 2f77 7777 2e61  ..  http://www.a
-00000240: 7061 6368 652e 6f72 672f 6c69 6365 6e73  pache.org/licens
-00000250: 6573 2f4c 4943 454e 5345 2d32 2e30 0a0a  es/LICENSE-2.0..
-00000260: 2020 556e 6c65 7373 2072 6571 7569 7265    Unless require
-00000270: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
-00000280: 6c61 7720 6f72 2061 6772 6565 6420 746f  law or agreed to
-00000290: 2069 6e20 7772 6974 696e 672c 0a20 2073   in writing,.  s
-000002a0: 6f66 7477 6172 6520 6469 7374 7269 6275  oftware distribu
-000002b0: 7465 6420 756e 6465 7220 7468 6520 4c69  ted under the Li
-000002c0: 6365 6e73 6520 6973 2064 6973 7472 6962  cense is distrib
-000002d0: 7574 6564 206f 6e20 616e 0a20 2022 4153  uted on an.  "AS
-000002e0: 2049 5322 2042 4153 4953 2c20 5749 5448   IS" BASIS, WITH
-000002f0: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
-00000300: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
-00000310: 414e 590a 2020 4b49 4e44 2c20 6569 7468  ANY.  KIND, eith
-00000320: 6572 2065 7870 7265 7373 206f 7220 696d  er express or im
-00000330: 706c 6965 642e 2020 5365 6520 7468 6520  plied.  See the 
-00000340: 4c69 6365 6e73 6520 666f 7220 7468 650a  License for the.
-00000350: 2020 7370 6563 6966 6963 206c 616e 6775    specific langu
-00000360: 6167 6520 676f 7665 726e 696e 6720 7065  age governing pe
-00000370: 726d 6973 7369 6f6e 7320 616e 6420 6c69  rmissions and li
-00000380: 6d69 7461 7469 6f6e 730a 2020 756e 6465  mitations.  unde
-00000390: 7220 7468 6520 4c69 6365 6e73 652e 0ae9  r the License...
-000003a0: 0000 0000 4e29 01da 084f 7074 696f 6e61  ....N)...Optiona
-000003b0: 6ce9 0100 0000 2906 da08 4170 6945 7272  l.....)...ApiErr
-000003c0: 6f72 da08 4578 6563 7574 6f72 da0e 4578  or..Executor..Ex
-000003d0: 6563 7574 6f72 5265 7375 6c74 da12 4a73  ecutorResult..Js
-000003e0: 6f6e 4578 6563 7574 6f72 5265 7375 6c74  onExecutorResult
-000003f0: da15 4a73 6f6e 5365 7145 7865 6375 746f  ..JsonSeqExecuto
-00000400: 7252 6573 756c 74da 1750 6c61 696e 5465  rResult..PlainTe
-00000410: 7874 4578 6563 7574 6f72 5265 7375 6c74  xtExecutorResult
-00000420: 2907 da10 6465 6661 756c 745f 6578 6563  )...default_exec
-00000430: 7574 6f72 7204 0000 0072 0500 0000 7206  utorr....r....r.
-00000440: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00000450: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000460: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00000470: 6401 7400 6a01 7600 5300 2902 4eda 0770  d.t.j.v.S.).N..p
-00000480: 796f 6469 6465 2902 da03 7379 73da 076d  yodide)...sys..m
-00000490: 6f64 756c 6573 a900 720e 0000 0072 0e00  odules..r....r..
-000004a0: 0000 fa3d 2f68 6f6d 652f 7275 6e6e 6572  ...=/home/runner
-000004b0: 2f77 6f72 6b2f 7364 6b2e 7079 2f73 646b  /work/sdk.py/sdk
-000004c0: 2e70 792f 6f70 7669 6f75 732f 6578 6563  .py/opvious/exec
-000004d0: 7574 6f72 732f 5f5f 696e 6974 5f5f 2e70  utors/__init__.p
-000004e0: 79da 115f 6973 5f75 7369 6e67 5f70 796f  y.._is_using_pyo
-000004f0: 6469 6465 2c00 0000 7302 0000 000a 0272  dide,...s......r
-00000500: 1000 0000 da07 6170 695f 7572 6cda 0d61  ......api_url..a
-00000510: 7574 686f 7269 7a61 7469 6f6e da06 7265  uthorization..re
-00000520: 7475 726e 6302 0000 0000 0000 0000 0000  turnc...........
-00000530: 0005 0000 0008 0000 0043 0000 0073 6600  .........C...sf.
-00000540: 0000 7400 8300 720f 6401 6402 6c01 6d02  ..t...r.d.d.l.m.
-00000550: 7d02 0100 7c02 7c00 7c01 6403 8d02 5300  }...|.|.|.d...S.
-00000560: 7a08 6401 6404 6c03 6d04 7d03 0100 5700  z.d.d.l.m.}...W.
-00000570: 6e15 0400 7405 792c 0100 0100 0100 6401  n...t.y,......d.
-00000580: 6405 6c06 6d07 7d04 0100 7c04 7c00 7c01  d.l.m.}...|.|.|.
-00000590: 6403 8d02 0600 5900 5300 7700 7c03 7c00  d.....Y.S.w.|.|.
-000005a0: 7c01 6403 8d02 5300 2906 7a34 496e 6665  |.d...S.).z4Infe
-000005b0: 7273 2074 6865 2062 6573 7420 6578 6563  rs the best exec
-000005c0: 7574 6f72 2066 6f72 2074 6865 2063 7572  utor for the cur
-000005d0: 7265 6e74 2065 6e76 6972 6f6e 6d65 6e74  rent environment
-000005e0: 7203 0000 0029 01da 0f50 796f 6469 6465  r....)...Pyodide
-000005f0: 4578 6563 7574 6f72 2902 7211 0000 0072  Executor).r....r
-00000600: 1200 0000 2901 da0f 4169 6f68 7474 7045  ....)...AiohttpE
-00000610: 7865 6375 746f 7229 01da 0e55 726c 6c69  xecutor)...Urlli
-00000620: 6245 7865 6375 746f 7229 0872 1000 0000  bExecutor).r....
-00000630: 720b 0000 0072 1400 0000 5a07 6169 6f68  r....r....Z.aioh
-00000640: 7474 7072 1500 0000 da0b 496d 706f 7274  ttpr......Import
-00000650: 4572 726f 72da 0675 726c 6c69 6272 1600  Error..urllibr..
-00000660: 0000 2905 7211 0000 0072 1200 0000 7214  ..).r....r....r.
-00000670: 0000 0072 1500 0000 7216 0000 0072 0e00  ...r....r....r..
-00000680: 0000 720e 0000 0072 0f00 0000 720a 0000  ..r....r....r...
-00000690: 0031 0000 0073 1800 0000 0604 0c01 0c02  .1...s..........
-000006a0: 0202 1001 0c01 0c01 1002 02fd 0205 0401  ................
-000006b0: 06ff 720a 0000 0029 014e 290f da07 5f5f  ..r....).N)...__
-000006c0: 646f 635f 5f72 0c00 0000 da06 7479 7069  doc__r......typi
-000006d0: 6e67 7202 0000 00da 0663 6f6d 6d6f 6e72  ngr......commonr
-000006e0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-000006f0: 0000 0072 0800 0000 7209 0000 00da 075f  ...r....r......_
-00000700: 5f61 6c6c 5f5f 7210 0000 00da 0373 7472  _all__r......str
-00000710: 720a 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000720: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000730: 6c65 3e01 0000 0073 1c00 0000 0400 0813  le>....s........
-00000740: 0c01 2002 080a 080b 0206 04ff 0201 02ff  .. .............
-00000750: 0601 02ff 0202 0efe                      ........
+00000060: 6d0a 5a0a 0100 6700 6406 a201 5a0b 0902  m.Z...g.d...Z...
+00000070: 6414 6407 650c 6408 6503 650c 1900 6409  d.d.e.d.e.e...d.
+00000080: 6506 6606 640a 640b 8405 5a0d 0902 6414  e.f.d.d...Z...d.
+00000090: 6407 650c 6408 6503 650c 1900 6409 6506  d.e.d.e.e...d.e.
+000000a0: 6606 640c 640d 8405 5a0e 0902 6414 6407  f.d.d...Z...d.d.
+000000b0: 650c 6408 6503 650c 1900 6409 6506 6606  e.d.e.e...d.e.f.
+000000c0: 640e 640f 8405 5a0f 6410 6411 8400 5a10  d.d...Z.d.d...Z.
+000000d0: 0902 6414 6407 650c 6408 6503 650c 1900  ..d.d.e.d.e.e...
+000000e0: 6409 6506 6606 6412 6413 8405 5a11 6402  d.e.f.d.d...Z.d.
+000000f0: 5300 2915 6100 0300 000a 4c69 6365 6e73  S.).a.....Licens
+00000100: 6564 2074 6f20 7468 6520 4170 6163 6865  ed to the Apache
+00000110: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
+00000120: 7469 6f6e 2028 4153 4629 2075 6e64 6572  tion (ASF) under
+00000130: 206f 6e65 0a6f 7220 6d6f 7265 2063 6f6e   one.or more con
+00000140: 7472 6962 7574 6f72 206c 6963 656e 7365  tributor license
+00000150: 2061 6772 6565 6d65 6e74 732e 2020 5365   agreements.  Se
+00000160: 6520 7468 6520 4e4f 5449 4345 2066 696c  e the NOTICE fil
+00000170: 650a 6469 7374 7269 6275 7465 6420 7769  e.distributed wi
+00000180: 7468 2074 6869 7320 776f 726b 2066 6f72  th this work for
+00000190: 2061 6464 6974 696f 6e61 6c20 696e 666f   additional info
+000001a0: 726d 6174 696f 6e0a 7265 6761 7264 696e  rmation.regardin
+000001b0: 6720 636f 7079 7269 6768 7420 6f77 6e65  g copyright owne
+000001c0: 7273 6869 702e 2020 5468 6520 4153 4620  rship.  The ASF 
+000001d0: 6c69 6365 6e73 6573 2074 6869 7320 6669  licenses this fi
+000001e0: 6c65 0a74 6f20 796f 7520 756e 6465 7220  le.to you under 
+000001f0: 7468 6520 4170 6163 6865 204c 6963 656e  the Apache Licen
+00000200: 7365 2c20 5665 7273 696f 6e20 322e 3020  se, Version 2.0 
+00000210: 2874 6865 0a22 4c69 6365 6e73 6522 293b  (the."License");
+00000220: 2079 6f75 206d 6179 206e 6f74 2075 7365   you may not use
+00000230: 2074 6869 7320 6669 6c65 2065 7863 6570   this file excep
+00000240: 7420 696e 2063 6f6d 706c 6961 6e63 650a  t in compliance.
+00000250: 7769 7468 2074 6865 204c 6963 656e 7365  with the License
+00000260: 2e20 2059 6f75 206d 6179 206f 6274 6169  .  You may obtai
+00000270: 6e20 6120 636f 7079 206f 6620 7468 6520  n a copy of the 
+00000280: 4c69 6365 6e73 6520 6174 0a0a 2020 6874  License at..  ht
+00000290: 7470 3a2f 2f77 7777 2e61 7061 6368 652e  tp://www.apache.
+000002a0: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
+000002b0: 454e 5345 2d32 2e30 0a0a 2020 556e 6c65  ENSE-2.0..  Unle
+000002c0: 7373 2072 6571 7569 7265 6420 6279 2061  ss required by a
+000002d0: 7070 6c69 6361 626c 6520 6c61 7720 6f72  pplicable law or
+000002e0: 2061 6772 6565 6420 746f 2069 6e20 7772   agreed to in wr
+000002f0: 6974 696e 672c 0a20 2073 6f66 7477 6172  iting,.  softwar
+00000300: 6520 6469 7374 7269 6275 7465 6420 756e  e distributed un
+00000310: 6465 7220 7468 6520 4c69 6365 6e73 6520  der the License 
+00000320: 6973 2064 6973 7472 6962 7574 6564 206f  is distributed o
+00000330: 6e20 616e 0a20 2022 4153 2049 5322 2042  n an.  "AS IS" B
+00000340: 4153 4953 2c20 5749 5448 4f55 5420 5741  ASIS, WITHOUT WA
+00000350: 5252 414e 5449 4553 204f 5220 434f 4e44  RRANTIES OR COND
+00000360: 4954 494f 4e53 204f 4620 414e 590a 2020  ITIONS OF ANY.  
+00000370: 4b49 4e44 2c20 6569 7468 6572 2065 7870  KIND, either exp
+00000380: 7265 7373 206f 7220 696d 706c 6965 642e  ress or implied.
+00000390: 2020 5365 6520 7468 6520 4c69 6365 6e73    See the Licens
+000003a0: 6520 666f 7220 7468 650a 2020 7370 6563  e for the.  spec
+000003b0: 6966 6963 206c 616e 6775 6167 6520 676f  ific language go
+000003c0: 7665 726e 696e 6720 7065 726d 6973 7369  verning permissi
+000003d0: 6f6e 7320 616e 6420 6c69 6d69 7461 7469  ons and limitati
+000003e0: 6f6e 730a 2020 756e 6465 7220 7468 6520  ons.  under the 
+000003f0: 4c69 6365 6e73 652e 0ae9 0000 0000 4e29  License.......N)
+00000400: 01da 084f 7074 696f 6e61 6ce9 0100 0000  ...Optional.....
+00000410: 2906 da08 4170 6945 7272 6f72 da08 4578  )...ApiError..Ex
+00000420: 6563 7574 6f72 da0e 4578 6563 7574 6f72  ecutor..Executor
+00000430: 5265 7375 6c74 da12 4a73 6f6e 4578 6563  Result..JsonExec
+00000440: 7574 6f72 5265 7375 6c74 da15 4a73 6f6e  utorResult..Json
+00000450: 5365 7145 7865 6375 746f 7252 6573 756c  SeqExecutorResul
+00000460: 74da 1750 6c61 696e 5465 7874 4578 6563  t..PlainTextExec
+00000470: 7574 6f72 5265 7375 6c74 2907 da10 6465  utorResult)...de
+00000480: 6661 756c 745f 6578 6563 7574 6f72 7204  fault_executorr.
+00000490: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
+000004a0: 0000 7208 0000 0072 0900 0000 da07 6170  ..r....r......ap
+000004b0: 695f 7572 6cda 0d61 7574 686f 7269 7a61  i_url..authoriza
+000004c0: 7469 6f6e da06 7265 7475 726e 6302 0000  tion..returnc...
+000004d0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000004e0: 0043 0000 0073 1600 0000 6401 6402 6c00  .C...s....d.d.l.
+000004f0: 6d01 7d02 0100 7c02 7c00 7c01 8302 5300  m.}...|.|.|...S.
+00000500: 2903 4e72 0300 0000 2901 da0f 4169 6f68  ).Nr....)...Aioh
+00000510: 7474 7045 7865 6375 746f 7229 025a 0761  ttpExecutor).Z.a
+00000520: 696f 6874 7470 720e 0000 0029 0372 0b00  iohttpr....).r..
+00000530: 0000 720c 0000 0072 0e00 0000 a900 720f  ..r....r......r.
+00000540: 0000 00fa 3d2f 686f 6d65 2f72 756e 6e65  ....=/home/runne
+00000550: 722f 776f 726b 2f73 646b 2e70 792f 7364  r/work/sdk.py/sd
+00000560: 6b2e 7079 2f6f 7076 696f 7573 2f65 7865  k.py/opvious/exe
+00000570: 6375 746f 7273 2f5f 5f69 6e69 745f 5f2e  cutors/__init__.
+00000580: 7079 da10 6169 6f68 7474 705f 6578 6563  py..aiohttp_exec
+00000590: 7574 6f72 2c00 0000 7304 0000 000c 030a  utor,...s.......
+000005a0: 0272 1100 0000 6302 0000 0000 0000 0000  .r....c.........
+000005b0: 0000 0003 0000 0004 0000 0043 0000 00f3  ...........C....
+000005c0: 1800 0000 6401 6402 6c00 6d01 7d02 0100  ....d.d.l.m.}...
+000005d0: 7c02 7c00 7c01 6403 8d02 5300 2904 4e72  |.|.|.d...S.).Nr
+000005e0: 0300 0000 2901 da0f 5079 6f64 6964 6545  ....)...PyodideE
+000005f0: 7865 6375 746f 72a9 0272 0b00 0000 720c  xecutor..r....r.
+00000600: 0000 0029 02da 0770 796f 6469 6465 7213  ...)...pyodider.
+00000610: 0000 0029 0372 0b00 0000 720c 0000 0072  ...).r....r....r
+00000620: 1300 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00000630: 0000 00da 1070 796f 6469 6465 5f65 7865  .....pyodide_exe
+00000640: 6375 746f 7234 0000 00f3 0400 0000 0c03  cutor4..........
+00000650: 0c02 7216 0000 0063 0200 0000 0000 0000  ..r....c........
+00000660: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000670: 7212 0000 0029 044e 7203 0000 0029 01da  r....).Nr....)..
+00000680: 0e55 726c 6c69 6245 7865 6375 746f 7272  .UrllibExecutorr
+00000690: 1400 0000 2902 da06 7572 6c6c 6962 7218  ....)...urllibr.
+000006a0: 0000 0029 0372 0b00 0000 720c 0000 0072  ...).r....r....r
+000006b0: 1800 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+000006c0: 0000 00da 0f75 726c 6c69 625f 6578 6563  .....urllib_exec
+000006d0: 7574 6f72 3c00 0000 7217 0000 0072 1a00  utor<...r....r..
+000006e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000006f0: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000700: 6401 7400 6a01 7600 5300 2902 4e72 1500  d.t.j.v.S.).Nr..
+00000710: 0000 2902 da03 7379 73da 076d 6f64 756c  ..)...sys..modul
+00000720: 6573 720f 0000 0072 0f00 0000 720f 0000  esr....r....r...
+00000730: 0072 1000 0000 da11 5f69 735f 7573 696e  .r......_is_usin
+00000740: 675f 7079 6f64 6964 6544 0000 0073 0200  g_pyodideD...s..
+00000750: 0000 0a02 721d 0000 0063 0200 0000 0000  ....r....c......
+00000760: 0000 0000 0000 0200 0000 0800 0000 4300  ..............C.
+00000770: 0000 7340 0000 0074 0083 0072 0974 017c  ..s@...t...r.t.|
+00000780: 007c 0164 018d 0253 007a 0774 027c 007c  .|.d...S.z.t.|.|
+00000790: 0164 018d 0257 0053 0004 0074 0379 1f01  .d...W.S...t.y..
+000007a0: 0001 0001 0074 047c 007c 0164 018d 0206  .....t.|.|.d....
+000007b0: 0059 0053 0077 0029 027a 3449 6e66 6572  .Y.S.w.).z4Infer
+000007c0: 7320 7468 6520 6265 7374 2065 7865 6375  s the best execu
+000007d0: 746f 7220 666f 7220 7468 6520 6375 7272  tor for the curr
+000007e0: 656e 7420 656e 7669 726f 6e6d 656e 7472  ent environmentr
+000007f0: 1400 0000 2905 721d 0000 0072 1600 0000  ....).r....r....
+00000800: 7211 0000 00da 0b49 6d70 6f72 7445 7272  r......ImportErr
+00000810: 6f72 721a 0000 0072 1400 0000 720f 0000  orr....r....r...
+00000820: 0072 0f00 0000 7210 0000 0072 0a00 0000  .r....r....r....
+00000830: 4900 0000 730e 0000 0006 040c 0102 010e  I...s...........
+00000840: 010c 0110 0102 ff72 0a00 0000 2901 4e29  .......r....).N)
+00000850: 12da 075f 5f64 6f63 5f5f 721b 0000 00da  ...__doc__r.....
+00000860: 0674 7970 696e 6772 0200 0000 da06 636f  .typingr......co
+00000870: 6d6d 6f6e 7204 0000 0072 0500 0000 7206  mmonr....r....r.
+00000880: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
+00000890: 0000 da07 5f5f 616c 6c5f 5fda 0373 7472  ....__all__..str
+000008a0: 7211 0000 0072 1600 0000 721a 0000 0072  r....r....r....r
+000008b0: 1d00 0000 720a 0000 0072 0f00 0000 720f  ....r....r....r.
+000008c0: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
+000008d0: 6d6f 6475 6c65 3e01 0000 0073 4c00 0000  module>....sL...
+000008e0: 0400 0813 0c01 2002 080a 020c 04ff 0201  ...... .........
+000008f0: 02ff 0601 02ff 0202 0afe 0209 04ff 0201  ................
+00000900: 02ff 0601 02ff 0202 0afe 0209 04ff 0201  ................
+00000910: 02ff 0601 02ff 0202 0afe 0808 0206 04ff  ................
+00000920: 0201 02ff 0601 02ff 0202 0efe            ............
```

### Comparing `opvious-0.9.3/opvious/executors/__pycache__/aiohttp.cpython-310.pyc` & `opvious-0.9.4/opvious/executors/__pycache__/aiohttp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 18:18:57 2023 UTC, .py size: 4068 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 915e 3064 e40f 0000  o........^0d....
+00000000: 6f0d 0d0a 0000 0000 0770 3064 e40f 0000  o........p0d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `opvious-0.9.3/opvious/executors/__pycache__/common.cpython-310.pyc` & `opvious-0.9.4/opvious/executors/__pycache__/common.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 18:18:57 2023 UTC, .py size: 8799 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,594 +1,606 @@
-00000000: 6f0d 0d0a 0000 0000 915e 3064 5f22 0000  o........^0d_"..
+00000000: 6f0d 0d0a 0000 0000 0770 3064 ee22 0000  o........p0d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 7401 0000 6400  .....@...st...d.
+00000020: 0007 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6401 6402 6c0d 5a0e 6404  m.Z...d.d.l.Z.d.
 00000080: 6405 6c0f 6d10 5a10 0100 6504 a011 6512  d.l.m.Z...e...e.
-00000090: a101 5a13 6406 5a14 6407 5a15 6516 6517  ..Z.d.Z.d.Z.e.e.
-000000a0: 6517 6602 1900 5a18 4700 6408 6409 8400  e.f...Z.G.d.d...
-000000b0: 6409 6519 8303 5a1a 0902 6427 640a 6517  d.e...Z...d'd.e.
-000000c0: 640b 650b 6517 1900 640c 6519 6606 640d  d.e.e...d.e.f.d.
-000000d0: 640e 8405 5a1b 0902 6427 640f 650b 6517  d...Z...d'd.e.e.
-000000e0: 1900 640b 650b 6517 1900 640c 6519 6606  ..d.e.e...d.e.f.
-000000f0: 6410 6411 8405 5a1c 6502 6a1d 4700 6412  d.d...Z.e.j.G.d.
-00000100: 6413 8400 6413 8302 8301 5a1e 6502 6a1d  d...d.....Z.e.j.
-00000110: 4700 6414 6415 8400 6415 651e 8303 8301  G.d.d...d.e.....
-00000120: 5a1f 4700 6416 6417 8400 6417 8302 5a20  Z.G.d.d...d...Z 
-00000130: 6502 6a1d 4700 6418 6419 8400 6419 651e  e.j.G.d.d...d.e.
-00000140: 8303 8301 5a21 6502 6a1d 4700 641a 641b  ....Z!e.j.G.d.d.
-00000150: 8400 641b 651e 8303 8301 5a22 641c 5a23  ..d.e.....Z"d.Z#
-00000160: 641d 6524 640c 6506 6604 641e 641f 8404  d.e$d.e.f.d.d...
-00000170: 5a25 650c 6420 651e 6421 8d02 5a26 4700  Z%e.d e.d!..Z&G.
-00000180: 6422 6423 8400 6423 8302 5a27 6424 6517  d"d#..d#..Z'd$e.
-00000190: 640c 6518 6604 6425 6426 8404 5a28 6402  d.e.f.d%d&..Z(d.
-000001a0: 5300 2928 6100 0300 000a 4c69 6365 6e73  S.)(a.....Licens
-000001b0: 6564 2074 6f20 7468 6520 4170 6163 6865  ed to the Apache
-000001c0: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
-000001d0: 7469 6f6e 2028 4153 4629 2075 6e64 6572  tion (ASF) under
-000001e0: 206f 6e65 0a6f 7220 6d6f 7265 2063 6f6e   one.or more con
-000001f0: 7472 6962 7574 6f72 206c 6963 656e 7365  tributor license
-00000200: 2061 6772 6565 6d65 6e74 732e 2020 5365   agreements.  Se
-00000210: 6520 7468 6520 4e4f 5449 4345 2066 696c  e the NOTICE fil
-00000220: 650a 6469 7374 7269 6275 7465 6420 7769  e.distributed wi
-00000230: 7468 2074 6869 7320 776f 726b 2066 6f72  th this work for
-00000240: 2061 6464 6974 696f 6e61 6c20 696e 666f   additional info
-00000250: 726d 6174 696f 6e0a 7265 6761 7264 696e  rmation.regardin
-00000260: 6720 636f 7079 7269 6768 7420 6f77 6e65  g copyright owne
-00000270: 7273 6869 702e 2020 5468 6520 4153 4620  rship.  The ASF 
-00000280: 6c69 6365 6e73 6573 2074 6869 7320 6669  licenses this fi
-00000290: 6c65 0a74 6f20 796f 7520 756e 6465 7220  le.to you under 
-000002a0: 7468 6520 4170 6163 6865 204c 6963 656e  the Apache Licen
-000002b0: 7365 2c20 5665 7273 696f 6e20 322e 3020  se, Version 2.0 
-000002c0: 2874 6865 0a22 4c69 6365 6e73 6522 293b  (the."License");
-000002d0: 2079 6f75 206d 6179 206e 6f74 2075 7365   you may not use
-000002e0: 2074 6869 7320 6669 6c65 2065 7863 6570   this file excep
-000002f0: 7420 696e 2063 6f6d 706c 6961 6e63 650a  t in compliance.
-00000300: 7769 7468 2074 6865 204c 6963 656e 7365  with the License
-00000310: 2e20 2059 6f75 206d 6179 206f 6274 6169  .  You may obtai
-00000320: 6e20 6120 636f 7079 206f 6620 7468 6520  n a copy of the 
-00000330: 4c69 6365 6e73 6520 6174 0a0a 2020 6874  License at..  ht
-00000340: 7470 3a2f 2f77 7777 2e61 7061 6368 652e  tp://www.apache.
-00000350: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
-00000360: 454e 5345 2d32 2e30 0a0a 2020 556e 6c65  ENSE-2.0..  Unle
-00000370: 7373 2072 6571 7569 7265 6420 6279 2061  ss required by a
-00000380: 7070 6c69 6361 626c 6520 6c61 7720 6f72  pplicable law or
-00000390: 2061 6772 6565 6420 746f 2069 6e20 7772   agreed to in wr
-000003a0: 6974 696e 672c 0a20 2073 6f66 7477 6172  iting,.  softwar
-000003b0: 6520 6469 7374 7269 6275 7465 6420 756e  e distributed un
-000003c0: 6465 7220 7468 6520 4c69 6365 6e73 6520  der the License 
-000003d0: 6973 2064 6973 7472 6962 7574 6564 206f  is distributed o
-000003e0: 6e20 616e 0a20 2022 4153 2049 5322 2042  n an.  "AS IS" B
-000003f0: 4153 4953 2c20 5749 5448 4f55 5420 5741  ASIS, WITHOUT WA
-00000400: 5252 414e 5449 4553 204f 5220 434f 4e44  RRANTIES OR COND
-00000410: 4954 494f 4e53 204f 4620 414e 590a 2020  ITIONS OF ANY.  
-00000420: 4b49 4e44 2c20 6569 7468 6572 2065 7870  KIND, either exp
-00000430: 7265 7373 206f 7220 696d 706c 6965 642e  ress or implied.
-00000440: 2020 5365 6520 7468 6520 4c69 6365 6e73    See the Licens
-00000450: 6520 666f 7220 7468 650a 2020 7370 6563  e for the.  spec
-00000460: 6966 6963 206c 616e 6775 6167 6520 676f  ific language go
-00000470: 7665 726e 696e 6720 7065 726d 6973 7369  verning permissi
-00000480: 6f6e 7320 616e 6420 6c69 6d69 7461 7469  ons and limitati
-00000490: 6f6e 730a 2020 756e 6465 7220 7468 6520  ons.  under the 
-000004a0: 4c69 6365 6e73 652e 0ae9 0000 0000 4e29  License.......N)
-000004b0: 07da 0341 6e79 da13 4173 796e 6343 6f6e  ...Any..AsyncCon
-000004c0: 7465 7874 4d61 6e61 6765 72da 0d41 7379  textManager..Asy
-000004d0: 6e63 4974 6572 6174 6f72 da04 5479 7065  ncIterator..Type
-000004e0: da07 4d61 7070 696e 67da 084f 7074 696f  ..Mapping..Optio
-000004f0: 6e61 6cda 0754 7970 6556 6172 e902 0000  nal..TypeVar....
-00000500: 00a9 01da 0b5f 5f76 6572 7369 6f6e 5f5f  .....__version__
-00000510: 7a0d 6f70 7669 6f75 732d 7472 6163 65fa  z.opvious-trace.
-00000520: 0c63 6f6e 7465 6e74 2d74 7970 6563 0000  .content-typec..
-00000530: 0000 0000 0000 0000 0000 0000 0000 0800  ................
-00000540: 0000 0000 0000 733c 0000 0065 005a 0164  ......s<...e.Z.d
-00000550: 005a 0264 015a 0309 0209 0264 0864 0365  .Z.d.Z.....d.d.e
-00000560: 0464 0465 0565 0619 0064 0565 0565 0719  .d.e.e...d.e.e..
-00000570: 0066 0687 0066 0164 0664 0784 0d5a 0887  .f...f.d.d...Z..
-00000580: 0004 005a 0953 0029 09da 0841 7069 4572  ...Z.S.)...ApiEr
-00000590: 726f 727a 344c 6f63 616c 2072 6570 7265  rorz4Local repre
-000005a0: 7365 6e74 6174 696f 6e20 6f66 2061 6e20  sentation of an 
-000005b0: 6572 726f 7220 7265 7475 726e 6564 2062  error returned b
-000005c0: 7920 7468 6520 4150 494e da06 7374 6174  y the APIN..stat
-000005d0: 7573 da05 7472 6163 65da 0464 6174 6163  us..trace..datac
-000005e0: 0400 0000 0000 0000 0000 0000 0500 0000  ................
-000005f0: 0400 0000 0300 0000 7352 0000 0064 017c  ........sR...d.|
-00000600: 019b 009d 027d 047c 0272 0f7c 0464 027c  .....}.|.r.|.d.|
-00000610: 029b 0064 039d 0337 007d 047c 0372 187c  ...d...7.}.|.r.|
-00000620: 0464 047c 039b 009d 0237 007d 0474 0083  .d.|.....7.}.t..
-00000630: 00a0 017c 04a1 0101 007c 017c 005f 027c  ...|.....|.|._.|
-00000640: 027c 005f 037c 037c 005f 0464 0053 0029  .|._.|.|._.d.S.)
-00000650: 054e 7a1c 4150 4920 6361 6c6c 2066 6169  .Nz.API call fai
-00000660: 6c65 6420 7769 7468 2073 7461 7475 7320  led with status 
-00000670: fa02 2028 fa01 29fa 023a 2029 05da 0573  .. (..)..: )...s
-00000680: 7570 6572 da08 5f5f 696e 6974 5f5f 720e  uper..__init__r.
-00000690: 0000 0072 0f00 0000 7210 0000 0029 05da  ...r....r....)..
-000006a0: 0473 656c 6672 0e00 0000 720f 0000 0072  .selfr....r....r
-000006b0: 1000 0000 da07 6d65 7373 6167 65a9 01da  ......message...
-000006c0: 095f 5f63 6c61 7373 5f5f a900 fa3b 2f68  .__class__...;/h
-000006d0: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
-000006e0: 7364 6b2e 7079 2f73 646b 2e70 792f 6f70  sdk.py/sdk.py/op
-000006f0: 7669 6f75 732f 6578 6563 7574 6f72 732f  vious/executors/
-00000700: 636f 6d6d 6f6e 2e70 7972 1500 0000 3500  common.pyr....5.
-00000710: 0000 7312 0000 000a 0604 0110 0104 010e  ..s.............
-00000720: 010c 0106 0106 010a 017a 1141 7069 4572  .........z.ApiEr
-00000730: 726f 722e 5f5f 696e 6974 5f5f 2902 4e4e  ror.__init__).NN
-00000740: 290a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000750: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000760: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-00000770: 0369 6e74 7207 0000 00da 0373 7472 7202  .intr......strr.
-00000780: 0000 0072 1500 0000 da0d 5f5f 636c 6173  ...r......__clas
-00000790: 7363 656c 6c5f 5f72 1a00 0000 721a 0000  scell__r....r...
-000007a0: 0072 1800 0000 721b 0000 0072 0d00 0000  .r....r....r....
-000007b0: 3200 0000 7316 0000 0008 0004 0102 0502  2...s...........
-000007c0: 0104 fc02 0202 fe06 0302 fd06 0416 fc72  ...............r
-000007d0: 0d00 0000 7217 0000 0072 0f00 0000 da06  ....r....r......
-000007e0: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
-000007f0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-00000800: 3200 0000 7400 6401 7c01 720a 6402 7c01  2...t.d.|.r.d.|.
-00000810: 9b00 6403 9d03 6e01 6404 1700 7c00 7215  ..d...n.d...|.r.
-00000820: 6405 7c00 9b00 9d02 1700 8301 5300 6404  d.|.........S.d.
-00000830: 1700 8301 5300 2906 4e7a 1355 6e65 7870  ....S.).Nz.Unexp
-00000840: 6563 7465 6420 7265 7370 6f6e 7365 7211  ected responser.
-00000850: 0000 0072 1200 0000 da00 7213 0000 0029  ...r......r....)
-00000860: 01da 0945 7863 6570 7469 6f6e a902 7217  ...Exception..r.
-00000870: 0000 0072 0f00 0000 721a 0000 0072 1a00  ...r....r....r..
-00000880: 0000 721b 0000 00da 1975 6e65 7870 6563  ..r......unexpec
-00000890: 7465 645f 7265 7370 6f6e 7365 5f65 7272  ted_response_err
-000008a0: 6f72 4600 0000 7314 0000 0002 0302 0112  orF...s.........
-000008b0: 0102 ff0c 0202 fe04 ff02 0302 fe04 ff72  ...............r
-000008c0: 2700 0000 da0c 636f 6e74 656e 745f 7479  '.....content_ty
-000008d0: 7065 6302 0000 0000 0000 0000 0000 0002  pec.............
-000008e0: 0000 0004 0000 0043 0000 0073 1200 0000  .......C...s....
-000008f0: 7400 6401 7c00 9b00 9d02 7c01 6402 8d02  t.d.|.....|.d...
-00000900: 5300 2903 4e7a 1a75 6e73 7570 706f 7274  S.).Nz.unsupport
-00000910: 6564 2063 6f6e 7465 6e74 2d74 7970 653a  ed content-type:
-00000920: 2072 2600 0000 2901 7227 0000 0029 0272   r&...).r'...).r
-00000930: 2800 0000 720f 0000 0072 1a00 0000 721a  (...r....r....r.
-00000940: 0000 0072 1b00 0000 da1e 756e 7375 7070  ...r......unsupp
-00000950: 6f72 7465 645f 636f 6e74 656e 745f 7479  orted_content_ty
-00000960: 7065 5f65 7272 6f72 5000 0000 7308 0000  pe_errorP...s...
-00000970: 0002 0308 0102 0106 fe72 2900 0000 6300  .........r)...c.
-00000980: 0000 0000 0000 0000 0000 0000 0000 0007  ................
-00000990: 0000 0040 0000 0073 8400 0000 6500 5a01  ...@...s....e.Z.
-000009a0: 6400 5a02 5500 6503 6504 6401 3c00 6505  d.Z.U.e.e.d.<.e.
-000009b0: 6506 1900 6504 6402 3c00 6403 6404 8400  e...e.d.<.d.d...
-000009c0: 5a07 6508 6405 6506 6602 6406 6407 8404  Z.e.d.e.f.d.d...
-000009d0: 8301 5a09 6508 6405 6506 6602 6408 6409  ..Z.e.d.e.f.d.d.
-000009e0: 8404 8301 5a0a 6411 6401 6503 640b 6505  ....Z.d.d.e.d.e.
-000009f0: 6506 1900 6405 640a 6606 640c 640d 8405  e...d.d.f.d.d...
-00000a00: 5a0b 650c 640e 6505 6506 1900 6405 650d  Z.e.d.e.e...d.e.
-00000a10: 6604 640f 6410 8404 8301 5a0e 640a 5300  f.d.d.....Z.d.S.
-00000a20: 2912 da0e 4578 6563 7574 6f72 5265 7375  )...ExecutorResu
-00000a30: 6c74 720e 0000 0072 0f00 0000 6301 0000  ltr....r....c...
-00000a40: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00000a50: 0043 0000 0073 1600 0000 7400 a001 6401  .C...s....t...d.
-00000a60: 7c00 6a02 7c00 6a03 a103 0100 6400 5300  |.j.|.j.....d.S.
-00000a70: 2902 4e7a 2747 6f74 2041 5049 2072 6573  ).Nz'Got API res
-00000a80: 706f 6e73 652e 205b 7374 6174 7573 3d25  ponse. [status=%
-00000a90: 732c 2074 7261 6365 3d25 735d 2904 da07  s, trace=%s])...
-00000aa0: 5f6c 6f67 6765 72da 0564 6562 7567 720e  _logger..debugr.
-00000ab0: 0000 0072 0f00 0000 a901 7216 0000 0072  ...r......r....r
-00000ac0: 1a00 0000 721a 0000 0072 1b00 0000 da0d  ....r....r......
-00000ad0: 5f5f 706f 7374 5f69 6e69 745f 5f5e 0000  __post_init__^..
-00000ae0: 0073 0600 0000 0401 0a01 08ff 7a1c 4578  .s..........z.Ex
-00000af0: 6563 7574 6f72 5265 7375 6c74 2e5f 5f70  ecutorResult.__p
-00000b00: 6f73 745f 696e 6974 5f5f 7223 0000 0063  ost_init__r#...c
-00000b10: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000b20: 0100 0000 4300 0000 f306 0000 0074 0083  ....C........t..
-00000b30: 0082 01a9 014e a901 da13 4e6f 7449 6d70  .....N....NotImp
-00000b40: 6c65 6d65 6e74 6564 4572 726f 7272 2d00  lementedErrorr-.
-00000b50: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000b60: 00da 0661 6363 6570 7463 0000 00f3 0200  ...acceptc......
-00000b70: 0000 0602 7a15 4578 6563 7574 6f72 5265  ....z.ExecutorRe
-00000b80: 7375 6c74 2e61 6363 6570 7463 0100 0000  sult.acceptc....
-00000b90: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000ba0: 4300 0000 722f 0000 0072 3000 0000 7231  C...r/...r0...r1
-00000bb0: 0000 0072 2d00 0000 721a 0000 0072 1a00  ...r-...r....r..
-00000bc0: 0000 721b 0000 0072 2800 0000 6700 0000  ..r....r(...g...
-00000bd0: 7234 0000 007a 1b45 7865 6375 746f 7252  r4...z.ExecutorR
-00000be0: 6573 756c 742e 636f 6e74 656e 745f 7479  esult.content_ty
-00000bf0: 7065 4eda 0474 6578 7463 0300 0000 0000  peN..textc......
-00000c00: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000c10: 0000 7320 0000 007c 006a 007c 016b 0272  ..s ...|.j.|.k.r
-00000c20: 0764 0053 0074 017c 006a 007c 006a 027c  .d.S.t.|.j.|.j.|
-00000c30: 0264 018d 0382 0129 024e a903 720e 0000  .d.....).N..r...
-00000c40: 0072 0f00 0000 7210 0000 0029 0372 0e00  .r....r....).r..
-00000c50: 0000 720d 0000 0072 0f00 0000 2903 7216  ..r....r....).r.
-00000c60: 0000 0072 0e00 0000 7235 0000 0072 1a00  ...r....r5...r..
-00000c70: 0000 721a 0000 0072 1b00 0000 da0e 5f61  ..r....r......_a
-00000c80: 7373 6572 745f 7374 6174 7573 6b00 0000  ssert_statusk...
-00000c90: 7306 0000 000a 0104 0112 017a 1d45 7865  s..........z.Exe
-00000ca0: 6375 746f 7252 6573 756c 742e 5f61 7373  cutorResult._ass
-00000cb0: 6572 745f 7374 6174 7573 da05 6374 7970  ert_status..ctyp
-00000cc0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00000cd0: 0000 0400 0000 4300 0000 731c 0000 0074  ......C...s....t
-00000ce0: 007c 016f 0c7c 01a0 0164 01a1 0164 0219  .|.o.|...d...d..
-00000cf0: 007c 006a 026b 0283 0153 0029 034e fa01  .|.j.k...S.).N..
-00000d00: 3b72 0100 0000 2903 da04 626f 6f6c da05  ;r....)...bool..
-00000d10: 7370 6c69 7472 2800 0000 2902 da03 636c  splitr(...)...cl
-00000d20: 7372 3800 0000 721a 0000 0072 1a00 0000  sr8...r....r....
-00000d30: 721b 0000 00da 0b69 735f 656c 6967 6962  r......is_eligib
-00000d40: 6c65 7000 0000 7302 0000 001c 027a 1a45  lep...s......z.E
-00000d50: 7865 6375 746f 7252 6573 756c 742e 6973  xecutorResult.is
-00000d60: 5f65 6c69 6769 626c 6572 3000 0000 290f  _eligibler0...).
-00000d70: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00000d80: 2000 0000 da0f 5f5f 616e 6e6f 7461 7469   .....__annotati
-00000d90: 6f6e 735f 5f72 0700 0000 7221 0000 0072  ons__r....r!...r
-00000da0: 2e00 0000 da08 7072 6f70 6572 7479 7233  ......propertyr3
-00000db0: 0000 0072 2800 0000 7237 0000 00da 0b63  ...r(...r7.....c
-00000dc0: 6c61 7373 6d65 7468 6f64 723a 0000 0072  lassmethodr:...r
-00000dd0: 3d00 0000 721a 0000 0072 1a00 0000 721a  =...r....r....r.
-00000de0: 0000 0072 1b00 0000 722a 0000 0059 0000  ...r....r*...Y..
-00000df0: 0073 1600 0000 0a00 0802 0c01 0802 0205  .s..............
-00000e00: 1001 0203 1001 1c03 0205 1c01 722a 0000  ............r*..
-00000e10: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000e20: 0000 0600 0000 4000 0000 7356 0000 0065  ......@...sV...e
-00000e30: 005a 0164 005a 0255 0064 015a 0364 025a  .Z.d.Z.U.d.Z.d.Z
-00000e40: 0465 056a 0664 0364 048d 015a 0765 0865  .e.j.d.d...Z.e.e
-00000e50: 0964 053c 0064 0665 0a66 0264 0764 0884  .d.<.d.e.f.d.d..
-00000e60: 045a 0b09 0964 0e64 0a65 0c65 0d19 0064  .Z...d.d.e.e...d
-00000e70: 0665 0e65 0a19 0066 0464 0b64 0c84 055a  .e.e...f.d.d...Z
-00000e80: 0f64 0d53 0029 0fda 1750 6c61 696e 5465  .d.S.)...PlainTe
-00000e90: 7874 4578 6563 7574 6f72 5265 7375 6c74  xtExecutorResult
-00000ea0: 7a1b 506c 6169 6e20 7465 7874 2065 7865  z.Plain text exe
-00000eb0: 6375 7469 6f6e 2072 6573 756c 74fa 0a74  cution result..t
-00000ec0: 6578 742f 706c 6169 6e46 a901 da04 7265  ext/plainF....re
-00000ed0: 7072 da06 7265 6164 6572 7223 0000 0063  pr..readerr#...c
-00000ee0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000ef0: 0700 0000 c300 0000 7336 0000 0081 0167  ........s6.....g
-00000f00: 007d 017c 006a 0064 0064 018d 0132 007a  .}.|.j.d.d...2.z
-00000f10: 0b33 0064 0048 0057 007d 027c 01a0 017c  .3.d.H.W.}.|...|
-00000f20: 02a1 0101 0071 0936 0064 02a0 027c 01a1  .....q.6.d...|..
-00000f30: 0153 0029 034e 2901 da0d 6173 7365 7274  .S.).N)...assert
-00000f40: 5f73 7461 7475 7372 2400 0000 2903 da05  _statusr$...)...
-00000f50: 6c69 6e65 73da 0661 7070 656e 64da 046a  lines..append..j
-00000f60: 6f69 6e29 0372 1600 0000 7247 0000 00da  oin).r....rG....
-00000f70: 046c 696e 6572 1a00 0000 721a 0000 0072  .liner....r....r
-00000f80: 1b00 0000 7235 0000 007c 0000 0073 0c00  ....r5...|...s..
-00000f90: 0000 0280 0401 1801 0c01 02ff 0a02 7a1c  ..............z.
-00000fa0: 506c 6169 6e54 6578 7445 7865 6375 746f  PlainTextExecuto
-00000fb0: 7252 6573 756c 742e 7465 7874 e9c8 0000  rResult.text....
-00000fc0: 0072 4600 0000 6302 0000 0000 0000 0000  .rF...c.........
-00000fd0: 0000 0005 0000 0007 0000 0043 0200 0073  ...........C...s
-00000fe0: c800 0000 8102 7c01 7208 7c00 a000 7c01  ......|.r.|...|.
-00000ff0: a101 0100 7401 7c00 6a02 7403 8302 721d  ....t.|.j.t...r.
-00001000: 7c00 6a02 6a04 6401 6402 8d01 4400 5d05  |.j.j.d.d...D.].
-00001010: 7d02 7c02 5600 0100 7115 6400 5300 7405  }.|.V...q.d.S.t.
-00001020: 8300 7d03 7406 7c00 6a02 6403 8302 723d  ..}.t.|.j.d...r=
-00001030: 7c00 6a02 3200 7a11 3300 6400 4800 5700  |.j.2.z.3.d.H.W.
-00001040: 7d04 7c03 a007 7c04 a101 4400 5d05 7d02  }.|...|...D.].}.
-00001050: 7c02 5600 0100 7134 7129 3600 6e20 7406  |.V...q4q)6.n t.
-00001060: 7c00 6a02 6404 8302 7255 7c00 6a02 4400  |.j.d...rU|.j.D.
-00001070: 5d0d 7d04 7c03 a007 7c04 a101 4400 5d05  ].}.|...|...D.].
-00001080: 7d02 7c02 5600 0100 714d 7146 6e08 7408  }.|.V...qMqFn.t.
-00001090: 6405 7c00 6a02 9b00 9d02 8301 8201 7c03  d.|.j.........|.
-000010a0: a009 a100 5600 0100 6400 5300 2906 4e54  ....V...d.S.).NT
-000010b0: a901 da08 6b65 6570 656e 6473 da09 5f5f  ....keepends..__
-000010c0: 6169 7465 725f 5fda 085f 5f69 7465 725f  aiter__..__iter_
-000010d0: 5ffa 154e 6f6e 2d69 7465 7261 626c 6520  _..Non-iterable 
-000010e0: 7265 6164 6572 3a20 290a 7237 0000 00da  reader: ).r7....
-000010f0: 0a69 7369 6e73 7461 6e63 6572 4500 0000  .isinstancerE...
-00001100: 7221 0000 00da 0a73 706c 6974 6c69 6e65  r!.....splitline
-00001110: 73da 0d5f 4c69 6e65 5370 6c69 7474 6572  s.._LineSplitter
-00001120: da07 6861 7361 7474 72da 0470 7573 6872  ..hasattr..pushr
-00001130: 2500 0000 da05 666c 7573 6829 0572 1600  %.....flush).r..
-00001140: 0000 7246 0000 0072 4a00 0000 da08 7370  ..rF...rJ.....sp
-00001150: 6c69 7474 6572 da05 6368 756e 6b72 1a00  litter..chunkr..
-00001160: 0000 721a 0000 0072 1b00 0000 7247 0000  ..r....r....rG..
-00001170: 0082 0000 0073 2c00 0000 0280 0403 0a01  .....s,.........
-00001180: 0c03 1201 0801 0401 0603 0c01 1201 0e01  ................
-00001190: 0801 02ff 04ff 0c03 0a01 0e01 0801 02ff  ................
-000011a0: 02ff 1004 0e01 7a1d 506c 6169 6e54 6578  ......z.PlainTex
-000011b0: 7445 7865 6375 746f 7252 6573 756c 742e  tExecutorResult.
-000011c0: 6c69 6e65 734e a901 724b 0000 0029 1072  linesN..rK...).r
-000011d0: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-000011e0: 0000 0072 2800 0000 da0b 6461 7461 636c  ...r(.....datacl
-000011f0: 6173 7365 73da 0566 6965 6c64 7245 0000  asses..fieldrE..
-00001200: 0072 0200 0000 723e 0000 0072 2100 0000  .r....r>...r!...
-00001210: 7235 0000 0072 0700 0000 7220 0000 0072  r5...r....r ...r
-00001220: 0400 0000 7247 0000 0072 1a00 0000 721a  ....rG...r....r.
-00001230: 0000 0072 1a00 0000 721b 0000 0072 4100  ...r....r....rA.
-00001240: 0000 7500 0000 7316 0000 000a 0004 0204  ..u...s.........
-00001250: 0214 010e 0202 0704 ff06 0102 ff06 020e  ................
-00001260: fe72 4100 0000 6300 0000 0000 0000 0000  .rA...c.........
-00001270: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-00001280: 3800 0000 6500 5a01 6400 5a02 6401 6402  8...e.Z.d.Z.d.d.
-00001290: 8400 5a03 6403 6504 6404 6505 6506 1900  ..Z.d.e.d.e.e...
-000012a0: 6604 6405 6406 8404 5a07 6404 6506 6602  f.d.d...Z.d.e.f.
-000012b0: 6407 6408 8404 5a08 6409 5300 290a 7253  d.d...Z.d.S.).rS
-000012c0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000012d0: 0100 0000 0200 0000 4300 0000 730a 0000  ........C...s...
-000012e0: 0064 017c 005f 0064 0053 00a9 024e 7224  .d.|._.d.S...Nr$
-000012f0: 0000 00a9 01da 075f 6275 6666 6572 722d  ......._bufferr-
-00001300: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00001310: 0000 7215 0000 009e 0000 0073 0200 0000  ..r........s....
-00001320: 0a01 7a16 5f4c 696e 6553 706c 6974 7465  ..z._LineSplitte
-00001330: 722e 5f5f 696e 6974 5f5f 7258 0000 0072  r.__init__rX...r
-00001340: 2300 0000 6302 0000 0000 0000 0000 0000  #...c...........
-00001350: 0003 0000 0003 0000 0043 0000 0073 5000  .........C...sP.
-00001360: 0000 7c01 a000 6401 a101 6a01 6402 6403  ..|...d...j.d.d.
-00001370: 8d01 7d02 7c00 6a02 7215 7c00 6a02 7c02  ..}.|.j.r.|.j.|.
-00001380: 6404 1900 1700 7c02 6404 3c00 7c02 6405  d.....|.d.<.|.d.
-00001390: 1900 a003 6406 a101 7221 6407 7c00 5f02  ....d...r!d.|._.
-000013a0: 7c02 5300 7c02 a004 a100 7c00 5f02 7c02  |.S.|.....|._.|.
-000013b0: 5300 2908 4eda 0475 7466 3854 724c 0000  S.).N..utf8TrL..
-000013c0: 0072 0100 0000 e9ff ffff ffda 010a 7224  .r............r$
-000013d0: 0000 0029 05da 0664 6563 6f64 6572 5200  ...)...decoderR.
-000013e0: 0000 725e 0000 00da 0865 6e64 7377 6974  ..r^.....endswit
-000013f0: 68da 0370 6f70 2903 7216 0000 0072 5800  h..pop).r....rX.
-00001400: 0000 7247 0000 0072 1a00 0000 721a 0000  ..rG...r....r...
-00001410: 0072 1b00 0000 7255 0000 00a1 0000 0073  .r....rU.......s
-00001420: 1000 0000 1201 0601 1201 0e01 0601 0403  ................
-00001430: 0aff 0401 7a12 5f4c 696e 6553 706c 6974  ....z._LineSplit
-00001440: 7465 722e 7075 7368 6301 0000 0000 0000  ter.pushc.......
-00001450: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00001460: 0073 1000 0000 7c00 6a00 7d01 6401 7c00  .s....|.j.}.d.|.
-00001470: 5f00 7c01 5300 725c 0000 0072 5d00 0000  _.|.S.r\...r]...
-00001480: 2902 7216 0000 00da 0362 7566 721a 0000  ).r......bufr...
-00001490: 0072 1a00 0000 721b 0000 0072 5600 0000  .r....r....rV...
-000014a0: ab00 0000 7306 0000 0006 0106 0104 017a  ....s..........z
-000014b0: 135f 4c69 6e65 5370 6c69 7474 6572 2e66  ._LineSplitter.f
-000014c0: 6c75 7368 4e29 0972 1c00 0000 721d 0000  lushN).r....r...
-000014d0: 0072 1e00 0000 7215 0000 00da 0562 7974  .r....r......byt
-000014e0: 6573 da04 6c69 7374 7221 0000 0072 5500  es..listr!...rU.
-000014f0: 0000 7256 0000 0072 1a00 0000 721a 0000  ..rV...r....r...
-00001500: 0072 1a00 0000 721b 0000 0072 5300 0000  .r....r....rS...
-00001510: 9d00 0000 7308 0000 0008 0008 0116 0312  ....s...........
-00001520: 0a72 5300 0000 6300 0000 0000 0000 0000  .rS...c.........
-00001530: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-00001540: 3e00 0000 6500 5a01 6400 5a02 5500 6401  >...e.Z.d.Z.U.d.
-00001550: 5a03 6402 5a04 6505 6a06 6403 6404 8d01  Z.d.Z.e.j.d.d...
-00001560: 5a07 6508 6509 6405 3c00 640c 6407 650a  Z.e.e.d.<.d.d.e.
-00001570: 6408 650b 6604 6409 640a 8405 5a0c 640b  d.e.f.d.d...Z.d.
-00001580: 5300 290d da12 4a73 6f6e 4578 6563 7574  S.)...JsonExecut
-00001590: 6f72 5265 7375 6c74 7a1b 556e 6172 7920  orResultz.Unary 
-000015a0: 4a53 4f4e 2065 7865 6375 7469 6f6e 2072  JSON execution r
-000015b0: 6573 756c 74fa 1061 7070 6c69 6361 7469  esult..applicati
-000015c0: 6f6e 2f6a 736f 6e46 7243 0000 0072 3500  on/jsonFrC...r5.
-000015d0: 0000 724b 0000 0072 0e00 0000 7223 0000  ..rK...r....r#..
-000015e0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000015f0: 0000 0400 0000 4300 0000 731a 0000 007c  ......C...s....|
-00001600: 00a0 007c 017c 006a 01a1 0201 0074 02a0  ...|.|.j.....t..
-00001610: 037c 006a 01a1 0153 0072 3000 0000 2904  .|.j...S.r0...).
-00001620: 7237 0000 0072 3500 0000 da04 6a73 6f6e  r7...r5.....json
-00001630: da05 6c6f 6164 7329 0272 1600 0000 720e  ..loads).r....r.
-00001640: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00001650: 0000 da09 6a73 6f6e 5f64 6174 61b8 0000  ....json_data...
-00001660: 0073 0400 0000 0e01 0c01 7a1c 4a73 6f6e  .s........z.Json
-00001670: 4578 6563 7574 6f72 5265 7375 6c74 2e6a  ExecutorResult.j
-00001680: 736f 6e5f 6461 7461 4e72 5900 0000 290d  son_dataNrY...).
-00001690: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-000016a0: 1f00 0000 7228 0000 0072 5a00 0000 725b  ....r(...rZ...r[
-000016b0: 0000 0072 3500 0000 7221 0000 0072 3e00  ...r5...r!...r>.
-000016c0: 0000 7220 0000 0072 0200 0000 726c 0000  ..r ...r....rl..
-000016d0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-000016e0: 721b 0000 0072 6800 0000 b100 0000 730a  r....rh.......s.
-000016f0: 0000 000a 0004 0204 0214 0118 0272 6800  .............rh.
-00001700: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001710: 0000 0003 0000 0040 0000 0073 3c00 0000  .......@...s<...
-00001720: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-00001730: 5a04 6505 6a06 6403 6404 8d01 5a07 6508  Z.e.j.d.d...Z.e.
-00001740: 6509 6405 3c00 6406 650a 6508 1900 6602  e.d.<.d.e.e...f.
-00001750: 6407 6408 8404 5a0b 6409 5300 290a da15  d.d...Z.d.S.)...
-00001760: 4a73 6f6e 5365 7145 7865 6375 746f 7252  JsonSeqExecutorR
-00001770: 6573 756c 747a 1f53 7472 6561 6d69 6e67  esultz.Streaming
-00001780: 204a 534f 4e20 6578 6563 7574 696f 6e20   JSON execution 
-00001790: 7265 7375 6c74 7a14 6170 706c 6963 6174  resultz.applicat
-000017a0: 696f 6e2f 6a73 6f6e 2d73 6571 4672 4300  ion/json-seqFrC.
-000017b0: 0000 7245 0000 0072 2300 0000 6301 0000  ..rE...r#...c...
-000017c0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-000017d0: 0043 0200 0073 7200 0000 8102 7c00 a000  .C...sr.....|...
-000017e0: 6401 a101 0100 7401 7c00 6a02 6402 8302  d.....t.|.j.d...
-000017f0: 721e 7c00 6a02 3200 7a0b 3300 6400 4800  r.|.j.2.z.3.d.H.
-00001800: 5700 7d01 7403 7c01 8301 5600 0100 710f  W.}.t.|...V...q.
-00001810: 3600 6400 5300 7401 7c00 6a02 6403 8302  6.d.S.t.|.j.d...
-00001820: 7231 7c00 6a02 4400 5d07 7d01 7403 7c01  r1|.j.D.].}.t.|.
-00001830: 8301 5600 0100 7127 6400 5300 7404 6404  ..V...q'd.S.t.d.
-00001840: 7c00 6a02 9b00 9d02 8301 8201 2905 4e72  |.j.........).Nr
-00001850: 4b00 0000 724e 0000 0072 4f00 0000 7250  K...rN...rO...rP
-00001860: 0000 0029 0572 3700 0000 7254 0000 0072  ...).r7...rT...r
-00001870: 4500 0000 da0e 5f6a 736f 6e5f 7365 715f  E....._json_seq_
-00001880: 6974 656d 7225 0000 0029 0272 1600 0000  itemr%...).r....
-00001890: 724a 0000 0072 1a00 0000 721a 0000 0072  rJ...r....r....r
-000018a0: 1b00 0000 da0d 6a73 6f6e 5f73 6571 5f64  ......json_seq_d
-000018b0: 6174 61c4 0000 0073 1600 0000 0280 0a01  ata....s........
-000018c0: 0c01 1201 0c01 06ff 0c02 0a02 0c01 04ff  ................
-000018d0: 1003 7a23 4a73 6f6e 5365 7145 7865 6375  ..z#JsonSeqExecu
-000018e0: 746f 7252 6573 756c 742e 6a73 6f6e 5f73  torResult.json_s
-000018f0: 6571 5f64 6174 614e 290c 721c 0000 0072  eq_dataN).r....r
-00001900: 1d00 0000 721e 0000 0072 1f00 0000 7228  ....r....r....r(
-00001910: 0000 0072 5a00 0000 725b 0000 0072 4500  ...rZ...r[...rE.
-00001920: 0000 7202 0000 0072 3e00 0000 7204 0000  ..r....r>...r...
-00001930: 0072 6f00 0000 721a 0000 0072 1a00 0000  .ro...r....r....
-00001940: 721a 0000 0072 1b00 0000 726d 0000 00bd  r....r....rm....
-00001950: 0000 0073 0a00 0000 0a00 0402 0402 1401  ...s............
-00001960: 1602 726d 0000 00f3 0100 0000 1e72 4a00  ..rm.........rJ.
-00001970: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001980: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
-00001990: 7c00 a000 7401 a101 720b 7c00 6401 6400  |...t...r.|.d.d.
-000019a0: 8502 1900 6e01 7c00 7d01 7402 a003 7c01  ....n.|.}.t...|.
-000019b0: a101 5300 2902 4ee9 0100 0000 2904 da0a  ..S.).N.....)...
-000019c0: 7374 6172 7473 7769 7468 da10 5245 434f  startswith..RECO
-000019d0: 5244 5f53 4550 4152 4154 4f52 726a 0000  RD_SEPARATORrj..
-000019e0: 0072 6b00 0000 2902 724a 0000 0072 1000  .rk...).rJ...r..
-000019f0: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00001a00: 0072 6e00 0000 d400 0000 7304 0000 001a  .rn.......s.....
-00001a10: 020a 0172 6e00 0000 da16 4578 7065 6374  ...rn.....Expect
-00001a20: 6564 4578 6563 7574 6f72 5265 7375 6c74  edExecutorResult
-00001a30: 2901 da05 626f 756e 6463 0000 0000 0000  )...boundc......
-00001a40: 0000 0000 0000 0000 0000 0f00 0000 4000  ..............@.
-00001a50: 0000 73b6 0000 0065 005a 0164 005a 0209  ..s....e.Z.d.Z..
-00001a60: 0164 1864 0265 0364 0365 0364 0465 0465  .d.d.e.d.e.d.e.e
-00001a70: 0319 0066 0664 0564 0684 055a 0564 0765  ...f.d.d...Z.d.e
-00001a80: 0364 0865 0364 0965 0664 0a65 0465 0719  .d.e.d.e.d.e.e..
-00001a90: 0064 0b65 0865 0919 0066 0a64 0c64 0d84  .d.e.e...f.d.d..
-00001aa0: 045a 0a65 0b6a 0c09 0e09 0109 0164 1964  .Z.e.j.......d.d
-00001ab0: 0f65 0d65 0e19 0064 1065 0364 0865 0364  .e.e...d.e.d.e.d
-00001ac0: 0965 0465 0619 0064 1165 0465 0f19 0064  .e.e...d.e.e...d
-00001ad0: 0b65 1065 0e19 0066 0c64 1264 1384 0583  .e.e...f.d.d....
-00001ae0: 015a 1109 0164 1864 1465 0364 1565 0465  .Z...d.d.e.d.e.e
-00001af0: 1265 0365 0f66 0219 0019 0064 0b65 0f66  .e.e.f.....d.e.f
-00001b00: 0664 1664 1784 055a 1364 0153 0029 1ada  .d.d...Z.d.S.)..
-00001b10: 0845 7865 6375 746f 724e da07 7661 7269  .ExecutorN..vari
-00001b20: 616e 74da 0761 7069 5f75 726c da0d 6175  ant..api_url..au
-00001b30: 7468 6f72 697a 6174 696f 6e63 0400 0000  thorizationc....
-00001b40: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001b50: 4300 0000 7330 0000 007c 027c 005f 0074  C...s0...|.|._.t
-00001b60: 017c 0183 017c 005f 027c 0372 0f7c 037c  .|...|._.|.r.|.|
-00001b70: 006a 0264 013c 0074 03a0 0464 027c 017c  .j.d.<.t...d.|.|
-00001b80: 02a1 0301 0064 0053 0029 034e 7279 0000  .....d.S.).Nry..
-00001b90: 007a 2249 6e73 7461 6e74 6961 7465 6420  .z"Instantiated 
-00001ba0: 2573 2065 7865 6375 746f 722e 205b 7572  %s executor. [ur
-00001bb0: 6c3d 2573 5d29 05da 085f 6170 695f 7572  l=%s])..._api_ur
-00001bc0: 6cda 105f 6465 6661 756c 745f 6865 6164  l.._default_head
-00001bd0: 6572 73da 085f 6865 6164 6572 7372 2b00  ers.._headersr+.
-00001be0: 0000 722c 0000 0029 0472 1600 0000 7277  ..r,...).r....rw
-00001bf0: 0000 0072 7800 0000 7279 0000 0072 1a00  ...rx...ry...r..
-00001c00: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
-00001c10: 00e0 0000 0073 0a00 0000 0603 0a01 0401  .....s..........
-00001c20: 0a01 1201 7a11 4578 6563 7574 6f72 2e5f  ....z.Executor._
-00001c30: 5f69 6e69 745f 5fda 0375 726c da06 6d65  _init__..url..me
-00001c40: 7468 6f64 da07 6865 6164 6572 73da 0462  thod..headers..b
-00001c50: 6f64 7972 2300 0000 6305 0000 0000 0000  odyr#...c.......
-00001c60: 0000 0000 0005 0000 0001 0000 0043 0000  .............C..
-00001c70: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
-00001c80: 2905 7216 0000 0072 7d00 0000 727e 0000  ).r....r}...r~..
-00001c90: 0072 7f00 0000 7280 0000 0072 1a00 0000  .r....r....r....
-00001ca0: 721a 0000 0072 1b00 0000 da05 5f73 656e  r....r......_sen
-00001cb0: 64e9 0000 0073 0200 0000 0603 7a0e 4578  d....s......z.Ex
-00001cc0: 6563 7574 6f72 2e5f 7365 6e64 da03 4745  ecutor._send..GE
-00001cd0: 54da 0b72 6573 756c 745f 7479 7065 da04  T..result_type..
-00001ce0: 7061 7468 726c 0000 0063 0600 0000 0000  pathrl...c......
-00001cf0: 0000 0000 0000 0b00 0000 0900 0000 4302  ..............C.
-00001d00: 0000 732c 0100 0081 027c 006a 00a0 01a1  ..s,.....|.j....
-00001d10: 007d 067c 0472 0d7c 06a0 027c 04a1 0101  .}.|.r.|...|....
-00001d20: 007c 0174 036b 0272 1464 017d 076e 157c  .|.t.k.r.d.}.n.|
-00001d30: 0174 046b 0272 1b64 027d 076e 0e7c 0174  .t.k.r.d.}.n.|.t
-00001d40: 056b 0272 2264 037d 076e 0774 0664 047c  .k.r"d.}.n.t.d.|
-00001d50: 019b 009d 0283 0182 017c 077c 0664 053c  .........|.|.d.<
-00001d60: 007c 0572 3c64 067c 0664 073c 0074 07a0  .|.r<d.|.d.<.t..
-00001d70: 087c 05a1 01a0 0964 08a1 017d 086e 0264  .|.....d...}.n.d
-00001d80: 007d 0874 0aa0 0b64 097c 0872 4774 0c7c  .}.t...d.|.rGt.|
-00001d90: 0883 016e 0164 0aa1 0201 007c 006a 0d74  ...n.d.....|.j.t
-00001da0: 0e6a 0fa0 107c 006a 117c 02a1 027c 037c  .j...|.j.|...|.|
-00001db0: 067c 0864 0b8d 0434 0049 0064 0048 009a  .|.d...4.I.d.H..
-00001dc0: 2c7d 0974 127c 097c 0183 0273 7b74 127c  ,}.t.|.|...s{t.|
-00001dd0: 0074 0583 0272 707c 00a0 13a1 0049 0064  .t...rp|.....I.d
-00001de0: 0048 007d 0a6e 0264 007d 0a74 147c 096a  .H.}.n.d.}.t.|.j
-00001df0: 157c 096a 167c 0a64 0c8d 0382 017c 0956  .|.j.|.d.....|.V
-00001e00: 0001 0057 0064 0004 0004 0083 0349 0064  ...W.d.......I.d
-00001e10: 0048 0001 0064 0053 0031 0049 0064 0048  .H...d.S.1.I.d.H
-00001e20: 0073 8f77 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-00001e30: 0053 0029 0d4e 7a26 6170 706c 6963 6174  .S.).Nz&applicat
-00001e40: 696f 6e2f 6a73 6f6e 3b71 3d31 2c20 7465  ion/json;q=1, te
-00001e50: 7874 2f70 6c61 696e 3b71 3d30 2e31 7a2a  xt/plain;q=0.1z*
-00001e60: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00001e70: 2d73 6571 3b71 3d31 2c20 7465 7874 2f70  -seq;q=1, text/p
-00001e80: 6c61 696e 3b71 3d30 2e31 7242 0000 007a  lain;q=0.1rB...z
-00001e90: 1955 6e73 7570 706f 7274 6564 2072 6573  .Unsupported res
-00001ea0: 756c 7420 7479 7065 3a20 7233 0000 0072  ult type: r3...r
-00001eb0: 6900 0000 720c 0000 0072 5f00 0000 7a20  i...r....r_...z 
-00001ec0: 5365 6e64 696e 6720 4150 4920 7265 7175  Sending API requ
-00001ed0: 6573 742e 2e2e 205b 7369 7a65 3d25 735d  est... [size=%s]
-00001ee0: 7201 0000 0029 0472 7d00 0000 727e 0000  r....).r}...r~..
-00001ef0: 0072 7f00 0000 7280 0000 0072 3600 0000  .r....r....r6...
-00001f00: 2917 727c 0000 00da 0463 6f70 79da 0675  ).r|.....copy..u
-00001f10: 7064 6174 6572 6800 0000 726d 0000 0072  pdaterh...rm...r
-00001f20: 4100 0000 7225 0000 0072 6a00 0000 da05  A...r%...rj.....
-00001f30: 6475 6d70 73da 0665 6e63 6f64 6572 2b00  dumps..encoder+.
-00001f40: 0000 722c 0000 00da 036c 656e 7281 0000  ..r,.....lenr...
-00001f50: 00da 0675 726c 6c69 62da 0570 6172 7365  ...urllib..parse
-00001f60: da07 7572 6c6a 6f69 6e72 7a00 0000 7251  ..urljoinrz...rQ
-00001f70: 0000 0072 3500 0000 720d 0000 0072 0e00  ...r5...r....r..
-00001f80: 0000 720f 0000 0029 0b72 1600 0000 7283  ..r....).r....r.
-00001f90: 0000 0072 8400 0000 727e 0000 0072 7f00  ...r....r~...r..
-00001fa0: 0000 726c 0000 005a 0b61 6c6c 5f68 6561  ..rl...Z.all_hea
-00001fb0: 6465 7273 7233 0000 0072 8000 0000 da06  dersr3...r......
-00001fc0: 7265 7375 6c74 7235 0000 0072 1a00 0000  resultr5...r....
-00001fd0: 721a 0000 0072 1b00 0000 da07 6578 6563  r....r......exec
-00001fe0: 7574 65ee 0000 0073 4600 0000 0280 0a09  ute....sF.......
-00001ff0: 0401 0a01 0802 0601 0801 0601 0801 0601  ................
-00002000: 0e02 0801 0402 0801 1201 0402 0402 1001  ................
-00002010: 04ff 0403 0e01 0201 0201 0201 0efc 0205  ................
-00002020: 0a01 0a01 1001 0402 0201 0a01 06ff 0803  ................
-00002030: 2ef2 7a10 4578 6563 7574 6f72 2e65 7865  ..z.Executor.exe
-00002040: 6375 7465 da05 7175 6572 79da 0976 6172  cute..query..var
-00002050: 6961 626c 6573 6303 0000 0000 0000 0000  iablesc.........
-00002060: 0000 0005 0000 0009 0000 00c3 0000 0073  ...............s
-00002070: 7e00 0000 8101 7c00 6a00 7401 6401 6402  ~.....|.j.t.d.d.
-00002080: 7c01 7c02 700a 6900 6403 9c02 6404 8d04  |.|.p.i.d...d...
-00002090: 3400 4900 6400 4800 9a0f 7d03 7c03 a002  4.I.d.H...}.|...
-000020a0: a100 7d04 5700 6400 0400 0400 8303 4900  ..}.W.d.......I.
-000020b0: 6400 4800 0100 6e0b 3100 4900 6400 4800  d.H...n.1.I.d.H.
-000020c0: 7328 7701 0100 0100 0100 5900 0100 7c04  s(w.......Y...|.
-000020d0: a003 6405 a101 723b 7404 7c03 6a05 7c03  ..d...r;t.|.j.|.
-000020e0: 6a06 7c04 6406 8d03 8201 7c04 6407 1900  j.|.d.....|.d...
-000020f0: 5300 2908 4e7a 082f 6772 6170 6871 6cda  S.).Nz./graphql.
-00002100: 0450 4f53 5429 0272 8f00 0000 7290 0000  .POST).r....r...
-00002110: 0029 0472 8300 0000 7284 0000 0072 7e00  .).r....r....r~.
-00002120: 0000 726c 0000 00da 0665 7272 6f72 7372  ..rl.....errorsr
-00002130: 3600 0000 7210 0000 0029 0772 8e00 0000  6...r....).r....
-00002140: 7268 0000 0072 6c00 0000 da03 6765 7472  rh...rl.....getr
-00002150: 0d00 0000 720e 0000 0072 0f00 0000 2905  ....r....r....).
-00002160: 7216 0000 0072 8f00 0000 7290 0000 0072  r....r....r....r
-00002170: 8d00 0000 7210 0000 0072 1a00 0000 721a  ....r....r....r.
-00002180: 0000 0072 1b00 0000 da15 6578 6563 7574  ...r......execut
-00002190: 655f 6772 6170 6871 6c5f 7175 6572 791e  e_graphql_query.
-000021a0: 0100 0073 1a00 0000 0280 0405 0201 0201  ...s............
-000021b0: 0201 0c01 0efc 0205 0a01 28fa 0a07 1201  ..........(.....
-000021c0: 0801 7a1e 4578 6563 7574 6f72 2e65 7865  ..z.Executor.exe
-000021d0: 6375 7465 5f67 7261 7068 716c 5f71 7565  cute_graphql_que
-000021e0: 7279 7230 0000 0029 0372 8200 0000 4e4e  ryr0...).r....NN
-000021f0: 2914 721c 0000 0072 1d00 0000 721e 0000  ).r....r....r...
-00002200: 0072 2100 0000 7207 0000 0072 1500 0000  .r!...r....r....
-00002210: da07 4865 6164 6572 7372 6600 0000 7203  ..Headersrf...r.
-00002220: 0000 0072 2a00 0000 7281 0000 00da 0a63  ...r*...r......c
-00002230: 6f6e 7465 7874 6c69 62da 1361 7379 6e63  ontextlib..async
-00002240: 636f 6e74 6578 746d 616e 6167 6572 7205  contextmanagerr.
-00002250: 0000 0072 7400 0000 7202 0000 0072 0400  ...rt...r....r..
-00002260: 0000 728e 0000 0072 0600 0000 7294 0000  ..r....r....r...
-00002270: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00002280: 721b 0000 0072 7600 0000 df00 0000 735a  r....rv.......sZ
-00002290: 0000 0008 0002 0204 ff02 0102 ff02 0102  ................
-000022a0: ff06 010a ff02 0902 0102 ff02 0102 ff02  ................
-000022b0: 0102 ff06 0102 ff06 020a fe04 0502 0502  ................
-000022c0: 0102 0104 fa06 0202 fe02 0302 fd02 0402  ................
-000022d0: fc06 0502 fb06 0602 fa06 070c f902 3204  ..............2.
-000022e0: fd02 0202 fe0e 0302 fd02 040e fc72 7600  .............rv.
-000022f0: 0000 da06 636c 6965 6e74 6301 0000 0000  ....clientc.....
-00002300: 0000 0000 0000 0001 0000 0006 0000 0043  ...............C
-00002310: 0000 0073 1600 0000 6401 6402 7400 9b00  ...s....d.d.t...
-00002320: 6403 7c00 9b00 6404 9d05 6901 5300 2905  d.|...d...i.S.).
-00002330: 4e7a 0e6f 7076 696f 7573 2d63 6c69 656e  Nz.opvious-clien
-00002340: 747a 0c50 7974 686f 6e20 5344 4b20 7672  tz.Python SDK vr
-00002350: 1100 0000 7212 0000 0072 0a00 0000 2901  ....r....r....).
-00002360: 7298 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00002370: 1b00 0000 727b 0000 002f 0100 0073 0400  ....r{.../...s..
-00002380: 0000 1202 04ff 727b 0000 0072 3000 0000  ......r{...r0...
-00002390: 2929 721f 0000 0072 9600 0000 725a 0000  ))r....r....rZ..
-000023a0: 0072 6a00 0000 da07 6c6f 6767 696e 67da  .rj.....logging.
-000023b0: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-000023c0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-000023d0: 7207 0000 0072 0800 0000 da0c 7572 6c6c  r....r......urll
-000023e0: 6962 2e70 6172 7365 728a 0000 00da 0663  ib.parser......c
-000023f0: 6f6d 6d6f 6e72 0b00 0000 da09 6765 744c  ommonr......getL
-00002400: 6f67 6765 7272 1c00 0000 722b 0000 005a  oggerr....r+...Z
-00002410: 0c54 5241 4345 5f48 4541 4445 525a 1343  .TRACE_HEADERZ.C
-00002420: 4f4e 5445 4e54 5f54 5950 455f 4845 4144  ONTENT_TYPE_HEAD
-00002430: 4552 da04 6469 6374 7221 0000 0072 9500  ER..dictr!...r..
-00002440: 0000 7225 0000 0072 0d00 0000 7227 0000  ..r%...r....r'..
-00002450: 0072 2900 0000 da09 6461 7461 636c 6173  .r).....dataclas
-00002460: 7372 2a00 0000 7241 0000 0072 5300 0000  sr*...rA...rS...
-00002470: 7268 0000 0072 6d00 0000 7273 0000 0072  rh...rm...rs...r
-00002480: 6600 0000 726e 0000 0072 7400 0000 7276  f...rn...rt...rv
-00002490: 0000 0072 7b00 0000 721a 0000 0072 1a00  ...r{...r....r..
-000024a0: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
-000024b0: 6f64 756c 653e 0100 0000 735a 0000 0004  odule>....sZ....
-000024c0: 0008 1308 0108 0108 0124 0108 090c 020a  .........$......
-000024d0: 0304 0304 030c 0310 0302 1504 ff02 0102  ................
-000024e0: ff06 0102 ff02 020a fe02 0b04 ff06 0102  ................
-000024f0: ff06 0102 ff02 020a fe04 0910 0104 1b12  ................
-00002500: 010e 2704 1412 0104 0b12 0104 1312 0302  ..'.............
-00002510: 0604 0106 ff0e 0516 50                   ........P
+00000090: a101 5a13 6406 5a14 6407 5a15 6408 5a16  ..Z.d.Z.d.Z.d.Z.
+000000a0: 6517 6518 6518 6602 1900 5a19 4700 6409  e.e.e.f...Z.G.d.
+000000b0: 640a 8400 640a 651a 8303 5a1b 0902 6428  d...d.e...Z...d(
+000000c0: 640b 6518 640c 650b 6518 1900 640d 651a  d.e.d.e.e...d.e.
+000000d0: 6606 640e 640f 8405 5a1c 0902 6428 6410  f.d.d...Z...d(d.
+000000e0: 650b 6518 1900 640c 650b 6518 1900 640d  e.e...d.e.e...d.
+000000f0: 651a 6606 6411 6412 8405 5a1d 6502 6a1e  e.f.d.d...Z.e.j.
+00000100: 4700 6413 6414 8400 6414 8302 8301 5a1f  G.d.d...d.....Z.
+00000110: 6502 6a1e 4700 6415 6416 8400 6416 651f  e.j.G.d.d...d.e.
+00000120: 8303 8301 5a20 4700 6417 6418 8400 6418  ....Z G.d.d...d.
+00000130: 8302 5a21 6502 6a1e 4700 6419 641a 8400  ..Z!e.j.G.d.d...
+00000140: 641a 651f 8303 8301 5a22 6502 6a1e 4700  d.e.....Z"e.j.G.
+00000150: 641b 641c 8400 641c 651f 8303 8301 5a23  d.d...d.e.....Z#
+00000160: 641d 5a24 641e 6525 640d 6506 6604 641f  d.Z$d.e%d.e.f.d.
+00000170: 6420 8404 5a26 650c 6421 651f 6422 8d02  d ..Z&e.d!e.d"..
+00000180: 5a27 4700 6423 6424 8400 6424 8302 5a28  Z'G.d#d$..d$..Z(
+00000190: 6425 6518 640d 6519 6604 6426 6427 8404  d%e.d.e.f.d&d'..
+000001a0: 5a29 6402 5300 2929 6100 0300 000a 4c69  Z)d.S.))a.....Li
+000001b0: 6365 6e73 6564 2074 6f20 7468 6520 4170  censed to the Ap
+000001c0: 6163 6865 2053 6f66 7477 6172 6520 466f  ache Software Fo
+000001d0: 756e 6461 7469 6f6e 2028 4153 4629 2075  undation (ASF) u
+000001e0: 6e64 6572 206f 6e65 0a6f 7220 6d6f 7265  nder one.or more
+000001f0: 2063 6f6e 7472 6962 7574 6f72 206c 6963   contributor lic
+00000200: 656e 7365 2061 6772 6565 6d65 6e74 732e  ense agreements.
+00000210: 2020 5365 6520 7468 6520 4e4f 5449 4345    See the NOTICE
+00000220: 2066 696c 650a 6469 7374 7269 6275 7465   file.distribute
+00000230: 6420 7769 7468 2074 6869 7320 776f 726b  d with this work
+00000240: 2066 6f72 2061 6464 6974 696f 6e61 6c20   for additional 
+00000250: 696e 666f 726d 6174 696f 6e0a 7265 6761  information.rega
+00000260: 7264 696e 6720 636f 7079 7269 6768 7420  rding copyright 
+00000270: 6f77 6e65 7273 6869 702e 2020 5468 6520  ownership.  The 
+00000280: 4153 4620 6c69 6365 6e73 6573 2074 6869  ASF licenses thi
+00000290: 7320 6669 6c65 0a74 6f20 796f 7520 756e  s file.to you un
+000002a0: 6465 7220 7468 6520 4170 6163 6865 204c  der the Apache L
+000002b0: 6963 656e 7365 2c20 5665 7273 696f 6e20  icense, Version 
+000002c0: 322e 3020 2874 6865 0a22 4c69 6365 6e73  2.0 (the."Licens
+000002d0: 6522 293b 2079 6f75 206d 6179 206e 6f74  e"); you may not
+000002e0: 2075 7365 2074 6869 7320 6669 6c65 2065   use this file e
+000002f0: 7863 6570 7420 696e 2063 6f6d 706c 6961  xcept in complia
+00000300: 6e63 650a 7769 7468 2074 6865 204c 6963  nce.with the Lic
+00000310: 656e 7365 2e20 2059 6f75 206d 6179 206f  ense.  You may o
+00000320: 6274 6169 6e20 6120 636f 7079 206f 6620  btain a copy of 
+00000330: 7468 6520 4c69 6365 6e73 6520 6174 0a0a  the License at..
+00000340: 2020 6874 7470 3a2f 2f77 7777 2e61 7061    http://www.apa
+00000350: 6368 652e 6f72 672f 6c69 6365 6e73 6573  che.org/licenses
+00000360: 2f4c 4943 454e 5345 2d32 2e30 0a0a 2020  /LICENSE-2.0..  
+00000370: 556e 6c65 7373 2072 6571 7569 7265 6420  Unless required 
+00000380: 6279 2061 7070 6c69 6361 626c 6520 6c61  by applicable la
+00000390: 7720 6f72 2061 6772 6565 6420 746f 2069  w or agreed to i
+000003a0: 6e20 7772 6974 696e 672c 0a20 2073 6f66  n writing,.  sof
+000003b0: 7477 6172 6520 6469 7374 7269 6275 7465  tware distribute
+000003c0: 6420 756e 6465 7220 7468 6520 4c69 6365  d under the Lice
+000003d0: 6e73 6520 6973 2064 6973 7472 6962 7574  nse is distribut
+000003e0: 6564 206f 6e20 616e 0a20 2022 4153 2049  ed on an.  "AS I
+000003f0: 5322 2042 4153 4953 2c20 5749 5448 4f55  S" BASIS, WITHOU
+00000400: 5420 5741 5252 414e 5449 4553 204f 5220  T WARRANTIES OR 
+00000410: 434f 4e44 4954 494f 4e53 204f 4620 414e  CONDITIONS OF AN
+00000420: 590a 2020 4b49 4e44 2c20 6569 7468 6572  Y.  KIND, either
+00000430: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
+00000440: 6965 642e 2020 5365 6520 7468 6520 4c69  ied.  See the Li
+00000450: 6365 6e73 6520 666f 7220 7468 650a 2020  cense for the.  
+00000460: 7370 6563 6966 6963 206c 616e 6775 6167  specific languag
+00000470: 6520 676f 7665 726e 696e 6720 7065 726d  e governing perm
+00000480: 6973 7369 6f6e 7320 616e 6420 6c69 6d69  issions and limi
+00000490: 7461 7469 6f6e 730a 2020 756e 6465 7220  tations.  under 
+000004a0: 7468 6520 4c69 6365 6e73 652e 0ae9 0000  the License.....
+000004b0: 0000 4e29 07da 0341 6e79 da13 4173 796e  ..N)...Any..Asyn
+000004c0: 6343 6f6e 7465 7874 4d61 6e61 6765 72da  cContextManager.
+000004d0: 0d41 7379 6e63 4974 6572 6174 6f72 da04  .AsyncIterator..
+000004e0: 5479 7065 da07 4d61 7070 696e 67da 084f  Type..Mapping..O
+000004f0: 7074 696f 6e61 6cda 0754 7970 6556 6172  ptional..TypeVar
+00000500: e902 0000 00a9 01da 0b5f 5f76 6572 7369  .........__versi
+00000510: 6f6e 5f5f 7a0d 6f70 7669 6f75 732d 7472  on__z.opvious-tr
+00000520: 6163 65da 0d61 7574 686f 7269 7a61 7469  ace..authorizati
+00000530: 6f6e fa0c 636f 6e74 656e 742d 7479 7065  on..content-type
+00000540: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000550: 0008 0000 0000 0000 0073 3c00 0000 6500  .........s<...e.
+00000560: 5a01 6400 5a02 6401 5a03 0902 0902 6408  Z.d.Z.d.Z.....d.
+00000570: 6403 6504 6404 6505 6506 1900 6405 6505  d.e.d.e.e...d.e.
+00000580: 6507 1900 6606 8700 6601 6406 6407 840d  e...f...f.d.d...
+00000590: 5a08 8700 0400 5a09 5300 2909 da08 4170  Z.....Z.S.)...Ap
+000005a0: 6945 7272 6f72 7a34 4c6f 6361 6c20 7265  iErrorz4Local re
+000005b0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+000005c0: 616e 2065 7272 6f72 2072 6574 7572 6e65  an error returne
+000005d0: 6420 6279 2074 6865 2041 5049 4eda 0673  d by the APIN..s
+000005e0: 7461 7475 73da 0574 7261 6365 da04 6461  tatus..trace..da
+000005f0: 7461 6304 0000 0000 0000 0000 0000 0005  tac.............
+00000600: 0000 0004 0000 0003 0000 0073 5200 0000  ...........sR...
+00000610: 6401 7c01 9b00 9d02 7d04 7c02 720f 7c04  d.|.....}.|.r.|.
+00000620: 6402 7c02 9b00 6403 9d03 3700 7d04 7c03  d.|...d...7.}.|.
+00000630: 7218 7c04 6404 7c03 9b00 9d02 3700 7d04  r.|.d.|.....7.}.
+00000640: 7400 8300 a001 7c04 a101 0100 7c01 7c00  t.....|.....|.|.
+00000650: 5f02 7c02 7c00 5f03 7c03 7c00 5f04 6400  _.|.|._.|.|._.d.
+00000660: 5300 2905 4e7a 1c41 5049 2063 616c 6c20  S.).Nz.API call 
+00000670: 6661 696c 6564 2077 6974 6820 7374 6174  failed with stat
+00000680: 7573 20fa 0220 28fa 0129 fa02 3a20 2905  us .. (..)..: ).
+00000690: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
+000006a0: 5f72 0f00 0000 7210 0000 0072 1100 0000  _r....r....r....
+000006b0: 2905 da04 7365 6c66 720f 0000 0072 1000  )...selfr....r..
+000006c0: 0000 7211 0000 00da 076d 6573 7361 6765  ..r......message
+000006d0: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
+000006e0: 3b2f 686f 6d65 2f72 756e 6e65 722f 776f  ;/home/runner/wo
+000006f0: 726b 2f73 646b 2e70 792f 7364 6b2e 7079  rk/sdk.py/sdk.py
+00000700: 2f6f 7076 696f 7573 2f65 7865 6375 746f  /opvious/executo
+00000710: 7273 2f63 6f6d 6d6f 6e2e 7079 7216 0000  rs/common.pyr...
+00000720: 0038 0000 0073 1200 0000 0a06 0401 1001  .8...s..........
+00000730: 0401 0e01 0c01 0601 0601 0a01 7a11 4170  ............z.Ap
+00000740: 6945 7272 6f72 2e5f 5f69 6e69 745f 5f29  iError.__init__)
+00000750: 024e 4e29 0ada 085f 5f6e 616d 655f 5fda  .NN)...__name__.
+00000760: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000770: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+00000780: 5f5f da03 696e 7472 0700 0000 da03 7374  __..intr......st
+00000790: 7272 0200 0000 7216 0000 00da 0d5f 5f63  rr....r......__c
+000007a0: 6c61 7373 6365 6c6c 5f5f 721b 0000 0072  lasscell__r....r
+000007b0: 1b00 0000 7219 0000 0072 1c00 0000 720e  ....r....r....r.
+000007c0: 0000 0035 0000 0073 1600 0000 0800 0401  ...5...s........
+000007d0: 0205 0201 04fc 0202 02fe 0603 02fd 0604  ................
+000007e0: 16fc 720e 0000 0072 1800 0000 7210 0000  ..r....r....r...
+000007f0: 00da 0672 6574 7572 6e63 0200 0000 0000  ...returnc......
+00000800: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00000810: 0000 7332 0000 0074 0064 017c 0172 0a64  ..s2...t.d.|.r.d
+00000820: 027c 019b 0064 039d 036e 0164 0417 007c  .|...d...n.d...|
+00000830: 0072 1564 057c 009b 009d 0217 0083 0153  .r.d.|.........S
+00000840: 0064 0417 0083 0153 0029 064e 7a13 556e  .d.....S.).Nz.Un
+00000850: 6578 7065 6374 6564 2072 6573 706f 6e73  expected respons
+00000860: 6572 1200 0000 7213 0000 00da 0072 1400  er....r......r..
+00000870: 0000 2901 da09 4578 6365 7074 696f 6ea9  ..)...Exception.
+00000880: 0272 1800 0000 7210 0000 0072 1b00 0000  .r....r....r....
+00000890: 721b 0000 0072 1c00 0000 da19 756e 6578  r....r......unex
+000008a0: 7065 6374 6564 5f72 6573 706f 6e73 655f  pected_response_
+000008b0: 6572 726f 7249 0000 0073 1400 0000 0203  errorI...s......
+000008c0: 0201 1201 02ff 0c02 02fe 04ff 0203 02fe  ................
+000008d0: 04ff 7228 0000 00da 0c63 6f6e 7465 6e74  ..r(.....content
+000008e0: 5f74 7970 6563 0200 0000 0000 0000 0000  _typec..........
+000008f0: 0000 0200 0000 0400 0000 4300 0000 7312  ..........C...s.
+00000900: 0000 0074 0064 017c 009b 009d 027c 0164  ...t.d.|.....|.d
+00000910: 028d 0253 0029 034e 7a1a 756e 7375 7070  ...S.).Nz.unsupp
+00000920: 6f72 7465 6420 636f 6e74 656e 742d 7479  orted content-ty
+00000930: 7065 3a20 7227 0000 0029 0172 2800 0000  pe: r'...).r(...
+00000940: 2902 7229 0000 0072 1000 0000 721b 0000  ).r)...r....r...
+00000950: 0072 1b00 0000 721c 0000 00da 1e75 6e73  .r....r......uns
+00000960: 7570 706f 7274 6564 5f63 6f6e 7465 6e74  upported_content
+00000970: 5f74 7970 655f 6572 726f 7253 0000 0073  _type_errorS...s
+00000980: 0800 0000 0203 0801 0201 06fe 722a 0000  ............r*..
+00000990: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000009a0: 0000 0700 0000 4000 0000 7384 0000 0065  ......@...s....e
+000009b0: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
+000009c0: 0065 0565 0619 0065 0464 023c 0064 0364  .e.e...e.d.<.d.d
+000009d0: 0484 005a 0765 0864 0565 0666 0264 0664  ...Z.e.d.e.f.d.d
+000009e0: 0784 0483 015a 0965 0864 0565 0666 0264  .....Z.e.d.e.f.d
+000009f0: 0864 0984 0483 015a 0a64 1164 0165 0364  .d.....Z.d.d.e.d
+00000a00: 0b65 0565 0619 0064 0564 0a66 0664 0c64  .e.e...d.d.f.d.d
+00000a10: 0d84 055a 0b65 0c64 0e65 0565 0619 0064  ...Z.e.d.e.e...d
+00000a20: 0565 0d66 0464 0f64 1084 0483 015a 0e64  .e.f.d.d.....Z.d
+00000a30: 0a53 0029 12da 0e45 7865 6375 746f 7252  .S.)...ExecutorR
+00000a40: 6573 756c 7472 0f00 0000 7210 0000 0063  esultr....r....c
+00000a50: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000a60: 0500 0000 4300 0000 7316 0000 0074 00a0  ....C...s....t..
+00000a70: 0164 017c 006a 027c 006a 03a1 0301 0064  .d.|.j.|.j.....d
+00000a80: 0053 0029 024e 7a27 476f 7420 4150 4920  .S.).Nz'Got API 
+00000a90: 7265 7370 6f6e 7365 2e20 5b73 7461 7475  response. [statu
+00000aa0: 733d 2573 2c20 7472 6163 653d 2573 5d29  s=%s, trace=%s])
+00000ab0: 04da 075f 6c6f 6767 6572 da05 6465 6275  ..._logger..debu
+00000ac0: 6772 0f00 0000 7210 0000 00a9 0172 1700  gr....r......r..
+00000ad0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000ae0: 00da 0d5f 5f70 6f73 745f 696e 6974 5f5f  ...__post_init__
+00000af0: 6100 0000 7306 0000 0004 010a 0108 ff7a  a...s..........z
+00000b00: 1c45 7865 6375 746f 7252 6573 756c 742e  .ExecutorResult.
+00000b10: 5f5f 706f 7374 5f69 6e69 745f 5f72 2400  __post_init__r$.
+00000b20: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000b30: 0000 0001 0000 0043 0000 00f3 0600 0000  .......C........
+00000b40: 7400 8300 8201 a901 4ea9 01da 134e 6f74  t.......N....Not
+00000b50: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00000b60: 722e 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00000b70: 1c00 0000 da06 6163 6365 7074 6600 0000  ......acceptf...
+00000b80: f302 0000 0006 027a 1545 7865 6375 746f  .......z.Executo
+00000b90: 7252 6573 756c 742e 6163 6365 7074 6301  rResult.acceptc.
+00000ba0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000bb0: 0000 0043 0000 0072 3000 0000 7231 0000  ...C...r0...r1..
+00000bc0: 0072 3200 0000 722e 0000 0072 1b00 0000  .r2...r....r....
+00000bd0: 721b 0000 0072 1c00 0000 7229 0000 006a  r....r....r)...j
+00000be0: 0000 0072 3500 0000 7a1b 4578 6563 7574  ...r5...z.Execut
+00000bf0: 6f72 5265 7375 6c74 2e63 6f6e 7465 6e74  orResult.content
+00000c00: 5f74 7970 654e da04 7465 7874 6303 0000  _typeN..textc...
+00000c10: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000c20: 0043 0000 0073 2000 0000 7c00 6a00 7c01  .C...s ...|.j.|.
+00000c30: 6b02 7207 6400 5300 7401 7c00 6a00 7c00  k.r.d.S.t.|.j.|.
+00000c40: 6a02 7c02 6401 8d03 8201 2902 4ea9 0372  j.|.d.....).N..r
+00000c50: 0f00 0000 7210 0000 0072 1100 0000 2903  ....r....r....).
+00000c60: 720f 0000 0072 0e00 0000 7210 0000 0029  r....r....r....)
+00000c70: 0372 1700 0000 720f 0000 0072 3600 0000  .r....r....r6...
+00000c80: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00000c90: 0e5f 6173 7365 7274 5f73 7461 7475 736e  ._assert_statusn
+00000ca0: 0000 0073 0600 0000 0a01 0401 1201 7a1d  ...s..........z.
+00000cb0: 4578 6563 7574 6f72 5265 7375 6c74 2e5f  ExecutorResult._
+00000cc0: 6173 7365 7274 5f73 7461 7475 73da 0563  assert_status..c
+00000cd0: 7479 7065 6302 0000 0000 0000 0000 0000  typec...........
+00000ce0: 0002 0000 0004 0000 0043 0000 0073 1c00  .........C...s..
+00000cf0: 0000 7400 7c01 6f0c 7c01 a001 6401 a101  ..t.|.o.|...d...
+00000d00: 6402 1900 7c00 6a02 6b02 8301 5300 2903  d...|.j.k...S.).
+00000d10: 4efa 013b 7201 0000 0029 03da 0462 6f6f  N..;r....)...boo
+00000d20: 6cda 0573 706c 6974 7229 0000 0029 02da  l..splitr)...)..
+00000d30: 0363 6c73 7239 0000 0072 1b00 0000 721b  .clsr9...r....r.
+00000d40: 0000 0072 1c00 0000 da0b 6973 5f65 6c69  ...r......is_eli
+00000d50: 6769 626c 6573 0000 0073 0200 0000 1c02  gibles...s......
+00000d60: 7a1a 4578 6563 7574 6f72 5265 7375 6c74  z.ExecutorResult
+00000d70: 2e69 735f 656c 6967 6962 6c65 7231 0000  .is_eligibler1..
+00000d80: 0029 0f72 1d00 0000 721e 0000 0072 1f00  .).r....r....r..
+00000d90: 0000 7221 0000 00da 0f5f 5f61 6e6e 6f74  ..r!.....__annot
+00000da0: 6174 696f 6e73 5f5f 7207 0000 0072 2200  ations__r....r".
+00000db0: 0000 722f 0000 00da 0870 726f 7065 7274  ..r/.....propert
+00000dc0: 7972 3400 0000 7229 0000 0072 3800 0000  yr4...r)...r8...
+00000dd0: da0b 636c 6173 736d 6574 686f 6472 3b00  ..classmethodr;.
+00000de0: 0000 723e 0000 0072 1b00 0000 721b 0000  ..r>...r....r...
+00000df0: 0072 1b00 0000 721c 0000 0072 2b00 0000  .r....r....r+...
+00000e00: 5c00 0000 7316 0000 000a 0008 020c 0108  \...s...........
+00000e10: 0202 0510 0102 0310 011c 0302 051c 0172  ...............r
+00000e20: 2b00 0000 6300 0000 0000 0000 0000 0000  +...c...........
+00000e30: 0000 0000 0006 0000 0040 0000 0073 5600  .........@...sV.
+00000e40: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000e50: 6402 5a04 6505 6a06 6403 6404 8d01 5a07  d.Z.e.j.d.d...Z.
+00000e60: 6508 6509 6405 3c00 6406 650a 6602 6407  e.e.d.<.d.e.f.d.
+00000e70: 6408 8404 5a0b 0909 640e 640a 650c 650d  d...Z...d.d.e.e.
+00000e80: 1900 6406 650e 650a 1900 6604 640b 640c  ..d.e.e...f.d.d.
+00000e90: 8405 5a0f 640d 5300 290f da17 506c 6169  ..Z.d.S.)...Plai
+00000ea0: 6e54 6578 7445 7865 6375 746f 7252 6573  nTextExecutorRes
+00000eb0: 756c 747a 1b50 6c61 696e 2074 6578 7420  ultz.Plain text 
+00000ec0: 6578 6563 7574 696f 6e20 7265 7375 6c74  execution result
+00000ed0: fa0a 7465 7874 2f70 6c61 696e 46a9 01da  ..text/plainF...
+00000ee0: 0472 6570 72da 0672 6561 6465 7272 2400  .repr..readerr$.
+00000ef0: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+00000f00: 0000 0007 0000 00c3 0000 0073 3600 0000  ...........s6...
+00000f10: 8101 6700 7d01 7c00 6a00 6400 6401 8d01  ..g.}.|.j.d.d...
+00000f20: 3200 7a0b 3300 6400 4800 5700 7d02 7c01  2.z.3.d.H.W.}.|.
+00000f30: a001 7c02 a101 0100 7109 3600 6402 a002  ..|.....q.6.d...
+00000f40: 7c01 a101 5300 2903 4e29 01da 0d61 7373  |...S.).N)...ass
+00000f50: 6572 745f 7374 6174 7573 7225 0000 0029  ert_statusr%...)
+00000f60: 03da 056c 696e 6573 da06 6170 7065 6e64  ...lines..append
+00000f70: da04 6a6f 696e 2903 7217 0000 0072 4800  ..join).r....rH.
+00000f80: 0000 da04 6c69 6e65 721b 0000 0072 1b00  ....liner....r..
+00000f90: 0000 721c 0000 0072 3600 0000 7f00 0000  ..r....r6.......
+00000fa0: 730c 0000 0002 8004 0118 010c 0102 ff0a  s...............
+00000fb0: 027a 1c50 6c61 696e 5465 7874 4578 6563  .z.PlainTextExec
+00000fc0: 7574 6f72 5265 7375 6c74 2e74 6578 74e9  utorResult.text.
+00000fd0: c800 0000 7247 0000 0063 0200 0000 0000  ....rG...c......
+00000fe0: 0000 0000 0000 0500 0000 0700 0000 4302  ..............C.
+00000ff0: 0000 73c8 0000 0081 027c 0172 087c 00a0  ..s......|.r.|..
+00001000: 007c 01a1 0101 0074 017c 006a 0274 0383  .|.....t.|.j.t..
+00001010: 0272 1d7c 006a 026a 0464 0164 028d 0144  .r.|.j.j.d.d...D
+00001020: 005d 057d 027c 0256 0001 0071 1564 0053  .].}.|.V...q.d.S
+00001030: 0074 0583 007d 0374 067c 006a 0264 0383  .t...}.t.|.j.d..
+00001040: 0272 3d7c 006a 0232 007a 1133 0064 0048  .r=|.j.2.z.3.d.H
+00001050: 0057 007d 047c 03a0 077c 04a1 0144 005d  .W.}.|...|...D.]
+00001060: 057d 027c 0256 0001 0071 3471 2936 006e  .}.|.V...q4q)6.n
+00001070: 2074 067c 006a 0264 0483 0272 557c 006a   t.|.j.d...rU|.j
+00001080: 0244 005d 0d7d 047c 03a0 077c 04a1 0144  .D.].}.|...|...D
+00001090: 005d 057d 027c 0256 0001 0071 4d71 466e  .].}.|.V...qMqFn
+000010a0: 0874 0864 057c 006a 029b 009d 0283 0182  .t.d.|.j........
+000010b0: 017c 03a0 09a1 0056 0001 0064 0053 0029  .|.....V...d.S.)
+000010c0: 064e 54a9 01da 086b 6565 7065 6e64 73da  .NT....keepends.
+000010d0: 095f 5f61 6974 6572 5f5f da08 5f5f 6974  .__aiter__..__it
+000010e0: 6572 5f5f fa15 4e6f 6e2d 6974 6572 6162  er__..Non-iterab
+000010f0: 6c65 2072 6561 6465 723a 2029 0a72 3800  le reader: ).r8.
+00001100: 0000 da0a 6973 696e 7374 616e 6365 7246  ....isinstancerF
+00001110: 0000 0072 2200 0000 da0a 7370 6c69 746c  ...r".....splitl
+00001120: 696e 6573 da0d 5f4c 696e 6553 706c 6974  ines.._LineSplit
+00001130: 7465 72da 0768 6173 6174 7472 da04 7075  ter..hasattr..pu
+00001140: 7368 7226 0000 00da 0566 6c75 7368 2905  shr&.....flush).
+00001150: 7217 0000 0072 4700 0000 724b 0000 00da  r....rG...rK....
+00001160: 0873 706c 6974 7465 72da 0563 6875 6e6b  .splitter..chunk
+00001170: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00001180: 4800 0000 8500 0000 732c 0000 0002 8004  H.......s,......
+00001190: 030a 010c 0312 0108 0104 0106 030c 0112  ................
+000011a0: 010e 0108 0102 ff04 ff0c 030a 010e 0108  ................
+000011b0: 0102 ff02 ff10 040e 017a 1d50 6c61 696e  .........z.Plain
+000011c0: 5465 7874 4578 6563 7574 6f72 5265 7375  TextExecutorResu
+000011d0: 6c74 2e6c 696e 6573 4ea9 0172 4c00 0000  lt.linesN..rL...
+000011e0: 2910 721d 0000 0072 1e00 0000 721f 0000  ).r....r....r...
+000011f0: 0072 2000 0000 7229 0000 00da 0b64 6174  .r ...r).....dat
+00001200: 6163 6c61 7373 6573 da05 6669 656c 6472  aclasses..fieldr
+00001210: 4600 0000 7202 0000 0072 3f00 0000 7222  F...r....r?...r"
+00001220: 0000 0072 3600 0000 7207 0000 0072 2100  ...r6...r....r!.
+00001230: 0000 7204 0000 0072 4800 0000 721b 0000  ..r....rH...r...
+00001240: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00001250: 7242 0000 0078 0000 0073 1600 0000 0a00  rB...x...s......
+00001260: 0402 0402 1401 0e02 0207 04ff 0601 02ff  ................
+00001270: 0602 0efe 7242 0000 0063 0000 0000 0000  ....rB...c......
+00001280: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00001290: 0000 7338 0000 0065 005a 0164 005a 0264  ..s8...e.Z.d.Z.d
+000012a0: 0164 0284 005a 0364 0365 0464 0465 0565  .d...Z.d.e.d.e.e
+000012b0: 0619 0066 0464 0564 0684 045a 0764 0465  ...f.d.d...Z.d.e
+000012c0: 0666 0264 0764 0884 045a 0864 0953 0029  .f.d.d...Z.d.S.)
+000012d0: 0a72 5400 0000 6301 0000 0000 0000 0000  .rT...c.........
+000012e0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+000012f0: 0a00 0000 6401 7c00 5f00 6400 5300 a902  ....d.|._.d.S...
+00001300: 4e72 2500 0000 a901 da07 5f62 7566 6665  Nr%......._buffe
+00001310: 7272 2e00 0000 721b 0000 0072 1b00 0000  rr....r....r....
+00001320: 721c 0000 0072 1600 0000 a100 0000 7302  r....r........s.
+00001330: 0000 000a 017a 165f 4c69 6e65 5370 6c69  .....z._LineSpli
+00001340: 7474 6572 2e5f 5f69 6e69 745f 5f72 5900  tter.__init__rY.
+00001350: 0000 7224 0000 0063 0200 0000 0000 0000  ..r$...c........
+00001360: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+00001370: 7350 0000 007c 01a0 0064 01a1 016a 0164  sP...|...d...j.d
+00001380: 0264 038d 017d 027c 006a 0272 157c 006a  .d...}.|.j.r.|.j
+00001390: 027c 0264 0419 0017 007c 0264 043c 007c  .|.d.....|.d.<.|
+000013a0: 0264 0519 00a0 0364 06a1 0172 2164 077c  .d.....d...r!d.|
+000013b0: 005f 027c 0253 007c 02a0 04a1 007c 005f  ._.|.S.|.....|._
+000013c0: 027c 0253 0029 084e da04 7574 6638 5472  .|.S.).N..utf8Tr
+000013d0: 4d00 0000 7201 0000 00e9 ffff ffff da01  M...r...........
+000013e0: 0a72 2500 0000 2905 da06 6465 636f 6465  .r%...)...decode
+000013f0: 7253 0000 0072 5f00 0000 da08 656e 6473  rS...r_.....ends
+00001400: 7769 7468 da03 706f 7029 0372 1700 0000  with..pop).r....
+00001410: 7259 0000 0072 4800 0000 721b 0000 0072  rY...rH...r....r
+00001420: 1b00 0000 721c 0000 0072 5600 0000 a400  ....r....rV.....
+00001430: 0000 7310 0000 0012 0106 0112 010e 0106  ..s.............
+00001440: 0104 030a ff04 017a 125f 4c69 6e65 5370  .......z._LineSp
+00001450: 6c69 7474 6572 2e70 7573 6863 0100 0000  litter.pushc....
+00001460: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00001470: 4300 0000 7310 0000 007c 006a 007d 0164  C...s....|.j.}.d
+00001480: 017c 005f 007c 0153 0072 5d00 0000 725e  .|._.|.S.r]...r^
+00001490: 0000 0029 0272 1700 0000 da03 6275 6672  ...).r......bufr
+000014a0: 1b00 0000 721b 0000 0072 1c00 0000 7257  ....r....r....rW
+000014b0: 0000 00ae 0000 0073 0600 0000 0601 0601  .......s........
+000014c0: 0401 7a13 5f4c 696e 6553 706c 6974 7465  ..z._LineSplitte
+000014d0: 722e 666c 7573 684e 2909 721d 0000 0072  r.flushN).r....r
+000014e0: 1e00 0000 721f 0000 0072 1600 0000 da05  ....r....r......
+000014f0: 6279 7465 73da 046c 6973 7472 2200 0000  bytes..listr"...
+00001500: 7256 0000 0072 5700 0000 721b 0000 0072  rV...rW...r....r
+00001510: 1b00 0000 721b 0000 0072 1c00 0000 7254  ....r....r....rT
+00001520: 0000 00a0 0000 0073 0800 0000 0800 0801  .......s........
+00001530: 1603 120a 7254 0000 0063 0000 0000 0000  ....rT...c......
+00001540: 0000 0000 0000 0000 0000 0500 0000 4000  ..............@.
+00001550: 0000 733e 0000 0065 005a 0164 005a 0255  ..s>...e.Z.d.Z.U
+00001560: 0064 015a 0364 025a 0465 056a 0664 0364  .d.Z.d.Z.e.j.d.d
+00001570: 048d 015a 0765 0865 0964 053c 0064 0c64  ...Z.e.e.d.<.d.d
+00001580: 0765 0a64 0865 0b66 0464 0964 0a84 055a  .e.d.e.f.d.d...Z
+00001590: 0c64 0b53 0029 0dda 124a 736f 6e45 7865  .d.S.)...JsonExe
+000015a0: 6375 746f 7252 6573 756c 747a 1b55 6e61  cutorResultz.Una
+000015b0: 7279 204a 534f 4e20 6578 6563 7574 696f  ry JSON executio
+000015c0: 6e20 7265 7375 6c74 fa10 6170 706c 6963  n result..applic
+000015d0: 6174 696f 6e2f 6a73 6f6e 4672 4400 0000  ation/jsonFrD...
+000015e0: 7236 0000 0072 4c00 0000 720f 0000 0072  r6...rL...r....r
+000015f0: 2400 0000 6302 0000 0000 0000 0000 0000  $...c...........
+00001600: 0002 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
+00001610: 0000 7c00 a000 7c01 7c00 6a01 a102 0100  ..|...|.|.j.....
+00001620: 7402 a003 7c00 6a01 a101 5300 7231 0000  t...|.j...S.r1..
+00001630: 0029 0472 3800 0000 7236 0000 00da 046a  .).r8...r6.....j
+00001640: 736f 6eda 056c 6f61 6473 2902 7217 0000  son..loads).r...
+00001650: 0072 0f00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00001660: 721c 0000 00da 096a 736f 6e5f 6461 7461  r......json_data
+00001670: bb00 0000 7304 0000 000e 010c 017a 1c4a  ....s........z.J
+00001680: 736f 6e45 7865 6375 746f 7252 6573 756c  sonExecutorResul
+00001690: 742e 6a73 6f6e 5f64 6174 614e 725a 0000  t.json_dataNrZ..
+000016a0: 0029 0d72 1d00 0000 721e 0000 0072 1f00  .).r....r....r..
+000016b0: 0000 7220 0000 0072 2900 0000 725b 0000  ..r ...r)...r[..
+000016c0: 0072 5c00 0000 7236 0000 0072 2200 0000  .r\...r6...r"...
+000016d0: 723f 0000 0072 2100 0000 7202 0000 0072  r?...r!...r....r
+000016e0: 6d00 0000 721b 0000 0072 1b00 0000 721b  m...r....r....r.
+000016f0: 0000 0072 1c00 0000 7269 0000 00b4 0000  ...r....ri......
+00001700: 0073 0a00 0000 0a00 0402 0402 1401 1802  .s..............
+00001710: 7269 0000 0063 0000 0000 0000 0000 0000  ri...c..........
+00001720: 0000 0000 0000 0300 0000 4000 0000 733c  ..........@...s<
+00001730: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00001740: 0364 025a 0465 056a 0664 0364 048d 015a  .d.Z.e.j.d.d...Z
+00001750: 0765 0865 0964 053c 0064 0665 0a65 0819  .e.e.d.<.d.e.e..
+00001760: 0066 0264 0764 0884 045a 0b64 0953 0029  .f.d.d...Z.d.S.)
+00001770: 0ada 154a 736f 6e53 6571 4578 6563 7574  ...JsonSeqExecut
+00001780: 6f72 5265 7375 6c74 7a1f 5374 7265 616d  orResultz.Stream
+00001790: 696e 6720 4a53 4f4e 2065 7865 6375 7469  ing JSON executi
+000017a0: 6f6e 2072 6573 756c 747a 1461 7070 6c69  on resultz.appli
+000017b0: 6361 7469 6f6e 2f6a 736f 6e2d 7365 7146  cation/json-seqF
+000017c0: 7244 0000 0072 4600 0000 7224 0000 0063  rD...rF...r$...c
+000017d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000017e0: 0700 0000 4302 0000 7372 0000 0081 027c  ....C...sr.....|
+000017f0: 00a0 0064 01a1 0101 0074 017c 006a 0264  ...d.....t.|.j.d
+00001800: 0283 0272 1e7c 006a 0232 007a 0b33 0064  ...r.|.j.2.z.3.d
+00001810: 0048 0057 007d 0174 037c 0183 0156 0001  .H.W.}.t.|...V..
+00001820: 0071 0f36 0064 0053 0074 017c 006a 0264  .q.6.d.S.t.|.j.d
+00001830: 0383 0272 317c 006a 0244 005d 077d 0174  ...r1|.j.D.].}.t
+00001840: 037c 0183 0156 0001 0071 2764 0053 0074  .|...V...q'd.S.t
+00001850: 0464 047c 006a 029b 009d 0283 0182 0129  .d.|.j.........)
+00001860: 054e 724c 0000 0072 4f00 0000 7250 0000  .NrL...rO...rP..
+00001870: 0072 5100 0000 2905 7238 0000 0072 5500  .rQ...).r8...rU.
+00001880: 0000 7246 0000 00da 0e5f 6a73 6f6e 5f73  ..rF....._json_s
+00001890: 6571 5f69 7465 6d72 2600 0000 2902 7217  eq_itemr&...).r.
+000018a0: 0000 0072 4b00 0000 721b 0000 0072 1b00  ...rK...r....r..
+000018b0: 0000 721c 0000 00da 0d6a 736f 6e5f 7365  ..r......json_se
+000018c0: 715f 6461 7461 c700 0000 7316 0000 0002  q_data....s.....
+000018d0: 800a 010c 0112 010c 0106 ff0c 020a 020c  ................
+000018e0: 0104 ff10 037a 234a 736f 6e53 6571 4578  .....z#JsonSeqEx
+000018f0: 6563 7574 6f72 5265 7375 6c74 2e6a 736f  ecutorResult.jso
+00001900: 6e5f 7365 715f 6461 7461 4e29 0c72 1d00  n_seq_dataN).r..
+00001910: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00001920: 0072 2900 0000 725b 0000 0072 5c00 0000  .r)...r[...r\...
+00001930: 7246 0000 0072 0200 0000 723f 0000 0072  rF...r....r?...r
+00001940: 0400 0000 7270 0000 0072 1b00 0000 721b  ....rp...r....r.
+00001950: 0000 0072 1b00 0000 721c 0000 0072 6e00  ...r....r....rn.
+00001960: 0000 c000 0000 730a 0000 000a 0004 0204  ......s.........
+00001970: 0214 0116 0272 6e00 0000 f301 0000 001e  .....rn.........
+00001980: 724b 0000 0063 0100 0000 0000 0000 0000  rK...c..........
+00001990: 0000 0200 0000 0300 0000 4300 0000 7324  ..........C...s$
+000019a0: 0000 007c 00a0 0074 01a1 0172 0b7c 0064  ...|...t...r.|.d
+000019b0: 0164 0085 0219 006e 017c 007d 0174 02a0  .d.....n.|.}.t..
+000019c0: 037c 01a1 0153 0029 024e e901 0000 0029  .|...S.).N.....)
+000019d0: 04da 0a73 7461 7274 7377 6974 68da 1052  ...startswith..R
+000019e0: 4543 4f52 445f 5345 5041 5241 544f 5272  ECORD_SEPARATORr
+000019f0: 6b00 0000 726c 0000 0029 0272 4b00 0000  k...rl...).rK...
+00001a00: 7211 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00001a10: 1c00 0000 726f 0000 00d7 0000 0073 0400  ....ro.......s..
+00001a20: 0000 1a02 0a01 726f 0000 00da 1645 7870  ......ro.....Exp
+00001a30: 6563 7465 6445 7865 6375 746f 7252 6573  ectedExecutorRes
+00001a40: 756c 7429 01da 0562 6f75 6e64 6300 0000  ult)...boundc...
+00001a50: 0000 0000 0000 0000 0000 0000 000f 0000  ................
+00001a60: 0040 0000 0073 c200 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001a70: 5a02 0901 641a 6402 6503 6403 6503 6404  Z...d.d.e.d.e.d.
+00001a80: 6504 6503 1900 6606 6405 6406 8405 5a05  e.e...f.d.d...Z.
+00001a90: 6506 6407 6408 8400 8301 5a07 6409 6503  e.d.d.....Z.d.e.
+00001aa0: 640a 6503 640b 6508 640c 6504 6509 1900  d.e.d.e.d.e.e...
+00001ab0: 640d 650a 650b 1900 660a 640e 640f 8404  d.e.e...f.d.d...
+00001ac0: 5a0c 650d 6a0e 0910 0901 0901 641b 6411  Z.e.j.......d.d.
+00001ad0: 650f 6510 1900 6412 6503 640a 6503 640b  e.e...d.e.d.e.d.
+00001ae0: 6504 6508 1900 6413 6504 6511 1900 640d  e.e...d.e.e...d.
+00001af0: 6512 6510 1900 660c 6414 6415 8405 8301  e.e...f.d.d.....
+00001b00: 5a13 0901 641a 6416 6503 6417 6504 6514  Z...d.d.e.d.e.e.
+00001b10: 6503 6511 6602 1900 1900 640d 6511 6606  e.e.f.....d.e.f.
+00001b20: 6418 6419 8405 5a15 6401 5300 291c da08  d.d...Z.d.S.)...
+00001b30: 4578 6563 7574 6f72 4eda 0776 6172 6961  ExecutorN..varia
+00001b40: 6e74 da07 6170 695f 7572 6c72 0c00 0000  nt..api_urlr....
+00001b50: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00001b60: 0005 0000 0043 0000 0073 3000 0000 7c02  .....C...s0...|.
+00001b70: 7c00 5f00 7401 7c01 8301 7c00 5f02 7c03  |._.t.|...|._.|.
+00001b80: 720f 7c03 7c00 6a02 7403 3c00 7404 a005  r.|.|.j.t.<.t...
+00001b90: 6401 7c01 7c02 a103 0100 6400 5300 2902  d.|.|.....d.S.).
+00001ba0: 4e7a 2249 6e73 7461 6e74 6961 7465 6420  Nz"Instantiated 
+00001bb0: 2573 2065 7865 6375 746f 722e 205b 7572  %s executor. [ur
+00001bc0: 6c3d 2573 5d29 06da 085f 6170 695f 7572  l=%s])..._api_ur
+00001bd0: 6cda 105f 6465 6661 756c 745f 6865 6164  l.._default_head
+00001be0: 6572 73da 085f 6865 6164 6572 73da 1441  ers.._headers..A
+00001bf0: 5554 484f 5249 5a41 5449 4f4e 5f48 4541  UTHORIZATION_HEA
+00001c00: 4445 5272 2c00 0000 722d 0000 0029 0472  DERr,...r-...).r
+00001c10: 1700 0000 7278 0000 0072 7900 0000 720c  ....rx...ry...r.
+00001c20: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
+00001c30: 0000 7216 0000 00e3 0000 0073 0a00 0000  ..r........s....
+00001c40: 0603 0a01 0401 0a01 1201 7a11 4578 6563  ..........z.Exec
+00001c50: 7574 6f72 2e5f 5f69 6e69 745f 5f63 0100  utor.__init__c..
+00001c60: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001c70: 0000 4300 0000 730a 0000 0074 007c 006a  ..C...s....t.|.j
+00001c80: 0176 0053 0072 3100 0000 2902 727d 0000  .v.S.r1...).r}..
+00001c90: 0072 7c00 0000 722e 0000 0072 1b00 0000  .r|...r....r....
+00001ca0: 721b 0000 0072 1c00 0000 da0d 6175 7468  r....r......auth
+00001cb0: 656e 7469 6361 7465 64ec 0000 0073 0200  enticated....s..
+00001cc0: 0000 0a02 7a16 4578 6563 7574 6f72 2e61  ....z.Executor.a
+00001cd0: 7574 6865 6e74 6963 6174 6564 da03 7572  uthenticated..ur
+00001ce0: 6cda 066d 6574 686f 64da 0768 6561 6465  l..method..heade
+00001cf0: 7273 da04 626f 6479 7224 0000 0063 0500  rs..bodyr$...c..
+00001d00: 0000 0000 0000 0000 0000 0500 0000 0100  ................
+00001d10: 0000 4300 0000 7230 0000 0072 3100 0000  ..C...r0...r1...
+00001d20: 7232 0000 0029 0572 1700 0000 727f 0000  r2...).r....r...
+00001d30: 0072 8000 0000 7281 0000 0072 8200 0000  .r....r....r....
+00001d40: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00001d50: 055f 7365 6e64 f000 0000 7302 0000 0006  ._send....s.....
+00001d60: 037a 0e45 7865 6375 746f 722e 5f73 656e  .z.Executor._sen
+00001d70: 64da 0347 4554 da0b 7265 7375 6c74 5f74  d..GET..result_t
+00001d80: 7970 65da 0470 6174 6872 6d00 0000 6306  ype..pathrm...c.
+00001d90: 0000 0000 0000 0000 0000 000b 0000 0009  ................
+00001da0: 0000 0043 0200 0073 2c01 0000 8102 7c00  ...C...s,.....|.
+00001db0: 6a00 a001 a100 7d06 7c04 720d 7c06 a002  j.....}.|.r.|...
+00001dc0: 7c04 a101 0100 7c01 7403 6b02 7214 6401  |.....|.t.k.r.d.
+00001dd0: 7d07 6e15 7c01 7404 6b02 721b 6402 7d07  }.n.|.t.k.r.d.}.
+00001de0: 6e0e 7c01 7405 6b02 7222 6403 7d07 6e07  n.|.t.k.r"d.}.n.
+00001df0: 7406 6404 7c01 9b00 9d02 8301 8201 7c07  t.d.|.........|.
+00001e00: 7c06 6405 3c00 7c05 723c 6406 7c06 6407  |.d.<.|.r<d.|.d.
+00001e10: 3c00 7407 a008 7c05 a101 a009 6408 a101  <.t...|.....d...
+00001e20: 7d08 6e02 6400 7d08 740a a00b 6409 7c08  }.n.d.}.t...d.|.
+00001e30: 7247 740c 7c08 8301 6e01 640a a102 0100  rGt.|...n.d.....
+00001e40: 7c00 6a0d 740e 6a0f a010 7c00 6a11 7c02  |.j.t.j...|.j.|.
+00001e50: a102 7c03 7c06 7c08 640b 8d04 3400 4900  ..|.|.|.d...4.I.
+00001e60: 6400 4800 9a2c 7d09 7412 7c09 7c01 8302  d.H..,}.t.|.|...
+00001e70: 737b 7412 7c00 7405 8302 7270 7c00 a013  s{t.|.t...rp|...
+00001e80: a100 4900 6400 4800 7d0a 6e02 6400 7d0a  ..I.d.H.}.n.d.}.
+00001e90: 7414 7c09 6a15 7c09 6a16 7c0a 640c 8d03  t.|.j.|.j.|.d...
+00001ea0: 8201 7c09 5600 0100 5700 6400 0400 0400  ..|.V...W.d.....
+00001eb0: 8303 4900 6400 4800 0100 6400 5300 3100  ..I.d.H...d.S.1.
+00001ec0: 4900 6400 4800 738f 7701 0100 0100 0100  I.d.H.s.w.......
+00001ed0: 5900 0100 6400 5300 290d 4e7a 2661 7070  Y...d.S.).Nz&app
+00001ee0: 6c69 6361 7469 6f6e 2f6a 736f 6e3b 713d  lication/json;q=
+00001ef0: 312c 2074 6578 742f 706c 6169 6e3b 713d  1, text/plain;q=
+00001f00: 302e 317a 2a61 7070 6c69 6361 7469 6f6e  0.1z*application
+00001f10: 2f6a 736f 6e2d 7365 713b 713d 312c 2074  /json-seq;q=1, t
+00001f20: 6578 742f 706c 6169 6e3b 713d 302e 3172  ext/plain;q=0.1r
+00001f30: 4300 0000 7a19 556e 7375 7070 6f72 7465  C...z.Unsupporte
+00001f40: 6420 7265 7375 6c74 2074 7970 653a 2072  d result type: r
+00001f50: 3400 0000 726a 0000 0072 0d00 0000 7260  4...rj...r....r`
+00001f60: 0000 007a 2053 656e 6469 6e67 2041 5049  ...z Sending API
+00001f70: 2072 6571 7565 7374 2e2e 2e20 5b73 697a   request... [siz
+00001f80: 653d 2573 5d72 0100 0000 2904 727f 0000  e=%s]r....).r...
+00001f90: 0072 8000 0000 7281 0000 0072 8200 0000  .r....r....r....
+00001fa0: 7237 0000 0029 1772 7c00 0000 da04 636f  r7...).r|.....co
+00001fb0: 7079 da06 7570 6461 7465 7269 0000 0072  py..updateri...r
+00001fc0: 6e00 0000 7242 0000 0072 2600 0000 726b  n...rB...r&...rk
+00001fd0: 0000 00da 0564 756d 7073 da06 656e 636f  .....dumps..enco
+00001fe0: 6465 722c 0000 0072 2d00 0000 da03 6c65  der,...r-.....le
+00001ff0: 6e72 8300 0000 da06 7572 6c6c 6962 da05  nr......urllib..
+00002000: 7061 7273 65da 0775 726c 6a6f 696e 727a  parse..urljoinrz
+00002010: 0000 0072 5200 0000 7236 0000 0072 0e00  ...rR...r6...r..
+00002020: 0000 720f 0000 0072 1000 0000 290b 7217  ..r....r....).r.
+00002030: 0000 0072 8500 0000 7286 0000 0072 8000  ...r....r....r..
+00002040: 0000 7281 0000 0072 6d00 0000 5a0b 616c  ..r....rm...Z.al
+00002050: 6c5f 6865 6164 6572 7372 3400 0000 7282  l_headersr4...r.
+00002060: 0000 00da 0672 6573 756c 7472 3600 0000  .....resultr6...
+00002070: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00002080: 0765 7865 6375 7465 f500 0000 7346 0000  .execute....sF..
+00002090: 0002 800a 0904 010a 0108 0206 0108 0106  ................
+000020a0: 0108 0106 010e 0208 0104 0208 0112 0104  ................
+000020b0: 0204 0210 0104 ff04 030e 0102 0102 0102  ................
+000020c0: 010e fc02 050a 010a 0110 0104 0202 010a  ................
+000020d0: 0106 ff08 032e f27a 1045 7865 6375 746f  .......z.Executo
+000020e0: 722e 6578 6563 7574 65da 0571 7565 7279  r.execute..query
+000020f0: da09 7661 7269 6162 6c65 7363 0300 0000  ..variablesc....
+00002100: 0000 0000 0000 0000 0500 0000 0900 0000  ................
+00002110: c300 0000 737e 0000 0081 017c 006a 0074  ....s~.....|.j.t
+00002120: 0164 0164 027c 017c 0270 0a69 0064 039c  .d.d.|.|.p.i.d..
+00002130: 0264 048d 0434 0049 0064 0048 009a 0f7d  .d...4.I.d.H...}
+00002140: 037c 03a0 02a1 007d 0457 0064 0004 0004  .|.....}.W.d....
+00002150: 0083 0349 0064 0048 0001 006e 0b31 0049  ...I.d.H...n.1.I
+00002160: 0064 0048 0073 2877 0101 0001 0001 0059  .d.H.s(w.......Y
+00002170: 0001 007c 04a0 0364 05a1 0172 3b74 047c  ...|...d...r;t.|
+00002180: 036a 057c 036a 067c 0464 068d 0382 017c  .j.|.j.|.d.....|
+00002190: 0464 0719 0053 0029 084e 7a08 2f67 7261  .d...S.).Nz./gra
+000021a0: 7068 716c da04 504f 5354 2902 7291 0000  phql..POST).r...
+000021b0: 0072 9200 0000 2904 7285 0000 0072 8600  .r....).r....r..
+000021c0: 0000 7280 0000 0072 6d00 0000 da06 6572  ..r....rm.....er
+000021d0: 726f 7273 7237 0000 0072 1100 0000 2907  rorsr7...r....).
+000021e0: 7290 0000 0072 6900 0000 726d 0000 00da  r....ri...rm....
+000021f0: 0367 6574 720e 0000 0072 0f00 0000 7210  .getr....r....r.
+00002200: 0000 0029 0572 1700 0000 7291 0000 0072  ...).r....r....r
+00002210: 9200 0000 728f 0000 0072 1100 0000 721b  ....r....r....r.
+00002220: 0000 0072 1b00 0000 721c 0000 00da 1565  ...r....r......e
+00002230: 7865 6375 7465 5f67 7261 7068 716c 5f71  xecute_graphql_q
+00002240: 7565 7279 2501 0000 731a 0000 0002 8004  uery%...s.......
+00002250: 0502 0102 0102 010c 010e fc02 050a 0128  ...............(
+00002260: fa0a 0712 0108 017a 1e45 7865 6375 746f  .......z.Executo
+00002270: 722e 6578 6563 7574 655f 6772 6170 6871  r.execute_graphq
+00002280: 6c5f 7175 6572 7972 3100 0000 2903 7284  l_queryr1...).r.
+00002290: 0000 004e 4e29 1672 1d00 0000 721e 0000  ...NN).r....r...
+000022a0: 0072 1f00 0000 7222 0000 0072 0700 0000  .r....r"...r....
+000022b0: 7216 0000 0072 4000 0000 727e 0000 00da  r....r@...r~....
+000022c0: 0748 6561 6465 7273 7267 0000 0072 0300  .Headersrg...r..
+000022d0: 0000 722b 0000 0072 8300 0000 da0a 636f  ..r+...r......co
+000022e0: 6e74 6578 746c 6962 da13 6173 796e 6363  ntextlib..asyncc
+000022f0: 6f6e 7465 7874 6d61 6e61 6765 7272 0500  ontextmanagerr..
+00002300: 0000 7275 0000 0072 0200 0000 7204 0000  ..ru...r....r...
+00002310: 0072 9000 0000 7206 0000 0072 9600 0000  .r....r....r....
+00002320: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00002330: 1c00 0000 7277 0000 00e2 0000 0073 5e00  ....rw.......s^.
+00002340: 0000 0800 0202 04ff 0201 02ff 0201 02ff  ................
+00002350: 0601 0aff 0209 0a01 0203 0201 02ff 0201  ................
+00002360: 02ff 0201 02ff 0601 02ff 0602 0afe 0405  ................
+00002370: 0205 0201 0201 04fa 0602 02fe 0203 02fd  ................
+00002380: 0204 02fc 0605 02fb 0606 02fa 0607 0cf9  ................
+00002390: 0232 04fd 0202 02fe 0e03 02fd 0204 0efc  .2..............
+000023a0: 7277 0000 00da 0663 6c69 656e 7463 0100  rw.....clientc..
+000023b0: 0000 0000 0000 0000 0000 0100 0000 0600  ................
+000023c0: 0000 4300 0000 7316 0000 0064 0164 0274  ..C...s....d.d.t
+000023d0: 009b 0064 037c 009b 0064 049d 0569 0153  ...d.|...d...i.S
+000023e0: 0029 054e 7a0e 6f70 7669 6f75 732d 636c  .).Nz.opvious-cl
+000023f0: 6965 6e74 7a0c 5079 7468 6f6e 2053 444b  ientz.Python SDK
+00002400: 2076 7212 0000 0072 1300 0000 720a 0000   vr....r....r...
+00002410: 0029 0172 9a00 0000 721b 0000 0072 1b00  .).r....r....r..
+00002420: 0000 721c 0000 0072 7b00 0000 3601 0000  ..r....r{...6...
+00002430: 7304 0000 0012 0204 ff72 7b00 0000 7231  s........r{...r1
+00002440: 0000 0029 2a72 2000 0000 7298 0000 0072  ...)*r ...r....r
+00002450: 5b00 0000 726b 0000 00da 076c 6f67 6769  [...rk.....loggi
+00002460: 6e67 da06 7479 7069 6e67 7202 0000 0072  ng..typingr....r
+00002470: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
+00002480: 0000 0072 0700 0000 7208 0000 00da 0c75  ...r....r......u
+00002490: 726c 6c69 622e 7061 7273 6572 8c00 0000  rllib.parser....
+000024a0: da06 636f 6d6d 6f6e 720b 0000 00da 0967  ..commonr......g
+000024b0: 6574 4c6f 6767 6572 721d 0000 0072 2c00  etLoggerr....r,.
+000024c0: 0000 5a0c 5452 4143 455f 4845 4144 4552  ..Z.TRACE_HEADER
+000024d0: 727d 0000 005a 1343 4f4e 5445 4e54 5f54  r}...Z.CONTENT_T
+000024e0: 5950 455f 4845 4144 4552 da04 6469 6374  YPE_HEADER..dict
+000024f0: 7222 0000 0072 9700 0000 7226 0000 0072  r"...r....r&...r
+00002500: 0e00 0000 7228 0000 0072 2a00 0000 da09  ....r(...r*.....
+00002510: 6461 7461 636c 6173 7372 2b00 0000 7242  dataclassr+...rB
+00002520: 0000 0072 5400 0000 7269 0000 0072 6e00  ...rT...ri...rn.
+00002530: 0000 7274 0000 0072 6700 0000 726f 0000  ..rt...rg...ro..
+00002540: 0072 7500 0000 7277 0000 0072 7b00 0000  .ru...rw...r{...
+00002550: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00002560: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00002570: 0000 735c 0000 0004 0008 1308 0108 0108  ..s\............
+00002580: 0124 0108 090c 020a 0304 0304 0304 030c  .$..............
+00002590: 0310 0302 1504 ff02 0102 ff06 0102 ff02  ................
+000025a0: 020a fe02 0b04 ff06 0102 ff06 0102 ff02  ................
+000025b0: 020a fe04 0910 0104 1b12 010e 2704 1412  ............'...
+000025c0: 0104 0b12 0104 1312 0302 0604 0106 ff0e  ................
+000025d0: 0516 54                                  ..T
```

### Comparing `opvious-0.9.3/opvious/executors/__pycache__/urllib.cpython-310.pyc` & `opvious-0.9.4/opvious/executors/__pycache__/urllib.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr  7 18:18:57 2023 UTC, .py size: 2685 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 915e 3064 7d0a 0000  o........^0d}...
+00000000: 6f0d 0d0a 0000 0000 0770 3064 7d0a 0000  o........p0d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a04 6401 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c06 6d07 5a07 6d08 5a08  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `opvious-0.9.3/opvious/executors/aiohttp.py` & `opvious-0.9.4/opvious/executors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/opvious/executors/common.py` & `opvious-0.9.4/opvious/executors/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 _logger = logging.getLogger(__name__)
 
 
 TRACE_HEADER = "opvious-trace"
 
 
+AUTHORIZATION_HEADER = "authorization"
+
+
 CONTENT_TYPE_HEADER = "content-type"
 
 
 Headers = dict[str, str]
 
 
 class ApiError(Exception):
@@ -223,17 +226,21 @@
 class Executor:
     def __init__(
         self, variant: str, api_url: str, authorization: Optional[str] = None
     ):
         self._api_url = api_url
         self._headers = _default_headers(variant)
         if authorization:
-            self._headers["authorization"] = authorization
+            self._headers[AUTHORIZATION_HEADER] = authorization
         _logger.debug("Instantiated %s executor. [url=%s]", variant, api_url)
 
+    @property
+    def authenticated(self):
+        return AUTHORIZATION_HEADER in self._headers
+
     def _send(
         self, url: str, method: str, headers: Headers, body: Optional[bytes]
     ) -> AsyncContextManager[ExecutorResult]:
         raise NotImplementedError()
 
     @contextlib.asynccontextmanager
     async def execute(
```

### Comparing `opvious-0.9.3/opvious/executors/pyodide.py` & `opvious-0.9.4/opvious/executors/pyodide.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/opvious/executors/urllib.py` & `opvious-0.9.4/opvious/executors/urllib.py`

 * *Files identical despite different names*

### Comparing `opvious-0.9.3/pyproject.toml` & `opvious-0.9.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opvious"
-version = "0.9.3"
+version = "0.9.4"
 description = "Opvious Python SDK"
 authors = ["Opvious Engineering <oss@opvious.io>"]
 readme = "README.md"
 repository = "https://github.com/opvious/sdk.py"
 packages = [{include = "opvious"}]
 
 [tool.poetry.dependencies]
```

### Comparing `opvious-0.9.3/setup.py` & `opvious-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['backoff>=2.2,<3.0', 'humanize>=4.4.0,<5.0.0', 'pandas>=1.4,<2.0']
 
 extras_require = \
 {'aio': ['aiohttp>=3.8,<4.0', 'Brotli>=1.0.9,<2.0.0']}
 
 setup_kwargs = {
     'name': 'opvious',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Opvious Python SDK',
     'long_description': '# Opvious Python SDK  [![CI](https://github.com/opvious/sdk.py/actions/workflows/ci.yml/badge.svg)](https://github.com/opvious/sdk.py/actions/workflows/ci.yml) [![Pypi badge](https://badge.fury.io/py/opvious.svg)](https://pypi.python.org/pypi/opvious/)\n\nThis package provides a lightweight SDK for solving optimization models with the\n[Opvious API][api]. Its main features are:\n\n+ Seamless data import/export via native support for [`pandas`][pandas]\n+ Powerful built-in debugging capabilities: automatic infeasibility relaxation,\n  variable pinning, and more\n+ Non-blocking APIs for performant parallel calls\n\n\n## Quickstart\n\nFirst, install this package and have an API access token handy (these can be\ngenerated [here][token]).\n\n```sh\npip install opvious[aio] # aio is recommended for improved performance\n```\n\nWith these steps out of the way, you are ready to optimize!\n\n```python\nimport opvious\n\n# Instantiate an API client from an API token\nclient = opvious.Client.from_token(TOKEN)\n\n# Solve a simple portfolio selection optimization model\nresponse = await client.solve(\n    sources=[\n      r"""\n          We find an allocation of assets which minimizes risk while satisfying\n          a minimum expected return:\n\n          + A collection of assets: $\\S^d_{asset}: A$\n          + Covariances: $\\S^p_{covariance}: c \\in \\mathbb{R}^{A \\times A}$\n          + Expected return: $\\S^p_{expectedReturn}: m \\in \\mathbb{R}^A$\n          + Minimum desired return: $\\S^p_{desiredReturn}: r \\in \\mathbb{R}$\n\n          The only output is the allocation per asset\n          $\\S^v_{allocation}: \\alpha \\in [0,1]^A$ chosen to minimize risk:\n          $\\S^o_{risk}: \\min \\sum_{a, b \\in A} c_{a,b} \\alpha_a \\alpha_b$.\n\n          Subject to the following constraints:\n\n          + $\\S^c_{atLeastMinimumReturn}: \\sum_{a \\in A} m_a \\alpha_a \\geq r$\n          + $\\S^c_{totalAllocation}: \\sum_{a \\in A} \\alpha_a = 1$\n      """\n    ],\n    parameters={\n        "covariance": {\n            ("AAPL", "AAPL"): 0.08,\n            # ...\n        },\n        "expectedReturn": {\n            "AAPL": 0.07,\n            # ..\n        },\n        "desiredReturn": 0.05,\n    },\n)\n\n# Print the optimal allocation, if any\nif isinstance(response.outcome, opvious.FeasibleOutcome):\n  print(response.outputs.variable("allocation"))\nelse:\n  print(f"Problem was {response.status}.") # INFEASIBLE, UNBOUNDED\n```\n\n\n## Environments\n\nClients are compatible with Pyodide environments, for example [JupyterLite][]\nkernels. Simply install the package as usual in a notebook, omitting the `aio`\noptional dependencies:\n\n```python\nimport piplite\nawait piplite.install(\'opvious\')\n```\n\nIn other environments, prefer using the `aiohttp`-powered clients as they are\nmore performant (this is the default if the `aio` dependencies were specified).\n\n\n## Next steps\n\nThis SDK is focused on solving optimization models. For convenient access to the\nrest of Opvious API\'s functionality, consider using the [TypeScript SDK and\nCLI][cli].\n\n\n[api]: https://www.opvious.io\n[cli]: https://www.opvious.io/sdk.ts\n[JupyterLite]: https://jupyterlite.readthedocs.io/\n[token]: https://hub.beta.opvious.io/authorizations\n[pandas]: https://pandas.pydata.org\n',
     'author': 'Opvious Engineering',
     'author_email': 'oss@opvious.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opvious/sdk.py',
```

### Comparing `opvious-0.9.3/PKG-INFO` & `opvious-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opvious
-Version: 0.9.3
+Version: 0.9.4
 Summary: Opvious Python SDK
 Home-page: https://github.com/opvious/sdk.py
 Author: Opvious Engineering
 Author-email: oss@opvious.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

