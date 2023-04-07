# Comparing `tmp/cassettedeck-2.2.0.tar.gz` & `tmp/cassettedeck-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cassettedeck-2.2.0.tar", last modified: Wed Jan 20 21:35:19 2021, max compression
+gzip compressed data, was "cassettedeck-2.2.1.tar", last modified: Fri Apr  7 19:48:03 2023, max compression
```

## Comparing `cassettedeck-2.2.0.tar` & `cassettedeck-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      633 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/test-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2405 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      593 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/vcr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/cassette.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5887 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/store.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3708 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/deck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/tests/test_vcr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5898 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/tests/test_works.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1333 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/tests/fixtures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/cassettedeck/request.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      633 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      590 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/cassettedeck.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2021-01-20 21:35:19.000000 cassettedeck-2.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      980 2021-01-20 21:34:35.000000 cassettedeck-2.2.0/setup.py
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.519632 cassettedeck-2.2.1/
+-rw-r--r--   0 ismael     (502) staff       (20)      359 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/MANIFEST.in
+-rw-r--r--   0 ismael     (502) staff       (20)      633 2023-04-07 19:48:03.520080 cassettedeck-2.2.1/PKG-INFO
+-rw-r--r--   0 ismael     (502) staff       (20)     3295 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/README.md
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.516685 cassettedeck-2.2.1/cassettedeck/
+-rw-r--r--   0 ismael     (502) staff       (20)      122 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/__init__.py
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/cassette.py
+-rw-r--r--   0 ismael     (502) staff       (20)     3708 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/deck.py
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/request.py
+-rw-r--r--   0 ismael     (502) staff       (20)     2405 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/service.py
+-rw-r--r--   0 ismael     (502) staff       (20)     5887 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/store.py
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.519460 cassettedeck-2.2.1/cassettedeck/tests/
+-rw-r--r--   0 ismael     (502) staff       (20)        0 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/__init__.py
+-rw-r--r--   0 ismael     (502) staff       (20)       49 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/conftest.py
+-rw-r--r--   0 ismael     (502) staff       (20)     1333 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/fixtures.py
+-rw-r--r--   0 ismael     (502) staff       (20)      594 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/test_vcr.py
+-rw-r--r--   0 ismael     (502) staff       (20)     5898 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/tests/test_works.py
+-rw-r--r--   0 ismael     (502) staff       (20)      593 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/cassettedeck/vcr.py
+drwxr-xr-x   0 ismael     (502) staff       (20)        0 2023-04-07 19:48:03.518436 cassettedeck-2.2.1/cassettedeck.egg-info/
+-rw-r--r--   0 ismael     (502) staff       (20)      633 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/PKG-INFO
+-rw-r--r--   0 ismael     (502) staff       (20)      590 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/SOURCES.txt
+-rw-r--r--   0 ismael     (502) staff       (20)        1 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/dependency_links.txt
+-rw-r--r--   0 ismael     (502) staff       (20)       41 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/requires.txt
+-rw-r--r--   0 ismael     (502) staff       (20)       13 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/top_level.txt
+-rw-r--r--   0 ismael     (502) staff       (20)        1 2023-04-07 19:48:03.000000 cassettedeck-2.2.1/cassettedeck.egg-info/zip-safe
+-rw-r--r--   0 ismael     (502) staff       (20)       80 2023-04-07 19:48:03.521123 cassettedeck-2.2.1/setup.cfg
+-rw-r--r--   0 ismael     (502) staff       (20)      980 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/setup.py
+-rw-r--r--   0 ismael     (502) staff       (20)       58 2023-04-07 19:47:24.000000 cassettedeck-2.2.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cassettedeck-2.2.0/PKG-INFO` & `cassettedeck-2.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassettedeck
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library store and replay aiohttp requests
 Home-page: http://github.com/onna/cassettedeck
 Author: Developer team at Onna Technologies
 Author-email: dev@onna.com
 License: Public
 Description: To simplify and speed up tests that make HTTP requests
 Platform: UNKNOWN
```

### Comparing `cassettedeck-2.2.0/README.md` & `cassettedeck-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/service.py` & `cassettedeck-2.2.1/cassettedeck/service.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/vcr.py` & `cassettedeck-2.2.1/cassettedeck/vcr.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/store.py` & `cassettedeck-2.2.1/cassettedeck/store.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/deck.py` & `cassettedeck-2.2.1/cassettedeck/deck.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/tests/test_vcr.py` & `cassettedeck-2.2.1/cassettedeck/tests/test_vcr.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/tests/test_works.py` & `cassettedeck-2.2.1/cassettedeck/tests/test_works.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck/tests/fixtures.py` & `cassettedeck-2.2.1/cassettedeck/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/cassettedeck.egg-info/PKG-INFO` & `cassettedeck-2.2.1/cassettedeck.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cassettedeck
-Version: 2.2.0
+Version: 2.2.1
 Summary: A library store and replay aiohttp requests
 Home-page: http://github.com/onna/cassettedeck
 Author: Developer team at Onna Technologies
 Author-email: dev@onna.com
 License: Public
 Description: To simplify and speed up tests that make HTTP requests
 Platform: UNKNOWN
```

### Comparing `cassettedeck-2.2.0/cassettedeck.egg-info/SOURCES.txt` & `cassettedeck-2.2.1/cassettedeck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cassettedeck-2.2.0/setup.py` & `cassettedeck-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 
 setup(
     name="cassettedeck",
-    version="2.2.0",
+    version="2.2.1",
     description="A library store and replay aiohttp requests",
     long_description="To simplify and speed up tests that make HTTP requests",
     author="Developer team at Onna Technologies",
     author_email="dev@onna.com",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Development Status :: 3 - Alpha",
@@ -22,11 +22,11 @@
     zip_safe=True,
     include_package_data=True,
     package_data={"": ["*.txt", "*.rst"]},
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "aiounittest",
-        "vcrpy==1.12.0",
+        "vcrpy>=1.12.0",
         "pyyaml",
     ],
 )
```

