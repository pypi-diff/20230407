# Comparing `tmp/anrg.saga-0.0.1.tar.gz` & `tmp/anrg.saga-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anrg.saga-0.0.1.tar", last modified: Thu Apr  6 16:54:09 2023, max compression
+gzip compressed data, was "anrg.saga-0.0.2.tar", last modified: Fri Apr  7 17:04:25 2023, max compression
```

## Comparing `anrg.saga-0.0.1.tar` & `anrg.saga-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-06 16:54:09.560182 anrg.saga-0.0.1/
--rw-r--r--   0 jared     (1000) jared     (1000)     1895 2023-04-06 16:54:09.560182 anrg.saga-0.0.1/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)     1266 2023-04-06 16:43:14.000000 anrg.saga-0.0.1/README.md
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-06 16:54:09.560182 anrg.saga-0.0.1/anrg.saga.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     1895 2023-04-06 16:54:09.000000 anrg.saga-0.0.1/anrg.saga.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)      227 2023-04-06 16:54:09.000000 anrg.saga-0.0.1/anrg.saga.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-04-06 16:54:09.000000 anrg.saga-0.0.1/anrg.saga.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       57 2023-04-06 16:54:09.000000 anrg.saga-0.0.1/anrg.saga.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        5 2023-04-06 16:54:09.000000 anrg.saga-0.0.1/anrg.saga.egg-info/top_level.txt
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-06 16:54:09.560182 anrg.saga-0.0.1/saga/
--rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:50:26.000000 anrg.saga-0.0.1/saga/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)      495 2023-04-05 15:01:34.000000 anrg.saga-0.0.1/saga/base.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1544 2023-04-05 14:51:04.000000 anrg.saga-0.0.1/saga/hybrid.py
--rw-r--r--   0 jared     (1000) jared     (1000)       38 2023-04-06 16:54:09.560182 anrg.saga-0.0.1/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)     1071 2023-04-06 16:54:03.000000 anrg.saga-0.0.1/setup.py
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:04:25.679500 anrg.saga-0.0.2/
+-rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 17:04:25.679500 anrg.saga-0.0.2/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)     1179 2023-04-06 16:54:49.000000 anrg.saga-0.0.2/README.md
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:04:25.679500 anrg.saga-0.0.2/anrg.saga.egg-info/
+-rw-r--r--   0 jared     (1000) jared     (1000)     1808 2023-04-07 17:04:25.000000 anrg.saga-0.0.2/anrg.saga.egg-info/PKG-INFO
+-rw-r--r--   0 jared     (1000) jared     (1000)      227 2023-04-07 17:04:25.000000 anrg.saga-0.0.2/anrg.saga.egg-info/SOURCES.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-04-07 17:04:25.000000 anrg.saga-0.0.2/anrg.saga.egg-info/dependency_links.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)       57 2023-04-07 17:04:25.000000 anrg.saga-0.0.2/anrg.saga.egg-info/requires.txt
+-rw-r--r--   0 jared     (1000) jared     (1000)        5 2023-04-07 17:04:25.000000 anrg.saga-0.0.2/anrg.saga.egg-info/top_level.txt
+drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-04-07 17:04:25.679500 anrg.saga-0.0.2/saga/
+-rw-r--r--   0 jared     (1000) jared     (1000)        0 2023-04-05 14:50:26.000000 anrg.saga-0.0.2/saga/__init__.py
+-rw-r--r--   0 jared     (1000) jared     (1000)      495 2023-04-05 15:01:34.000000 anrg.saga-0.0.2/saga/base.py
+-rw-r--r--   0 jared     (1000) jared     (1000)     1544 2023-04-05 14:51:04.000000 anrg.saga-0.0.2/saga/hybrid.py
+-rw-r--r--   0 jared     (1000) jared     (1000)       38 2023-04-07 17:04:25.679500 anrg.saga-0.0.2/setup.cfg
+-rw-r--r--   0 jared     (1000) jared     (1000)     1071 2023-04-07 17:02:16.000000 anrg.saga-0.0.2/setup.py
```

### Comparing `anrg.saga-0.0.1/PKG-INFO` & `anrg.saga-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anrg.saga
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of schedulers for distributed computing
 Home-page: https://github.com/ANRGUSC/saga
 Author: Jared Coleman
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,17 +36,15 @@
     * Stochastic HEFT
     * Mean HEFT
 
 ## Usage
 ### Installation
 Clone the repository and install the requirements:
 ```bash
-git clone <repo>
-cd <repo>
-pip install -e . # -e flag is optional - it installs the package in editable mode
+pip install anrg.saga
 ```
 
 ### Running the algorithms
 The algorithms are implemented as python modules.
 The following example shows how to run the HEFT algorithm on a workflow:
 ```python
 from saga.common.heft import HeftScheduler
```

### Comparing `anrg.saga-0.0.1/README.md` & `anrg.saga-0.0.2/anrg.saga.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: anrg.saga
+Version: 0.0.2
+Summary: Collection of schedulers for distributed computing
+Home-page: https://github.com/ANRGUSC/saga
+Author: Jared Coleman
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Saga
 Saga: **S**cheduling **A**lgorithms **Ga**thered.
 
 ## Introduction
 This repository contains a collection of scheduling algorithms. 
 The algorithms are implemented in python using a common interface.
 Scripts for validating the schedules produced by the algorithms are also provided.
@@ -19,17 +36,15 @@
     * Stochastic HEFT
     * Mean HEFT
 
 ## Usage
 ### Installation
 Clone the repository and install the requirements:
 ```bash
-git clone <repo>
-cd <repo>
-pip install -e . # -e flag is optional - it installs the package in editable mode
+pip install anrg.saga
 ```
 
 ### Running the algorithms
 The algorithms are implemented as python modules.
 The following example shows how to run the HEFT algorithm on a workflow:
 ```python
 from saga.common.heft import HeftScheduler
```

### Comparing `anrg.saga-0.0.1/saga/hybrid.py` & `anrg.saga-0.0.2/saga/hybrid.py`

 * *Files identical despite different names*

### Comparing `anrg.saga-0.0.1/setup.py` & `anrg.saga-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 thisdir = pathlib.Path(__file__).parent.absolute()
 
 long_description = (thisdir / "README.md").read_text()
 
 setup(
     name='anrg.saga',
-    version='0.0.1',
+    version='0.0.2',
     description='Collection of schedulers for distributed computing',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ANRGUSC/saga',
     author='Jared Coleman',
     packages=['saga'],
     classifiers=[
```

