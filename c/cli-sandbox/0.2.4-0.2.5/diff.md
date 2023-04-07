# Comparing `tmp/cli-sandbox-0.2.4.tar.gz` & `tmp/cli-sandbox-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-sandbox-0.2.4.tar", last modified: Fri Apr  7 19:18:29 2023, max compression
+gzip compressed data, was "cli-sandbox-0.2.5.tar", last modified: Fri Apr  7 19:22:57 2023, max compression
```

## Comparing `cli-sandbox-0.2.4.tar` & `cli-sandbox-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/
--rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/PKG-INFO
--rw-r--r--   0 github    (1001) github    (1001)       70 2023-04-07 17:59:25.000000 cli-sandbox-0.2.4/README.md
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/cli-sandbox/
--rw-r--r--   0 github    (1001) github    (1001)      107 2023-04-07 19:18:24.000000 cli-sandbox-0.2.4/cli-sandbox/__init__.py
--rw-r--r--   0 github    (1001) github    (1001)       41 2023-04-07 17:59:25.000000 cli-sandbox-0.2.4/cli-sandbox/app.py
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/cli_sandbox.egg-info/
--rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 github    (1001) github    (1001)      235 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 github    (1001) github    (1001)        1 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 github    (1001) github    (1001)       26 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/requires.txt
--rw-r--r--   0 github    (1001) github    (1001)       12 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/top_level.txt
--rw-r--r--   0 github    (1001) github    (1001)       38 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/setup.cfg
--rw-r--r--   0 github    (1001) github    (1001)      759 2023-04-07 19:18:24.000000 cli-sandbox-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:22:57.636004 cli-sandbox-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:22:57.636004 cli-sandbox-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 19:22:49.000000 cli-sandbox-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:22:57.632004 cli-sandbox-0.2.5/cli-sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 19:22:49.000000 cli-sandbox-0.2.5/cli-sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 19:22:49.000000 cli-sandbox-0.2.5/cli-sandbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:22:57.632004 cli-sandbox-0.2.5/cli_sandbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 19:22:57.000000 cli-sandbox-0.2.5/cli_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 19:22:57.000000 cli-sandbox-0.2.5/cli_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:22:57.000000 cli-sandbox-0.2.5/cli_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 19:22:57.000000 cli-sandbox-0.2.5/cli_sandbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 19:22:57.000000 cli-sandbox-0.2.5/cli_sandbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:22:57.636004 cli-sandbox-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-07 19:22:49.000000 cli-sandbox-0.2.5/setup.py
```

### Comparing `cli-sandbox-0.2.4/PKG-INFO` & `cli-sandbox-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.4
+Version: 0.2.5
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.4/cli_sandbox.egg-info/PKG-INFO` & `cli-sandbox-0.2.5/cli_sandbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.4
+Version: 0.2.5
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.4/setup.py` & `cli-sandbox-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-sandbox',
-    version='0.2.4',
+    version='0.2.5',
     description='cli experiments',
     author='Your Name',
     author_email='hughes036@gmail.com',
     url='https://github.com/AllenCell/cli-sandbox',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

