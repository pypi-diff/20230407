# Comparing `tmp/electron-0.0.3.tar.gz` & `tmp/electron-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electron-0.0.3.tar", last modified: Fri Apr  7 17:51:24 2023, max compression
+gzip compressed data, was "electron-0.0.4.tar", last modified: Fri Apr  7 17:57:13 2023, max compression
```

## Comparing `electron-0.0.3.tar` & `electron-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:51:24.313210 electron-0.0.3/
--rw-------   0 u0_a689  (10689) u0_a689  (10689)      413 2023-04-07 17:51:24.313210 electron-0.0.3/PKG-INFO
-drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:51:24.313210 electron-0.0.3/electron/
--rw-------   0 u0_a689  (10689) u0_a689  (10689)       41 2023-04-07 17:50:39.000000 electron-0.0.3/electron/__init__.py
--rw-------   0 u0_a689  (10689) u0_a689  (10689)       62 2023-04-07 17:42:11.000000 electron-0.0.3/electron/electron.py
--rw-------   0 u0_a689  (10689) u0_a689  (10689)       61 2023-04-07 17:50:08.000000 electron-0.0.3/electron/hello.py
-drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:51:24.313210 electron-0.0.3/electron.egg-info/
--rw-------   0 u0_a689  (10689) u0_a689  (10689)      413 2023-04-07 17:51:24.000000 electron-0.0.3/electron.egg-info/PKG-INFO
--rw-------   0 u0_a689  (10689) u0_a689  (10689)      196 2023-04-07 17:51:24.000000 electron-0.0.3/electron.egg-info/SOURCES.txt
--rw-------   0 u0_a689  (10689) u0_a689  (10689)        1 2023-04-07 17:51:24.000000 electron-0.0.3/electron.egg-info/dependency_links.txt
--rw-------   0 u0_a689  (10689) u0_a689  (10689)        9 2023-04-07 17:51:24.000000 electron-0.0.3/electron.egg-info/top_level.txt
--rw-------   0 u0_a689  (10689) u0_a689  (10689)       38 2023-04-07 17:51:24.313210 electron-0.0.3/setup.cfg
--rw-------   0 u0_a689  (10689) u0_a689  (10689)      620 2023-04-07 17:51:16.000000 electron-0.0.3/setup.py
+drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:57:13.933210 electron-0.0.4/
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)      413 2023-04-07 17:57:13.933210 electron-0.0.4/PKG-INFO
+drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:57:13.929210 electron-0.0.4/electron/
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)       29 2023-04-07 17:56:07.000000 electron-0.0.4/electron/__init__.py
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)       62 2023-04-07 17:42:11.000000 electron-0.0.4/electron/electron.py
+drwx------   0 u0_a689  (10689) u0_a689  (10689)        0 2023-04-07 17:57:13.929210 electron-0.0.4/electron.egg-info/
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)      413 2023-04-07 17:57:13.000000 electron-0.0.4/electron.egg-info/PKG-INFO
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)      178 2023-04-07 17:57:13.000000 electron-0.0.4/electron.egg-info/SOURCES.txt
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)        1 2023-04-07 17:57:13.000000 electron-0.0.4/electron.egg-info/dependency_links.txt
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)        9 2023-04-07 17:57:13.000000 electron-0.0.4/electron.egg-info/top_level.txt
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)       38 2023-04-07 17:57:13.933210 electron-0.0.4/setup.cfg
+-rw-------   0 u0_a689  (10689) u0_a689  (10689)      620 2023-04-07 17:54:46.000000 electron-0.0.4/setup.py
```

### Comparing `electron-0.0.3/setup.py` & `electron-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="electron",
-    version="0.0.3",
+    version="0.0.4",
     author="CrowXeo",
     author_email="crowxeo@gmail.com",
     description="A web framework for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pornhub.com",
     packages=setuptools.find_packages(),
```

