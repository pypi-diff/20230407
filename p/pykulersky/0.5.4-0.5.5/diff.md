# Comparing `tmp/pykulersky-0.5.4.tar.gz` & `tmp/pykulersky-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykulersky-0.5.4.tar", last modified: Tue May  3 16:53:04 2022, max compression
+gzip compressed data, was "pykulersky-0.5.5.tar", last modified: Fri Apr  7 17:14:02 2023, max compression
```

## Comparing `pykulersky-0.5.4.tar` & `pykulersky-0.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:53:04.671999 pykulersky-0.5.4/
--rw-r--r--   0 emilylovemills   (502) staff       (20)     3031 2021-11-23 15:01:40.000000 pykulersky-0.5.4/CONTRIBUTING.rst
--rw-r--r--   0 emilylovemills   (502) staff       (20)      583 2021-11-23 15:01:40.000000 pykulersky-0.5.4/LICENSE
--rw-r--r--   0 emilylovemills   (502) staff       (20)      217 2021-11-23 15:01:40.000000 pykulersky-0.5.4/MANIFEST.in
--rw-r--r--   0 emilylovemills   (502) staff       (20)     5819 2022-05-03 16:53:04.672252 pykulersky-0.5.4/PKG-INFO
--rw-r--r--   0 emilylovemills   (502) staff       (20)     5076 2022-05-03 16:52:21.000000 pykulersky-0.5.4/README.rst
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:53:04.664346 pykulersky-0.5.4/pykulersky/
--rw-r--r--   0 emilylovemills   (502) staff       (20)      260 2022-05-03 16:52:34.000000 pykulersky-0.5.4/pykulersky/__init__.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     2027 2021-11-23 15:01:40.000000 pykulersky-0.5.4/pykulersky/cli.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)      992 2021-11-23 15:01:40.000000 pykulersky-0.5.4/pykulersky/discovery.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)      119 2021-11-23 15:01:40.000000 pykulersky-0.5.4/pykulersky/exceptions.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     5573 2021-11-23 15:01:40.000000 pykulersky-0.5.4/pykulersky/light.py
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:53:04.668619 pykulersky-0.5.4/pykulersky.egg-info/
--rw-r--r--   0 emilylovemills   (502) staff       (20)     5819 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/PKG-INFO
--rw-r--r--   0 emilylovemills   (502) staff       (20)      495 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/SOURCES.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/dependency_links.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       52 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/entry_points.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2021-11-23 15:01:56.000000 pykulersky-0.5.4/pykulersky.egg-info/not-zip-safe
--rw-r--r--   0 emilylovemills   (502) staff       (20)       25 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/requires.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       11 2022-05-03 16:53:04.000000 pykulersky-0.5.4/pykulersky.egg-info/top_level.txt
--rw-r--r--   0 emilylovemills   (502) staff       (20)       92 2022-05-03 16:53:04.673040 pykulersky-0.5.4/setup.cfg
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1432 2021-11-23 15:14:54.000000 pykulersky-0.5.4/setup.py
-drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2022-05-03 16:53:04.671194 pykulersky-0.5.4/tests/
--rw-r--r--   0 emilylovemills   (502) staff       (20)       40 2021-11-23 15:01:40.000000 pykulersky-0.5.4/tests/__init__.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1074 2021-11-23 15:01:40.000000 pykulersky-0.5.4/tests/conftest.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     1777 2021-11-23 15:01:40.000000 pykulersky-0.5.4/tests/test_discovery.py
--rw-r--r--   0 emilylovemills   (502) staff       (20)     5306 2021-11-23 15:01:40.000000 pykulersky-0.5.4/tests/test_light.py
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-04-07 17:14:02.988457 pykulersky-0.5.5/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     3031 2021-11-23 15:01:40.000000 pykulersky-0.5.5/CONTRIBUTING.rst
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      583 2021-11-23 15:01:40.000000 pykulersky-0.5.5/LICENSE
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      217 2021-11-23 15:01:40.000000 pykulersky-0.5.5/MANIFEST.in
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5886 2023-04-07 17:14:02.988683 pykulersky-0.5.5/PKG-INFO
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5143 2023-04-07 17:08:41.000000 pykulersky-0.5.5/README.rst
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-04-07 17:14:02.981433 pykulersky-0.5.5/pykulersky/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      260 2023-04-07 17:03:13.000000 pykulersky-0.5.5/pykulersky/__init__.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     2027 2021-11-23 15:01:40.000000 pykulersky-0.5.5/pykulersky/cli.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      992 2021-11-23 15:01:40.000000 pykulersky-0.5.5/pykulersky/discovery.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      119 2021-11-23 15:01:40.000000 pykulersky-0.5.5/pykulersky/exceptions.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5573 2021-11-23 15:01:40.000000 pykulersky-0.5.5/pykulersky/light.py
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-04-07 17:14:02.984965 pykulersky-0.5.5/pykulersky.egg-info/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5886 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/PKG-INFO
+-rw-r--r--   0 emilylovemills   (502) staff       (20)      495 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/SOURCES.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/dependency_links.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       52 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/entry_points.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)        1 2021-11-23 15:01:56.000000 pykulersky-0.5.5/pykulersky.egg-info/not-zip-safe
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       25 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/requires.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       11 2023-04-07 17:14:02.000000 pykulersky-0.5.5/pykulersky.egg-info/top_level.txt
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       92 2023-04-07 17:14:02.989640 pykulersky-0.5.5/setup.cfg
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     1432 2023-04-07 17:01:53.000000 pykulersky-0.5.5/setup.py
+drwxr-xr-x   0 emilylovemills   (502) staff       (20)        0 2023-04-07 17:14:02.987918 pykulersky-0.5.5/tests/
+-rw-r--r--   0 emilylovemills   (502) staff       (20)       40 2021-11-23 15:01:40.000000 pykulersky-0.5.5/tests/__init__.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     1074 2021-11-23 15:01:40.000000 pykulersky-0.5.5/tests/conftest.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     1757 2023-04-07 17:00:28.000000 pykulersky-0.5.5/tests/test_discovery.py
+-rw-r--r--   0 emilylovemills   (502) staff       (20)     5306 2021-11-23 15:01:40.000000 pykulersky-0.5.5/tests/test_light.py
```

### Comparing `pykulersky-0.5.4/CONTRIBUTING.rst` & `pykulersky-0.5.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/LICENSE` & `pykulersky-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/PKG-INFO` & `pykulersky-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykulersky
-Version: 0.5.4
+Version: 0.5.5
 Summary: Library to control Brightech Kuler Sky Bluetooth LED smart lamps
 Home-page: https://github.com/emlove/pykulersky
 Author: Emily Love Mills
 Author-email: emily@emlove.me
 License: Apache Software License 2.0
 Keywords: pykulersky
 Platform: UNKNOWN
@@ -170,14 +170,18 @@
             await light.disconnect()
 
     asyncio.get_event_loop().run_until_complete(main())
 
 
 Changelog
 ---------
+0.5.5 (2023-04-07)
+~~~~~~~~~~~~~~~~~~
+- Support CI for bleak 0.20
+
 0.5.4 (2022-05-03)
 ~~~~~~~~~~~~~~~~~~
 - Unpin test dependencies
 
 0.5.3 (2021-11-23)
 ~~~~~~~~~~~~~~~~~~
 - Support CI for bleak 0.13
```

### Comparing `pykulersky-0.5.4/README.rst` & `pykulersky-0.5.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,18 @@
             await light.disconnect()
 
     asyncio.get_event_loop().run_until_complete(main())
 
 
 Changelog
 ---------
+0.5.5 (2023-04-07)
+~~~~~~~~~~~~~~~~~~
+- Support CI for bleak 0.20
+
 0.5.4 (2022-05-03)
 ~~~~~~~~~~~~~~~~~~
 - Unpin test dependencies
 
 0.5.3 (2021-11-23)
 ~~~~~~~~~~~~~~~~~~
 - Support CI for bleak 0.13
```

### Comparing `pykulersky-0.5.4/pykulersky/cli.py` & `pykulersky-0.5.5/pykulersky/cli.py`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/pykulersky/discovery.py` & `pykulersky-0.5.5/pykulersky/discovery.py`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/pykulersky/light.py` & `pykulersky-0.5.5/pykulersky/light.py`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/pykulersky.egg-info/PKG-INFO` & `pykulersky-0.5.5/pykulersky.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykulersky
-Version: 0.5.4
+Version: 0.5.5
 Summary: Library to control Brightech Kuler Sky Bluetooth LED smart lamps
 Home-page: https://github.com/emlove/pykulersky
 Author: Emily Love Mills
 Author-email: emily@emlove.me
 License: Apache Software License 2.0
 Keywords: pykulersky
 Platform: UNKNOWN
@@ -170,14 +170,18 @@
             await light.disconnect()
 
     asyncio.get_event_loop().run_until_complete(main())
 
 
 Changelog
 ---------
+0.5.5 (2023-04-07)
+~~~~~~~~~~~~~~~~~~
+- Support CI for bleak 0.20
+
 0.5.4 (2022-05-03)
 ~~~~~~~~~~~~~~~~~~
 - Unpin test dependencies
 
 0.5.3 (2021-11-23)
 ~~~~~~~~~~~~~~~~~~
 - Support CI for bleak 0.13
```

### Comparing `pykulersky-0.5.4/setup.py` & `pykulersky-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pykulersky import __author__, __email__, __version__
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 requirements = [
     'Click>=7.0',
-    'bleak>=0.11.0',
+    'bleak>=0.20.0',
 ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author=__author__,
     author_email=__email__,
```

### Comparing `pykulersky-0.5.4/tests/conftest.py` & `pykulersky-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pykulersky-0.5.4/tests/test_discovery.py` & `pykulersky-0.5.5/tests/test_discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,37 @@
     """Test the CLI."""
     async def scan(*args, **kwargs):
         """Simulate a scanning response"""
         return [
             bleak.backends.device.BLEDevice(
                 'AA:BB:CC:11:22:33',
                 'Living Room',
+                {},
+                0,
                 uuids=[
                     "8d96a001-0002-64c2-0001-9acc4838521c",
                 ],
-                manufacturer_data={}
             ),
             bleak.backends.device.BLEDevice(
-                address='AA:BB:CC:44:55:66',
-                name='Bedroom',
+                'AA:BB:CC:44:55:66',
+                'Bedroom',
+                {},
+                0,
                 uuids=[
                     "8d96a001-0002-64c2-0001-9acc4838521c",
                 ],
-                manufacturer_data={}
             ),
             bleak.backends.device.BLEDevice(
-                address='DD:EE:FF:11:22:33',
-                name='Other',
+                'DD:EE:FF:11:22:33',
+                'Other',
+                {},
+                0,
                 uuids=[
                     "0000fe9f-0000-1000-8000-00805f9b34fb",
                 ],
-                manufacturer_data={}
             ),
         ]
 
     scanner.discover.side_effect = scan
 
     devices = await discover(15)
```

### Comparing `pykulersky-0.5.4/tests/test_light.py` & `pykulersky-0.5.5/tests/test_light.py`

 * *Files identical despite different names*

