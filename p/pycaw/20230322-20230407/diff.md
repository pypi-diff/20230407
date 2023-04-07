# Comparing `tmp/pycaw-20230322.tar.gz` & `tmp/pycaw-20230407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaw-20230322.tar", last modified: Wed Mar 22 15:19:34 2023, max compression
+gzip compressed data, was "pycaw-20230407.tar", last modified: Fri Apr  7 21:38:45 2023, max compression
```

## Comparing `pycaw-20230322.tar` & `pycaw-20230407.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.865658 pycaw-20230322/
--rw-rw-rw-   0        0        0     1098 2023-03-22 15:18:32.000000 pycaw-20230322/LICENSE
--rw-rw-rw-   0        0        0     1681 2023-03-22 15:19:34.865658 pycaw-20230322/PKG-INFO
--rw-rw-rw-   0        0        0     1447 2023-03-22 15:18:32.000000 pycaw-20230322/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw/
--rw-rw-rw-   0        0        0        0 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw/api/
--rw-rw-rw-   0        0        0        0 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw/api/audioclient/
--rw-rw-rw-   0        0        0     4680 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/audioclient/__init__.py
--rw-rw-rw-   0        0        0      351 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/audioclient/depend.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw/api/audiopolicy/
--rw-rw-rw-   0        0        0    10383 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/audiopolicy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw/api/endpointvolume/
--rw-rw-rw-   0        0        0     6075 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/endpointvolume/__init__.py
--rw-rw-rw-   0        0        0      450 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/endpointvolume/depend.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.865658 pycaw-20230322/pycaw/api/mmdeviceapi/
--rw-rw-rw-   0        0        0     5807 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/mmdeviceapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.865658 pycaw-20230322/pycaw/api/mmdeviceapi/depend/
--rw-rw-rw-   0        0        0     1405 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/mmdeviceapi/depend/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/api/mmdeviceapi/depend/structures.py
--rw-rw-rw-   0        0        0    13721 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/callbacks.py
--rw-rw-rw-   0        0        0     1015 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/constants.py
--rw-rw-rw-   0        0        0    29677 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/magic.py
--rw-rw-rw-   0        0        0     1380 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/pycaw.py
--rw-rw-rw-   0        0        0     9276 2023-03-22 15:18:32.000000 pycaw-20230322/pycaw/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.850034 pycaw-20230322/pycaw.egg-info/
--rw-rw-rw-   0        0        0     1681 2023-03-22 15:19:34.000000 pycaw-20230322/pycaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-03-22 15:19:34.000000 pycaw-20230322/pycaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 15:19:34.000000 pycaw-20230322/pycaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-22 15:19:34.000000 pycaw-20230322/pycaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-22 15:19:34.000000 pycaw-20230322/pycaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 15:19:34.865658 pycaw-20230322/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-03-22 15:18:32.000000 pycaw-20230322/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 15:19:34.865658 pycaw-20230322/tests/
--rw-rw-rw-   0        0        0     2420 2023-03-22 15:18:32.000000 pycaw-20230322/tests/test_core.py
--rw-rw-rw-   0        0        0     1741 2023-03-22 15:18:32.000000 pycaw-20230322/tests/test_examples.py
--rw-rw-rw-   0        0        0     2710 2023-03-22 15:18:32.000000 pycaw-20230322/tests/test_magic.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/
+-rw-rw-rw-   0        0        0     1098 2023-04-07 21:37:58.000000 pycaw-20230407/LICENSE
+-rw-rw-rw-   0        0        0     1681 2023-04-07 21:38:45.196156 pycaw-20230407/PKG-INFO
+-rw-rw-rw-   0        0        0     1447 2023-04-07 21:37:58.000000 pycaw-20230407/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/audioclient/
+-rw-rw-rw-   0        0        0     4680 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/audioclient/__init__.py
+-rw-rw-rw-   0        0        0      351 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/audioclient/depend.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/audiopolicy/
+-rw-rw-rw-   0        0        0    10383 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/audiopolicy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/endpointvolume/
+-rw-rw-rw-   0        0        0     6075 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/endpointvolume/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/endpointvolume/depend.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/mmdeviceapi/
+-rw-rw-rw-   0        0        0     5807 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/mmdeviceapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw/api/mmdeviceapi/depend/
+-rw-rw-rw-   0        0        0     1405 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/mmdeviceapi/depend/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/api/mmdeviceapi/depend/structures.py
+-rw-rw-rw-   0        0        0    13721 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/callbacks.py
+-rw-rw-rw-   0        0        0     1015 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/constants.py
+-rw-rw-rw-   0        0        0    29677 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/magic.py
+-rw-rw-rw-   0        0        0     1380 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/pycaw.py
+-rw-rw-rw-   0        0        0     9233 2023-04-07 21:37:58.000000 pycaw-20230407/pycaw/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/pycaw.egg-info/
+-rw-rw-rw-   0        0        0     1681 2023-04-07 21:38:45.000000 pycaw-20230407/pycaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-04-07 21:38:45.000000 pycaw-20230407/pycaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 21:38:45.000000 pycaw-20230407/pycaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-07 21:38:45.000000 pycaw-20230407/pycaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-07 21:38:45.000000 pycaw-20230407/pycaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 21:38:45.196156 pycaw-20230407/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-04-07 21:37:58.000000 pycaw-20230407/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:38:45.196156 pycaw-20230407/tests/
+-rw-rw-rw-   0        0        0     2420 2023-04-07 21:37:58.000000 pycaw-20230407/tests/test_core.py
+-rw-rw-rw-   0        0        0     1741 2023-04-07 21:37:58.000000 pycaw-20230407/tests/test_examples.py
+-rw-rw-rw-   0        0        0     2710 2023-04-07 21:37:58.000000 pycaw-20230407/tests/test_magic.py
```

### Comparing `pycaw-20230322/LICENSE` & `pycaw-20230407/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/PKG-INFO` & `pycaw-20230407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaw
-Version: 20230322
+Version: 20230407
 Summary: Python Core Audio Windows Library
 Home-page: https://github.com/AndreMiras/pycaw
 Author: Andre Miras
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pycaw
```

### Comparing `pycaw-20230322/README.md` & `pycaw-20230407/README.md`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/audioclient/__init__.py` & `pycaw-20230407/pycaw/api/audioclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/audiopolicy/__init__.py` & `pycaw-20230407/pycaw/api/audiopolicy/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/endpointvolume/__init__.py` & `pycaw-20230407/pycaw/api/endpointvolume/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/mmdeviceapi/__init__.py` & `pycaw-20230407/pycaw/api/mmdeviceapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/mmdeviceapi/depend/__init__.py` & `pycaw-20230407/pycaw/api/mmdeviceapi/depend/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/api/mmdeviceapi/depend/structures.py` & `pycaw-20230407/pycaw/api/mmdeviceapi/depend/structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ctypes import Structure, Union
+from ctypes import Structure, Union, byref, windll
 from ctypes.wintypes import DWORD, LONG, LPWSTR, ULARGE_INTEGER, VARIANT_BOOL, WORD
 
 from comtypes import GUID
 from comtypes.automation import VARTYPE, VT_BOOL, VT_CLSID, VT_LPWSTR, VT_UI4
 
 
 class PROPVARIANT_UNION(Union):
@@ -36,14 +36,17 @@
         elif vt == VT_CLSID:
             # TODO
             # return (Guid)Marshal.PtrToStructure(union.puuid, typeof(Guid))
             return
         else:
             return "%s:?" % (vt)
 
+    def clear(self):
+        windll.ole32.PropVariantClear(byref(self))
+
 
 class PROPERTYKEY(Structure):
     _fields_ = [
         ("fmtid", GUID),
         ("pid", DWORD),
     ]
```

### Comparing `pycaw-20230322/pycaw/callbacks.py` & `pycaw-20230407/pycaw/callbacks.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/constants.py` & `pycaw-20230407/pycaw/constants.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/magic.py` & `pycaw-20230407/pycaw/magic.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/pycaw.py` & `pycaw-20230407/pycaw/pycaw.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/pycaw/utils.py` & `pycaw-20230407/pycaw/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,15 @@
                     v = value.GetValue()
                 except COMError as exc:
                     warnings.warn(
                         "COMError attempting to get property %r "
                         "from device %r: %r" % (j, dev, exc)
                     )
                     continue
-                # TODO
-                # PropVariantClear(byref(value))
+                value.clear()
                 name = str(pk)
                 properties[name] = v
         audioState = AudioDeviceState(state)
         return AudioDevice(id, audioState, properties, dev)
 
     @staticmethod
     def GetAllDevices():
```

### Comparing `pycaw-20230322/pycaw.egg-info/PKG-INFO` & `pycaw-20230407/pycaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaw
-Version: 20230322
+Version: 20230407
 Summary: Python Core Audio Windows Library
 Home-page: https://github.com/AndreMiras/pycaw
 Author: Andre Miras
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pycaw
```

### Comparing `pycaw-20230322/pycaw.egg-info/SOURCES.txt` & `pycaw-20230407/pycaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/setup.py` & `pycaw-20230407/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 install_requires = ["comtypes", "psutil"]
 setup(
     name="pycaw",
-    version="20230322",
+    version="20230407",
     description="Python Core Audio Windows Library",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Andre Miras",
     url="https://github.com/AndreMiras/pycaw",
     packages=find_packages(exclude=("tests", "examples")),
     install_requires=install_requires,
```

### Comparing `pycaw-20230322/tests/test_core.py` & `pycaw-20230407/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/tests/test_examples.py` & `pycaw-20230407/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pycaw-20230322/tests/test_magic.py` & `pycaw-20230407/tests/test_magic.py`

 * *Files identical despite different names*

