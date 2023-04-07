# Comparing `tmp/isimport-0.1.tar.gz` & `tmp/isimport-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isimport-0.1.tar", last modified: Fri Apr  7 16:07:06 2023, max compression
+gzip compressed data, was "isimport-0.2.tar", last modified: Fri Apr  7 16:31:13 2023, max compression
```

## Comparing `isimport-0.1.tar` & `isimport-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 16:07:06.143205 isimport-0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-07 15:33:16.000000 isimport-0.1/LICENSE
--rw-rw-rw-   0        0        0      624 2023-04-07 16:07:06.142197 isimport-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-07 15:44:00.000000 isimport-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 16:07:06.114199 isimport-0.1/isimport/
--rw-rw-rw-   0        0        0     2900 2023-04-07 15:14:51.000000 isimport-0.1/isimport/__init__.py
--rw-rw-rw-   0        0        0       73 2023-04-07 14:53:40.000000 isimport-0.1/isimport/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:07:06.130053 isimport-0.1/isimport.egg-info/
--rw-rw-rw-   0        0        0      624 2023-04-07 16:07:05.000000 isimport-0.1/isimport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-07 16:07:06.000000 isimport-0.1/isimport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 16:07:05.000000 isimport-0.1/isimport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-07 16:07:05.000000 isimport-0.1/isimport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 16:07:05.000000 isimport-0.1/isimport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 16:07:06.144213 isimport-0.1/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-04-07 15:55:51.000000 isimport-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:31:13.974753 isimport-0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-07 15:33:16.000000 isimport-0.2/LICENSE
+-rw-rw-rw-   0        0        0      624 2023-04-07 16:31:13.961906 isimport-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-07 15:44:00.000000 isimport-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 16:31:13.939297 isimport-0.2/isimport/
+-rw-rw-rw-   0        0        0     2900 2023-04-07 15:14:51.000000 isimport-0.2/isimport/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-04-07 14:53:40.000000 isimport-0.2/isimport/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:31:13.959907 isimport-0.2/isimport.egg-info/
+-rw-rw-rw-   0        0        0      624 2023-04-07 16:31:13.000000 isimport-0.2/isimport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-07 16:31:13.000000 isimport-0.2/isimport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:31:13.000000 isimport-0.2/isimport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-07 16:31:13.000000 isimport-0.2/isimport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-07 16:31:13.000000 isimport-0.2/isimport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 16:31:13.974753 isimport-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2023-04-07 16:30:15.000000 isimport-0.2/setup.py
```

### Comparing `isimport-0.1/LICENSE` & `isimport-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isimport-0.1/PKG-INFO` & `isimport-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimport
-Version: 0.1
+Version: 0.2
 Summary: Check required pip module for program.
 Author: Ankush Bhagat (Ankush Bhagat)
 Author-email: <ankushbhagatofficial@gmail.com>
 Keywords: python,module,import,package,find
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `isimport-0.1/isimport/__init__.py` & `isimport-0.2/isimport/__init__.py`

 * *Files identical despite different names*

### Comparing `isimport-0.1/isimport.egg-info/PKG-INFO` & `isimport-0.2/isimport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isimport
-Version: 0.1
+Version: 0.2
 Summary: Check required pip module for program.
 Author: Ankush Bhagat (Ankush Bhagat)
 Author-email: <ankushbhagatofficial@gmail.com>
 Keywords: python,module,import,package,find
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `isimport-0.1/setup.py` & `isimport-0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1'
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = '0.2'
 DESCRIPTION = 'Check required pip module for program.'
 LONG_DESCRIPTION = 'A package that check required pip module to be installed on system.'
 
 # Setting up
 setup(
     name="isimport",
     version=VERSION,
```

