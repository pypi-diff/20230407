# Comparing `tmp/motion_python-0.1.23.tar.gz` & `tmp/motion_python-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.23.tar", max compression
+gzip compressed data, was "motion_python-0.1.24.tar", max compression
```

## Comparing `motion_python-0.1.23.tar` & `motion_python-0.1.24.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-07 21:35:06.799552 motion_python-0.1.23/README.md
--rw-r--r--   0        0        0      641 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/api/models.py
--rw-r--r--   0        0        0     2582 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/cli.py
--rw-r--r--   0        0        0     6675 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/client.py
--rw-r--r--   0        0        0    21748 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/cursor.py
--rw-r--r--   0        0        0     8099 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      421 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1351 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4564 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     4754 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     1771 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/routing.py
--rw-r--r--   0        0        0     2671 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/task.py
--rw-r--r--   0        0        0     5010 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-07 21:35:06.799552 motion_python-0.1.23/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-07 21:35:26.044870 motion_python-0.1.23/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0     2819 2023-04-07 21:44:48.090970 motion_python-0.1.24/README.md
+-rw-r--r--   0        0        0      641 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/api/__init__.py
+-rw-r--r--   0        0        0     6702 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/api/models.py
+-rw-r--r--   0        0        0     2582 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/cli.py
+-rw-r--r--   0        0        0     6675 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/client.py
+-rw-r--r--   0        0        0    21748 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/cursor.py
+-rw-r--r--   0        0        0     8099 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1934 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      421 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1351 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4564 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     4754 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     1771 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/routing.py
+-rw-r--r--   0        0        0     2671 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/schema.py
+-rw-r--r--   0        0        0    14188 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/store.py
+-rw-r--r--   0        0        0     3741 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/task.py
+-rw-r--r--   0        0        0     5010 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/trigger.py
+-rw-r--r--   0        0        0     1092 2023-04-07 21:44:48.094970 motion_python-0.1.24/motion/utils.py
+-rw-r--r--   0        0        0     1416 2023-04-07 21:45:11.380379 motion_python-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.24/PKG-INFO
```

### Comparing `motion_python-0.1.23/README.md` & `motion_python-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/__init__.py` & `motion_python-0.1.24/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/api/api.py` & `motion_python-0.1.24/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/api/models.py` & `motion_python-0.1.24/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/cli.py` & `motion_python-0.1.24/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/client.py` & `motion_python-0.1.24/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/cursor.py` & `motion_python-0.1.24/motion/cursor.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/entry.py` & `motion_python-0.1.24/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/examples/cooking/dashboard.py` & `motion_python-0.1.24/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/examples/cooking/test.py` & `motion_python-0.1.24/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.24/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.24/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/routing.py` & `motion_python-0.1.24/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/schema.py` & `motion_python-0.1.24/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/store.py` & `motion_python-0.1.24/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/task.py` & `motion_python-0.1.24/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/trigger.py` & `motion_python-0.1.24/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/motion/utils.py` & `motion_python-0.1.24/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.23/pyproject.toml` & `motion_python-0.1.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.23"
+version = "0.1.24"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.23/PKG-INFO` & `motion_python-0.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.23
+Version: 0.1.24
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

