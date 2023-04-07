# Comparing `tmp/hillclimbers-0.0.1.tar.gz` & `tmp/hillclimbers-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hillclimbers-0.0.1.tar", last modified: Fri Apr  7 17:53:01 2023, max compression
+gzip compressed data, was "hillclimbers-0.1.0.tar", last modified: Fri Apr  7 18:29:14 2023, max compression
```

## Comparing `hillclimbers-0.0.1.tar` & `hillclimbers-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:53:01.728996 hillclimbers-0.0.1/
--rw-rw-r--   0 matthill   (501) staff       (20)       77 2023-04-07 17:52:05.000000 hillclimbers-0.0.1/CHANGELOG.txt
--rw-rw-r--   0 matthill   (501) staff       (20)     1047 2023-04-07 17:23:05.000000 hillclimbers-0.0.1/LICENCE.txt
--rw-rw-r--   0 matthill   (501) staff       (20)       26 2020-04-20 13:20:58.000000 hillclimbers-0.0.1/MANIFEST.in
--rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:53:01.728350 hillclimbers-0.0.1/PKG-INFO
--rw-rw-r--   0 matthill   (501) staff       (20)       65 2023-04-07 17:16:22.000000 hillclimbers-0.0.1/README.txt
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:53:01.723523 hillclimbers-0.0.1/hillclimbers/
--rw-rw-r--   0 matthill   (501) staff       (20)     7931 2023-04-07 17:51:29.000000 hillclimbers-0.0.1/hillclimbers/__init__.py
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:53:01.727198 hillclimbers-0.0.1/hillclimbers.egg-info/
--rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:53:01.000000 hillclimbers-0.0.1/hillclimbers.egg-info/PKG-INFO
--rw-r--r--   0 matthill   (501) staff       (20)      261 2023-04-07 17:53:01.000000 hillclimbers-0.0.1/hillclimbers.egg-info/SOURCES.txt
--rw-r--r--   0 matthill   (501) staff       (20)        1 2023-04-07 17:53:01.000000 hillclimbers-0.0.1/hillclimbers.egg-info/dependency_links.txt
--rw-r--r--   0 matthill   (501) staff       (20)       39 2023-04-07 17:53:01.000000 hillclimbers-0.0.1/hillclimbers.egg-info/requires.txt
--rw-r--r--   0 matthill   (501) staff       (20)       13 2023-04-07 17:53:01.000000 hillclimbers-0.0.1/hillclimbers.egg-info/top_level.txt
--rw-r--r--   0 matthill   (501) staff       (20)       38 2023-04-07 17:53:01.729303 hillclimbers-0.0.1/setup.cfg
--rw-rw-r--   0 matthill   (501) staff       (20)      905 2023-04-07 17:52:15.000000 hillclimbers-0.0.1/setup.py
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 18:29:14.272241 hillclimbers-0.1.0/
+-rw-rw-r--   0 matthill   (501) staff       (20)       77 2023-04-07 18:28:26.000000 hillclimbers-0.1.0/CHANGELOG.txt
+-rw-rw-r--   0 matthill   (501) staff       (20)     1047 2023-04-07 17:23:05.000000 hillclimbers-0.1.0/LICENCE.txt
+-rw-rw-r--   0 matthill   (501) staff       (20)       26 2020-04-20 13:20:58.000000 hillclimbers-0.1.0/MANIFEST.in
+-rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 18:29:14.271409 hillclimbers-0.1.0/PKG-INFO
+-rw-rw-r--   0 matthill   (501) staff       (20)       65 2023-04-07 17:16:22.000000 hillclimbers-0.1.0/README.txt
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 18:29:14.265623 hillclimbers-0.1.0/hillclimbers/
+-rw-rw-r--   0 matthill   (501) staff       (20)     8202 2023-04-07 18:24:54.000000 hillclimbers-0.1.0/hillclimbers/__init__.py
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 18:29:14.270343 hillclimbers-0.1.0/hillclimbers.egg-info/
+-rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 18:29:14.000000 hillclimbers-0.1.0/hillclimbers.egg-info/PKG-INFO
+-rw-r--r--   0 matthill   (501) staff       (20)      261 2023-04-07 18:29:14.000000 hillclimbers-0.1.0/hillclimbers.egg-info/SOURCES.txt
+-rw-r--r--   0 matthill   (501) staff       (20)        1 2023-04-07 18:29:14.000000 hillclimbers-0.1.0/hillclimbers.egg-info/dependency_links.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       29 2023-04-07 18:29:14.000000 hillclimbers-0.1.0/hillclimbers.egg-info/requires.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       13 2023-04-07 18:29:14.000000 hillclimbers-0.1.0/hillclimbers.egg-info/top_level.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       38 2023-04-07 18:29:14.272524 hillclimbers-0.1.0/setup.cfg
+-rw-rw-r--   0 matthill   (501) staff       (20)      892 2023-04-07 18:28:40.000000 hillclimbers-0.1.0/setup.py
```

### Comparing `hillclimbers-0.0.1/LICENCE.txt` & `hillclimbers-0.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `hillclimbers-0.0.1/PKG-INFO` & `hillclimbers-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillclimbers
-Version: 0.0.1
+Version: 0.1.0
 Summary: A module to iteratively blend machine learning model predictions.
 Home-page: UNKNOWN
 Author: Matt-OP
 License: MIT
 Keywords: python,data,dataframe,machine learning,predictions,blending,pandas,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,12 +18,12 @@
 License-File: LICENCE.txt
 
 A module to iteratively blend machine learning model predictions.
 
 Change Log
 ==========
 
-0.0.1 (4/07/2023)
+0.1.0 (4/07/2023)
 -------------------
 - First Release
```

### Comparing `hillclimbers-0.0.1/hillclimbers/__init__.py` & `hillclimbers-0.1.0/hillclimbers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
-import functools
-from functools import partial
 from colorama import Fore, Back, Style
 
 
+class partial:
+    def __init__(self, func, *args, **kwargs):
+        self.func = func
+        self.args = args
+        self.kwargs = kwargs
+
+    def __call__(self, *args, **kwargs):
+        new_args = self.args + args
+        new_kwargs = {**self.kwargs, **kwargs}
+        return self.func(*new_args, **new_kwargs)
+
+
 def climb_hill(
     df_concat_mode: str = "default", 
     train: pd.DataFrame = None, 
     test: pd.DataFrame = None,
     oof_pred_df: pd.DataFrame = None, 
     test_pred_df: pd.DataFrame = None, 
     target: str = None,
```

### Comparing `hillclimbers-0.0.1/hillclimbers.egg-info/PKG-INFO` & `hillclimbers-0.1.0/hillclimbers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillclimbers
-Version: 0.0.1
+Version: 0.1.0
 Summary: A module to iteratively blend machine learning model predictions.
 Home-page: UNKNOWN
 Author: Matt-OP
 License: MIT
 Keywords: python,data,dataframe,machine learning,predictions,blending,pandas,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,12 +18,12 @@
 License-File: LICENCE.txt
 
 A module to iteratively blend machine learning model predictions.
 
 Change Log
 ==========
 
-0.0.1 (4/07/2023)
+0.1.0 (4/07/2023)
 -------------------
 - First Release
```

### Comparing `hillclimbers-0.0.1/setup.py` & `hillclimbers-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
   "Operating System :: Microsoft :: Windows",
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='hillclimbers',
-  version='0.0.1',
+  version='0.1.0',
   description='A module to iteratively blend machine learning model predictions.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Matt-OP',
   license='MIT', 
   classifiers=classifiers,
   keywords=['python', 'data', 'dataframe', 'machine learning', 'predictions', 'blending', 'pandas', 'numpy'], 
   packages=find_packages(),
-  install_requires=['pandas', 'numpy', 'plotly', 'functools', 'colorama'] 
+  install_requires=['pandas', 'numpy', 'plotly', 'colorama'] 
 )
```

