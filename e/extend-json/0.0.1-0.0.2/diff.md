# Comparing `tmp/extend-json-0.0.1.tar.gz` & `tmp/extend-json-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend-json-0.0.1.tar", last modified: Fri Apr  7 15:13:13 2023, max compression
+gzip compressed data, was "extend-json-0.0.2.tar", last modified: Fri Apr  7 15:42:48 2023, max compression
```

## Comparing `extend-json-0.0.1.tar` & `extend-json-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 15:13:13.534798 extend-json-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-04-07 12:07:07.000000 extend-json-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      756 2023-04-07 15:13:13.533797 extend-json-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-04-07 15:03:47.000000 extend-json-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 15:13:13.498802 extend-json-0.0.1/_core/
-drwxrwxrwx   0        0        0        0 2023-04-07 15:13:13.508798 extend-json-0.0.1/_core/extend_json.egg-info/
--rw-rw-rw-   0        0        0      756 2023-04-07 15:13:13.000000 extend-json-0.0.1/_core/extend_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-07 15:13:13.000000 extend-json-0.0.1/_core/extend_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 15:13:13.000000 extend-json-0.0.1/_core/extend_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-07 15:13:13.000000 extend-json-0.0.1/_core/extend_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    19089 2023-04-07 13:01:25.000000 extend-json-0.0.1/_core/extend_json.py
--rw-rw-rw-   0        0        0       42 2023-04-07 15:13:13.534798 extend-json-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-04-07 15:13:06.000000 extend-json-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:13:13.532798 extend-json-0.0.1/tests/
--rw-rw-rw-   0        0        0     2566 2023-04-07 15:04:56.000000 extend-json-0.0.1/tests/testsuite_io.py
--rw-rw-rw-   0        0        0     4859 2023-04-07 15:04:56.000000 extend-json-0.0.1/tests/testsuite_privates.py
--rw-rw-rw-   0        0        0    21481 2023-04-07 15:04:57.000000 extend-json-0.0.1/tests/testsuite_publics.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:42:48.958701 extend-json-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-07 12:07:07.000000 extend-json-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      979 2023-04-07 15:42:48.957700 extend-json-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-07 15:41:30.000000 extend-json-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 15:42:48.942700 extend-json-0.0.2/_core/
+drwxrwxrwx   0        0        0        0 2023-04-07 15:42:48.953727 extend-json-0.0.2/_core/extend_json.egg-info/
+-rw-rw-rw-   0        0        0      979 2023-04-07 15:42:48.000000 extend-json-0.0.2/_core/extend_json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-07 15:42:48.000000 extend-json-0.0.2/_core/extend_json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 15:42:48.000000 extend-json-0.0.2/_core/extend_json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-07 15:42:48.000000 extend-json-0.0.2/_core/extend_json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19089 2023-04-07 13:01:25.000000 extend-json-0.0.2/_core/extend_json.py
+-rw-rw-rw-   0        0        0       42 2023-04-07 15:42:48.958701 extend-json-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-04-07 15:42:20.000000 extend-json-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:42:48.956700 extend-json-0.0.2/tests/
+-rw-rw-rw-   0        0        0     2566 2023-04-07 15:04:56.000000 extend-json-0.0.2/tests/testsuite_io.py
+-rw-rw-rw-   0        0        0     4859 2023-04-07 15:04:56.000000 extend-json-0.0.2/tests/testsuite_privates.py
+-rw-rw-rw-   0        0        0    21481 2023-04-07 15:04:57.000000 extend-json-0.0.2/tests/testsuite_publics.py
```

### Comparing `extend-json-0.0.1/LICENSE` & `extend-json-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `extend-json-0.0.1/PKG-INFO` & `extend-json-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend-json
-Version: 0.0.1
+Version: 0.0.2
 Summary: additional methods for handling json files in python
 Home-page: https://github.com/Schnilsibus/jsonExtended.git
 Author: Nils Urbach
 Author-email: ndu01u@gmail.com
 License: MIT
 Keywords: json,extended
 Classifier: Development Status :: 3 - Alpha
@@ -16,7 +16,19 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json_extended
 Additional methods for handling json files in python.
+
+## Install
+
+### Windows
+install using pip : ```py -m pip install extend-json```
+
+### Others
+idk
+
+## Usage
+import: ```import extend_json``` or ```from extend_json import ...```
+overview: ```help(extend_json)```
```

### Comparing `extend-json-0.0.1/_core/extend_json.egg-info/PKG-INFO` & `extend-json-0.0.2/_core/extend_json.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend-json
-Version: 0.0.1
+Version: 0.0.2
 Summary: additional methods for handling json files in python
 Home-page: https://github.com/Schnilsibus/jsonExtended.git
 Author: Nils Urbach
 Author-email: ndu01u@gmail.com
 License: MIT
 Keywords: json,extended
 Classifier: Development Status :: 3 - Alpha
@@ -16,7 +16,19 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json_extended
 Additional methods for handling json files in python.
+
+## Install
+
+### Windows
+install using pip : ```py -m pip install extend-json```
+
+### Others
+idk
+
+## Usage
+import: ```import extend_json``` or ```from extend_json import ...```
+overview: ```help(extend_json)```
```

### Comparing `extend-json-0.0.1/_core/extend_json.py` & `extend-json-0.0.2/_core/extend_json.py`

 * *Files identical despite different names*

### Comparing `extend-json-0.0.1/setup.py` & `extend-json-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name = "extend-json",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Nils Urbach",
     author_email = "ndu01u@gmail.com",
     description = "additional methods for handling json files in python",
     long_description = long_description,
     long_description_content_type="text/markdown",
     license = "MIT",
     keywords = [
```

### Comparing `extend-json-0.0.1/tests/testsuite_io.py` & `extend-json-0.0.2/tests/testsuite_io.py`

 * *Files identical despite different names*

### Comparing `extend-json-0.0.1/tests/testsuite_privates.py` & `extend-json-0.0.2/tests/testsuite_privates.py`

 * *Files identical despite different names*

### Comparing `extend-json-0.0.1/tests/testsuite_publics.py` & `extend-json-0.0.2/tests/testsuite_publics.py`

 * *Files identical despite different names*

