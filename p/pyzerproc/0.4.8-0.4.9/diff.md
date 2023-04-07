# Comparing `tmp/pyzerproc-0.4.8.tar.gz` & `tmp/pyzerproc-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyzerproc-0.4.8.tar", last modified: Fri Feb 12 20:11:06 2021, max compression
+gzip compressed data, was "dist/pyzerproc-0.4.9.tar", last modified: Sun Mar 28 22:50:49 2021, max compression
```

## Comparing `pyzerproc-0.4.8.tar` & `pyzerproc-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/
--rw-r--r--   0 emily     (1000) emily     (1000)       85 2020-12-18 00:20:12.000000 pyzerproc-0.4.8/.coveragerc
--rw-r--r--   0 emily     (1000) emily     (1000)      292 2020-05-03 21:48:25.000000 pyzerproc-0.4.8/.editorconfig
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/.github/
--rw-r--r--   0 emily     (1000) emily     (1000)      320 2020-05-03 22:06:07.000000 pyzerproc-0.4.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 emily     (1000) emily     (1000)     1196 2020-05-03 21:48:25.000000 pyzerproc-0.4.8/.gitignore
--rw-r--r--   0 emily     (1000) emily     (1000)     3021 2020-05-03 22:05:52.000000 pyzerproc-0.4.8/CONTRIBUTING.rst
--rw-r--r--   0 emily     (1000) emily     (1000)      583 2020-05-03 21:48:25.000000 pyzerproc-0.4.8/LICENSE
--rw-r--r--   0 emily     (1000) emily     (1000)      217 2020-05-03 22:01:12.000000 pyzerproc-0.4.8/MANIFEST.in
--rw-r--r--   0 emily     (1000) emily     (1000)     1838 2020-05-03 22:01:48.000000 pyzerproc-0.4.8/Makefile
--rw-r--r--   0 emily     (1000) emily     (1000)     8863 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/PKG-INFO
--rw-r--r--   0 emily     (1000) emily     (1000)     6089 2021-02-12 20:07:56.000000 pyzerproc-0.4.8/README.rst
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/pyzerproc/
--rw-r--r--   0 emily     (1000) emily     (1000)      266 2021-02-12 20:07:56.000000 pyzerproc-0.4.8/pyzerproc/__init__.py
--rw-r--r--   0 emily     (1000) emily     (1000)     3223 2020-12-17 21:54:13.000000 pyzerproc-0.4.8/pyzerproc/cli.py
--rw-r--r--   0 emily     (1000) emily     (1000)     1032 2020-12-23 17:22:34.000000 pyzerproc-0.4.8/pyzerproc/discovery.py
--rw-r--r--   0 emily     (1000) emily     (1000)      112 2020-05-09 18:04:15.000000 pyzerproc-0.4.8/pyzerproc/exceptions.py
--rw-r--r--   0 emily     (1000) emily     (1000)     7726 2020-12-20 21:53:54.000000 pyzerproc-0.4.8/pyzerproc/light.py
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/pyzerproc.egg-info/
--rw-r--r--   0 emily     (1000) emily     (1000)     8863 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/PKG-INFO
--rw-r--r--   0 emily     (1000) emily     (1000)      584 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/SOURCES.txt
--rw-r--r--   0 emily     (1000) emily     (1000)        1 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/dependency_links.txt
--rw-r--r--   0 emily     (1000) emily     (1000)       50 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/entry_points.txt
--rw-r--r--   0 emily     (1000) emily     (1000)        1 2020-05-03 22:07:06.000000 pyzerproc-0.4.8/pyzerproc.egg-info/not-zip-safe
--rw-r--r--   0 emily     (1000) emily     (1000)       25 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/requires.txt
--rw-r--r--   0 emily     (1000) emily     (1000)       10 2021-02-12 20:11:05.000000 pyzerproc-0.4.8/pyzerproc.egg-info/top_level.txt
--rw-r--r--   0 emily     (1000) emily     (1000)      215 2021-02-12 20:03:21.000000 pyzerproc-0.4.8/requirements_dev.txt
--rw-r--r--   0 emily     (1000) emily     (1000)      132 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/setup.cfg
--rw-r--r--   0 emily     (1000) emily     (1000)     1426 2021-02-12 19:12:23.000000 pyzerproc-0.4.8/setup.py
-drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-02-12 20:11:06.000000 pyzerproc-0.4.8/tests/
--rw-r--r--   0 emily     (1000) emily     (1000)       39 2020-05-03 21:48:26.000000 pyzerproc-0.4.8/tests/__init__.py
--rw-r--r--   0 emily     (1000) emily     (1000)      976 2021-02-12 20:03:21.000000 pyzerproc-0.4.8/tests/conftest.py
--rw-r--r--   0 emily     (1000) emily     (1000)     2048 2020-12-17 23:13:00.000000 pyzerproc-0.4.8/tests/test_discovery.py
--rw-r--r--   0 emily     (1000) emily     (1000)     7205 2021-02-12 20:03:21.000000 pyzerproc-0.4.8/tests/test_light.py
--rw-r--r--   0 emily     (1000) emily     (1000)      541 2021-02-12 20:03:21.000000 pyzerproc-0.4.8/tox.ini
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/
+-rw-r--r--   0 emily     (1000) emily     (1000)       85 2020-12-18 00:20:12.000000 pyzerproc-0.4.9/.coveragerc
+-rw-r--r--   0 emily     (1000) emily     (1000)      292 2020-05-03 21:48:25.000000 pyzerproc-0.4.9/.editorconfig
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/.github/
+-rw-r--r--   0 emily     (1000) emily     (1000)      320 2020-05-03 22:06:07.000000 pyzerproc-0.4.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 emily     (1000) emily     (1000)     1196 2020-05-03 21:48:25.000000 pyzerproc-0.4.9/.gitignore
+-rw-r--r--   0 emily     (1000) emily     (1000)     3021 2020-05-03 22:05:52.000000 pyzerproc-0.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 emily     (1000) emily     (1000)      583 2020-05-03 21:48:25.000000 pyzerproc-0.4.9/LICENSE
+-rw-r--r--   0 emily     (1000) emily     (1000)      217 2020-05-03 22:01:12.000000 pyzerproc-0.4.9/MANIFEST.in
+-rw-r--r--   0 emily     (1000) emily     (1000)     1838 2020-05-03 22:01:48.000000 pyzerproc-0.4.9/Makefile
+-rw-r--r--   0 emily     (1000) emily     (1000)     9017 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/PKG-INFO
+-rw-r--r--   0 emily     (1000) emily     (1000)     6211 2021-03-28 22:49:56.000000 pyzerproc-0.4.9/README.rst
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc/
+-rw-r--r--   0 emily     (1000) emily     (1000)      266 2021-03-28 22:47:56.000000 pyzerproc-0.4.9/pyzerproc/__init__.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     3223 2020-12-17 21:54:13.000000 pyzerproc-0.4.9/pyzerproc/cli.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     1032 2020-12-23 17:22:34.000000 pyzerproc-0.4.9/pyzerproc/discovery.py
+-rw-r--r--   0 emily     (1000) emily     (1000)      112 2020-05-09 18:04:15.000000 pyzerproc-0.4.9/pyzerproc/exceptions.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     7726 2020-12-20 21:53:54.000000 pyzerproc-0.4.9/pyzerproc/light.py
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/
+-rw-r--r--   0 emily     (1000) emily     (1000)     9017 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/PKG-INFO
+-rw-r--r--   0 emily     (1000) emily     (1000)      584 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/SOURCES.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)        1 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/dependency_links.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)       50 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/entry_points.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)        1 2020-05-03 22:07:06.000000 pyzerproc-0.4.9/pyzerproc.egg-info/not-zip-safe
+-rw-r--r--   0 emily     (1000) emily     (1000)       25 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/requires.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)       10 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/pyzerproc.egg-info/top_level.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)      215 2021-03-28 22:45:48.000000 pyzerproc-0.4.9/requirements_dev.txt
+-rw-r--r--   0 emily     (1000) emily     (1000)      132 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/setup.cfg
+-rw-r--r--   0 emily     (1000) emily     (1000)     1430 2021-03-28 22:45:48.000000 pyzerproc-0.4.9/setup.py
+drwxr-xr-x   0 emily     (1000) emily     (1000)        0 2021-03-28 22:50:49.000000 pyzerproc-0.4.9/tests/
+-rw-r--r--   0 emily     (1000) emily     (1000)       39 2020-05-03 21:48:26.000000 pyzerproc-0.4.9/tests/__init__.py
+-rw-r--r--   0 emily     (1000) emily     (1000)      976 2021-03-28 22:35:33.000000 pyzerproc-0.4.9/tests/conftest.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     2048 2020-12-17 23:13:00.000000 pyzerproc-0.4.9/tests/test_discovery.py
+-rw-r--r--   0 emily     (1000) emily     (1000)     7251 2021-03-28 22:45:48.000000 pyzerproc-0.4.9/tests/test_light.py
+-rw-r--r--   0 emily     (1000) emily     (1000)      551 2021-03-28 22:45:48.000000 pyzerproc-0.4.9/tox.ini
```

### Comparing `pyzerproc-0.4.8/.gitignore` & `pyzerproc-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/CONTRIBUTING.rst` & `pyzerproc-0.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/LICENSE` & `pyzerproc-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/Makefile` & `pyzerproc-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/PKG-INFO` & `pyzerproc-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyzerproc
-Version: 0.4.8
+Version: 0.4.9
 Summary: Async library to control Zerproc Bluetooth LED smart string lights
 Home-page: https://github.com/emlove/pyzerproc
 Author: Emily Mills
 Author-email: emily@emlove.me
 License: Apache Software License 2.0
 Description: =========
         pyzerproc
@@ -173,14 +173,18 @@
                         print("Off")
                 finally:
                     await light.disconnect()
         
         
         Changelog
         ---------
+        0.4.9 (2021-03-28)
+        ~~~~~~~~~~~~~~~~~~
+        - Upgrade to `bleak 0.11.0 <https://github.com/hbldh/bleak/releases/tag/v0.11.0>`_
+        
         0.4.8 (2021-02-12)
         ~~~~~~~~~~~~~~~~~~
         - Dependency cleanup `(#1) <https://github.com/emlove/pyzerproc/pull/1>`_ `(#3) <https://github.com/emlove/pyzerproc/issues/3>`_ `@fabaff <https://github.com/fabaff>`_
         
         0.4.7 (2020-12-20)
         ~~~~~~~~~~~~~~~~~~
         - Include a default timeout on all remote calls
```

### Comparing `pyzerproc-0.4.8/README.rst` & `pyzerproc-0.4.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -165,14 +165,18 @@
                 print("Off")
         finally:
             await light.disconnect()
 
 
 Changelog
 ---------
+0.4.9 (2021-03-28)
+~~~~~~~~~~~~~~~~~~
+- Upgrade to `bleak 0.11.0 <https://github.com/hbldh/bleak/releases/tag/v0.11.0>`_
+
 0.4.8 (2021-02-12)
 ~~~~~~~~~~~~~~~~~~
 - Dependency cleanup `(#1) <https://github.com/emlove/pyzerproc/pull/1>`_ `(#3) <https://github.com/emlove/pyzerproc/issues/3>`_ `@fabaff <https://github.com/fabaff>`_
 
 0.4.7 (2020-12-20)
 ~~~~~~~~~~~~~~~~~~
 - Include a default timeout on all remote calls
```

### Comparing `pyzerproc-0.4.8/pyzerproc/cli.py` & `pyzerproc-0.4.9/pyzerproc/cli.py`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/pyzerproc/discovery.py` & `pyzerproc-0.4.9/pyzerproc/discovery.py`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/pyzerproc/light.py` & `pyzerproc-0.4.9/pyzerproc/light.py`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/pyzerproc.egg-info/PKG-INFO` & `pyzerproc-0.4.9/pyzerproc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pyzerproc
-Version: 0.4.8
+Version: 0.4.9
 Summary: Async library to control Zerproc Bluetooth LED smart string lights
 Home-page: https://github.com/emlove/pyzerproc
 Author: Emily Mills
 Author-email: emily@emlove.me
 License: Apache Software License 2.0
 Description: =========
         pyzerproc
@@ -173,14 +173,18 @@
                         print("Off")
                 finally:
                     await light.disconnect()
         
         
         Changelog
         ---------
+        0.4.9 (2021-03-28)
+        ~~~~~~~~~~~~~~~~~~
+        - Upgrade to `bleak 0.11.0 <https://github.com/hbldh/bleak/releases/tag/v0.11.0>`_
+        
         0.4.8 (2021-02-12)
         ~~~~~~~~~~~~~~~~~~
         - Dependency cleanup `(#1) <https://github.com/emlove/pyzerproc/pull/1>`_ `(#3) <https://github.com/emlove/pyzerproc/issues/3>`_ `@fabaff <https://github.com/fabaff>`_
         
         0.4.7 (2020-12-20)
         ~~~~~~~~~~~~~~~~~~
         - Include a default timeout on all remote calls
```

### Comparing `pyzerproc-0.4.8/pyzerproc.egg-info/SOURCES.txt` & `pyzerproc-0.4.9/pyzerproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/setup.py` & `pyzerproc-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from pyzerproc import __author__, __email__, __version__
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 requirements = [
     'Click>=7.0',
-    'bleak>=0.10.0',
+    'bleak>=0.11.0',
 ]
 
-test_requirements = ['pytest>=3', ]
+test_requirements = ['pytest>=6.2.2', ]
 
 setup(
     author=__author__,
     author_email=__email__,
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `pyzerproc-0.4.8/tests/conftest.py` & `pyzerproc-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/tests/test_discovery.py` & `pyzerproc-0.4.9/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pyzerproc-0.4.8/tests/test_light.py` & `pyzerproc-0.4.9/tests/test_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,26 @@
 
 
 @pytest.mark.asyncio
 async def test_is_connected(client):
     """Test turning on the light."""
     light = Light("00:11:22")
     await light.connect()
-    client.is_connected.side_effect = None
 
-    client.is_connected.return_value = False
+    connected = False
+
+    async def is_connected():
+        nonlocal connected
+        return connected
+
+    client.is_connected.side_effect = is_connected
 
     assert not await light.is_connected()
 
-    client.is_connected.return_value = True
+    connected = True
 
     assert await light.is_connected()
 
     client.is_connected.side_effect = asyncio.TimeoutError("Mock timeout")
 
     assert not await light.is_connected()
```

### Comparing `pyzerproc-0.4.8/tox.ini` & `pyzerproc-0.4.9/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     PYTHONPATH = {toxinidir}
 deps =
     -r{toxinidir}/requirements_dev.txt
 ; If you want to make tox run the tests with the same versions, create a
 ; requirements.txt with the pinned versions and uncomment the following line:
 ;     -r{toxinidir}/requirements.txt
 commands =
-    pytest --cov --cov-report term-missing
+    pytest --cov --cov-report term-missing {posargs}
 
 [testenv:flake8]
 basepython = python
 commands = flake8 pyzerproc tests
 
 [testenv:{py36,py37}]
 deps =
```

