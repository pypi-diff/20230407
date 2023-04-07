# Comparing `tmp/mypy-boto3-docdb-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-docdb-1.26.109.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:20 2022, max compression
+gzip compressed data, was "mypy-boto3-docdb-1.26.109.tar", last modified: Fri Apr  7 19:33:57 2023, max compression
```

## Comparing `mypy-boto3-docdb-1.26.0.post1.tar` & `mypy-boto3-docdb-1.26.109.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.524823 mypy-boto3-docdb-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22621 2022-11-01 21:43:20.520823 mypy-boto3-docdb-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21188 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.520823 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    51111 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    51036 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9943 2022-11-01 21:33:03.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    17389 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    17374 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    60383 2022-11-01 21:33:04.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    60330 2022-11-01 21:33:03.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:20.520823 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22621 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-01 21:43:20.000000 mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:20.524823 mypy-boto3-docdb-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-11-01 21:33:02.000000 mypy-boto3-docdb-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:33:57.751627 mypy-boto3-docdb-1.26.109/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22647 2023-04-07 19:33:57.747627 mypy-boto3-docdb-1.26.109/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:33:57.747627 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51084 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60427 2023-04-07 19:31:59.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60374 2023-04-07 19:31:59.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 19:31:58.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:33:57.747627 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22647 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-07 19:33:57.000000 mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:33:57.751627 mypy-boto3-docdb-1.26.109/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-07 19:31:57.000000 mypy-boto3-docdb-1.26.109/setup.py
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/LICENSE` & `mypy-boto3-docdb-1.26.109/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/PKG-INFO` & `mypy-boto3-docdb-1.26.109/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DocDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.109
+Summary: Type annotations for boto3.DocDB 1.26.109 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.26.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -571,42 +572,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/README.md` & `mypy-boto3-docdb-1.26.109/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.26.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -540,42 +540,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__init__.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__init__.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/__main__.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDB 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.DocDB 1.26.109\nVersion:         1.26.109\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.109")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/client.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,15 +943,16 @@
         EngineVersion: str = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
+        DBClusterParameterGroupName: str = ...
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot or cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#restore_db_cluster_from_snapshot)
         """
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/client.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -886,15 +886,16 @@
         EngineVersion: str = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
+        DBClusterParameterGroupName: str = ...
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot or cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/client/#restore_db_cluster_from_snapshot)
         """
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/literals.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -108,27 +109,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -157,14 +162,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -209,51 +215,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -285,28 +297,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -315,14 +331,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -333,55 +350,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -422,21 +447,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/literals.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/literals.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -106,27 +107,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -155,14 +160,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -207,51 +213,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -283,28 +295,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -313,14 +329,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -331,55 +348,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -420,21 +445,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/paginator.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/paginator.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/type_defs.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1065,14 +1065,15 @@
         "Port": int,
         "DBSubnetGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
         "EnableCloudwatchLogsExports": Sequence[str],
         "DeletionProtection": bool,
+        "DBClusterParameterGroupName": str,
     },
     total=False,
 )
 
 
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/type_defs.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1032,14 +1032,15 @@
         "Port": int,
         "DBSubnetGroupName": str,
         "VpcSecurityGroupIds": Sequence[str],
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
         "EnableCloudwatchLogsExports": Sequence[str],
         "DeletionProtection": bool,
+        "DBClusterParameterGroupName": str,
     },
     total=False,
 )
 
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/waiter.py` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb/waiter.pyi` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/PKG-INFO` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.DocDB 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.109
+Summary: Type annotations for boto3.DocDB 1.26.109 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.26.109](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -571,42 +572,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-docdb-1.26.0.post1/mypy_boto3_docdb.egg-info/SOURCES.txt` & `mypy-boto3-docdb-1.26.109/mypy_boto3_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.26.0.post1/setup.py` & `mypy-boto3-docdb-1.26.109/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """
 Setup script for mypy-boto3-docdb.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb",
-    version="1.26.0.post1",
+    version="1.26.109",
     packages=["mypy_boto3_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDB 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.DocDB 1.26.109 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 docdb type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_docdb": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_docdb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

