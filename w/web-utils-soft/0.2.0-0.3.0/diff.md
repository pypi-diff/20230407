# Comparing `tmp/web-utils-soft-0.2.0.tar.gz` & `tmp/web-utils-soft-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-utils-soft-0.2.0.tar", last modified: Fri Apr  7 20:40:17 2023, max compression
+gzip compressed data, was "web-utils-soft-0.3.0.tar", last modified: Fri Apr  7 21:02:56 2023, max compression
```

## Comparing `web-utils-soft-0.2.0.tar` & `web-utils-soft-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:40:17.198688 web-utils-soft-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-07 20:40:03.000000 web-utils-soft-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 20:40:17.198688 web-utils-soft-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1320 2023-04-07 20:40:03.000000 web-utils-soft-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-04-07 20:40:17.198688 web-utils-soft-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      617 2023-04-07 20:40:15.000000 web-utils-soft-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:40:17.194688 web-utils-soft-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:40:17.198688 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 20:40:17.000000 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2023-04-07 20:40:17.000000 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:40:17.000000 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-07 20:40:17.000000 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:40:17.000000 web-utils-soft-0.2.0/src/web_utils_soft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-07 21:02:55.000000 web-utils-soft-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:02:56.612409 web-utils-soft-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/src/image_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/src/image_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/src/image_utils/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/src/json_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/src/json_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-04-07 21:02:42.000000 web-utils-soft-0.3.0/src/json_utils/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 21:02:56.616409 web-utils-soft-0.3.0/src/web_utils_soft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-04-07 21:02:56.000000 web-utils-soft-0.3.0/src/web_utils_soft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-07 21:02:56.000000 web-utils-soft-0.3.0/src/web_utils_soft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 21:02:56.000000 web-utils-soft-0.3.0/src/web_utils_soft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-07 21:02:56.000000 web-utils-soft-0.3.0/src/web_utils_soft.egg-info/top_level.txt
```

### Comparing `web-utils-soft-0.2.0/LICENSE` & `web-utils-soft-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web-utils-soft-0.2.0/README.md` & `web-utils-soft-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `web-utils-soft-0.2.0/setup.py` & `web-utils-soft-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 setup(
     name="web-utils-soft",
     version=__version__,
     description="Python Project package",
     long_description="Project to set web utils to get data from the web",
     author="Wilson Ramirez",
     author_email="wil_ramirez02@hotmail.com",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     # install_requires=["numpy", "pandas"],
-    entry_points={
-        "console_scripts": [
-            "get-data=src.json_utils:get_json",
-            "get-image=src.image_utils:get_image",
-        ]
-    },
+    # entry_points={
+    #     "console_scripts": [
+    #         "get-data=src.json_utils:get_json",
+    #         "get-image=src.image_utils:get_image",
+    #     ]
+    # },
 )
```

