# Comparing `tmp/robotcode_core-0.32.2.tar.gz` & `tmp/robotcode_core-0.32.3.tar.gz`

## Comparing `robotcode_core-0.32.2.tar` & `robotcode_core-0.32.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/async_cache.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/async_itertools.py
--rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0    15285 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/dataclasses.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/event.py
--rw-r--r--   0        0        0    15842 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/logging.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/py.typed
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/uri.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/pyproject.toml
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.32.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/async_cache.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/async_itertools.py
+-rw-r--r--   0        0        0    21484 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0    15277 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/dataclasses.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/event.py
+-rw-r--r--   0        0        0    15842 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/logging.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/README.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/pyproject.toml
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 robotcode_core-0.32.3/PKG-INFO
```

### Comparing `robotcode_core-0.32.2/src/robotcode/core/async_cache.py` & `robotcode_core-0.32.3/src/robotcode/core/async_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/async_itertools.py` & `robotcode_core-0.32.3/src/robotcode/core/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/async_tools.py` & `robotcode_core-0.32.3/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/dataclasses.py` & `robotcode_core-0.32.3/src/robotcode/core/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,23 +123,23 @@
 
 def __get_config(obj: Any, entry_protocol: Type[_T]) -> _T:
     if isinstance(obj, entry_protocol):
         return obj
     return cast(_T, __get_default_config())
 
 
-def __encode_case(obj: Any, field: dataclasses.Field) -> str:  # type: ignore
+def encode_case(obj: Any, field: dataclasses.Field) -> str:  # type: ignore
     alias = field.metadata.get("alias", None)
     if alias:
         return str(alias)
 
     return __get_config(obj, HasCaseEncoder)._encode_case(field.name)  # type: ignore
 
 
-def __decode_case(type: Type[_T], name: str) -> str:
+def decode_case(type: Type[_T], name: str) -> str:
     if dataclasses.is_dataclass(type):
         field = next(
             (f for f in dataclasses.fields(type) if f.metadata.get("alias", None) == name),
             None,
         )
         if field:
             return field.name
@@ -149,15 +149,15 @@
 
 def __default(o: Any) -> Any:
     if dataclasses.is_dataclass(o):
         return {
             name: value
             for name, value, field in (
                 (
-                    __encode_case(o, field),
+                    encode_case(o, field),
                     getattr(o, field.name),
                     field,
                 )
                 for field in dataclasses.fields(o)
                 if field.init or field.metadata.get("force_json", False)
             )
             if value is not None or field.default == dataclasses.MISSING
@@ -259,15 +259,15 @@
         for t in types:
             args = get_args(t)
             origin = get_origin(t)
 
             if origin is Literal:
                 continue
 
-            cased_value: Dict[str, Any] = {__decode_case(t, k): v for k, v in value.items()}
+            cased_value: Dict[str, Any] = {decode_case(t, k): v for k, v in value.items()}
             type_hints = get_type_hints(origin or t)
             try:
                 signature = inspect.signature(origin or t)
             except ValueError:
                 continue
 
             non_default_parameters = {
```

### Comparing `robotcode_core-0.32.2/src/robotcode/core/event.py` & `robotcode_core-0.32.3/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/logging.py` & `robotcode_core-0.32.3/src/robotcode/core/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/uri.py` & `robotcode_core-0.32.3/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/net.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/src/robotcode/core/utils/version.py` & `robotcode_core-0.32.3/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/.gitignore` & `robotcode_core-0.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/LICENSE.txt` & `robotcode_core-0.32.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/README.md` & `robotcode_core-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/pyproject.toml` & `robotcode_core-0.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.32.2/PKG-INFO` & `robotcode_core-0.32.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-core
-Version: 0.32.2
+Version: 0.32.3
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

