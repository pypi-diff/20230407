# Comparing `tmp/sachin_pkg-Sachinsen1295-0.0.1.tar.gz` & `tmp/sachin_pkg-Sachinsen1295-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Sachin_pkg/Sachin_pkg/dist/.tmp-6w_jpha6/sachin_pkg-Sachinsen1295-0.0.1.tar", last modified: Fri Apr  7 18:58:51 2023, max compression
+gzip compressed data, was "/home/runner/work/Sachin_pkg/Sachin_pkg/dist/.tmp-093urj5o/sachin_pkg-Sachinsen1295-0.0.3.tar", last modified: Fri Apr  7 18:35:47 2023, max compression
```

## Comparing `sachin_pkg-Sachinsen1295-0.0.1.tar` & `sachin_pkg-Sachinsen1295-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-07 18:58:41.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin/perceptron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 18:58:51.000000 sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-07 18:35:35.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin/perceptron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 18:35:47.000000 sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/top_level.txt
```

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/LICENSE` & `sachin_pkg-Sachinsen1295-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/PKG-INFO` & `sachin_pkg-Sachinsen1295-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: sachin_pkg-Sachinsen1295
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small package for perceptron
 Home-page: https://github.com/Sachinsen1295/sachin-pkg
 Author: Sachinsen1295
 Author-email: sachin.sen1295@gmail.com
 Project-URL: Bug Tracker, https://github.com/Sachinsen1295/sachin-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sachin Test python package
+# oneNeuron python package
 
 ## How to use this package
 ```python
-from sachin.perceptron import Perceptron
+from oneNeuron.perceptron import Perceptron
 model = Perceptron(eta=0.3, epochs=10)
 ```
 
 ## References - 
 
 * [Official python docs for PYPI](https://packaging.python.org/tutorials/packaging-projects/)
```

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/README.md` & `sachin_pkg-Sachinsen1295-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Sachin Test python package
+# oneNeuron python package
 
 ## How to use this package
 ```python
-from sachin.perceptron import Perceptron
+from oneNeuron.perceptron import Perceptron
 model = Perceptron(eta=0.3, epochs=10)
 ```
 
 ## References - 
 
 * [Official python docs for PYPI](https://packaging.python.org/tutorials/packaging-projects/)
```

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/setup.py` & `sachin_pkg-Sachinsen1295-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 PKG_NAME = "sachin_pkg"
 USER_NAME = "Sachinsen1295"
 PROJECT_NAME = "sachin-pkg"
 
 setuptools.setup(
     name=f"{PKG_NAME}-{USER_NAME}",
-    version="0.0.1",
+    version="0.0.3",
     author=USER_NAME,
     author_email="sachin.sen1295@gmail.com",
     description="A small package for perceptron",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{USER_NAME}/{PROJECT_NAME}",
     project_urls={
```

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/src/sachin/perceptron.py` & `sachin_pkg-Sachinsen1295-0.0.3/src/sachin/perceptron.py`

 * *Files identical despite different names*

### Comparing `sachin_pkg-Sachinsen1295-0.0.1/src/sachin_pkg_Sachinsen1295.egg-info/PKG-INFO` & `sachin_pkg-Sachinsen1295-0.0.3/src/sachin_pkg_Sachinsen1295.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: sachin-pkg-Sachinsen1295
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small package for perceptron
 Home-page: https://github.com/Sachinsen1295/sachin-pkg
 Author: Sachinsen1295
 Author-email: sachin.sen1295@gmail.com
 Project-URL: Bug Tracker, https://github.com/Sachinsen1295/sachin-pkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sachin Test python package
+# oneNeuron python package
 
 ## How to use this package
 ```python
-from sachin.perceptron import Perceptron
+from oneNeuron.perceptron import Perceptron
 model = Perceptron(eta=0.3, epochs=10)
 ```
 
 ## References - 
 
 * [Official python docs for PYPI](https://packaging.python.org/tutorials/packaging-projects/)
```

