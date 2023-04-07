# Comparing `tmp/iamlogic_idm_package-1.1.1.tar.gz` & `tmp/iamlogic_idm_package-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlogic_idm_package-1.1.1.tar", last modified: Wed Apr  5 19:05:46 2023, max compression
+gzip compressed data, was "iamlogic_idm_package-1.1.2.tar", last modified: Wed Apr  5 19:44:16 2023, max compression
```

## Comparing `iamlogic_idm_package-1.1.1.tar` & `iamlogic_idm_package-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 19:05:46.017489 iamlogic_idm_package-1.1.1/
--rw-rw-rw-   0        0        0      453 2023-04-05 19:05:46.016494 iamlogic_idm_package-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-05 19:05:46.000111 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-05 19:05:45.000000 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-05 19:05:45.000000 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 19:05:45.000000 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-05 19:05:45.000000 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-05 19:05:45.000000 iamlogic_idm_package-1.1.1/iamlogic_idm_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 19:05:46.013489 iamlogic_idm_package-1.1.1/idm_operation/
--rw-rw-rw-   0        0        0     8837 2023-04-05 19:05:14.000000 iamlogic_idm_package-1.1.1/idm_operation/IDM_Operation.py
--rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm_package-1.1.1/idm_operation/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-05 19:05:46.018491 iamlogic_idm_package-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-05 19:05:42.000000 iamlogic_idm_package-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.691003 iamlogic_idm_package-1.1.2/
+-rw-rw-rw-   0        0        0      453 2023-04-05 19:44:16.687999 iamlogic_idm_package-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.661244 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-05 19:44:16.000000 iamlogic_idm_package-1.1.2/iamlogic_idm_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-05 19:44:16.686000 iamlogic_idm_package-1.1.2/idm_operation/
+-rw-rw-rw-   0        0        0     8837 2023-04-05 19:42:58.000000 iamlogic_idm_package-1.1.2/idm_operation/IDM_Operation.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:53:08.000000 iamlogic_idm_package-1.1.2/idm_operation/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-05 19:44:16.691003 iamlogic_idm_package-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-05 19:43:06.000000 iamlogic_idm_package-1.1.2/setup.py
```

### Comparing `iamlogic_idm_package-1.1.1/idm_operation/IDM_Operation.py` & `iamlogic_idm_package-1.1.2/idm_operation/IDM_Operation.py`

 * *Files identical despite different names*

### Comparing `iamlogic_idm_package-1.1.1/setup.py` & `iamlogic_idm_package-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iamlogic_idm_package',
-    version='1.1.1',
+    version='1.1.2',
     description='IDM package',
     author='Prabhu S',
     author_email='prabhu@iamlogic.com',
     packages=find_packages(),
     install_requires=[
         'requests',
         'cryptography',
```

