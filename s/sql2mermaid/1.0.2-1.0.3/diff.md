# Comparing `tmp/sql2mermaid-1.0.2.tar.gz` & `tmp/sql2mermaid-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2mermaid-1.0.2.tar", max compression
+gzip compressed data, was "sql2mermaid-1.0.3.tar", max compression
```

## Comparing `sql2mermaid-1.0.2.tar` & `sql2mermaid-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1551 2023-04-07 18:19:05.247020 sql2mermaid-1.0.2/README.md
--rw-r--r--   0        0        0     1184 2023-04-07 18:16:17.629888 sql2mermaid-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       71 2023-04-07 18:16:23.447148 sql2mermaid-1.0.2/sql2mermaid/__init__.py
--rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.0.2/sql2mermaid/dependencies.py
--rw-r--r--   0        0        0     3256 2023-04-07 16:38:18.111127 sql2mermaid-1.0.2/sql2mermaid/main.py
--rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.0.2/sql2mermaid/tables.py
--rw-r--r--   0        0        0      313 2023-04-06 13:34:47.882454 sql2mermaid-1.0.2/sql2mermaid/utils.py
--rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 sql2mermaid-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1537 2023-04-07 18:27:39.373474 sql2mermaid-1.0.3/README.md
+-rw-r--r--   0        0        0     1184 2023-04-07 18:27:39.383777 sql2mermaid-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-04-07 18:27:39.384497 sql2mermaid-1.0.3/sql2mermaid/__init__.py
+-rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.0.3/sql2mermaid/dependencies.py
+-rw-r--r--   0        0        0     3256 2023-04-07 16:38:18.111127 sql2mermaid-1.0.3/sql2mermaid/main.py
+-rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.0.3/sql2mermaid/tables.py
+-rw-r--r--   0        0        0      313 2023-04-06 13:34:47.882454 sql2mermaid-1.0.3/sql2mermaid/utils.py
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 sql2mermaid-1.0.3/PKG-INFO
```

### Comparing `sql2mermaid-1.0.2/LICENSE.md` & `sql2mermaid-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.2/README.md` & `sql2mermaid-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/top-image.drawio.svg" width="1200px">
+<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/top-image.png" width="1200px">
 
 ---
 
 ![PyPI - License](https://img.shields.io/pypi/l/sql2mermaid)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nkato/sql2mermaid/python-tox.yml?event=push&label=pytest%20with%20py38)
 ![PyPI](https://img.shields.io/pypi/v/sql2mermaid)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sql2mermaid)
@@ -53,15 +53,15 @@
 
 You can get a diagram of the table dependencies by pasting this into [Mermaid Live Editor](https://mermaid.live/), [Diagrams.net (Draw.io)](https://www.draw.io/), etc.
 
 ## Options
 
 You can change the name of the root and whether the FROM, JOIN clause is displayed.
 
-<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.drawio.svg" width="1200px">
+<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.png" width="1200px">
 
 ## Author
 
 - [nkato](https://github.com/nkato)
 
 ## License
```

### Comparing `sql2mermaid-1.0.2/pyproject.toml` & `sql2mermaid-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql2mermaid"
-version = "1.0.2"
+version = "1.0.3"
 description = "Convert SQL table dependencies to mermaid.js"
 authors = ["nkato <naokato.aq@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/nkato/sql2mermaid"
 
 [tool.poetry.dependencies]
```

### Comparing `sql2mermaid-1.0.2/sql2mermaid/main.py` & `sql2mermaid-1.0.3/sql2mermaid/main.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.2/sql2mermaid/tables.py` & `sql2mermaid-1.0.3/sql2mermaid/tables.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.2/PKG-INFO` & `sql2mermaid-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql2mermaid
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert SQL table dependencies to mermaid.js
 Home-page: https://github.com/nkato/sql2mermaid
 License: MIT
 Author: nkato
 Author-email: naokato.aq@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlparse (>=0.4.3,<0.5.0)
 Project-URL: Repository, https://github.com/nkato/sql2mermaid
 Description-Content-Type: text/markdown
 
-<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/top-image.drawio.svg" width="1200px">
+<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/top-image.png" width="1200px">
 
 ---
 
 ![PyPI - License](https://img.shields.io/pypi/l/sql2mermaid)
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nkato/sql2mermaid/python-tox.yml?event=push&label=pytest%20with%20py38)
 ![PyPI](https://img.shields.io/pypi/v/sql2mermaid)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sql2mermaid)
@@ -71,15 +71,15 @@
 
 You can get a diagram of the table dependencies by pasting this into [Mermaid Live Editor](https://mermaid.live/), [Diagrams.net (Draw.io)](https://www.draw.io/), etc.
 
 ## Options
 
 You can change the name of the root and whether the FROM, JOIN clause is displayed.
 
-<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.drawio.svg" width="1200px">
+<img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.png" width="1200px">
 
 ## Author
 
 - [nkato](https://github.com/nkato)
 
 ## License
```

