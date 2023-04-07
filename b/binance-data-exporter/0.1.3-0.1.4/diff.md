# Comparing `tmp/binance_data_exporter-0.1.3.tar.gz` & `tmp/binance_data_exporter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_data_exporter-0.1.3.tar", last modified: Fri Apr  7 20:39:23 2023, max compression
+gzip compressed data, was "binance_data_exporter-0.1.4.tar", last modified: Fri Apr  7 20:49:44 2023, max compression
```

## Comparing `binance_data_exporter-0.1.3.tar` & `binance_data_exporter-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:23.492179 binance_data_exporter-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:39:23.492179 binance_data_exporter-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-07 20:39:13.000000 binance_data_exporter-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:23.492179 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:39:23.000000 binance_data_exporter-0.1.3/binance_data_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:39:23.492179 binance_data_exporter-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 20:39:13.000000 binance_data_exporter-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:49:44.429950 binance_data_exporter-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:49:44.429950 binance_data_exporter-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-07 20:49:29.000000 binance_data_exporter-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:49:44.429950 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:49:44.000000 binance_data_exporter-0.1.4/binance_data_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:49:44.429950 binance_data_exporter-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-07 20:49:29.000000 binance_data_exporter-0.1.4/setup.py
```

### Comparing `binance_data_exporter-0.1.3/PKG-INFO` & `binance_data_exporter-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance_data_exporter
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for exporting in JSON format the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Retrieval
```

### Comparing `binance_data_exporter-0.1.3/README.md` & `binance_data_exporter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `binance_data_exporter-0.1.3/binance_data_exporter.egg-info/PKG-INFO` & `binance_data_exporter-0.1.4/binance_data_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-data-exporter
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for exporting in JSON format the historical data of a symbol from Binance
 Author: zestones
 Author-email: idrissbenguezzou@gmail.com
 Description-Content-Type: text/markdown
 
 # Binance API Data Retrieval
```

### Comparing `binance_data_exporter-0.1.3/setup.py` & `binance_data_exporter-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='binance_data_exporter',
-    version='0.1.3',
+    version='0.1.4',
     description='A tool for exporting in JSON format the historical data of a symbol from Binance',
     author='zestones',
     author_email='idrissbenguezzou@gmail.com',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'binance_data_exporter=binance_data_exporter:main'
         ]
     },
     install_requires=[
-        'datetime',
         'requests',
         'colorama',
         'tabulate',
-        'json>=2.0'
     ],
 
     long_description=long_description,
     long_description_content_type="text/markdown"
 )
```

