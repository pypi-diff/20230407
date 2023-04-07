# Comparing `tmp/httpie-hmac-1.1.0.tar.gz` & `tmp/httpie-hmac-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-hmac-1.1.0.tar", last modified: Tue Mar 28 05:30:38 2023, max compression
+gzip compressed data, was "httpie-hmac-1.1.1.tar", last modified: Fri Apr  7 20:46:39 2023, max compression
```

## Comparing `httpie-hmac-1.1.0.tar` & `httpie-hmac-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:30:38.562412 httpie-hmac-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-28 05:30:29.000000 httpie-hmac-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-28 05:30:38.562412 httpie-hmac-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-28 05:30:29.000000 httpie-hmac-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:30:38.558412 httpie-hmac-1.1.0/httpie_hmac/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-28 05:30:29.000000 httpie-hmac-1.1.0/httpie_hmac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-28 05:30:29.000000 httpie-hmac-1.1.0/httpie_hmac/httpie_hmac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 05:30:38.562412 httpie-hmac-1.1.0/httpie_hmac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 05:30:38.000000 httpie-hmac-1.1.0/httpie_hmac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-28 05:30:29.000000 httpie-hmac-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 05:30:38.562412 httpie-hmac-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.170649 httpie-hmac-1.1.1/httpie_hmac/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/httpie_hmac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/httpie_hmac/httpie_hmac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/httpie_hmac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 20:46:39.000000 httpie-hmac-1.1.1/httpie_hmac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 20:46:30.000000 httpie-hmac-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:46:39.174649 httpie-hmac-1.1.1/setup.cfg
```

### Comparing `httpie-hmac-1.1.0/LICENSE` & `httpie-hmac-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-hmac-1.1.0/PKG-INFO` & `httpie-hmac-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: httpie-hmac
-Version: 1.1.0
+Version: 1.1.1
 Summary: HMAC Auth Plugin for Httpie
-Author-email: Martyn Pittuck-Schols <12006448+martynp@users.noreply.github.com>
+Author-email: Martyn Pittuck-Schols <martyn@rustfoo.com>
 License: MIT
 Project-URL: homepage, https://github.com/martynp/httpie-hmac/
 Project-URL: repository, https://github.com/martynp/httpie-hmac.git
 Keywords: httpie,auth,hmac,aws4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `httpie-hmac-1.1.0/README.md` & `httpie-hmac-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `httpie-hmac-1.1.0/httpie_hmac/httpie_hmac.py` & `httpie-hmac-1.1.1/httpie_hmac/httpie_hmac.py`

 * *Files identical despite different names*

### Comparing `httpie-hmac-1.1.0/httpie_hmac.egg-info/PKG-INFO` & `httpie-hmac-1.1.1/httpie_hmac.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: httpie-hmac
-Version: 1.1.0
+Version: 1.1.1
 Summary: HMAC Auth Plugin for Httpie
-Author-email: Martyn Pittuck-Schols <12006448+martynp@users.noreply.github.com>
+Author-email: Martyn Pittuck-Schols <martyn@rustfoo.com>
 License: MIT
 Project-URL: homepage, https://github.com/martynp/httpie-hmac/
 Project-URL: repository, https://github.com/martynp/httpie-hmac.git
 Keywords: httpie,auth,hmac,aws4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `httpie-hmac-1.1.0/pyproject.toml` & `httpie-hmac-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "httpie-hmac"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
-    {name = "Martyn Pittuck-Schols", email = "12006448+martynp@users.noreply.github.com"},
+    {name = "Martyn Pittuck-Schols", email = "martyn@rustfoo.com"},
 ]
 description = "HMAC Auth Plugin for Httpie"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["httpie", "auth", "hmac", "aws4"]
 license = {text = "MIT"}
 classifiers = [
```

