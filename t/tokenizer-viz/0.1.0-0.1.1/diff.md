# Comparing `tmp/tokenizer-viz-0.1.0.tar.gz` & `tmp/tokenizer-viz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenizer-viz-0.1.0.tar", last modified: Fri Apr  7 20:41:32 2023, max compression
+gzip compressed data, was "tokenizer-viz-0.1.1.tar", last modified: Fri Apr  7 20:49:34 2023, max compression
```

## Comparing `tokenizer-viz-0.1.0.tar` & `tokenizer-viz-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:41:32.401595 tokenizer-viz-0.1.0/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2976 2023-04-07 20:41:32.401466 tokenizer-viz-0.1.0/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)     2334 2023-04-07 20:41:09.000000 tokenizer-viz-0.1.0/README.md
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-07 20:41:32.401646 tokenizer-viz-0.1.0/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)      950 2023-04-07 19:08:30.000000 tokenizer-viz-0.1.0/setup.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:41:32.400604 tokenizer-viz-0.1.0/tokenizer_viz/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-04-07 19:06:23.000000 tokenizer-viz-0.1.0/tokenizer_viz/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2832 2023-04-07 19:42:40.000000 tokenizer-viz-0.1.0/tokenizer_viz/viz_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:41:32.401276 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)     2976 2023-04-07 20:41:32.000000 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      255 2023-04-07 20:41:32.000000 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-07 20:41:32.000000 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       11 2023-04-07 20:41:32.000000 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-07 20:41:32.000000 tokenizer-viz-0.1.0/tokenizer_viz.egg-info/top_level.txt
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.321115 tokenizer-viz-0.1.1/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1055 2023-03-29 16:29:39.000000 tokenizer-viz-0.1.1/LICENSE
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2982 2023-04-07 20:49:34.321003 tokenizer-viz-0.1.1/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2331 2023-04-07 20:47:47.000000 tokenizer-viz-0.1.1/README.md
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-07 20:49:34.321159 tokenizer-viz-0.1.1/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)      956 2023-04-07 20:49:31.000000 tokenizer-viz-0.1.1/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.319927 tokenizer-viz-0.1.1/tokenizer_viz/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-04-07 19:06:23.000000 tokenizer-viz-0.1.1/tokenizer_viz/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2832 2023-04-07 19:42:40.000000 tokenizer-viz-0.1.1/tokenizer_viz/viz_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-07 20:49:34.320828 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2982 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      263 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       14 2023-04-07 20:49:34.000000 tokenizer-viz-0.1.1/tokenizer_viz.egg-info/top_level.txt
```

### Comparing `tokenizer-viz-0.1.0/PKG-INFO` & `tokenizer-viz-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to visualize tokenization of text using HTML
-Home-page: https://github.com/yourusername/tokenizer-visualizer
+Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# Tokenizer Visualizer
+# Tokenizer Viz
 
-Tokenizer Visualizer is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
+Tokenizer Viz is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
 
 ---
 
 ## Project Layout
 
 ```terminal
 tokenizer-viz/
 │
 ├── tokenizer_viz/
 │   ├── __init__.py
 │   └── viz—utils.py
 │
 ├── .gitignore
+├── LICENSE
 ├── README.md
 └── setup.py
 ```
 
 ---
 
 ## Installation
 
-You can install the tokenizer-visualizer package using pip:
+You can install the tokenizer-viz package using pip:
 
 ```bash
 pip install tokenizer-visualizer
 ```
 
 ---
```

### Comparing `tokenizer-viz-0.1.0/README.md` & `tokenizer-viz-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# Tokenizer Visualizer
+# Tokenizer Viz
 
-Tokenizer Visualizer is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
+Tokenizer Viz is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
 
 ---
 
 ## Project Layout
 
 ```terminal
 tokenizer-viz/
 │
 ├── tokenizer_viz/
 │   ├── __init__.py
 │   └── viz—utils.py
 │
 ├── .gitignore
+├── LICENSE
 ├── README.md
 └── setup.py
 ```
 
 ---
 
 ## Installation
 
-You can install the tokenizer-visualizer package using pip:
+You can install the tokenizer-viz package using pip:
 
 ```bash
 pip install tokenizer-visualizer
 ```
 
 ---
```

### Comparing `tokenizer-viz-0.1.0/setup.py` & `tokenizer-viz-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tokenizer-viz",
-    version="0.1.0",
+    version="0.1.1",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization of text using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/tokenizer-visualizer",
+    url="https://github.com/ds08tf/tokenizer-viz",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     install_requires=[
         "matplotlib",
+        "IPython",
     ],
     python_requires='>=3.7',
 )
```

### Comparing `tokenizer-viz-0.1.0/tokenizer_viz/viz_utils.py` & `tokenizer-viz-0.1.1/tokenizer_viz/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tokenizer-viz-0.1.0/tokenizer_viz.egg-info/PKG-INFO` & `tokenizer-viz-0.1.1/tokenizer_viz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: tokenizer-viz
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to visualize tokenization of text using HTML
-Home-page: https://github.com/yourusername/tokenizer-visualizer
+Home-page: https://github.com/ds08tf/tokenizer-viz
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# Tokenizer Visualizer
+# Tokenizer Viz
 
-Tokenizer Visualizer is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
+Tokenizer Viz is a Python package that generates HTML to visualize the tokenization of text. It highlights tokens with different colors and customizable styles, making it easier to understand how a text is tokenized.
 
 ---
 
 ## Project Layout
 
 ```terminal
 tokenizer-viz/
 │
 ├── tokenizer_viz/
 │   ├── __init__.py
 │   └── viz—utils.py
 │
 ├── .gitignore
+├── LICENSE
 ├── README.md
 └── setup.py
 ```
 
 ---
 
 ## Installation
 
-You can install the tokenizer-visualizer package using pip:
+You can install the tokenizer-viz package using pip:
 
 ```bash
 pip install tokenizer-visualizer
 ```
 
 ---
```

