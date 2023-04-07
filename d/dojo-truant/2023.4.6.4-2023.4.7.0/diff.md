# Comparing `tmp/dojo_truant-2023.4.6.4.tar.gz` & `tmp/dojo_truant-2023.4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.4.6.4.tar", last modified: Fri Apr  7 05:35:40 2023, max compression
+gzip compressed data, was "dojo_truant-2023.4.7.0.tar", last modified: Fri Apr  7 20:00:40 2023, max compression
```

## Comparing `dojo_truant-2023.4.6.4.tar` & `dojo_truant-2023.4.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 05:35:40.879993 dojo_truant-2023.4.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 05:35:40.879993 dojo_truant-2023.4.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 05:35:40.875993 dojo_truant-2023.4.6.4/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 05:35:40.879993 dojo_truant-2023.4.6.4/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 05:35:40.000000 dojo_truant-2023.4.6.4/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-07 05:35:40.000000 dojo_truant-2023.4.6.4/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 05:35:40.000000 dojo_truant-2023.4.6.4/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 05:35:40.000000 dojo_truant-2023.4.6.4/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 05:35:40.000000 dojo_truant-2023.4.6.4/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-07 05:35:26.000000 dojo_truant-2023.4.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 05:35:40.879993 dojo_truant-2023.4.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:00:40.759018 dojo_truant-2023.4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 20:00:40.755018 dojo_truant-2023.4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:00:40.755018 dojo_truant-2023.4.7.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:00:40.755018 dojo_truant-2023.4.7.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 20:00:40.000000 dojo_truant-2023.4.7.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-07 20:00:40.000000 dojo_truant-2023.4.7.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:00:40.000000 dojo_truant-2023.4.7.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 20:00:40.000000 dojo_truant-2023.4.7.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 20:00:40.000000 dojo_truant-2023.4.7.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-07 20:00:25.000000 dojo_truant-2023.4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:00:40.759018 dojo_truant-2023.4.7.0/setup.cfg
```

### Comparing `dojo_truant-2023.4.6.4/LICENSE.txt` & `dojo_truant-2023.4.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.6.4/PKG-INFO` & `dojo_truant-2023.4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.4.6.4
+Version: 2023.4.7.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.4.6.4/dojo/api.py` & `dojo_truant-2023.4.7.0/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.6.4/dojo/dojo_group.py` & `dojo_truant-2023.4.7.0/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.6.4/dojo/product.py` & `dojo_truant-2023.4.7.0/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.6.4/dojo/product_type.py` & `dojo_truant-2023.4.7.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.4.6.4/dojo/write_chain.py` & `dojo_truant-2023.4.7.0/dojo/write_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     for tk, tv in template:
         expanded_template[tk] = json.dumps(tv)
 
     if isinstance(data, dict):
         expanded_data = dict()
         for k, v in data.items():
             if isinstance(v, (list, tuple)):
-                expanded_data[k] = [expand_data(vi) for vi in v]
+                expanded_data[k] = [expand_data(vi, template) for vi in v]
             else:
-                expanded_data[k] = expand_data(v)
+                expanded_data[k] = expand_data(v, template)
 
     elif isinstance(data, string.Template):
         expanded_data = data.safe_substitute(**expanded_template)
     else:
         expanded_data = data
 
     return expanded_data
```

### Comparing `dojo_truant-2023.4.6.4/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.4.7.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.4.6.4
+Version: 2023.4.7.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.4.6.4/pyproject.toml` & `dojo_truant-2023.4.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.04.06.4"
+version = "2023.04.07.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["defectDojo"]
```

