# Comparing `tmp/startstop-1.0.3.tar.gz` & `tmp/startstop-1.0.4.tar.gz`

## Comparing `startstop-1.0.3.tar` & `startstop-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 startstop-1.0.3/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.3/startstop/__about__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 startstop-1.0.3/startstop/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 startstop-1.0.3/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 startstop-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 startstop-1.0.4/example.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.4/startstop/__about__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 startstop-1.0.4/startstop/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 startstop-1.0.4/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 startstop-1.0.4/PKG-INFO
```

### Comparing `startstop-1.0.3/.gitignore` & `startstop-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `startstop-1.0.3/LICENSE.txt` & `startstop-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `startstop-1.0.3/PKG-INFO` & `startstop-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: startstop
-Version: 1.0.3
+Version: 1.0.4
 Summary: Start and stop a python profiler
 Project-URL: homepage, https://github.com/1081/startstop
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: profiler,simple
 Requires-Python: >=3.7
 Requires-Dist: pyinstrument
```

