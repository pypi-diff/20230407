# Comparing `tmp/sql2mermaid-1.0.0.tar.gz` & `tmp/sql2mermaid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2mermaid-1.0.0.tar", max compression
+gzip compressed data, was "sql2mermaid-1.0.1.tar", max compression
```

## Comparing `sql2mermaid-1.0.0.tar` & `sql2mermaid-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     1227 2023-04-07 16:38:43.568343 sql2mermaid-1.0.0/README.md
--rw-r--r--   0        0        0     1184 2023-04-07 17:22:55.081481 sql2mermaid-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-04-07 17:22:55.083252 sql2mermaid-1.0.0/sql2mermaid/__init__.py
--rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.0.0/sql2mermaid/dependencies.py
--rw-r--r--   0        0        0     3256 2023-04-07 16:38:18.111127 sql2mermaid-1.0.0/sql2mermaid/main.py
--rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.0.0/sql2mermaid/tables.py
--rw-r--r--   0        0        0      313 2023-04-06 13:34:47.882454 sql2mermaid-1.0.0/sql2mermaid/utils.py
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 sql2mermaid-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     1588 2023-04-07 17:57:22.719310 sql2mermaid-1.0.1/README.md
+-rw-r--r--   0        0        0     1184 2023-04-07 17:48:59.635650 sql2mermaid-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-04-07 17:49:09.143640 sql2mermaid-1.0.1/sql2mermaid/__init__.py
+-rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.0.1/sql2mermaid/dependencies.py
+-rw-r--r--   0        0        0     3256 2023-04-07 16:38:18.111127 sql2mermaid-1.0.1/sql2mermaid/main.py
+-rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.0.1/sql2mermaid/tables.py
+-rw-r--r--   0        0        0      313 2023-04-06 13:34:47.882454 sql2mermaid-1.0.1/sql2mermaid/utils.py
+-rw-r--r--   0        0        0     2235 1970-01-01 00:00:00.000000 sql2mermaid-1.0.1/PKG-INFO
```

### Comparing `sql2mermaid-1.0.0/LICENSE.md` & `sql2mermaid-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.0/pyproject.toml` & `sql2mermaid-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql2mermaid"
-version = "1.0.0"
+version = "1.0.1"
 description = "Convert SQL table dependencies to mermaid.js"
 authors = ["nkato <naokato.aq@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/nkato/sql2mermaid"
 
 [tool.poetry.dependencies]
```

### Comparing `sql2mermaid-1.0.0/sql2mermaid/main.py` & `sql2mermaid-1.0.1/sql2mermaid/main.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.0/sql2mermaid/tables.py` & `sql2mermaid-1.0.1/sql2mermaid/tables.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.0/PKG-INFO` & `sql2mermaid-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql2mermaid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert SQL table dependencies to mermaid.js
 Home-page: https://github.com/nkato/sql2mermaid
 License: MIT
 Author: nkato
 Author-email: naokato.aq@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,23 +16,32 @@
 Project-URL: Repository, https://github.com/nkato/sql2mermaid
 Description-Content-Type: text/markdown
 
 <img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/top-image.png" width="1200px">
 
 ---
 
-![tox badge](https://github.com/nkato/sql2mermaid/actions/workflows/python-tox.yml/badge.svg?event=push)
+![PyPI - License](https://img.shields.io/pypi/l/sql2mermaid)
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nkato/sql2mermaid/python-tox.yml?event=push&label=Tests%20with%20Python3.8)
+[![PyPI version](https://badge.fury.io/py/sql2mermaid.svg)](https://badge.fury.io/py/sql2mermaid)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sql2mermaid)
 
 # sql2mermaid
 
 Convert SQL table dependencies to the text of [mermaid.js](https://mermaid.js.org/) style!
 
+# Required
+
+Python >=3.8.1
+
 ## Installation
 
-WIP
+```shell
+pip install sql2mermaid
+```
 
 ## Getting Started
 
 ```python
 import sql2mermaid
 
 sql = """
```

