# Comparing `tmp/pyttsx4-3.0.2-py3-none-any.whl.zip` & `tmp/pyttsx4-3.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 32814 bytes, number of entries: 16
+Zip file size: 33067 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      814 b- defN 23-Apr-07 13:37 pyttsx4/__init__.py
--rw-r--r--  2.0 unx     6878 b- defN 23-Apr-07 14:20 pyttsx4/driver.py
+-rw-r--r--  2.0 unx     7429 b- defN 23-Apr-07 17:19 pyttsx4/driver.py
 -rw-r--r--  2.0 unx     7224 b- defN 23-Apr-07 13:37 pyttsx4/engine.py
 -rw-r--r--  2.0 unx    29524 b- defN 23-Apr-07 13:37 pyttsx4/six.py
 -rw-r--r--  2.0 unx      431 b- defN 23-Apr-07 13:37 pyttsx4/voice.py
 -rw-r--r--  2.0 unx      853 b- defN 23-Apr-07 13:37 pyttsx4/drivers/__init__.py
 -rw-r--r--  2.0 unx    19495 b- defN 23-Apr-07 13:37 pyttsx4/drivers/_espeak.py
 -rw-r--r--  2.0 unx     6182 b- defN 23-Apr-07 13:37 pyttsx4/drivers/dummy.py
 -rw-r--r--  2.0 unx     6801 b- defN 23-Apr-07 13:37 pyttsx4/drivers/espeak.py
 -rw-r--r--  2.0 unx     3729 b- defN 23-Apr-07 14:49 pyttsx4/drivers/nsss.py
--rw-r--r--  2.0 unx     5877 b- defN 23-Apr-07 14:27 pyttsx4/drivers/sapi5.py
--rw-r--r--  2.0 unx    17098 b- defN 23-Apr-07 14:53 pyttsx4-3.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1821 b- defN 23-Apr-07 14:53 pyttsx4-3.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 14:53 pyttsx4-3.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-07 14:53 pyttsx4-3.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-07 14:53 pyttsx4-3.0.2.dist-info/RECORD
-16 files, 108071 bytes uncompressed, 30794 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx     6047 b- defN 23-Apr-07 16:55 pyttsx4/drivers/sapi5.py
+-rw-r--r--  2.0 unx    17098 b- defN 23-Apr-07 17:24 pyttsx4-3.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-07 17:24 pyttsx4-3.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 17:24 pyttsx4-3.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-07 17:24 pyttsx4-3.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-07 17:24 pyttsx4-3.0.3.dist-info/RECORD
+16 files, 108792 bytes uncompressed, 31047 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyttsx4/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx4/drivers/sapi5.py
 Comment: 
 
-Filename: pyttsx4-3.0.2.dist-info/LICENSE
+Filename: pyttsx4-3.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyttsx4-3.0.2.dist-info/METADATA
+Filename: pyttsx4-3.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyttsx4-3.0.2.dist-info/WHEEL
+Filename: pyttsx4-3.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyttsx4-3.0.2.dist-info/top_level.txt
+Filename: pyttsx4-3.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyttsx4-3.0.2.dist-info/RECORD
+Filename: pyttsx4-3.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx4/driver.py

```diff
@@ -86,15 +86,15 @@
         while (not self._busy) and len(self._queue):
             cmd = self._queue.pop(0)
             self._name = cmd[2]
             try:
                 cmd[0](*cmd[1])
             except Exception as e:
                 self.notify('error', exception=e)
-                print('ERROR',e)
+                print('ERROR:pyttsx4-driver: _pump ',e)
                 if self._debug:
                     traceback.print_exc()
 
     def notify(self, topic, **kwargs):
         '''
         Sends a notification to the engine from the driver.
 
@@ -185,14 +185,22 @@
         self._push(self._driver.setProperty, (name, value))
 
     def runAndWait(self):
         '''
         Called by the engine to start an event loop, process all commands in
         the queue at the start of the loop, and then exit the loop.
         '''
+        # actually there are no setBusy(True) in the old code and it works.
+        # the error ocurrs when i added an sapi save_to_memory function.
+        # after that, when the result is saved to memory, the busy is not set to True, so next runAndWait will
+        # DEAD wait.
+        # I don't know why it don't work for memory.
+        # but here add setBusy(True) seem ok for the issue.
+        # here first setBusy(True), and push the endLoop event, and setBusy(False) in startLoop，
+        self.setBusy(True)
         self._push(self._engine.endLoop, tuple())
         self._driver.startLoop()
 
     def startLoop(self, useDriverLoop):
         '''
         Called by the engine to start an event loop.
         '''
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## pyttsx4/drivers/sapi5.py

```diff
@@ -82,15 +82,15 @@
         stream = comtypes.client.CreateObject('SAPI.SpMemoryStream')
         temp_stream = self._tts.AudioOutputStream
         self._tts.AudioOutputStream = stream
         self._tts.Speak(fromUtf8(toUtf8(text)))
         self._tts.AudioOutputStream = temp_stream
         data = stream.GetData()
         olist.write(bytes(data))
-        stream.close()
+        del stream
 
     def _toVoice(self, attr):
         return Voice(attr.Id, attr.GetDescription())
 
     def _tokenFromId(self, id_):
         tokens = self._tts.GetVoices()
         for token in tokens:
@@ -118,14 +118,19 @@
             self._tts.Voice = token
             a, b = E_REG.get(value, E_REG[MSMARY])
             self._tts.Rate = int(math.log(self._rateWpm / a, b))
         elif name == 'rate':
             id_ = self._tts.Voice.Id
             a, b = E_REG.get(id_, E_REG[MSMARY])
             try:
+                rate = int(math.log(value / a, b))
+                if rate<-10:
+                    rate = -10
+                if rate>10:
+                    rate = 10
                 self._tts.Rate = int(math.log(value / a, b))
             except TypeError as e:
                 raise ValueError(str(e))
             self._rateWpm = value
         elif name == 'volume':
             try:
                 self._tts.Volume = int(round(value * 100, 2))
@@ -133,16 +138,16 @@
                 raise ValueError(str(e))
         elif name == 'pitch':
             print("Pitch adjustment not supported when using SAPI5")
         else:
             raise KeyError('unknown property %s' % name)
 
     def startLoop(self):
-        first = True
         self._looping = True
+        first = True
         while self._looping:
             if first:
                 self._proxy.setBusy(False)
                 first = False
             pythoncom.PumpWaitingMessages()
             time.sleep(0.05)
```

## Comparing `pyttsx4-3.0.2.dist-info/LICENSE` & `pyttsx4-3.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyttsx4-3.0.2.dist-info/METADATA` & `pyttsx4-3.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttsx4
-Version: 3.0.2
+Version: 3.0.3
 Summary: Text to Speech (TTS) library for Python 3. Works without internet connection or delay. Supports multiple TTS engines, including Sapi5, nsss, and espeak.
 Home-page: https://github.com/Jiangshan00001/pyttsx4
 Author: Natesh M Bhat
 Author-email: 710806594@qq.com
 License: UNKNOWN
 Keywords: pyttsx,ivona,pyttsx for python3,TTS for python3,pyttsx3,text to speech for python,tts,text to speech,speech,speech synthesis,offline text to speech,offline tts,gtts
 Platform: UNKNOWN
```

## Comparing `pyttsx4-3.0.2.dist-info/RECORD` & `pyttsx4-3.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 pyttsx4/__init__.py,sha256=pO2FX679OZHgpn2vBVIZDoBQff4uOUMe6yBpNRbaw-4,814
-pyttsx4/driver.py,sha256=GrKVB4NHUex375QjHHvC6x9vHQJzpWjqVQ1t2h1UL7U,6878
+pyttsx4/driver.py,sha256=uQI4OAbaRRKBEwBeh_cFW5nsev-8btlBP9xEGEaPLs4,7429
 pyttsx4/engine.py,sha256=UJBrPIcN3KXmBCABrb2uY4F_AeAaFlC5h6n_L3V0euA,7224
 pyttsx4/six.py,sha256=yVeu0rLX2Qv1P1UaJtvamDmMrjnxNsJkSuztEvVyGG8,29524
 pyttsx4/voice.py,sha256=GYZLgGtnmjLrg93Wh7_lqDcs6zMaTS_QRr3KZM7RZnY,431
 pyttsx4/drivers/__init__.py,sha256=EFf83iBpSVF4joEh4gQmq5Rl22tngVNuR1zBeWfCdjQ,853
 pyttsx4/drivers/_espeak.py,sha256=Gj0N4aFf3YGZO9fq8K5BFbiwkIExqDu1nBXUn7EZVzY,19495
 pyttsx4/drivers/dummy.py,sha256=d7K46sijjOxwmAJHbgEALwbYwGcktLfW1FcX1iG5I8E,6182
 pyttsx4/drivers/espeak.py,sha256=p2-L60Qrl6wVoSrGlQM6jWQhammXJL-UvCxsDoPZaow,6801
 pyttsx4/drivers/nsss.py,sha256=n849K4ugK87S4ejtc_7xYp5W__maB6vfRX_sxIWlGIU,3729
-pyttsx4/drivers/sapi5.py,sha256=_KPHJdxEUdR13vnltalb8UCWxEcldpjNm9cawYfE6T4,5877
-pyttsx4-3.0.2.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-pyttsx4-3.0.2.dist-info/METADATA,sha256=5pHt2RXkqIUKRALTC06Y_lA4ZOIXfuUTJDtT5WKMF1A,1821
-pyttsx4-3.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyttsx4-3.0.2.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
-pyttsx4-3.0.2.dist-info/RECORD,,
+pyttsx4/drivers/sapi5.py,sha256=ZZ4sd9Ef0RAMX3aDnPPUSTNaqogjY-06vR-4v6Hzv6k,6047
+pyttsx4-3.0.3.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+pyttsx4-3.0.3.dist-info/METADATA,sha256=YBFkFDKlbOlwjEmFN_mevkhVyzXWgGdM2jf2C7yhgx8,1821
+pyttsx4-3.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyttsx4-3.0.3.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
+pyttsx4-3.0.3.dist-info/RECORD,,
```

