# Comparing `tmp/onnx_vis-1.0.6.tar.gz` & `tmp/onnx_vis-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx_vis-1.0.6.tar", last modified: Sun Apr  2 08:56:12 2023, max compression
+gzip compressed data, was "onnx_vis-1.0.7.tar", last modified: Fri Apr  7 16:19:16 2023, max compression
```

## Comparing `onnx_vis-1.0.6.tar` & `onnx_vis-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-02 08:56:12.282396 onnx_vis-1.0.6/
--rw-r--r--   0 levi      (1000) hp        (1000)       33 2023-04-01 19:16:46.000000 onnx_vis-1.0.6/MANIFEST.in
--rw-r--r--   0 levi      (1000) hp        (1000)     2104 2023-04-02 08:56:12.282396 onnx_vis-1.0.6/PKG-INFO
--rw-r--r--   0 levi      (1000) hp        (1000)     1555 2023-04-01 19:34:18.000000 onnx_vis-1.0.6/README.md
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-02 08:56:12.278395 onnx_vis-1.0.6/onnx_vis/
--rw-r--r--   0 levi      (1000) hp        (1000)        0 2023-04-01 18:46:14.000000 onnx_vis-1.0.6/onnx_vis/__init__.py
--rw-r--r--   0 levi      (1000) hp        (1000)       22 2023-04-01 18:47:29.000000 onnx_vis-1.0.6/onnx_vis/__main__.py
--rw-r--r--   0 levi      (1000) hp        (1000)     2965 2023-04-02 06:32:25.000000 onnx_vis-1.0.6/onnx_vis/onnx_vis.py
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-02 08:56:12.278395 onnx_vis-1.0.6/onnx_vis/static/
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-02 08:56:12.278395 onnx_vis-1.0.6/onnx_vis/static/assets/
--rw-r--r--   0 levi      (1000) hp        (1000)    16960 2023-03-31 14:26:55.000000 onnx_vis-1.0.6/onnx_vis/static/assets/index-01359380.css
--rw-r--r--   0 levi      (1000) hp        (1000)  1717744 2023-04-02 08:53:23.000000 onnx_vis-1.0.6/onnx_vis/static/assets/index-3de14fb7.js
--rw-r--r--   0 levi      (1000) hp        (1000)      460 2023-03-31 14:26:55.000000 onnx_vis-1.0.6/onnx_vis/static/index.html
--rw-r--r--   0 levi      (1000) hp        (1000)     1497 2023-03-31 14:26:55.000000 onnx_vis-1.0.6/onnx_vis/static/vite.svg
-drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-02 08:56:12.278395 onnx_vis-1.0.6/onnx_vis.egg-info/
--rw-r--r--   0 levi      (1000) hp        (1000)     2104 2023-04-02 08:56:12.000000 onnx_vis-1.0.6/onnx_vis.egg-info/PKG-INFO
--rw-r--r--   0 levi      (1000) hp        (1000)      391 2023-04-02 08:56:12.000000 onnx_vis-1.0.6/onnx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 levi      (1000) hp        (1000)        1 2023-04-02 08:56:12.000000 onnx_vis-1.0.6/onnx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 levi      (1000) hp        (1000)       53 2023-04-02 08:56:12.000000 onnx_vis-1.0.6/onnx_vis.egg-info/entry_points.txt
--rw-r--r--   0 levi      (1000) hp        (1000)        9 2023-04-02 08:56:12.000000 onnx_vis-1.0.6/onnx_vis.egg-info/top_level.txt
--rw-r--r--   0 levi      (1000) hp        (1000)       38 2023-04-02 08:56:12.282396 onnx_vis-1.0.6/setup.cfg
--rw-r--r--   0 levi      (1000) hp        (1000)     1083 2023-04-02 08:55:36.000000 onnx_vis-1.0.6/setup.py
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/
+-rw-r--r--   0 levi      (1000) hp        (1000)       33 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/MANIFEST.in
+-rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/PKG-INFO
+-rw-r--r--   0 levi      (1000) hp        (1000)     1537 2023-04-07 16:08:58.000000 onnx_vis-1.0.7/README.md
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.570918 onnx_vis-1.0.7/onnx_vis/
+-rw-r--r--   0 levi      (1000) hp        (1000)        0 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/onnx_vis/__init__.py
+-rw-r--r--   0 levi      (1000) hp        (1000)       22 2023-04-07 11:21:52.000000 onnx_vis-1.0.7/onnx_vis/__main__.py
+-rw-r--r--   0 levi      (1000) hp        (1000)     3069 2023-04-07 16:13:43.000000 onnx_vis-1.0.7/onnx_vis/onnx_vis.py
+drwxr-xr-x   0 levi      (1000) hp        (1000)        0 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/onnx_vis.egg-info/
+-rw-r--r--   0 levi      (1000) hp        (1000)     2086 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 levi      (1000) hp        (1000)      256 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)        1 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)       53 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/entry_points.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)        9 2023-04-07 16:19:16.000000 onnx_vis-1.0.7/onnx_vis.egg-info/top_level.txt
+-rw-r--r--   0 levi      (1000) hp        (1000)       38 2023-04-07 16:19:16.574913 onnx_vis-1.0.7/setup.cfg
+-rw-r--r--   0 levi      (1000) hp        (1000)     1083 2023-04-07 16:19:10.000000 onnx_vis-1.0.7/setup.py
```

### Comparing `onnx_vis-1.0.6/PKG-INFO` & `onnx_vis-1.0.7/onnx_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: onnx_vis
-Version: 1.0.6
+Name: onnx-vis
+Version: 1.0.7
 Summary: This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model.
 Home-page: https://github.com/sleepingsaint/onnx_visualizer
 Author: sleepingsaint
 Author-email: suryasantosh14523@gmail.com
 License: MIT
 Keywords: example documentation tutorial
 Platform: UNKNOWN
@@ -41,15 +41,15 @@
 ```
 
 Example:
 
 ```bash
  python3 -m onnx_vis resnet18.onnx -p 63325
 ```
-you can access the visualization on http://127.0.0.1:63325/static/index.html
+you can access the visualization on http://127.0.0.1:63325
 
 
 ## TODO
 
 - [x] Make Visualization graph of ONNX Nodes
 - [ ] Add node attributes like kernels shape, bias shape to node metadata
 - [ ] Add Sidebar to get more detailed information about nodes
```

### Comparing `onnx_vis-1.0.6/README.md` & `onnx_vis-1.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```
 
 Example:
 
 ```bash
  python3 -m onnx_vis resnet18.onnx -p 63325
 ```
-you can access the visualization on http://127.0.0.1:63325/static/index.html
+you can access the visualization on http://127.0.0.1:63325
 
 
 ## TODO
 
 - [x] Make Visualization graph of ONNX Nodes
 - [ ] Add node attributes like kernels shape, bias shape to node metadata
 - [ ] Add Sidebar to get more detailed information about nodes
```

### Comparing `onnx_vis-1.0.6/onnx_vis/onnx_vis.py` & `onnx_vis-1.0.7/onnx_vis/onnx_vis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import onnx
 import argparse
 from flask import Flask, send_from_directory
 from flask_cors import CORS
 
-
 class ONNXVisualizer:
     def __init__(self, path) -> None:
         self.model = onnx.load(path)
         self.nodes, self.edges = [], []
         self.store = {}
 
         self._initStore()
@@ -76,24 +75,29 @@
 
     onnx_vis = ONNXVisualizer(model_path)
 
     app = Flask(__name__)
 
     ROOT_PATH = os.path.dirname(os.path.abspath(__file__))
     app.static_folder = os.path.join(ROOT_PATH, "static")
+
     CORS(app)
 
     @app.route("/")
+    def getHomePage():
+        return send_from_directory(app.static_folder, "index.html")
+
+    @app.route("/onnx")
     def getNodes():
         return {
             "nodes": onnx_vis.nodes,
             "edges": onnx_vis.edges
         } 
 
     @app.route("/edges")
     def getEdges():
         return onnx_vis.edges
 
-    app.run(debug=True, port=args.port)
+    app.run(port=args.port)
 
 if __name__ == "__main__":
     main()
```

### Comparing `onnx_vis-1.0.6/onnx_vis.egg-info/PKG-INFO` & `onnx_vis-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: onnx-vis
-Version: 1.0.6
+Name: onnx_vis
+Version: 1.0.7
 Summary: This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model.
 Home-page: https://github.com/sleepingsaint/onnx_visualizer
 Author: sleepingsaint
 Author-email: suryasantosh14523@gmail.com
 License: MIT
 Keywords: example documentation tutorial
 Platform: UNKNOWN
@@ -41,15 +41,15 @@
 ```
 
 Example:
 
 ```bash
  python3 -m onnx_vis resnet18.onnx -p 63325
 ```
-you can access the visualization on http://127.0.0.1:63325/static/index.html
+you can access the visualization on http://127.0.0.1:63325
 
 
 ## TODO
 
 - [x] Make Visualization graph of ONNX Nodes
 - [ ] Add node attributes like kernels shape, bias shape to node metadata
 - [ ] Add Sidebar to get more detailed information about nodes
```

### Comparing `onnx_vis-1.0.6/setup.py` & `onnx_vis-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "onnx_vis",
-    version = "1.0.6",
+    version = "1.0.7",
     author = "sleepingsaint",
     author_email = "suryasantosh14523@gmail.com",
     description = ("This package help you visualize the ONNX model graph. Client-Server based architecture lets you share the model, using just a url instead of sharing the entire model."),
     license = "MIT",
     keywords = "example documentation tutorial",
     url = "https://github.com/sleepingsaint/onnx_visualizer",
     packages=['onnx_vis'],
```

