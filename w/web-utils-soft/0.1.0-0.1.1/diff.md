# Comparing `tmp/web-utils-soft-0.1.0.tar.gz` & `tmp/web-utils-soft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-utils-soft-0.1.0.tar", last modified: Fri Apr  7 19:36:44 2023, max compression
+gzip compressed data, was "web-utils-soft-0.1.1.tar", last modified: Fri Apr  7 20:29:36 2023, max compression
```

## Comparing `web-utils-soft-0.1.0.tar` & `web-utils-soft-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 19:36:44.434732 web-utils-soft-0.1.0/
--rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-04-07 14:32:33.000000 web-utils-soft-0.1.0/LICENSE
--rw-r--r--   0 edward    (1000) edward    (1000)      239 2023-04-07 19:36:44.434732 web-utils-soft-0.1.0/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     1320 2023-04-07 17:13:38.000000 web-utils-soft-0.1.0/README.md
--rw-r--r--   0 edward    (1000) edward    (1000)      112 2023-04-07 19:36:44.434732 web-utils-soft-0.1.0/setup.cfg
--rw-r--r--   0 edward    (1000) edward    (1000)      577 2023-04-07 19:36:26.000000 web-utils-soft-0.1.0/setup.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 19:36:44.434732 web-utils-soft-0.1.0/tests/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-04-07 14:14:51.000000 web-utils-soft-0.1.0/tests/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3138 2023-04-07 16:20:26.000000 web-utils-soft-0.1.0/tests/test_image_utils.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1632 2023-04-07 16:26:45.000000 web-utils-soft-0.1.0/tests/test_json_utils.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-04-07 19:36:44.434732 web-utils-soft-0.1.0/web_utils_soft.egg-info/
--rw-r--r--   0 edward    (1000) edward    (1000)      239 2023-04-07 19:36:44.000000 web-utils-soft-0.1.0/web_utils_soft.egg-info/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)      298 2023-04-07 19:36:44.000000 web-utils-soft-0.1.0/web_utils_soft.egg-info/SOURCES.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-04-07 19:36:44.000000 web-utils-soft-0.1.0/web_utils_soft.egg-info/dependency_links.txt
--rw-r--r--   0 edward    (1000) edward    (1000)       91 2023-04-07 19:36:44.000000 web-utils-soft-0.1.0/web_utils_soft.egg-info/entry_points.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        6 2023-04-07 19:36:44.000000 web-utils-soft-0.1.0/web_utils_soft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:29:36.540899 web-utils-soft-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-07 20:29:22.000000 web-utils-soft-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 20:29:36.540899 web-utils-soft-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-07 20:29:22.000000 web-utils-soft-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-07 20:29:36.540899 web-utils-soft-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-07 20:29:34.000000 web-utils-soft-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:29:36.540899 web-utils-soft-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 20:29:22.000000 web-utils-soft-0.1.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-04-07 20:29:22.000000 web-utils-soft-0.1.1/tests/test_image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-07 20:29:22.000000 web-utils-soft-0.1.1/tests/test_json_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:29:36.540899 web-utils-soft-0.1.1/web_utils_soft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 20:29:36.000000 web-utils-soft-0.1.1/web_utils_soft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-07 20:29:36.000000 web-utils-soft-0.1.1/web_utils_soft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:29:36.000000 web-utils-soft-0.1.1/web_utils_soft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-07 20:29:36.000000 web-utils-soft-0.1.1/web_utils_soft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-07 20:29:36.000000 web-utils-soft-0.1.1/web_utils_soft.egg-info/top_level.txt
```

### Comparing `web-utils-soft-0.1.0/LICENSE` & `web-utils-soft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web-utils-soft-0.1.0/README.md` & `web-utils-soft-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `web-utils-soft-0.1.0/setup.py` & `web-utils-soft-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 setup(
     name="web-utils-soft",
     version=__version__,
     description="Python Project package",
     long_description="Project to set web utils to get data from the web",
     author="Wilson Ramirez",
```

### Comparing `web-utils-soft-0.1.0/tests/test_image_utils.py` & `web-utils-soft-0.1.1/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `web-utils-soft-0.1.0/tests/test_json_utils.py` & `web-utils-soft-0.1.1/tests/test_json_utils.py`

 * *Files identical despite different names*

