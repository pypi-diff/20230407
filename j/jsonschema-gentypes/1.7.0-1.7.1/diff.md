# Comparing `tmp/jsonschema_gentypes-1.7.0.tar.gz` & `tmp/jsonschema_gentypes-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-1.7.0.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-1.7.1.tar", max compression
```

## Comparing `jsonschema_gentypes-1.7.0.tar` & `jsonschema_gentypes-1.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1304 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/LICENSE
--rw-r--r--   0        0        0     3554 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/README.md
--rw-r--r--   0        0        0    39080 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2429 2023-04-06 08:27:52.351949 jsonschema_gentypes-1.7.0/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     5956 2023-04-06 08:27:52.791948 jsonschema_gentypes-1.7.0/jsonschema_gentypes/jsonschema.py
--rw-r--r--   0        0        0        0 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     2842 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     5413 2023-04-06 08:25:03.108236 jsonschema_gentypes-1.7.0/jsonschema_gentypes/validate.py
--rw-r--r--   0        0        0     2500 2023-04-06 08:27:59.167936 jsonschema_gentypes-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 jsonschema_gentypes-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/LICENSE
+-rw-r--r--   0        0        0     3554 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/README.md
+-rw-r--r--   0        0        0    39080 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2429 2023-04-07 20:27:45.723875 jsonschema_gentypes-1.7.1/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     5956 2023-04-07 20:27:45.971897 jsonschema_gentypes-1.7.1/jsonschema_gentypes/jsonschema.py
+-rw-r--r--   0        0        0        0 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     2842 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     5413 2023-04-07 20:25:00.961019 jsonschema_gentypes-1.7.1/jsonschema_gentypes/validate.py
+-rw-r--r--   0        0        0     2500 2023-04-07 20:27:51.956477 jsonschema_gentypes-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5051 1970-01-01 00:00:00.000000 jsonschema_gentypes-1.7.1/PKG-INFO
```

### Comparing `jsonschema_gentypes-1.7.0/LICENSE` & `jsonschema_gentypes-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/README.md` & `jsonschema_gentypes-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Automatically generated file from a JSON schema.
 """
 
 
-from typing import Union, Dict, Literal, Any, List, TypedDict
+from typing import List, Any, TypedDict, Union, Dict, Literal
 from typing_extensions import Required
 
 
 AdditionalProperties = Union[Literal["Always"], Literal["Only explicit"]]
 """
 Additional properties.
```

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/jsonschema.py` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/jsonschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Automatically generated file from a JSON schema.
 """
 
 
-from typing import Union, Dict, Literal, Any, List, TypedDict
+from typing import List, Any, TypedDict, Union, Dict, Literal
 
 
 CORE_SCHEMA_META_SCHEMA_DEFAULT = True
 """Default value of the field path 'JSONSchema'"""
```

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/jsonschema_gentypes/validate.py` & `jsonschema_gentypes-1.7.1/jsonschema_gentypes/validate.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-1.7.0/pyproject.toml` & `jsonschema_gentypes-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "1.7.0"
+version = "1.7.1"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
```

### Comparing `jsonschema_gentypes-1.7.0/PKG-INFO` & `jsonschema_gentypes-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 1.7.0
+Version: 1.7.1
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
```

