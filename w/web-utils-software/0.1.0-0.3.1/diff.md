# Comparing `tmp/web_utils_software-0.1.0.tar.gz` & `tmp/web_utils_software-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_utils_software-0.1.0.tar", last modified: Fri Apr  7 21:06:40 2023, max compression
+gzip compressed data, was "web_utils_software-0.3.1.tar", last modified: Fri Apr  7 21:25:18 2023, max compression
```

## Comparing `web_utils_software-0.1.0.tar` & `web_utils_software-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.354290 web_utils_software-0.1.0/
--rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-04-07 14:32:33.000000 web_utils_software-0.1.0/LICENSE
--rw-r--r--   0 edward    (1000) edward    (1000)      243 2023-04-07 21:06:40.354290 web_utils_software-0.1.0/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     1320 2023-04-07 17:13:38.000000 web_utils_software-0.1.0/README.md
--rw-r--r--   0 edward    (1000) edward    (1000)      133 2023-04-07 21:06:40.354290 web_utils_software-0.1.0/setup.cfg
--rw-r--r--   0 edward    (1000) edward    (1000)      633 2023-04-07 21:06:24.000000 web_utils_software-0.1.0/setup.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.344290 web_utils_software-0.1.0/src/
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.344290 web_utils_software-0.1.0/src/image_utils/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-04-07 14:26:40.000000 web_utils_software-0.1.0/src/image_utils/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)      890 2023-04-07 16:35:48.000000 web_utils_software-0.1.0/src/image_utils/get.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.344290 web_utils_software-0.1.0/src/json_utils/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-04-07 20:52:24.000000 web_utils_software-0.1.0/src/json_utils/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)      438 2023-04-07 16:35:33.000000 web_utils_software-0.1.0/src/json_utils/get.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.354290 web_utils_software-0.1.0/src/web_utils_software.egg-info/
--rw-r--r--   0 edward    (1000) edward    (1000)      243 2023-04-07 21:06:40.000000 web_utils_software-0.1.0/src/web_utils_software.egg-info/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)      371 2023-04-07 21:06:40.000000 web_utils_software-0.1.0/src/web_utils_software.egg-info/SOURCES.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-04-07 21:06:40.000000 web_utils_software-0.1.0/src/web_utils_software.egg-info/dependency_links.txt
--rw-r--r--   0 edward    (1000) edward    (1000)       23 2023-04-07 21:06:40.000000 web_utils_software-0.1.0/src/web_utils_software.egg-info/top_level.txt
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 21:06:40.354290 web_utils_software-0.1.0/tests/
--rw-r--r--   0 edward    (1000) edward    (1000)     3142 2023-04-07 20:55:24.000000 web_utils_software-0.1.0/tests/test_image_utils.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1776 2023-04-07 20:55:08.000000 web_utils_software-0.1.0/tests/test_json_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:25:18.649129 web_utils_software-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-07 21:25:18.649129 web_utils_software-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-07 21:25:18.649129 web_utils_software-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-07 21:25:16.000000 web_utils_software-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:25:18.645129 web_utils_software-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:25:18.645129 web_utils_software-0.3.1/src/image_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/src/image_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/src/image_utils/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:25:18.649129 web_utils_software-0.3.1/src/json_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/src/json_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-07 21:25:04.000000 web_utils_software-0.3.1/src/json_utils/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:25:18.649129 web_utils_software-0.3.1/src/web_utils_software.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-07 21:25:18.000000 web_utils_software-0.3.1/src/web_utils_software.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-07 21:25:18.000000 web_utils_software-0.3.1/src/web_utils_software.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 21:25:18.000000 web_utils_software-0.3.1/src/web_utils_software.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-07 21:25:18.000000 web_utils_software-0.3.1/src/web_utils_software.egg-info/top_level.txt
```

### Comparing `web_utils_software-0.1.0/LICENSE` & `web_utils_software-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web_utils_software-0.1.0/README.md` & `web_utils_software-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `web_utils_software-0.1.0/setup.py` & `web_utils_software-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.1.0"
+__version__ = "0.3.1"
 
 setup(
     name="web_utils_software",
     version=__version__,
     description="Python Project package",
     long_description="Project to set web utils to get data from the web",
     author="Wilson Ramirez",
```

### Comparing `web_utils_software-0.1.0/src/image_utils/get.py` & `web_utils_software-0.3.1/src/image_utils/get.py`

 * *Files identical despite different names*

