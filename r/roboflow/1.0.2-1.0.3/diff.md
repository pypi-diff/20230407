# Comparing `tmp/roboflow-1.0.2.tar.gz` & `tmp/roboflow-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.0.2.tar", last modified: Fri Mar 31 18:20:11 2023, max compression
+gzip compressed data, was "roboflow-1.0.3.tar", last modified: Fri Apr  7 16:09:55 2023, max compression
```

## Comparing `roboflow-1.0.2.tar` & `roboflow-1.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-31 18:19:45.000000 roboflow-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-03-31 18:20:11.610482 roboflow-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-03-31 18:19:45.000000 roboflow-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 18:19:45.000000 roboflow-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.606482 roboflow-1.0.2/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.606482 roboflow-1.0.2/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.606482 roboflow-1.0.2/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22648 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.606482 roboflow-1.0.2/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-03-31 18:19:45.000000 roboflow-1.0.2/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.606482 roboflow-1.0.2/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-03-31 18:20:11.000000 roboflow-1.0.2/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-31 18:20:11.000000 roboflow-1.0.2/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:20:11.000000 roboflow-1.0.2/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 18:20:11.000000 roboflow-1.0.2/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 18:20:11.000000 roboflow-1.0.2/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 18:20:11.610482 roboflow-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-31 18:19:45.000000 roboflow-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:20:11.610482 roboflow-1.0.2/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-31 18:19:45.000000 roboflow-1.0.2/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.390012 roboflow-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-07 16:09:27.000000 roboflow-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-07 16:09:55.390012 roboflow-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-07 16:09:27.000000 roboflow-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 16:09:27.000000 roboflow-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22648 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-07 16:09:27.000000 roboflow-1.0.3/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-07 16:09:55.000000 roboflow-1.0.3/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-07 16:09:55.000000 roboflow-1.0.3/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:09:55.000000 roboflow-1.0.3/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-07 16:09:55.000000 roboflow-1.0.3/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-07 16:09:55.000000 roboflow-1.0.3/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:09:55.390012 roboflow-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-07 16:09:27.000000 roboflow-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.386012 roboflow-1.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.390012 roboflow-1.0.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.390012 roboflow-1.0.3/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:09:55.390012 roboflow-1.0.3/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 16:09:27.000000 roboflow-1.0.3/tests/util/test_versions.py
```

### Comparing `roboflow-1.0.2/LICENSE` & `roboflow-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/PKG-INFO` & `roboflow-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.2
+Version: 1.0.3
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.2 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.3 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.2/README.md` & `roboflow-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/__init__.py` & `roboflow-1.0.3/roboflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
@@ -68,17 +68,25 @@
     r = check_key(api_key)
     w = r["workspace"]
 
     return Roboflow(api_key, w)
 
 
 def login(workspace=None, force=False):
+    os_name = os.name
+
+    if os_name == "nt":
+        default_path = os.getenv("USERPROFILE") + "\\roboflow\\config.json"
+    else:
+        default_path = os.getenv("HOME") + "/.config/roboflow/config.json"
+
+    # default configuration location
     conf_location = os.getenv(
         "ROBOFLOW_CONFIG_DIR",
-        default=os.getenv("HOME") + "/.config/roboflow/config.json",
+        default=default_path,
     )
 
     if os.path.isfile(conf_location) and not force:
         write_line(
             "You are already logged into Roboflow. To make a different login, run roboflow.login(force=True)."
         )
         return None
```

### Comparing `roboflow-1.0.2/roboflow/archive/plot.py` & `roboflow-1.0.3/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/config.py` & `roboflow-1.0.3/roboflow/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,25 @@
     Args:
         key (string): The name of the configuration variable.
         default (string): The default value of the configuration variable.
     Returns:
         string: The value of the conditional configuration variable.
     """
 
+    os_name = os.name
+
+    if os_name == "nt":
+        default_path = os.getenv("USERPROFILE") + "\\roboflow\\config.json"
+    else:
+        default_path = os.getenv("HOME") + "/.config/roboflow/config.json"
+
     # default configuration location
     conf_location = os.getenv(
         "ROBOFLOW_CONFIG_DIR",
-        default=os.getenv("HOME") + "/.config/roboflow/config.json",
+        default=default_path,
     )
 
     # read config file for roboflow if logged in from python or CLI
     if os.path.exists(conf_location):
         with open(conf_location) as f:
             config = json.load(f)
     else:
```

### Comparing `roboflow-1.0.2/roboflow/core/project.py` & `roboflow-1.0.3/roboflow/core/project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/core/version.py` & `roboflow-1.0.3/roboflow/core/version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/core/workspace.py` & `roboflow-1.0.3/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/models/classification.py` & `roboflow-1.0.3/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/models/inference.py` & `roboflow-1.0.3/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/models/instance_segmentation.py` & `roboflow-1.0.3/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/models/object_detection.py` & `roboflow-1.0.3/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/models/semantic_segmentation.py` & `roboflow-1.0.3/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/active_learning_utils.py` & `roboflow-1.0.3/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/clip_compare_utils.py` & `roboflow-1.0.3/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/image_utils.py` & `roboflow-1.0.3/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/prediction.py` & `roboflow-1.0.3/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/two_stage_utils.py` & `roboflow-1.0.3/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow/util/versions.py` & `roboflow-1.0.3/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/roboflow.egg-info/PKG-INFO` & `roboflow-1.0.3/roboflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.2
+Version: 1.0.3
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.2 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.3 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.2/roboflow.egg-info/SOURCES.txt` & `roboflow-1.0.3/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/setup.py` & `roboflow-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/models/test_instance_segmentation.py` & `roboflow-1.0.3/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/models/test_object_detection.py` & `roboflow-1.0.3/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/models/test_semantic_segmentation.py` & `roboflow-1.0.3/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/test_project.py` & `roboflow-1.0.3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/test_queries.py` & `roboflow-1.0.3/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/test_version.py` & `roboflow-1.0.3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/util/test_image_utils.py` & `roboflow-1.0.3/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.2/tests/util/test_versions.py` & `roboflow-1.0.3/tests/util/test_versions.py`

 * *Files identical despite different names*

