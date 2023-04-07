# Comparing `tmp/startstop-1.0.1.tar.gz` & `tmp/startstop-1.0.2.tar.gz`

## Comparing `startstop-1.0.1.tar` & `startstop-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 startstop-1.0.1/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.1/startstop/__about__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 startstop-1.0.1/startstop/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 startstop-1.0.1/README.md
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 startstop-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 startstop-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 startstop-1.0.2/example.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.2/startstop/__about__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 startstop-1.0.2/startstop/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 startstop-1.0.2/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 startstop-1.0.2/PKG-INFO
```

### Comparing `startstop-1.0.1/.gitignore` & `startstop-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `startstop-1.0.1/LICENSE.txt` & `startstop-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `startstop-1.0.1/PKG-INFO` & `startstop-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: startstop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Start and stop a python profiler
+Project-URL: homepage, https://github.com/1081/startstop
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: profiler,simple
 Requires-Python: >=3.7
 Requires-Dist: pyinstrument
 Description-Content-Type: text/markdown
```

