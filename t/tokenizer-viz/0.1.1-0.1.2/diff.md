# Comparing `tmp/tokenizer-viz-0.1.1.tar.gz` & `tmp/tokenizer-viz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizer-viz-0.1.1.tar", last modified: Fri Apr  7 20:49:34 2023, max compression
+gzip compressed data, was "tokenizer-viz-0.1.2.tar", last modified: Fri Apr  7 20:51:35 2023, max compression
```

## Comparing `tokenizer-viz-0.1.1.tar` & `tokenizer-viz-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.321115 tokenizer-viz-0.1.1/
--rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.1.1/LICENSE
--rw-r--r--   0 darienschettler   (501) staff       (20)     2982 2023-04-07 20:49:34.321003 tokenizer-viz-0.1.1/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)     2331 2023-04-07 20:47:47.000000 tokenizer-viz-0.1.1/README.md
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-07 20:49:34.321159 tokenizer-viz-0.1.1/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)      956 2023-04-07 20:49:31.000000 tokenizer-viz-0.1.1/setup.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.319927 tokenizer-viz-0.1.1/tokenizer_viz/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-04-07 19:06:23.000000 tokenizer-viz-0.1.1/tokenizer_viz/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2832 2023-04-07 19:42:40.000000 tokenizer-viz-0.1.1/tokenizer_viz/viz_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.320828 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2982 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      263 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/top_level.txt
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.813204 tokenizer-viz-0.1.2/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.1.2/LICENSE
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2975 2023-04-07 20:51:35.813101 tokenizer-viz-0.1.2/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2324 2023-04-07 20:51:22.000000 tokenizer-viz-0.1.2/README.md
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-07 20:51:35.813242 tokenizer-viz-0.1.2/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)      956 2023-04-07 20:51:16.000000 tokenizer-viz-0.1.2/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.812254 tokenizer-viz-0.1.2/tokenizer_viz/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-04-07 19:06:23.000000 tokenizer-viz-0.1.2/tokenizer_viz/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2832 2023-04-07 19:42:40.000000 tokenizer-viz-0.1.2/tokenizer_viz/viz_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:51:35.812949 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2975 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      263 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-07 20:51:35.000000 tokenizer-viz-0.1.2/tokenizer_viz.egg-info/top_level.txt
```

### Comparing `tokenizer-viz-0.1.1/LICENSE` & `tokenizer-viz-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.1.1/PKG-INFO` & `tokenizer-viz-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 ---
 
 ## Installation
 
 You can install the tokenizer-viz package using pip:
 
 ```bash
-pip install tokenizer-visualizer
+pip install tokenizer-viz
 ```
 
 ---
 
 ## Usage
 
 Here's a quick example of how to use the package:
```

### Comparing `tokenizer-viz-0.1.1/README.md` & `tokenizer-viz-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ---
 
 ## Installation
 
 You can install the tokenizer-viz package using pip:
 
 ```bash
-pip install tokenizer-visualizer
+pip install tokenizer-viz
 ```
 
 ---
 
 ## Usage
 
 Here's a quick example of how to use the package:
```

### Comparing `tokenizer-viz-0.1.1/setup.py` & `tokenizer-viz-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tokenizer-viz",
-    version="0.1.1",
+    version="0.1.2",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization of text using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/tokenizer-viz",
     packages=find_packages(),
```

### Comparing `tokenizer-viz-0.1.1/tokenizer_viz/viz_utils.py` & `tokenizer-viz-0.1.2/tokenizer_viz/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.1.1/tokenizer_viz.egg-info/PKG-INFO` & `tokenizer-viz-0.1.2/tokenizer_viz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 ---
 
 ## Installation
 
 You can install the tokenizer-viz package using pip:
 
 ```bash
-pip install tokenizer-visualizer
+pip install tokenizer-viz
 ```
 
 ---
 
 ## Usage
 
 Here's a quick example of how to use the package:
```

