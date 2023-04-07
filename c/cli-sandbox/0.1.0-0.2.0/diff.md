# Comparing `tmp/cli-sandbox-0.1.0.tar.gz` & `tmp/cli-sandbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-sandbox-0.1.0.tar", last modified: Fri Apr  7 15:50:35 2023, max compression
+gzip compressed data, was "cli-sandbox-0.2.0.tar", last modified: Fri Apr  7 16:50:16 2023, max compression
```

## Comparing `cli-sandbox-0.1.0.tar` & `cli-sandbox-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 15:50:35.779899 cli-sandbox-0.1.0/
--rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 15:50:35.779525 cli-sandbox-0.1.0/PKG-INFO
--rw-r--r--   0 chrishu    (503) staff       (20)       70 2023-04-07 14:46:06.000000 cli-sandbox-0.1.0/README.md
-drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 15:50:35.778959 cli-sandbox-0.1.0/cli_sandbox.egg-info/
--rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 15:50:35.000000 cli-sandbox-0.1.0/cli_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 chrishu    (503) staff       (20)      192 2023-04-07 15:50:35.000000 cli-sandbox-0.1.0/cli_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrishu    (503) staff       (20)        1 2023-04-07 15:50:35.000000 cli-sandbox-0.1.0/cli_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrishu    (503) staff       (20)       26 2023-04-07 15:50:35.000000 cli-sandbox-0.1.0/cli_sandbox.egg-info/requires.txt
--rw-r--r--   0 chrishu    (503) staff       (20)        1 2023-04-07 15:50:35.000000 cli-sandbox-0.1.0/cli_sandbox.egg-info/top_level.txt
--rw-r--r--   0 chrishu    (503) staff       (20)       38 2023-04-07 15:50:35.780010 cli-sandbox-0.1.0/setup.cfg
--rw-r--r--   0 chrishu    (503) staff       (20)      759 2023-04-07 15:50:31.000000 cli-sandbox-0.1.0/setup.py
+drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.375546 cli-sandbox-0.2.0/
+-rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 16:50:16.375070 cli-sandbox-0.2.0/PKG-INFO
+-rw-r--r--   0 chrishu    (503) staff       (20)       70 2023-04-07 14:46:06.000000 cli-sandbox-0.2.0/README.md
+drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.370060 cli-sandbox-0.2.0/cli-sandbox/
+-rw-r--r--   0 chrishu    (503) staff       (20)      107 2023-04-07 16:33:46.000000 cli-sandbox-0.2.0/cli-sandbox/__init__.py
+drwxr-xr-x   0 chrishu    (503) staff       (20)        0 2023-04-07 16:50:16.373940 cli-sandbox-0.2.0/cli_sandbox.egg-info/
+-rw-r--r--   0 chrishu    (503) staff       (20)      595 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrishu    (503) staff       (20)      216 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrishu    (503) staff       (20)        1 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrishu    (503) staff       (20)       26 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/requires.txt
+-rw-r--r--   0 chrishu    (503) staff       (20)       12 2023-04-07 16:50:16.000000 cli-sandbox-0.2.0/cli_sandbox.egg-info/top_level.txt
+-rw-r--r--   0 chrishu    (503) staff       (20)       38 2023-04-07 16:50:16.375672 cli-sandbox-0.2.0/setup.cfg
+-rw-r--r--   0 chrishu    (503) staff       (20)      759 2023-04-07 16:33:46.000000 cli-sandbox-0.2.0/setup.py
```

### Comparing `cli-sandbox-0.1.0/PKG-INFO` & `cli-sandbox-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.1.0/cli_sandbox.egg-info/PKG-INFO` & `cli-sandbox-0.2.0/cli_sandbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-sandbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: cli experiments
 Home-page: https://github.com/AllenCell/cli-sandbox
 Author: Your Name
 Author-email: hughes036@gmail.com
 License: UNKNOWN
 Keywords: your keywords here
 Platform: UNKNOWN
```

### Comparing `cli-sandbox-0.1.0/setup.py` & `cli-sandbox-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cli-sandbox',
-    version='0.1.0',
+    version='0.2.0',
     description='cli experiments',
     author='Your Name',
     author_email='hughes036@gmail.com',
     url='https://github.com/AllenCell/cli-sandbox',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

