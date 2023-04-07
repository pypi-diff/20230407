# Comparing `tmp/allencell-ml-segmenter-0.0.5.tar.gz` & `tmp/allencell-ml-segmenter-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allencell-ml-segmenter-0.0.5.tar", last modified: Fri Apr  7 21:01:59 2023, max compression
+gzip compressed data, was "allencell-ml-segmenter-0.0.6.tar", last modified: Fri Apr  7 21:03:46 2023, max compression
```

## Comparing `allencell-ml-segmenter-0.0.5.tar` & `allencell-ml-segmenter-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:01:59.759184 allencell-ml-segmenter-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-07 21:01:51.000000 allencell-ml-segmenter-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 21:01:51.000000 allencell-ml-segmenter-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-07 21:01:59.759184 allencell-ml-segmenter-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-07 21:01:51.000000 allencell-ml-segmenter-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-07 21:01:51.000000 allencell-ml-segmenter-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-07 21:01:59.763184 allencell-ml-segmenter-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-07 21:01:51.000000 allencell-ml-segmenter-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:01:59.759184 allencell-ml-segmenter-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:01:59.759184 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:01:59.000000 allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:03:46.585183 allencell-ml-segmenter-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-07 21:03:37.000000 allencell-ml-segmenter-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 21:03:37.000000 allencell-ml-segmenter-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-07 21:03:46.585183 allencell-ml-segmenter-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-07 21:03:37.000000 allencell-ml-segmenter-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-07 21:03:37.000000 allencell-ml-segmenter-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-07 21:03:46.585183 allencell-ml-segmenter-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-07 21:03:37.000000 allencell-ml-segmenter-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:03:46.585183 allencell-ml-segmenter-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:03:46.585183 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:03:46.000000 allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/top_level.txt
```

### Comparing `allencell-ml-segmenter-0.0.5/LICENSE` & `allencell-ml-segmenter-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `allencell-ml-segmenter-0.0.5/PKG-INFO` & `allencell-ml-segmenter-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allencell-ml-segmenter
-Version: 0.0.5
+Version: 0.0.6
 Summary: A plugin to leverage ML segmentation in napari.
 Home-page: https://github.com/AllenCell/allencell-ml-segmenter
 Author: brian kim
 Author-email: brian.kim@alleninstitute.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/AllenCell/allencell-ml-segmenter/issues
 Project-URL: Documentation, https://github.com/AllenCell/allencell-ml-segmenter#README.md
```

### Comparing `allencell-ml-segmenter-0.0.5/README.md` & `allencell-ml-segmenter-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `allencell-ml-segmenter-0.0.5/setup.cfg` & `allencell-ml-segmenter-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = allencell-ml-segmenter
-version = 0.0.5
+version = 0.0.6
 description = A plugin to leverage ML segmentation in napari.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AllenCell/allencell-ml-segmenter
 author = brian kim
 author_email = brian.kim@alleninstitute.org
 license = BSD-3-Clause
```

### Comparing `allencell-ml-segmenter-0.0.5/src/allencell_ml_segmenter.egg-info/PKG-INFO` & `allencell-ml-segmenter-0.0.6/src/allencell_ml_segmenter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allencell-ml-segmenter
-Version: 0.0.5
+Version: 0.0.6
 Summary: A plugin to leverage ML segmentation in napari.
 Home-page: https://github.com/AllenCell/allencell-ml-segmenter
 Author: brian kim
 Author-email: brian.kim@alleninstitute.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/AllenCell/allencell-ml-segmenter/issues
 Project-URL: Documentation, https://github.com/AllenCell/allencell-ml-segmenter#README.md
```

