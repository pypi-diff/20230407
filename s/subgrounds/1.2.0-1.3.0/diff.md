# Comparing `tmp/subgrounds-1.2.0.tar.gz` & `tmp/subgrounds-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgrounds-1.2.0.tar", max compression
+gzip compressed data, was "subgrounds-1.3.0.tar", max compression
```

## Comparing `subgrounds-1.2.0.tar` & `subgrounds-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11347 2023-04-02 20:33:21.994934 subgrounds-1.2.0/LICENSE
--rw-r--r--   0        0        0     8929 2023-04-02 20:33:21.994934 subgrounds-1.2.0/README.md
--rw-r--r--   0        0        0     1601 2023-04-02 20:34:54.184375 subgrounds-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      224 2023-04-02 20:34:54.168375 subgrounds-1.2.0/subgrounds/__init__.py
--rw-r--r--   0        0        0     3524 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/client.py
--rw-r--r--   0        0        0     4260 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/dash_wrappers.py
--rw-r--r--   0        0        0    10062 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/dataframe_utils.py
--rw-r--r--   0        0        0     1027 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/pagination/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/pagination/pagination.py
--rw-r--r--   0        0        0    10550 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/pagination/preprocess.py
--rw-r--r--   0        0        0    17076 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/pagination/strategies.py
--rw-r--r--   0        0        0     1530 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/pagination/utils.py
--rw-r--r--   0        0        0     6789 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/plotly_wrappers.py
--rw-r--r--   0        0        0    62329 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/query.py
--rw-r--r--   0        0        0    12720 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/schema.py
--rw-r--r--   0        0        0      308 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgraph/__init__.py
--rw-r--r--   0        0        0    38895 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgraph/fieldpath.py
--rw-r--r--   0        0        0     1669 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgraph/filter.py
--rw-r--r--   0        0        0     4754 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgraph/object.py
--rw-r--r--   0        0        0     2552 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgraph/subgraph.py
--rw-r--r--   0        0        0    21569 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/subgrounds.py
--rw-r--r--   0        0        0    19756 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/transform.py
--rw-r--r--   0        0        0     6901 2023-04-02 20:33:21.998935 subgrounds-1.2.0/subgrounds/utils.py
--rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 subgrounds-1.2.0/setup.py
--rw-r--r--   0        0        0     9799 1970-01-01 00:00:00.000000 subgrounds-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-04-07 18:51:29.779610 subgrounds-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8929 2023-04-07 18:51:29.779610 subgrounds-1.3.0/README.md
+-rw-r--r--   0        0        0     1601 2023-04-07 18:51:52.139923 subgrounds-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-04-07 18:51:52.123922 subgrounds-1.3.0/subgrounds/__init__.py
+-rw-r--r--   0        0        0     4521 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/client.py
+-rw-r--r--   0        0        0     4260 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/dash_wrappers.py
+-rw-r--r--   0        0        0    10062 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/dataframe_utils.py
+-rw-r--r--   0        0        0      395 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/errors.py
+-rw-r--r--   0        0        0     1027 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/pagination.py
+-rw-r--r--   0        0        0    10550 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/preprocess.py
+-rw-r--r--   0        0        0    17076 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/strategies.py
+-rw-r--r--   0        0        0     1530 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/utils.py
+-rw-r--r--   0        0        0     6789 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/plotly_wrappers.py
+-rw-r--r--   0        0        0    62357 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/query.py
+-rw-r--r--   0        0        0    12755 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/schema.py
+-rw-r--r--   0        0        0      308 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/__init__.py
+-rw-r--r--   0        0        0    38895 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/fieldpath.py
+-rw-r--r--   0        0        0     1669 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/filter.py
+-rw-r--r--   0        0        0     4754 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/object.py
+-rw-r--r--   0        0        0     2552 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/subgraph.py
+-rw-r--r--   0        0        0    21569 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgrounds.py
+-rw-r--r--   0        0        0    20072 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/transform.py
+-rw-r--r--   0        0        0     6901 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/utils.py
+-rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 subgrounds-1.3.0/setup.py
+-rw-r--r--   0        0        0     9799 1970-01-01 00:00:00.000000 subgrounds-1.3.0/PKG-INFO
```

### Comparing `subgrounds-1.2.0/LICENSE` & `subgrounds-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/README.md` & `subgrounds-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/pyproject.toml` & `subgrounds-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subgrounds"
-version = "1.2.0"
+version = "1.3.0"
 description = "A Pythonic data access layer for applications querying data from The Graph Network."
 authors = [
     "cvauclair <cvauclair@playgrounds.network>",
     "0xMochan <mochan@playgrounds.network>",
 ]
 repository = "https://github.com/0xPlaygrounds/subgrounds"
```

### Comparing `subgrounds-1.2.0/subgrounds/client.py` & `subgrounds-1.3.0/subgrounds/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 
 import logging
 from typing import Any
 
 import requests
 
-from subgrounds.utils import default_header
+from .errors import GraphQLError, ServerError
+from .utils import default_header
 
 logger = logging.getLogger("subgrounds")
 
 
 INTROSPECTION_QUERY: str = """
   query IntrospectionQuery {
     __schema {
@@ -108,29 +109,44 @@
     :attr:`url` and returns the result. In case of errors, an exception containing
     the error message is thrown.
 
     Args:
       url (str): The url of the GraphQL API
 
     Raises:
-      Exception: In case of GraphQL server error
+      HttpError: If the request response resulted in an error
+      ServerError: If server responds back non-json content
+      GraphQLError: If the GraphQL query failed or other grapql server errors
 
     Returns:
       dict[str, Any]: The GraphQL API's schema in JSON
     """
+
     resp = requests.post(
         url,
         json={"query": INTROSPECTION_QUERY},
         headers=default_header() | headers,
-    ).json()
+    )
+
+    resp.raise_for_status()
 
     try:
-        return resp["data"]
-    except KeyError as exn:
-        raise Exception(resp["errors"]) from exn
+        raw_data = resp.json()
+
+    except requests.JSONDecodeError:
+        raise ServerError(
+            f"Server ({url}) did not respond with proper JSON"
+            f"\nDid you query a proper GraphQL endpoint?"
+            f"\n\n{resp.content}"
+        )
+
+    if (data := raw_data.get("data")) is None:
+        raise GraphQLError(raw_data.get("errors", "Unknown Error(s) Found"))
+
+    return data
 
 
 def query(
     url: str,
     query_str: str,
     variables: dict[str, Any] = {},
     headers: dict[str, Any] = {},
@@ -143,28 +159,42 @@
     Args:
       url (str): The URL of the GraphQL API
       query_str (str): The GraphQL query string
       variables (dict[str, Any], optional): Variables for the GraphQL query.
         Defaults to {}.
 
     Raises:
-      Exception: GraphQL error
+      HttpError: If the request response resulted in an error
+      ServerError: If server responds back non-json content
+      GraphQLError: If the GraphQL query failed or other grapql server errors
 
     Returns:
       dict[str, Any]: Response data
     """
 
     logger.info(f"client.query: url = {url}, variables = {variables}\n{query_str}")
     resp = requests.post(
         url,
         json=(
             {"query": query_str}
             if variables == {}
             else {"query": query_str, "variables": variables}
         ),
         headers=default_header() | headers,
-    ).json()
+    )
+
+    resp.raise_for_status()
 
     try:
-        return resp["data"]
-    except KeyError as exn:
-        raise Exception(resp["errors"]) from exn
+        raw_data = resp.json()
+
+    except requests.JSONDecodeError:
+        raise ServerError(
+            f"Server ({url}) did not respond with proper JSON"
+            f"\nDid you query a proper GraphQL endpoint?"
+            f"\n\n{resp.content}"
+        )
+
+    if (data := raw_data.get("data")) is None:
+        raise GraphQLError(raw_data.get("errors", "Unknown Error(s) Found"))
+
+    return data
```

### Comparing `subgrounds-1.2.0/subgrounds/dash_wrappers.py` & `subgrounds-1.3.0/subgrounds/dash_wrappers.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/dataframe_utils.py` & `subgrounds-1.3.0/subgrounds/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/pagination/__init__.py` & `subgrounds-1.3.0/subgrounds/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/pagination/pagination.py` & `subgrounds-1.3.0/subgrounds/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/pagination/preprocess.py` & `subgrounds-1.3.0/subgrounds/pagination/preprocess.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/pagination/strategies.py` & `subgrounds-1.3.0/subgrounds/pagination/strategies.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/pagination/utils.py` & `subgrounds-1.3.0/subgrounds/pagination/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/plotly_wrappers.py` & `subgrounds-1.3.0/subgrounds/plotly_wrappers.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/query.py` & `subgrounds-1.3.0/subgrounds/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 import warnings
 from dataclasses import dataclass, field
 from functools import partial, reduce
 from typing import Any, Callable, Iterator, Literal, Optional, Protocol, TypeVar
 
 from pipe import map, take, traverse, where
 
-from subgrounds.schema import SchemaMeta, TypeMeta, TypeRef
-from subgrounds.utils import (
+from .errors import SubgroundsError
+from .schema import SchemaMeta, TypeMeta, TypeRef
+from .utils import (
     extract_data,
     filter_map,
     filter_none,
     identity,
     rel_complement,
     union,
 )
@@ -545,15 +546,15 @@
                         | map(partial(Selection.map, map_f=map_f, priority=priority))
                     ),
                 )
 
                 return map_f(new_selection)
 
             case _:
-                raise Exception(f"map: invalid priority {priority}")
+                raise SubgroundsError(f"map: invalid priority {priority}")
 
     def map_args(
         self,
         map_f: Callable[[Argument], Argument | list[Argument]],
         recurse: bool = True,
     ) -> Selection:
         """Replaces each ``Argument`` ``arg`` in the current ``Selection`` with ``map_f(arg)``
@@ -866,15 +867,15 @@
         return (
             list(self.selection | map(Selection.infer_variable_definitions) | traverse)
             + var_defs
         )
 
     def combine(self: Selection, other: Selection) -> Selection:
         if self.key != other.key:
-            raise Exception(f"Selection.combine: {self.key} != {other.key}")
+            raise SubgroundsError(f"Selection.combine: {self.key} != {other.key}")
 
         return Selection(
             fmeta=self.fmeta,
             alias=self.alias,
             arguments=self.arguments,
             selection=filter_none(
                 union(
```

### Comparing `subgrounds-1.2.0/subgrounds/schema.py` & `subgrounds-1.3.0/subgrounds/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import warnings
 from typing import Annotated, Literal
 
 from pipe import map, where
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Field, root_validator
 
+from .errors import SchemaError
+
 warnings.simplefilter("default")
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
         allow_population_by_field_name = True
 
@@ -157,15 +159,15 @@
             try:
                 return next(
                     self.arguments
                     | where(lambda argmeta: argmeta.name == argname)
                     | map(lambda arg: arg.type_)
                 )
             except StopIteration:
-                raise Exception(
+                raise SchemaError(
                     f"TypeMeta.FieldMeta.type_of_arg: no argument named {argname} for field {self.name}"
                 )
 
     class ScalarMeta(T):
         kind: Literal["SCALAR"] = "SCALAR"
         """ Class representing an scalar definition."""
```

### Comparing `subgrounds-1.2.0/subgrounds/subgraph/fieldpath.py` & `subgrounds-1.3.0/subgrounds/subgraph/fieldpath.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/subgraph/filter.py` & `subgrounds-1.3.0/subgrounds/subgraph/filter.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/subgraph/object.py` & `subgrounds-1.3.0/subgrounds/subgraph/object.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/subgraph/subgraph.py` & `subgrounds-1.3.0/subgrounds/subgraph/subgraph.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/subgrounds.py` & `subgrounds-1.3.0/subgrounds/subgrounds.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/subgrounds/transform.py` & `subgrounds-1.3.0/subgrounds/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 import logging
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable
 
 from pipe import map, traverse
 
-from subgrounds.query import DataRequest, Document, Query, Selection
-from subgrounds.schema import TypeMeta, TypeRef
-from subgrounds.utils import flatten, union
+from .errors import TransformError
+from .query import DataRequest, Document, Query, Selection
+from .schema import TypeMeta, TypeRef
+from .utils import flatten, union
 
 if TYPE_CHECKING:
-    from subgrounds.subgraph import Subgraph
+    from .subgraph import Subgraph
 
 logger = logging.getLogger("subgrounds")
 
 
 def select_data(select: Selection, data: dict) -> list[Any]:
     match (select, data):
         case (
@@ -51,15 +52,17 @@
             dict() as data,
         ) if name in data:
             return list(
                 inner_select | map(partial(select_data, data=data[name])) | traverse
             )
 
         case (select, data):
-            raise Exception(f"select_data: invalid selection {select} for data {data}")
+            raise TransformError(
+                f"select_data: invalid selection {select} for data {data}"
+            )
 
     assert False  # Suppress mypy missing return statement warning
 
 
 class RequestTransform(ABC):
     """Abstract class representing a transformation layer to be applied to entire
     :class:`DataRequest` objects.
@@ -159,15 +162,16 @@
         super().__init__()
 
     def transform_document(self: TypeTransform, doc: Document) -> Document:
         return doc
 
     def transform_response(self, doc: Document, data: dict[str, Any]) -> dict[str, Any]:
         def transform(select: Selection, data: dict[str, Any]) -> None:
-            # TODO: Handle NonNull and List more graciously (i.e.: without using TypeRef.root_type_name)
+            # TODO: Handle NonNull and List more graciously
+            #  (i.e.: without using TypeRef.root_type_name)
             match (select, data):
                 # Type matches
                 case (
                     Selection(
                         TypeMeta.FieldMeta(name=name, type_=ftype), None, _, [] | None
                     )
                     | Selection(
@@ -207,21 +211,23 @@
                                     transform(select, elt)
                         case dict() as elt:
                             for select in inner_select:
                                 transform(select, elt)
                         case None:
                             return None
                         case _:
-                            raise Exception(
-                                f"transform_data_type: data for selection {select} is neither list or dict {data[name]}"
+                            raise TransformError(
+                                f"transform_data_type: data for selection {select} is"
+                                f" neither list or dict {data[name]}"
                             )
 
                 case (select, data):
-                    raise Exception(
-                        f"transform_data_type: invalid selection {select} for data {data}"
+                    raise TransformError(
+                        f"transform_data_type: invalid selection {select}"
+                        f" for data {data}"
                     )
 
         for select in doc.query.selection:
             transform(select, data)
 
         return data
 
@@ -288,15 +294,17 @@
                     alias,
                     args,
                     inner_select,
                 ):
                     new_inner_select = list(inner_select | map(transform) | traverse)
                     return Selection(select_fmeta, alias, args, new_inner_select)
                 case _:
-                    raise Exception(f"transform_document: unhandled selection {select}")
+                    raise TransformError(
+                        f"transform_document: unhandled selection {select}"
+                    )
 
             assert False  # Suppress mypy missing return statement warning
 
         def transform_on_type(select: Selection) -> Selection:
             match select:
                 case Selection(
                     TypeMeta.FieldMeta(type_=type_) as select_fmeta,
@@ -330,42 +338,45 @@
         def transform(select: Selection, data: dict) -> None:
             match (select, data):
                 case (
                     Selection(TypeMeta.FieldMeta(name=name), None, _, [] | None)
                     | Selection(TypeMeta.FieldMeta(), name, _, [] | None),
                     dict() as data,
                 ) if name == self.fmeta.name and name not in data:
-                    # Case where the selection selects a the syntheticfield of the curren transform
-                    # that is not in the data blob and there are no inner selections
+                    # Case where the selection selects a the syntheticfield of the
+                    #  current transform that is not in the data blob and there are
+                    #  no inner selections
 
-                    # Try to grab the arguments to the synthetic field transform in the data blob
+                    # Try to grab the arguments to the synthetic field transform in
+                    #  the data blob
                     arg_values = flatten(
                         list(self.args | map(partial(select_data, data=data)))
                     )
 
                     try:
                         data[name] = self.f(*arg_values)
                     except Exception:
                         data[name] = self.default
 
                 case (
                     Selection(TypeMeta.FieldMeta(name=name), None, _, [] | None)
                     | Selection(TypeMeta.FieldMeta(), name, _, [] | None),
                     dict() as data,
                 ) if name not in data:
-                    # Case where the selection selects a regular field but it is not in the data blob (caused by None value at higher selection)
+                    # Case where the selection selects a regular field but it is not in
+                    #  the data blob (caused by None value at higher selection)
                     data[name] = None
 
                 case (
                     Selection(TypeMeta.FieldMeta(name=name), None, _, [] | None)
                     | Selection(TypeMeta.FieldMeta(), name, _, [] | None),
                     dict() as data,
                 ):
-                    # Case where the selection selects a regular field and there are no inner selections
-                    # (nothing to do)
+                    # Case where the selection selects a regular field and there are
+                    #  no inner selections (nothing to do)
                     pass
 
                 case (
                     Selection(TypeMeta.FieldMeta(name=name), None, _, inner_select)
                     | Selection(TypeMeta.FieldMeta(), name, _, inner_select),
                     dict() as data,
                 ) if name in data:
@@ -381,21 +392,23 @@
 
                         case None:
                             data[name] = {}
                             for select in inner_select:
                                 transform(select, data[name])
 
                         case _:
-                            raise Exception(
-                                f"transform_response: data for selection {select} is neither list or dict {data[name]}"
+                            raise TransformError(
+                                f"transform_response: data for selection {select} is"
+                                f" neither list or dict {data[name]}"
                             )
 
                 case (select, data):
-                    raise Exception(
-                        f"transform_response: invalid selection {select} for data {data}"
+                    raise TransformError(
+                        f"transform_response: invalid selection {select}"
+                        f" for data {data}"
                     )
 
         def transform_on_type(select: Selection, data: dict) -> None:
             match select:
                 case Selection(TypeMeta.FieldMeta(type_=type_), None, _, _) | Selection(
                     TypeMeta.FieldMeta(type_=type_), _, _, _
                 ) if type_.name == self.type_.name:
```

### Comparing `subgrounds-1.2.0/subgrounds/utils.py` & `subgrounds-1.3.0/subgrounds/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.2.0/setup.py` & `subgrounds-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'requests>=2.27.1,<3.0.0']
 
 extras_require = \
 {'dash': ['dash>=2.3.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'subgrounds',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'A Pythonic data access layer for applications querying data from The Graph Network.',
     'long_description': "# Subgrounds\n<!-- [![GitHub Actions](https://github.com/0xPlaygrounds/subgrounds/workflows/CI/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions) -->\n[![PyPI](https://img.shields.io/pypi/v/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n<br>\n\n[![Discord](https://img.shields.io/discord/896944341598208070?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/gMSSh5bjvk)\n[![Twitter Follow](https://img.shields.io/twitter/follow/Playgrounds0x?color=%231fa1f2&label=Playgrounds%20Analytics&logo=Twitter&logoColor=1fa1f2&style=flat-square)](https://twitter.com/Playgrounds0x)\n\n\n<!-- start elevator-pitch -->\nAn intuitive python library for interfacing with Subgraphs.\n\n## Features\n- **Simple**: Leverage a Pythonic API to easily build queries and transformations without the need for raw GraphQL manipulation.\n- **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.\n- **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.\n\n<!-- end elevator-pitch -->\n\n## Resources\n- [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation\n- [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly\n- [**Community projects**](http://docs.playgrounds.network//examples/): An ever growing list of projects created by our community members\n- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO \n\n## Installation\n> Subgrounds **requires** atleast Python 3.10+\n\nSubgrounds is available on PyPi. To install it, run the following:<br>\n`pip install subgrounds`.\n\nSubgrounds also comes bundled with some handy `dash` wrappers. To use those wrappers, you can install the extra `dash` dependencies.<br>\n`pip install subgrounds[dash]`.\n\n## Simple example\n<!-- start simple-example -->\n```python\n>>> from subgrounds import Subgrounds\n\n>>> sg = Subgrounds()\n\n>>> # Load\n>>> aave_v2 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/messari/aave-v2-ethereum')\n\n>>> # Construct the query\n>>> latest = aave_v2.Query.markets(\n  orderBy=aave_v2.Market.totalValueLockedUSD,\n  orderDirection='desc',\n  first=5,\n)\n\n>>> # Return query to a dataframe\n>>> sg.query_df([\n  latest.name,\n  latest.totalValueLockedUSD,\n])\n                  markets_name  markets_totalValueLockedUSD\n0  Aave interest bearing STETH                 1.522178e+09\n1   Aave interest bearing WETH                 1.221299e+09\n2   Aave interest bearing USDC                 8.140547e+08\n3   Aave interest bearing WBTC                 6.615692e+08\n4   Aave interest bearing USDT                 3.734017e+08\n```\n<!-- end simple-example -->\n\n\n## About Us\nPlaygrounds Analytics is a data solutions company providing serverless on-chain data infrastructures and services for data teams, analysts, and engineers. Checkout us out [here](https://playgrounds.network/) to learn more!\n\n\n\n\n<!-- TODO: Move this to github pages docs -->\n<!-- # Dash and Plotly wrappers\nSubgrounds provides wrappers for Plotly objects and Dash components to facilitate visualization of data from The Graph.\n\nPlotly wrappers can be found in the `subgrounds.plotly_wrappers` submodule. The wrappers include a `Figure` wrapper as well as wrappers for most Plotly traces (see https://plotly.com/python/reference/). All Plotly trace wrappers accept the same arguments as their underlying Plotly trace with the notable difference being that Subgrounds `FieldPath` objects can be used as arguments wherever one would usually provide data to the traces.\n\n```python\nfrom subgrounds.plotly_wrappers import Bar, Figure\nfrom subgrounds.dash_wrappers import Graph\n\nborrows = aave_v2.Query.borrows(\n  orderBy=aave_v2.Borrow.timestamp,\n  orderDirection='desc',\n  first=100\n)\n\nrepays = aave_v2.Query.repays(\n  orderBy=aave_v2.Repay.timestamp,\n  orderDirection='desc',\n  first=100\n)\n\n# Dashboard\napp = dash.Dash(__name__)\n\napp.layout = html.Div(\n  html.Div([\n    html.H4('Entities'),\n    html.Div([\n      # Subgrounds Graph Dash component\n      Graph(\n        # A Subgrounds Plotly figure \n        Figure(\n          subgrounds=sg,\n          traces=[\n            # Subgrounds Plotly traces\n            Bar(x=borrows.reserve.symbol, y=borrows.amount),\n            Bar(x=repays.reserve.symbol, y=repays.amount)\n          ]\n        )\n      )\n    ])\n  ])\n)\n``` -->\n\n<!-- Generates the following Dash dashboard (at time of writing):\n![Alt text](https://raw.githubusercontent.com/Protean-Labs/subgrounds/main/img/bar-chart-example.png) -->\n\n<!-- # Examples and resources\nSee the `examples/` directory for an evergrowing list of examples. -->\n\n\n## Acknowledgments\nThis software project would not be possible without the support of The Graph Foundation. You can learn more about The Graph and its mission [here](https://thegraph.com/).\n\n<!-- TODO: Move this to github pages docs -->\n<!-- # Notes\n## Non-subgraph GraphQL APIs\nAlthough Subgrounds has been developed with subgraph APIs in mind, most features will also work with any GraphQL API. However, Subgrounds has not been tested with non-subgraph GraphQL APIs and some features will definitely break if the non-subgraph APIs do not follow the same conventions as subgraph APIs (e.g.: automatic pagination relies on each entity having a unique `id` field).\n\nIt is nonetheless possible to use Subgrounds with non-subgraph GraphQL APIs by using `load_api` instead of `load_subgraph`. This will bypass Subgrounds automatic pagination feature and pagination will therefore have to be done manually. Below is an example of using Subgrounds with the snapshot GraphQL API.\n```python\n>>> from datetime import datetime\n\n>>> from subgrounds.subgrounds import Subgrounds\n>>> from subgrounds.subgraph import SyntheticField\n\n>>> sg = Subgrounds()\n>>> snapshot = sg.load_api('https://hub.snapshot.org/graphql')\n\n>>> snapshot.Proposal.datetime = SyntheticField(\n...   lambda timestamp: str(datetime.fromtimestamp(timestamp)),\n...   SyntheticField.STRING,\n...   snapshot.Proposal.end,\n... )\n\n>>> proposals = snapshot.Query.proposals(\n...   orderBy='created',\n...   orderDirection='desc',\n...   first=100,\n...   where=[\n...     snapshot.Proposal.space == 'olympusdao.eth',\n...     snapshot.Proposal.state == 'closed'\n...   ]\n... )\n\n>>> sg.query_df([\n...   proposals.datetime,\n...   proposals.title,\n...   proposals.votes,\n... ])\n     proposals_datetime                                    proposals_title  proposals_votes\n0   2022-03-25 15:33:00  OIP-87: BeraChain Investment + Strategic Partn...              184\n1   2022-03-25 12:00:00                 OIP-86: Uniswap Migration Proposal              146\n2   2022-03-25 13:12:00                    TAP 8 - Yearn Finance Whitelist              137\n3   2022-03-22 15:10:10                      OIP-85: Emissions Adjustments              167\n4   2022-03-13 20:17:26                  TAP 7 - Anchor Protocol Whitelist              141\n..                  ...                                                ...              ...\n95  2021-11-20 23:00:00                 OlympusDAO Add ETH to the Treasury               52\n96  2022-01-31 12:00:00                            Add BTC to the Treasury              232\n97  2021-11-29 23:00:00   OlympusDAO OlympusDAO Launch OHM on POLYGON c...              234\n98  2021-11-29 23:00:00                 OlympusDAO Launch OHM on BSC chain               92\n99  2021-11-20 23:00:00  Suggestions to add more video operation guidan...               53\n\n[100 rows x 3 columns]\n```\n\n## GraphQL Aliases\nThe use of the alias `xf608864358427cfb` in the query string is to prevent conflict when merging fieldpaths that select the same fields with different arguments. For example, in the following code, the `borrows` query field is selected twice with different arguments:\n```python\n>>> latest_borrows = aave_v2.Query.borrows(\n...  orderBy=aave_v2.Borrow.timestamp,\n...  orderDirection='desc',\n...  first=100\n...)\n\n>>> largest_borrows = aave_v2.Query.borrows(\n...  orderBy=aave_v2.Borrow.amount,\n...  orderDirection='desc',\n...  first=100\n...)\n\n>>> req = sg.mk_request([\n...   latest_borrows.reserve.symbol,\n...   latest_borrows.amount,\n...   largest_borrows.reserve.symbol,\n...   largest_borrows.amount,\n... ])\n>>> print(req.graphql)\nquery {\n  x8b3edf3dc6501837: borrows(first: 100, orderBy: amount, orderDirection: desc) {\n    reserve {\n      symbol\n    }\n    amount\n  }\n  xf608864358427cfb: borrows(first: 100, orderBy: timestamp, orderDirection: desc) {\n    reserve {\n      symbol\n    }\n    amount\n  }\n}\n``` -->\n",
     'author': 'cvauclair',
     'author_email': 'cvauclair@playgrounds.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xPlaygrounds/subgrounds',
```

### Comparing `subgrounds-1.2.0/PKG-INFO` & `subgrounds-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subgrounds
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Pythonic data access layer for applications querying data from The Graph Network.
 Home-page: https://github.com/0xPlaygrounds/subgrounds
 Keywords: graph,subgrounds,graphql,subgraph
 Author: cvauclair
 Author-email: cvauclair@playgrounds.network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

