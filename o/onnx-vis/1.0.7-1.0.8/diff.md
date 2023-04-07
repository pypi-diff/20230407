# Comparing `tmp/onnx_vis-1.0.7.tar.gz` & `tmp/onnx_vis-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_vis-1.0.7.tar", last modified: Fri Apr  7 16:19:16 2023, max compression
+gzip compressed data, was "onnx_vis-1.0.8.tar", last modified: Fri Apr  7 16:24:23 2023, max compression
```

## Comparing `onnx_vis-1.0.7.tar` & `onnx_vis-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/
--rw-r--r--   0 levi      (1000) hp        (1000)       33 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/MANIFEST.in
--rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/PKG-INFO
--rw-r--r--   0 levi      (1000) hp        (1000)     1537 2023-04-07 16:08:58.000000 onnx_vis-1.0.7/README.md
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.570918 onnx_vis-1.0.7/onnx_vis/
--rw-r--r--   0 levi      (1000) hp        (1000)        0 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/onnx_vis/__init__.py
--rw-r--r--   0 levi      (1000) hp        (1000)       22 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/onnx_vis/__main__.py
--rw-r--r--   0 levi      (1000) hp        (1000)     3069 2023-04-07 16:13:43.000000 onnx_vis-1.0.7/onnx_vis/onnx_vis.py
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/onnx_vis.egg-info/
--rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/PKG-INFO
--rw-r--r--   0 levi      (1000) hp        (1000)      256 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 levi      (1000) hp        (1000)        1 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 levi      (1000) hp        (1000)       53 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/entry_points.txt
--rw-r--r--   0 levi      (1000) hp        (1000)        9 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/top_level.txt
--rw-r--r--   0 levi      (1000) hp        (1000)       38 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/setup.cfg
--rw-r--r--   0 levi      (1000) hp        (1000)     1083 2023-04-07 16:19:10.000000 onnx_vis-1.0.7/setup.py
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:24:23.085934 onnx_vis-1.0.8/
+-rw-r--r--   0 levi      (1000) hp        (1000)       33 2023-04-07 11:21:52.000000 onnx_vis-1.0.8/MANIFEST.in
+-rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:24:23.085934 onnx_vis-1.0.8/PKG-INFO
+-rw-r--r--   0 levi      (1000) hp        (1000)     1537 2023-04-07 16:08:58.000000 onnx_vis-1.0.8/README.md
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:24:23.085934 onnx_vis-1.0.8/onnx_vis/
+-rw-r--r--   0 levi      (1000) hp        (1000)        0 2023-04-07 11:21:52.000000 onnx_vis-1.0.8/onnx_vis/__init__.py
+-rw-r--r--   0 levi      (1000) hp        (1000)       22 2023-04-07 11:21:52.000000 onnx_vis-1.0.8/onnx_vis/__main__.py
+-rw-r--r--   0 levi      (1000) hp        (1000)     3069 2023-04-07 16:13:43.000000 onnx_vis-1.0.8/onnx_vis/onnx_vis.py
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:24:23.085934 onnx_vis-1.0.8/onnx_vis.egg-info/
+-rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 levi      (1000) hp        (1000)      287 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)        1 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)       53 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/entry_points.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)       22 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/requires.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)        9 2023-04-07 16:24:23.000000 onnx_vis-1.0.8/onnx_vis.egg-info/top_level.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)       38 2023-04-07 16:24:23.085934 onnx_vis-1.0.8/setup.cfg
+-rw-r--r--   0 levi      (1000) hp        (1000)     1168 2023-04-07 16:24:11.000000 onnx_vis-1.0.8/setup.py
```

### Comparing `onnx_vis-1.0.7/PKG-INFO` & `onnx_vis-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx_vis
-Version: 1.0.7
+Version: 1.0.8
 Summary: This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model.
 Home-page: https://github.com/sleepingsaint/onnx_visualizer
 Author: sleepingsaint
 Author-email: suryasantosh14523@gmail.com
 License: MIT
 Keywords: example documentation tutorial
 Platform: UNKNOWN
```

### Comparing `onnx_vis-1.0.7/README.md` & `onnx_vis-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `onnx_vis-1.0.7/onnx_vis/onnx_vis.py` & `onnx_vis-1.0.8/onnx_vis/onnx_vis.py`

 * *Files identical despite different names*

### Comparing `onnx_vis-1.0.7/onnx_vis.egg-info/PKG-INFO` & `onnx_vis-1.0.8/onnx_vis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-vis
-Version: 1.0.7
+Version: 1.0.8
 Summary: This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model.
 Home-page: https://github.com/sleepingsaint/onnx_visualizer
 Author: sleepingsaint
 Author-email: suryasantosh14523@gmail.com
 License: MIT
 Keywords: example documentation tutorial
 Platform: UNKNOWN
```

### Comparing `onnx_vis-1.0.7/setup.py` & `onnx_vis-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "onnx_vis",
-    version = "1.0.7",
+    version = "1.0.8",
     author = "sleepingsaint",
     author_email = "suryasantosh14523@gmail.com",
     description = ("This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model."),
     license = "MIT",
     keywords = "example documentation tutorial",
     url = "https://github.com/sleepingsaint/onnx_visualizer",
     packages=['onnx_vis'],
@@ -26,10 +26,15 @@
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     classifiers=[
         # "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
     ],
+    install_requires = [
+        "onnx",
+        "flask",
+        "flask-cors"
+    ]
 )
```

