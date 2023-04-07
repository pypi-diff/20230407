# Comparing `tmp/hillclimbers-1.0.0.tar.gz` & `tmp/hillclimbers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hillclimbers-1.0.0.tar", last modified: Fri Apr  7 17:29:14 2023, max compression
+gzip compressed data, was "hillclimbers-1.0.1.tar", last modified: Fri Apr  7 17:43:48 2023, max compression
```

## Comparing `hillclimbers-1.0.0.tar` & `hillclimbers-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:29:14.604284 hillclimbers-1.0.0/
--rw-rw-r--   0 matthill   (501) staff       (20)       77 2023-04-07 17:14:45.000000 hillclimbers-1.0.0/CHANGELOG.txt
--rw-rw-r--   0 matthill   (501) staff       (20)     1047 2023-04-07 17:23:05.000000 hillclimbers-1.0.0/LICENCE.txt
--rw-rw-r--   0 matthill   (501) staff       (20)       26 2020-04-20 13:20:58.000000 hillclimbers-1.0.0/MANIFEST.in
--rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:29:14.603716 hillclimbers-1.0.0/PKG-INFO
--rw-rw-r--   0 matthill   (501) staff       (20)       65 2023-04-07 17:16:22.000000 hillclimbers-1.0.0/README.txt
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:29:14.597649 hillclimbers-1.0.0/hillclimbers/
--rw-rw-r--   0 matthill   (501) staff       (20)     7885 2023-04-07 17:22:50.000000 hillclimbers-1.0.0/hillclimbers/__init__.py
-drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:29:14.602995 hillclimbers-1.0.0/hillclimbers.egg-info/
--rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:29:14.000000 hillclimbers-1.0.0/hillclimbers.egg-info/PKG-INFO
--rw-r--r--   0 matthill   (501) staff       (20)      261 2023-04-07 17:29:14.000000 hillclimbers-1.0.0/hillclimbers.egg-info/SOURCES.txt
--rw-r--r--   0 matthill   (501) staff       (20)        1 2023-04-07 17:29:14.000000 hillclimbers-1.0.0/hillclimbers.egg-info/dependency_links.txt
--rw-r--r--   0 matthill   (501) staff       (20)       29 2023-04-07 17:29:14.000000 hillclimbers-1.0.0/hillclimbers.egg-info/requires.txt
--rw-r--r--   0 matthill   (501) staff       (20)       13 2023-04-07 17:29:14.000000 hillclimbers-1.0.0/hillclimbers.egg-info/top_level.txt
--rw-r--r--   0 matthill   (501) staff       (20)       38 2023-04-07 17:29:14.604460 hillclimbers-1.0.0/setup.cfg
--rw-rw-r--   0 matthill   (501) staff       (20)      892 2023-04-07 17:26:45.000000 hillclimbers-1.0.0/setup.py
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:43:48.496648 hillclimbers-1.0.1/
+-rw-rw-r--   0 matthill   (501) staff       (20)       77 2023-04-07 17:14:45.000000 hillclimbers-1.0.1/CHANGELOG.txt
+-rw-rw-r--   0 matthill   (501) staff       (20)     1047 2023-04-07 17:23:05.000000 hillclimbers-1.0.1/LICENCE.txt
+-rw-rw-r--   0 matthill   (501) staff       (20)       26 2020-04-20 13:20:58.000000 hillclimbers-1.0.1/MANIFEST.in
+-rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:43:48.496056 hillclimbers-1.0.1/PKG-INFO
+-rw-rw-r--   0 matthill   (501) staff       (20)       65 2023-04-07 17:16:22.000000 hillclimbers-1.0.1/README.txt
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:43:48.490684 hillclimbers-1.0.1/hillclimbers/
+-rw-rw-r--   0 matthill   (501) staff       (20)     7915 2023-04-07 17:39:44.000000 hillclimbers-1.0.1/hillclimbers/__init__.py
+drwxr-xr-x   0 matthill   (501) staff       (20)        0 2023-04-07 17:43:48.495181 hillclimbers-1.0.1/hillclimbers.egg-info/
+-rw-r--r--   0 matthill   (501) staff       (20)      839 2023-04-07 17:43:48.000000 hillclimbers-1.0.1/hillclimbers.egg-info/PKG-INFO
+-rw-r--r--   0 matthill   (501) staff       (20)      261 2023-04-07 17:43:48.000000 hillclimbers-1.0.1/hillclimbers.egg-info/SOURCES.txt
+-rw-r--r--   0 matthill   (501) staff       (20)        1 2023-04-07 17:43:48.000000 hillclimbers-1.0.1/hillclimbers.egg-info/dependency_links.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       39 2023-04-07 17:43:48.000000 hillclimbers-1.0.1/hillclimbers.egg-info/requires.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       13 2023-04-07 17:43:48.000000 hillclimbers-1.0.1/hillclimbers.egg-info/top_level.txt
+-rw-r--r--   0 matthill   (501) staff       (20)       38 2023-04-07 17:43:48.496847 hillclimbers-1.0.1/setup.cfg
+-rw-rw-r--   0 matthill   (501) staff       (20)      905 2023-04-07 17:43:10.000000 hillclimbers-1.0.1/setup.py
```

### Comparing `hillclimbers-1.0.0/LICENCE.txt` & `hillclimbers-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `hillclimbers-1.0.0/PKG-INFO` & `hillclimbers-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillclimbers
-Version: 1.0.0
+Version: 1.0.1
 Summary: A module to iteratively blend machine learning model predictions.
 Home-page: UNKNOWN
 Author: Matt-OP
 License: MIT
 Keywords: python,data,dataframe,machine learning,predictions,blending,pandas,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hillclimbers-1.0.0/hillclimbers/__init__.py` & `hillclimbers-1.0.1/hillclimbers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import plotly.express as px
+from functools import partial
 from colorama import Fore, Back, Style
 
 
 def climb_hill(
     df_concat_mode: str = "default", 
     train: pd.DataFrame = None, 
     test: pd.DataFrame = None,
```

### Comparing `hillclimbers-1.0.0/hillclimbers.egg-info/PKG-INFO` & `hillclimbers-1.0.1/hillclimbers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hillclimbers
-Version: 1.0.0
+Version: 1.0.1
 Summary: A module to iteratively blend machine learning model predictions.
 Home-page: UNKNOWN
 Author: Matt-OP
 License: MIT
 Keywords: python,data,dataframe,machine learning,predictions,blending,pandas,numpy
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hillclimbers-1.0.0/setup.py` & `hillclimbers-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
   "Operating System :: Microsoft :: Windows",
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='hillclimbers',
-  version='1.0.0',
+  version='1.0.1',
   description='A module to iteratively blend machine learning model predictions.',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Matt-OP',
   license='MIT', 
   classifiers=classifiers,
   keywords=['python', 'data', 'dataframe', 'machine learning', 'predictions', 'blending', 'pandas', 'numpy'], 
   packages=find_packages(),
-  install_requires=['pandas', 'numpy', 'plotly', 'colorama'] 
+  install_requires=['pandas', 'numpy', 'plotly', 'functools', 'colorama'] 
 )
```

