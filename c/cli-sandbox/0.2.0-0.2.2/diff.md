# Comparing `tmp/cli-sandbox-0.2.0.tar.gz` & `tmp/cli-sandbox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-sandbox-0.2.0.tar", last modified: Fri Apr  7 16:50:16 2023, max compression
+gzip compressed data, was "cli-sandbox-0.2.2.tar", last modified: Fri Apr  7 18:35:46 2023, max compression
```

## Comparing `cli-sandbox-0.2.0.tar` & `cli-sandbox-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.375546 cli-sandbox-0.2.0/
--rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 16:50:16.375070 cli-sandbox-0.2.0/PKG-INFO
--rw-r--r--   0 chrishu    (503) staff       (20)       70 2023-04-07 14:46:06.000000 cli-sandbox-0.2.0/README.md
-drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.370060 cli-sandbox-0.2.0/cli-sandbox/
--rw-r--r--   0 chrishu    (503) staff       (20)      107 2023-04-07 16:33:46.000000 cli-sandbox-0.2.0/cli-sandbox/__init__.py
-drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.373940 cli-sandbox-0.2.0/cli_sandbox.egg-info/
--rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 chrishu    (503) staff       (20)      216 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrishu    (503) staff       (20)        1 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrishu    (503) staff       (20)       26 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/requires.txt
--rw-r--r--   0 chrishu    (503) staff       (20)       12 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/top_level.txt
--rw-r--r--   0 chrishu    (503) staff       (20)       38 2023-04-07 16:50:16.375672 cli-sandbox-0.2.0/setup.cfg
--rw-r--r--   0 chrishu    (503) staff       (20)      759 2023-04-07 16:33:46.000000 cli-sandbox-0.2.0/setup.py
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:35:46.276720 cli-sandbox-0.2.2/
+-rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 18:35:46.276720 cli-sandbox-0.2.2/PKG-INFO
+-rw-r--r--   0 github    (1001) github    (1001)       70 2023-04-07 17:59:25.000000 cli-sandbox-0.2.2/README.md
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:35:46.272720 cli-sandbox-0.2.2/cli-sandbox/
+-rw-r--r--   0 github    (1001) github    (1001)      107 2023-04-07 18:35:41.000000 cli-sandbox-0.2.2/cli-sandbox/__init__.py
+-rw-r--r--   0 github    (1001) github    (1001)       41 2023-04-07 17:59:25.000000 cli-sandbox-0.2.2/cli-sandbox/app.py
+drwxr-xr-x   0 github    (1001) github    (1001)        0 2023-04-07 18:35:46.276720 cli-sandbox-0.2.2/cli_sandbox.egg-info/
+-rw-r--r--   0 github    (1001) github    (1001)      595 2023-04-07 18:35:46.000000 cli-sandbox-0.2.2/cli_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 github    (1001) github    (1001)      235 2023-04-07 18:35:46.000000 cli-sandbox-0.2.2/cli_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 github    (1001) github    (1001)        1 2023-04-07 18:35:46.000000 cli-sandbox-0.2.2/cli_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 github    (1001) github    (1001)       26 2023-04-07 18:35:46.000000 cli-sandbox-0.2.2/cli_sandbox.egg-info/requires.txt
+-rw-r--r--   0 github    (1001) github    (1001)       12 2023-04-07 18:35:46.000000 cli-sandbox-0.2.2/cli_sandbox.egg-info/top_level.txt
+-rw-r--r--   0 github    (1001) github    (1001)       38 2023-04-07 18:35:46.276720 cli-sandbox-0.2.2/setup.cfg
+-rw-r--r--   0 github    (1001) github    (1001)      759 2023-04-07 18:35:41.000000 cli-sandbox-0.2.2/setup.py
```

### Comparing `cli-sandbox-0.2.0/PKG-INFO` & `cli-sandbox-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.0
+Version: 0.2.2
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.0/cli_sandbox.egg-info/PKG-INFO` & `cli-sandbox-0.2.2/cli_sandbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.2.0
+Version: 0.2.2
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.2.0/setup.py` & `cli-sandbox-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-sandbox',
-    version='0.2.0',
+    version='0.2.2',
     description='cli experiments',
     author='Your Name',
     author_email='hughes036@gmail.com',
     url='https://github.com/AllenCell/cli-sandbox',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

