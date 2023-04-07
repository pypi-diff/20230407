# Comparing `tmp/inviz-0.0.3.tar.gz` & `tmp/inviz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.3.tar", last modified: Fri Apr  7 20:54:43 2023, max compression
+gzip compressed data, was "inviz-0.0.4.tar", last modified: Fri Apr  7 21:00:19 2023, max compression
```

## Comparing `inviz-0.0.3.tar` & `inviz-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:54:43.431991 inviz-0.0.3/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-04-07 20:46:41.000000 inviz-0.0.3/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-04-07 20:46:41.000000 inviz-0.0.3/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 20:54:43.431991 inviz-0.0.3/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2036 2023-04-07 20:46:41.000000 inviz-0.0.3/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:54:43.431991 inviz-0.0.3/inviz/
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:54:43.431991 inviz-0.0.3/inviz/inviz.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 20:54:43.000000 inviz-0.0.3/inviz/inviz.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-07 20:54:43.000000 inviz-0.0.3/inviz/inviz.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-07 20:54:43.000000 inviz-0.0.3/inviz/inviz.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-07 20:54:43.000000 inviz-0.0.3/inviz/inviz.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-07 20:54:43.000000 inviz-0.0.3/inviz/inviz.egg-info/top_level.txt
--rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9387 2023-04-07 20:46:42.000000 inviz-0.0.3/inviz/inviz.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-07 20:54:43.431991 inviz-0.0.3/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1162 2023-04-07 20:54:10.000000 inviz-0.0.3/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-04-07 20:46:41.000000 inviz-0.0.4/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-04-07 20:46:41.000000 inviz-0.0.4/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 21:00:19.304737 inviz-0.0.4/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2036 2023-04-07 20:46:41.000000 inviz-0.0.4/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/inviz/
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 21:00:19.304737 inviz-0.0.4/inviz/inviz.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2606 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-07 21:00:19.000000 inviz-0.0.4/inviz/inviz.egg-info/top_level.txt
+-rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9387 2023-04-07 20:46:42.000000 inviz-0.0.4/inviz/inviz.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-07 21:00:19.304737 inviz-0.0.4/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1162 2023-04-07 20:59:46.000000 inviz-0.0.4/setup.py
```

### Comparing `inviz-0.0.3/LICENSE` & `inviz-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.3/PKG-INFO` & `inviz-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.3
+Version: 0.0.4
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Platform: UNKNOWN
```

### Comparing `inviz-0.0.3/README.md` & `inviz-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.0.3/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.0.4/inviz/inviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.3
+Version: 0.0.4
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Platform: UNKNOWN
```

### Comparing `inviz-0.0.3/inviz/inviz.py` & `inviz-0.0.4/inviz/inviz.py`

 * *Files identical despite different names*

### Comparing `inviz-0.0.3/setup.py` & `inviz-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
@@ -26,10 +26,10 @@
     ],
     python_requires='>=3.6',
     install_requires=["holoviews==1.15.4",
                       "spatialpandas==0.4.7",
                       "hvplot==0.8.3",
                       "numpy==1.23.5",
                       "matplotlib==3.7.1",
-                      "bokeh==3.1.0"]
+                      "bokeh==2.4.0"]
     )
```

