# Comparing `tmp/cli-sandbox-0.2.7.tar.gz` & `tmp/cli-sandbox-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-sandbox-0.2.7.tar", last modified: Fri Apr  7 19:54:34 2023, max compression
+gzip compressed data, was "cli-sandbox-0.2.8.tar", last modified: Fri Apr  7 19:58:37 2023, max compression
```

## Comparing `cli-sandbox-0.2.7.tar` & `cli-sandbox-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:54:34.266520 cli-sandbox-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:54:34.266520 cli-sandbox-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 19:54:24.000000 cli-sandbox-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:54:34.262520 cli-sandbox-0.2.7/cli-sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 19:54:24.000000 cli-sandbox-0.2.7/cli-sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 19:54:24.000000 cli-sandbox-0.2.7/cli-sandbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:54:34.266520 cli-sandbox-0.2.7/cli_sandbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:54:34.000000 cli-sandbox-0.2.7/cli_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 19:54:34.000000 cli-sandbox-0.2.7/cli_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:54:34.000000 cli-sandbox-0.2.7/cli_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 19:54:34.000000 cli-sandbox-0.2.7/cli_sandbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 19:54:34.000000 cli-sandbox-0.2.7/cli_sandbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:54:34.266520 cli-sandbox-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-07 19:54:24.000000 cli-sandbox-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:58:37.115978 cli-sandbox-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:58:37.115978 cli-sandbox-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 19:58:26.000000 cli-sandbox-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:58:37.115978 cli-sandbox-0.2.8/cli-sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 19:58:26.000000 cli-sandbox-0.2.8/cli-sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 19:58:26.000000 cli-sandbox-0.2.8/cli-sandbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:58:37.115978 cli-sandbox-0.2.8/cli_sandbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:58:37.000000 cli-sandbox-0.2.8/cli_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 19:58:37.000000 cli-sandbox-0.2.8/cli_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:58:37.000000 cli-sandbox-0.2.8/cli_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 19:58:37.000000 cli-sandbox-0.2.8/cli_sandbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 19:58:37.000000 cli-sandbox-0.2.8/cli_sandbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:58:37.115978 cli-sandbox-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-07 19:58:26.000000 cli-sandbox-0.2.8/setup.py
```

### Comparing `cli-sandbox-0.2.7/PKG-INFO` & `cli-sandbox-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.7
+Version: 0.2.8
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.7/cli_sandbox.egg-info/PKG-INFO` & `cli-sandbox-0.2.8/cli_sandbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.7
+Version: 0.2.8
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.7/setup.py` & `cli-sandbox-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-sandbox',
-    version='0.2.7',
+    version='0.2.8',
     description='cli experiments',
     author='Your Name',
     author_email='hughes036@gmail.com',
     url='https://github.com/AllenCell/cli-sandbox',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

