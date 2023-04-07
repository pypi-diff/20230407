# Comparing `tmp/cli-sandbox-0.2.3.tar.gz` & `tmp/cli-sandbox-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-sandbox-0.2.3.tar", last modified: Fri Apr  7 18:59:18 2023, max compression
+gzip compressed data, was "cli-sandbox-0.2.4.tar", last modified: Fri Apr  7 19:18:29 2023, max compression
```

## Comparing `cli-sandbox-0.2.3.tar` & `cli-sandbox-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:59:18.379773 cli-sandbox-0.2.3/
--rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 18:59:18.379773 cli-sandbox-0.2.3/PKG-INFO
--rw-r--r--   0 github    (1001) github    (1001)       70 2023-04-07 17:59:25.000000 cli-sandbox-0.2.3/README.md
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:59:18.379773 cli-sandbox-0.2.3/cli-sandbox/
--rw-r--r--   0 github    (1001) github    (1001)      107 2023-04-07 18:59:14.000000 cli-sandbox-0.2.3/cli-sandbox/__init__.py
--rw-r--r--   0 github    (1001) github    (1001)       41 2023-04-07 17:59:25.000000 cli-sandbox-0.2.3/cli-sandbox/app.py
-drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:59:18.379773 cli-sandbox-0.2.3/cli_sandbox.egg-info/
--rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 18:59:18.000000 cli-sandbox-0.2.3/cli_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 github    (1001) github    (1001)      235 2023-04-07 18:59:18.000000 cli-sandbox-0.2.3/cli_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 github    (1001) github    (1001)        1 2023-04-07 18:59:18.000000 cli-sandbox-0.2.3/cli_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 github    (1001) github    (1001)       26 2023-04-07 18:59:18.000000 cli-sandbox-0.2.3/cli_sandbox.egg-info/requires.txt
--rw-r--r--   0 github    (1001) github    (1001)       12 2023-04-07 18:59:18.000000 cli-sandbox-0.2.3/cli_sandbox.egg-info/top_level.txt
--rw-r--r--   0 github    (1001) github    (1001)       38 2023-04-07 18:59:18.379773 cli-sandbox-0.2.3/setup.cfg
--rw-r--r--   0 github    (1001) github    (1001)      759 2023-04-07 18:59:14.000000 cli-sandbox-0.2.3/setup.py
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/
+-rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/PKG-INFO
+-rw-r--r--   0 github    (1001) github    (1001)       70 2023-04-07 17:59:25.000000 cli-sandbox-0.2.4/README.md
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/cli-sandbox/
+-rw-r--r--   0 github    (1001) github    (1001)      107 2023-04-07 19:18:24.000000 cli-sandbox-0.2.4/cli-sandbox/__init__.py
+-rw-r--r--   0 github    (1001) github    (1001)       41 2023-04-07 17:59:25.000000 cli-sandbox-0.2.4/cli-sandbox/app.py
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/cli_sandbox.egg-info/
+-rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 github    (1001) github    (1001)      235 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 github    (1001) github    (1001)        1 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 github    (1001) github    (1001)       26 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/requires.txt
+-rw-r--r--   0 github    (1001) github    (1001)       12 2023-04-07 19:18:29.000000 cli-sandbox-0.2.4/cli_sandbox.egg-info/top_level.txt
+-rw-r--r--   0 github    (1001) github    (1001)       38 2023-04-07 19:18:29.885996 cli-sandbox-0.2.4/setup.cfg
+-rw-r--r--   0 github    (1001) github    (1001)      759 2023-04-07 19:18:24.000000 cli-sandbox-0.2.4/setup.py
```

### Comparing `cli-sandbox-0.2.3/PKG-INFO` & `cli-sandbox-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.3
+Version: 0.2.4
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.3/cli_sandbox.egg-info/PKG-INFO` & `cli-sandbox-0.2.4/cli_sandbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.3
+Version: 0.2.4
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.3/setup.py` & `cli-sandbox-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-sandbox',
-    version='0.2.3',
+    version='0.2.4',
     description='cli experiments',
     author='Your Name',
     author_email='hughes036@gmail.com',
     url='https://github.com/AllenCell/cli-sandbox',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

