# Comparing `tmp/motion_python-0.1.20.tar.gz` & `tmp/motion_python-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.20.tar", max compression
+gzip compressed data, was "motion_python-0.1.21.tar", max compression
```

## Comparing `motion_python-0.1.20.tar` & `motion_python-0.1.21.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-07 20:00:04.000788 motion_python-0.1.20/README.md
--rw-r--r--   0        0        0      641 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/api/models.py
--rw-r--r--   0        0        0     2582 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/cli.py
--rw-r--r--   0        0        0     6675 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/client.py
--rw-r--r--   0        0        0    21748 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/cursor.py
--rw-r--r--   0        0        0     8091 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      421 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1351 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4564 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     4754 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     1771 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/routing.py
--rw-r--r--   0        0        0     2671 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-07 20:00:04.000788 motion_python-0.1.20/motion/task.py
--rw-r--r--   0        0        0     5010 2023-04-07 20:00:04.004788 motion_python-0.1.20/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-07 20:00:04.004788 motion_python-0.1.20/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-07 20:00:25.301192 motion_python-0.1.20/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0     2819 2023-04-07 21:09:44.840269 motion_python-0.1.21/README.md
+-rw-r--r--   0        0        0      641 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/api/__init__.py
+-rw-r--r--   0        0        0     6702 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/api/models.py
+-rw-r--r--   0        0        0     2582 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/cli.py
+-rw-r--r--   0        0        0     6675 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/client.py
+-rw-r--r--   0        0        0    21748 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/cursor.py
+-rw-r--r--   0        0        0     8091 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1934 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1351 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4564 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     4754 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     1771 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/routing.py
+-rw-r--r--   0        0        0     2671 2023-04-07 21:09:44.840269 motion_python-0.1.21/motion/schema.py
+-rw-r--r--   0        0        0    14188 2023-04-07 21:09:44.844269 motion_python-0.1.21/motion/store.py
+-rw-r--r--   0        0        0     3741 2023-04-07 21:09:44.844269 motion_python-0.1.21/motion/task.py
+-rw-r--r--   0        0        0     5010 2023-04-07 21:09:44.844269 motion_python-0.1.21/motion/trigger.py
+-rw-r--r--   0        0        0     1092 2023-04-07 21:09:44.844269 motion_python-0.1.21/motion/utils.py
+-rw-r--r--   0        0        0     1416 2023-04-07 21:10:04.420034 motion_python-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.21/PKG-INFO
```

### Comparing `motion_python-0.1.20/README.md` & `motion_python-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/__init__.py` & `motion_python-0.1.21/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/api/api.py` & `motion_python-0.1.21/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/api/models.py` & `motion_python-0.1.21/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/cli.py` & `motion_python-0.1.21/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/client.py` & `motion_python-0.1.21/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/cursor.py` & `motion_python-0.1.21/motion/cursor.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/entry.py` & `motion_python-0.1.21/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/examples/cooking/dashboard.py` & `motion_python-0.1.21/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/examples/cooking/test.py` & `motion_python-0.1.21/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.21/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.21/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/routing.py` & `motion_python-0.1.21/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/schema.py` & `motion_python-0.1.21/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/store.py` & `motion_python-0.1.21/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/task.py` & `motion_python-0.1.21/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/trigger.py` & `motion_python-0.1.21/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/motion/utils.py` & `motion_python-0.1.21/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.20/pyproject.toml` & `motion_python-0.1.21/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.20"
+version = "0.1.21"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.20/PKG-INFO` & `motion_python-0.1.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.20
+Version: 0.1.21
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

