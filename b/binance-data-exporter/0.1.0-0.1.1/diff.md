# Comparing `tmp/binance_data_exporter-0.1.0.tar.gz` & `tmp/binance_data_exporter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_data_exporter-0.1.0.tar", last modified: Fri Apr  7 20:17:27 2023, max compression
+gzip compressed data, was "binance_data_exporter-0.1.1.tar", last modified: Fri Apr  7 20:22:53 2023, max compression
```

## Comparing `binance_data_exporter-0.1.0.tar` & `binance_data_exporter-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:17:27.402822 binance_data_exporter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 20:17:27.402822 binance_data_exporter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-07 20:17:17.000000 binance_data_exporter-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:17:27.402822 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:17:27.000000 binance_data_exporter-0.1.0/binance_data_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:17:27.402822 binance_data_exporter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-07 20:17:17.000000 binance_data_exporter-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:53.258219 binance_data_exporter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:22:53.258219 binance_data_exporter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-07 20:22:44.000000 binance_data_exporter-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:22:53.258219 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:22:53.000000 binance_data_exporter-0.1.1/binance_data_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:22:53.258219 binance_data_exporter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-07 20:22:44.000000 binance_data_exporter-0.1.1/setup.py
```

### Comparing `binance_data_exporter-0.1.0/README.md` & `binance_data_exporter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `binance_data_exporter-0.1.0/setup.py` & `binance_data_exporter-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
 setup(
     name='binance_data_exporter',
-    version='0.1.0',
+    version='0.1.1',
     description='A tool for exporting in JSON format the historical data of a symbol from Binance',
     author='zestones',
     author_email='idrissbenguezzou@gmail.com',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'binance_data_exporter=binance_data_exporter:main'
@@ -14,9 +17,11 @@
     },
     install_requires=[
         'datetime',
         'requests',
         'colorama',
         'tabulate',
         'json'
-    ]
+    ],
+    long_description=long_description,
+    long_description_content_type="text/markdown"
 )
```

