# Comparing `tmp/fairscape_cli-0.1.3.tar.gz` & `tmp/fairscape_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.3.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.4.tar", max compression
```

## Comparing `fairscape_cli-0.1.3.tar` & `fairscape_cli-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.3/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.3/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.3/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.3/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0        0 2023-03-27 17:10:03.768235 fairscape_cli-0.1.3/fairscape_cli/cli.py
--rw-r--r--   0        0        0      397 2023-03-27 17:19:39.488146 fairscape_cli-0.1.3/fairscape_cli/main.py
--rw-r--r--   0        0        0      221 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0      291 2023-04-05 21:07:55.345808 fairscape_cli-0.1.3/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/models/models.py
--rw-r--r--   0        0        0      924 2023-04-06 16:03:52.996807 fairscape_cli-0.1.3/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0      128 2023-04-05 21:07:30.355812 fairscape_cli-0.1.3/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    14576 2023-04-07 17:58:08.150148 fairscape_cli-0.1.3/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-04-07 16:01:30.543608 fairscape_cli-0.1.3/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.3/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1477 2023-04-07 17:58:40.790144 fairscape_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 fairscape_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.4/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:10:03.768235 fairscape_cli-0.1.4/fairscape_cli/cli.py
+-rw-r--r--   0        0        0      397 2023-03-27 17:19:39.488146 fairscape_cli-0.1.4/fairscape_cli/main.py
+-rw-r--r--   0        0        0      221 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-05 21:07:55.345808 fairscape_cli-0.1.4/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0      924 2023-04-06 16:03:52.996807 fairscape_cli-0.1.4/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0      128 2023-04-05 21:07:30.355812 fairscape_cli-0.1.4/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    14576 2023-04-07 17:58:08.150148 fairscape_cli-0.1.4/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-04-07 16:01:30.543608 fairscape_cli-0.1.4/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.4/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1476 2023-04-07 18:56:09.799649 fairscape_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 fairscape_cli-0.1.4/PKG-INFO
```

### Comparing `fairscape_cli-0.1.3/LICENSE` & `fairscape_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/README.md` & `fairscape_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.4/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/models/rocrate.py` & `fairscape_cli-0.1.4/fairscape_cli/models/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.4/fairscape_cli/rocrate/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.4/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.4/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.3/pyproject.toml` & `fairscape_cli-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = ["mlev71 <max.adam.levinson@gmail.com>"]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.6"
 pydantic = "^1.10.7"
 pyld = "^2.0.3"
 click = "^8.1.3"
 fairscape-models = "^0.1.2"
 
 
 [tool.poetry.scripts]
```

### Comparing `fairscape_cli-0.1.3/PKG-INFO` & `fairscape_cli-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: mlev71
 Author-email: max.adam.levinson@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fairscape-models (>=0.1.2,<0.2.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyld (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
```

