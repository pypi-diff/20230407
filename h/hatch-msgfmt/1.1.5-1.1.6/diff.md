# Comparing `tmp/hatch-msgfmt-1.1.5.tar.gz` & `tmp/hatch-msgfmt-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch-msgfmt-1.1.5.tar", last modified: Thu Jan 26 22:41:24 2023, max compression
+gzip compressed data, was "hatch-msgfmt-1.1.6.tar", last modified: Fri Apr  7 20:57:22 2023, max compression
```

## Comparing `hatch-msgfmt-1.1.5.tar` & `hatch-msgfmt-1.1.6.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1078 2023-01-26 18:21:33.772191 hatch-msgfmt-1.1.5/README.md
--rw-r--r--   0        0        0      760 2023-01-26 22:41:15.735307 hatch-msgfmt-1.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-04 23:21:38.651403 hatch-msgfmt-1.1.5/src/hatch_msgfmt/__init__.py
--rw-r--r--   0        0        0      145 2023-01-05 19:01:47.788051 hatch-msgfmt-1.1.5/src/hatch_msgfmt/hooks.py
--rw-r--r--   0        0        0     1039 2023-01-26 22:40:39.810263 hatch-msgfmt-1.1.5/src/hatch_msgfmt/plugin.py
--rw-r--r--   0        0        0        0 2023-01-05 00:11:10.150540 hatch-msgfmt-1.1.5/src/hatch_msgfmt/py.typed
--rw-r--r--   0        0        0     1355 2023-01-11 16:56:45.972027 hatch-msgfmt-1.1.5/src/hatch_msgfmt/tempfile.py
--rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 hatch-msgfmt-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-01-04 23:04:59.095348 hatch-msgfmt-1.1.6/.gitignore
+-rw-r--r--   0        0        0     1077 2023-01-04 23:04:59.095348 hatch-msgfmt-1.1.6/LICENSE
+-rw-r--r--   0        0        0     1444 2023-04-07 20:54:30.856696 hatch-msgfmt-1.1.6/README.md
+-rw-r--r--   0        0        0      760 2023-04-07 20:54:30.856696 hatch-msgfmt-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-04 23:21:38.651403 hatch-msgfmt-1.1.6/src/hatch_msgfmt/__init__.py
+-rw-r--r--   0        0        0      145 2023-01-05 19:01:47.788051 hatch-msgfmt-1.1.6/src/hatch_msgfmt/hooks.py
+-rw-r--r--   0        0        0     1553 2023-04-07 20:54:30.856696 hatch-msgfmt-1.1.6/src/hatch_msgfmt/plugin.py
+-rw-r--r--   0        0        0        0 2023-01-05 00:11:10.150540 hatch-msgfmt-1.1.6/src/hatch_msgfmt/py.typed
+-rw-r--r--   0        0        0     1355 2023-01-11 16:56:45.972027 hatch-msgfmt-1.1.6/src/hatch_msgfmt/tempfile.py
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 hatch-msgfmt-1.1.6/PKG-INFO
```

### Comparing `hatch-msgfmt-1.1.5/pyproject.toml` & `hatch-msgfmt-1.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'hatch-msgfmt'
-version = '1.1.5'
+version = '1.1.6'
 description = 'Msgfmt build hook, replacing all po with mo in build'
 license = {text = 'MIT'}
 readme = 'README.md'
 requires-python= '>=3.7'
 dependencies = [
   'hatchling',
 ]
```

### Comparing `hatch-msgfmt-1.1.5/src/hatch_msgfmt/tempfile.py` & `hatch-msgfmt-1.1.6/src/hatch_msgfmt/tempfile.py`

 * *Files identical despite different names*

### Comparing `hatch-msgfmt-1.1.5/PKG-INFO` & `hatch-msgfmt-1.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-msgfmt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Msgfmt build hook, replacing all po with mo in build
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Maintainer-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -21,19 +21,30 @@
 point for this, but it's not as capable as GNU Gettext, and doesn't support
 plural forms.  Even with a fresh implementation, handling the file encoding
 from the header is challenging, especially for variable-length encodings like
 EUC-JP, which could feasibly cause particular problems.
 
 Better to just use the system one for now.  If somebody wants to submit a pure-
 python implementation that functions, I'll gladly integrate it as a separate
-msgfmtpy plugin in the same repository.
+`msgfmtpy` plugin in the same repository.
 
-Depends on the `locales` and `destinations` plugin config parameters,
-specifying where the source locale files and destination compiled locale files
-should be found.
+# Config parameters
+
+* `locales`: The location of the source `.po` files.
+
+* `destination`: The location of the destination `.mo` files.  They will be put
+  into this location in the same structure as the source tree relative to the
+  `locales` path.
+
+* `pathsub_regex` (optional): An input regex to match against source files for
+  name changes.
+
+* `pathsub_replace` (required if `pathsub_regex` is present): An replacement
+  pattern to use for name changes.
 
 # Copyright
 
-This plugin is Copyright 2023 Absolute Performance, Inc.
+This plugin is Copyright 2023 Absolute Performance, Inc. with contributions by
+[Adrián Chaves](https://github.com/Gallaecio).
 
 MIT licensed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

