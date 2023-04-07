# Comparing `tmp/render50-9.1.0.tar.gz` & `tmp/render50-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render50-9.1.0.tar", last modified: Thu Jan 26 03:38:13 2023, max compression
+gzip compressed data, was "render50-9.1.1.tar", last modified: Fri Apr  7 21:32:34 2023, max compression
```

## Comparing `render50-9.1.0.tar` & `render50-9.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 03:38:13.542574 render50-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-26 03:37:52.000000 render50-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-26 03:38:13.542574 render50-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-26 03:37:52.000000 render50-9.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    20289 2023-01-26 03:37:52.000000 render50-9.1.0/render50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 03:38:13.542574 render50-9.1.0/render50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-26 03:38:13.000000 render50-9.1.0/render50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-26 03:38:13.000000 render50-9.1.0/render50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 03:38:13.000000 render50-9.1.0/render50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-26 03:38:13.000000 render50-9.1.0/render50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 03:38:13.000000 render50-9.1.0/render50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 03:38:13.542574 render50-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-26 03:37:52.000000 render50-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:32:34.235087 render50-9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-07 21:32:13.000000 render50-9.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 21:32:34.235087 render50-9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 21:32:13.000000 render50-9.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20439 2023-04-07 21:32:13.000000 render50-9.1.1/render50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:32:34.235087 render50-9.1.1/render50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:32:34.000000 render50-9.1.1/render50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:32:34.235087 render50-9.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-07 21:32:13.000000 render50-9.1.1/setup.py
```

### Comparing `render50-9.1.0/LICENSE` & `render50-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `render50-9.1.0/render50` & `render50-9.1.1/render50`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 
 from signal import SIGINT, signal
 signal(SIGINT, lambda signum, frame: sys.exit(1))
 
 import io
 import os
+import pygments.lexers.sql
 import re
-import sys
 import requests
+import sys
 import termcolor
 
 from argparse import ArgumentParser
 from backports.shutil_get_terminal_size import get_terminal_size
 from braceexpand import braceexpand
 from bs4 import BeautifulSoup
 from copy import copy
@@ -40,14 +41,18 @@
 try:
     d = get_distribution("render50")
 except DistributionNotFound:
     __version__ = "UNKNOWN"
 else:
     __version__ = d.version
 
+# Prioritize these languages
+# https://github.com/pygments/pygments/issues/2405
+pygments.lexers.sql.SqlLexer.priority = 1
+
 
 def main():
 
     # Exit on ctrl-c
     def handler(signum, frame):
         cprint("")
         cancel(1)
```

### Comparing `render50-9.1.0/setup.py` & `render50-9.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     keywords=["render", "render50"],
     license="GPLv3",
     long_description_content_type="text/markdown",
     name="render50",
     python_requires=">=3.6",
     scripts=["render50"],
     url="https://github.com/cs50/render50",
-    version="9.1.0"
+    version="9.1.1"
 )
```

