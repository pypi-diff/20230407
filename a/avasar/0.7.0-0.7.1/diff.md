# Comparing `tmp/avasar-0.7.0.tar.gz` & `tmp/avasar-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avasar-0.7.0.tar", max compression
+gzip compressed data, was "avasar-0.7.1.tar", max compression
```

## Comparing `avasar-0.7.0.tar` & `avasar-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2023-03-05 22:20:25.812195 avasar-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-03-06 12:07:52.085967 avasar-0.7.0/avasar/__init__.py
--rw-r--r--   0        0        0       28 2023-03-06 16:54:29.691949 avasar-0.7.0/avasar/__main__.py
--rw-r--r--   0        0        0     2056 2023-03-10 15:32:27.684561 avasar-0.7.0/avasar/data/blades.toml
--rw-r--r--   0        0        0    35236 2023-03-06 15:42:15.961145 avasar-0.7.0/avasar/data/firstname-english-female.toml
--rw-r--r--   0        0        0    26690 2023-03-06 15:41:34.137528 avasar-0.7.0/avasar/data/firstname-english-male.toml
--rw-r--r--   0        0        0     7542 2023-03-06 15:41:44.906625 avasar-0.7.0/avasar/data/firstname-german-female.toml
--rw-r--r--   0        0        0     7884 2023-03-06 15:41:14.424307 avasar-0.7.0/avasar/data/firstname-german-male.toml
--rw-r--r--   0        0        0    14297 2023-03-06 17:26:54.618482 avasar-0.7.0/avasar/data/lastname-english.toml
--rw-r--r--   0        0        0    25462 2023-03-06 17:26:07.218468 avasar-0.7.0/avasar/data/lastname-german.toml
--rw-r--r--   0        0        0      851 2023-03-06 21:05:01.348209 avasar-0.7.0/avasar/data/person.py
--rw-r--r--   0        0        0     9824 2023-03-10 15:29:59.807367 avasar-0.7.0/avasar/data/person.toml
--rw-r--r--   0        0        0     3079 2023-04-07 19:28:33.599285 avasar-0.7.0/avasar/data/places.toml
--rw-r--r--   0        0        0    10442 2023-04-07 19:58:18.751725 avasar-0.7.0/avasar/dsl.py
--rw-r--r--   0        0        0      922 2023-04-07 16:00:11.905943 avasar-0.7.0/avasar/main.py
--rw-r--r--   0        0        0      761 2023-04-07 20:02:49.401173 avasar-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 avasar-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 22:20:25.812195 avasar-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-06 12:07:52.085967 avasar-0.7.1/avasar/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-06 16:54:29.691949 avasar-0.7.1/avasar/__main__.py
+-rw-r--r--   0        0        0     2056 2023-03-10 15:32:27.684561 avasar-0.7.1/avasar/data/blades.toml
+-rw-r--r--   0        0        0    35236 2023-03-06 15:42:15.961145 avasar-0.7.1/avasar/data/firstname-english-female.toml
+-rw-r--r--   0        0        0    26690 2023-03-06 15:41:34.137528 avasar-0.7.1/avasar/data/firstname-english-male.toml
+-rw-r--r--   0        0        0     7542 2023-03-06 15:41:44.906625 avasar-0.7.1/avasar/data/firstname-german-female.toml
+-rw-r--r--   0        0        0     7884 2023-03-06 15:41:14.424307 avasar-0.7.1/avasar/data/firstname-german-male.toml
+-rw-r--r--   0        0        0    14297 2023-03-06 17:26:54.618482 avasar-0.7.1/avasar/data/lastname-english.toml
+-rw-r--r--   0        0        0    25462 2023-03-06 17:26:07.218468 avasar-0.7.1/avasar/data/lastname-german.toml
+-rw-r--r--   0        0        0      851 2023-03-06 21:05:01.348209 avasar-0.7.1/avasar/data/person.py
+-rw-r--r--   0        0        0     9824 2023-03-10 15:29:59.807367 avasar-0.7.1/avasar/data/person.toml
+-rw-r--r--   0        0        0     3079 2023-04-07 19:28:33.599285 avasar-0.7.1/avasar/data/places.toml
+-rw-r--r--   0        0        0    10499 2023-04-07 20:10:42.162679 avasar-0.7.1/avasar/dsl.py
+-rw-r--r--   0        0        0      865 2023-04-07 20:07:27.731915 avasar-0.7.1/avasar/main.py
+-rw-r--r--   0        0        0      761 2023-04-07 20:11:21.690021 avasar-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 avasar-0.7.1/PKG-INFO
```

### Comparing `avasar-0.7.0/avasar/data/blades.toml` & `avasar-0.7.1/avasar/data/blades.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/firstname-english-female.toml` & `avasar-0.7.1/avasar/data/firstname-english-female.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/firstname-english-male.toml` & `avasar-0.7.1/avasar/data/firstname-english-male.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/firstname-german-female.toml` & `avasar-0.7.1/avasar/data/firstname-german-female.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/firstname-german-male.toml` & `avasar-0.7.1/avasar/data/firstname-german-male.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/lastname-english.toml` & `avasar-0.7.1/avasar/data/lastname-english.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/lastname-german.toml` & `avasar-0.7.1/avasar/data/lastname-german.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/person.py` & `avasar-0.7.1/avasar/data/person.py`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/person.toml` & `avasar-0.7.1/avasar/data/person.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/data/places.toml` & `avasar-0.7.1/avasar/data/places.toml`

 * *Files identical despite different names*

### Comparing `avasar-0.7.0/avasar/dsl.py` & `avasar-0.7.1/avasar/dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,15 @@
     setattr(cur, parts[-1], value)
 
 
 def build_context():
     context = Context()
     read_toml(context)
 
+    context.__dict__["set_groups"] = context._set_groups
     return context
 
 
 def build_config(avasar):
     count = 1
     if "count" in avasar:
         count = avasar["count"]
```

### Comparing `avasar-0.7.0/avasar/main.py` & `avasar-0.7.1/avasar/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pathlib import Path
 from os.path import expanduser
 import sys
 
 
 def run():
     context = build_context()
-    context.__dict__["set_groups"] = context._set_groups
     if len(sys.argv) > 1:
         if sys.argv[1] == "test":
             print(context.fstr("{gen.character}"))
             sys.exit(0)
 
     if "libedit" in readline.__doc__:
         readline.parse_and_bind("bind ^I rl_complete")
```

### Comparing `avasar-0.7.0/pyproject.toml` & `avasar-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avasar"
-version = "0.7.0"
+version = "0.7.1"
 description = "Text generation DSL in python"
 authors = ["Streampunk <glad.car1474@fastmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `avasar-0.7.0/PKG-INFO` & `avasar-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avasar
-Version: 0.7.0
+Version: 0.7.1
 Summary: Text generation DSL in python
 License: AGPL-3.0-or-later
 Author: Streampunk
 Author-email: glad.car1474@fastmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

