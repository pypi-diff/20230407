# Comparing `tmp/data_ecosystem_dependencies-202304.0.2.tar.gz` & `tmp/data_ecosystem_dependencies-202304.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202304.0.2.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202304.0.3.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202304.0.2.tar` & `data_ecosystem_dependencies-202304.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-04-07 20:15:04.525763 data_ecosystem_dependencies-202304.0.2/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-04-07 20:15:04.525763 data_ecosystem_dependencies-202304.0.2/license.md
--rw-r--r--   0        0        0     2541 2023-04-07 20:17:35.821103 data_ecosystem_dependencies-202304.0.2/pyproject.toml
--rw-r--r--   0        0        0      341 2023-04-07 20:15:04.525763 data_ecosystem_dependencies-202304.0.2/readme.md
--rw-r--r--   0        0        0      160 2023-04-07 20:15:04.525763 data_ecosystem_dependencies-202304.0.2/setup.cfg
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202304.0.2/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-04-07 20:17:31.568747 data_ecosystem_dependencies-202304.0.3/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-04-07 20:17:31.568747 data_ecosystem_dependencies-202304.0.3/license.md
+-rw-r--r--   0        0        0     2541 2023-04-07 20:20:26.634632 data_ecosystem_dependencies-202304.0.3/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-04-07 20:17:31.568747 data_ecosystem_dependencies-202304.0.3/readme.md
+-rw-r--r--   0        0        0      160 2023-04-07 20:17:31.568747 data_ecosystem_dependencies-202304.0.3/setup.cfg
+-rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202304.0.3/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202304.0.2/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202304.0.3/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.2/license.md` & `data_ecosystem_dependencies-202304.0.3/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.2/pyproject.toml` & `data_ecosystem_dependencies-202304.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202304.0.2"
+version="202304.0.3"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
```

### Comparing `data_ecosystem_dependencies-202304.0.2/PKG-INFO` & `data_ecosystem_dependencies-202304.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202304.0.2
+Version: 202304.0.3
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

