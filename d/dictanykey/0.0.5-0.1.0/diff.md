# Comparing `tmp/dictanykey-0.0.5.tar.gz` & `tmp/dictanykey-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictanykey-0.0.5.tar", last modified: Fri Jan 20 16:28:25 2023, max compression
+gzip compressed data, was "dictanykey-0.1.0.tar", last modified: Fri Apr  7 18:41:16 2023, max compression
```

## Comparing `dictanykey-0.0.5.tar` & `dictanykey-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-01-20 16:28:25.626127 dictanykey-0.0.5/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2245 2023-01-20 16:28:25.626002 dictanykey-0.0.5/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1706 2023-01-20 16:26:17.000000 dictanykey-0.0.5/README.md
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-01-20 16:28:25.625261 dictanykey-0.0.5/dictanykey/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      186 2023-01-20 16:24:06.000000 dictanykey-0.0.5/dictanykey/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1808 2023-01-20 16:24:20.000000 dictanykey-0.0.5/dictanykey/default_dictanykey.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     5824 2023-01-20 16:25:23.000000 dictanykey-0.0.5/dictanykey/dictanykey.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1785 2023-01-20 16:25:26.000000 dictanykey-0.0.5/dictanykey/frozen_dictanykey.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1679 2023-01-20 16:25:30.000000 dictanykey-0.0.5/dictanykey/iterables.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1374 2023-01-20 16:25:34.000000 dictanykey-0.0.5/dictanykey/iterators.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      211 2023-01-20 16:25:36.000000 dictanykey-0.0.5/dictanykey/parent.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     3071 2023-01-20 16:25:46.000000 dictanykey-0.0.5/dictanykey/unhashmap.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      324 2023-01-20 16:25:50.000000 dictanykey-0.0.5/dictanykey/utils.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1332 2023-01-20 16:26:03.000000 dictanykey-0.0.5/dictanykey/view_objects.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-01-20 16:28:25.625842 dictanykey-0.0.5/dictanykey.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2245 2023-01-20 16:28:25.000000 dictanykey-0.0.5/dictanykey.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      407 2023-01-20 16:28:25.000000 dictanykey-0.0.5/dictanykey.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-01-20 16:28:25.000000 dictanykey-0.0.5/dictanykey.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)       11 2023-01-20 16:28:25.000000 dictanykey-0.0.5/dictanykey.egg-info/top_level.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-01-20 16:28:25.626161 dictanykey-0.0.5/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)      859 2023-01-20 16:26:51.000000 dictanykey-0.0.5/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-04-07 18:41:16.484112 dictanykey-0.1.0/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2245 2023-04-07 18:41:16.483909 dictanykey-0.1.0/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1706 2022-09-12 21:38:43.000000 dictanykey-0.1.0/README.md
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-04-07 18:41:16.478616 dictanykey-0.1.0/dictanykey/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      186 2023-04-07 18:37:35.000000 dictanykey-0.1.0/dictanykey/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1041 2023-04-07 18:38:33.000000 dictanykey-0.1.0/dictanykey/counts.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1808 2022-09-12 21:38:43.000000 dictanykey-0.1.0/dictanykey/default_dictanykey.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     5824 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/dictanykey.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1785 2022-09-12 21:38:43.000000 dictanykey-0.1.0/dictanykey/frozen_dictanykey.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1679 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/iterables.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1374 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/iterators.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      211 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/parent.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3071 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/unhashmap.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      324 2022-07-19 18:53:31.000000 dictanykey-0.1.0/dictanykey/utils.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1332 2023-04-07 15:52:02.000000 dictanykey-0.1.0/dictanykey/view_objects.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-04-07 18:41:16.482449 dictanykey-0.1.0/dictanykey.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2245 2023-04-07 18:41:16.000000 dictanykey-0.1.0/dictanykey.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      510 2023-04-07 18:41:16.000000 dictanykey-0.1.0/dictanykey.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-04-07 18:41:16.000000 dictanykey-0.1.0/dictanykey.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       11 2023-04-07 18:41:16.000000 dictanykey-0.1.0/dictanykey.egg-info/top_level.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       38 2023-04-07 18:41:16.484170 dictanykey-0.1.0/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      859 2023-04-07 18:37:28.000000 dictanykey-0.1.0/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-04-07 18:41:16.483490 dictanykey-0.1.0/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     9439 2022-09-12 21:38:43.000000 dictanykey-0.1.0/tests/test_anykeydict.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)    10891 2022-07-21 15:37:22.000000 dictanykey-0.1.0/tests/test_default_anykeydict.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     7117 2022-09-12 21:38:43.000000 dictanykey-0.1.0/tests/test_unhashmap.py
```

### Comparing `dictanykey-0.0.5/PKG-INFO` & `dictanykey-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictanykey
-Version: 0.0.5
+Version: 0.1.0
 Summary: A dict that can use unhashable keys
 Home-page: https://github.com/eddiethedean/dictanykey
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dictanykey-0.0.5/README.md` & `dictanykey-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/default_dictanykey.py` & `dictanykey-0.1.0/dictanykey/default_dictanykey.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/dictanykey.py` & `dictanykey-0.1.0/dictanykey/dictanykey.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/frozen_dictanykey.py` & `dictanykey-0.1.0/dictanykey/frozen_dictanykey.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/iterables.py` & `dictanykey-0.1.0/dictanykey/iterables.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/iterators.py` & `dictanykey-0.1.0/dictanykey/iterators.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/unhashmap.py` & `dictanykey-0.1.0/dictanykey/unhashmap.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey/view_objects.py` & `dictanykey-0.1.0/dictanykey/view_objects.py`

 * *Files identical despite different names*

### Comparing `dictanykey-0.0.5/dictanykey.egg-info/PKG-INFO` & `dictanykey-0.1.0/dictanykey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictanykey
-Version: 0.0.5
+Version: 0.1.0
 Summary: A dict that can use unhashable keys
 Home-page: https://github.com/eddiethedean/dictanykey
 Author: Odos Matthews
 Author-email: odosmatthews@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dictanykey-0.0.5/setup.py` & `dictanykey-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="dictanykey",
-    version="0.0.5",
+    version="0.1.0",
     description="A dict that can use unhashable keys",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/eddiethedean/dictanykey",
     author="Odos Matthews",
     author_email="odosmatthews@gmail.com",
     license="MIT",
```

