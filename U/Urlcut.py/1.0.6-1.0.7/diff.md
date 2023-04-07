# Comparing `tmp/Urlcut.py-1.0.6.tar.gz` & `tmp/Urlcut.py-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Urlcut.py-1.0.6.tar", last modified: Fri Apr  7 19:13:36 2023, max compression
+gzip compressed data, was "Urlcut.py-1.0.7.tar", last modified: Fri Apr  7 19:21:31 2023, max compression
```

## Comparing `Urlcut.py-1.0.6.tar` & `Urlcut.py-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:13:36.929234 Urlcut.py-1.0.6/
--rw-rw-rw-   0        0        0     1051 2023-04-07 18:51:06.000000 Urlcut.py-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      708 2023-04-07 19:13:36.928213 Urlcut.py-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-04-07 19:08:10.000000 Urlcut.py-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 19:13:36.924691 Urlcut.py-1.0.6/Urlcut.py.egg-info/
--rw-rw-rw-   0        0        0      708 2023-04-07 19:13:36.000000 Urlcut.py-1.0.6/Urlcut.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-04-07 19:13:36.000000 Urlcut.py-1.0.6/Urlcut.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:13:36.000000 Urlcut.py-1.0.6/Urlcut.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 19:13:36.000000 Urlcut.py-1.0.6/Urlcut.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 19:13:36.000000 Urlcut.py-1.0.6/Urlcut.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 19:13:36.930234 Urlcut.py-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-04-07 19:13:32.000000 Urlcut.py-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:13:36.925691 Urlcut.py-1.0.6/urlcutpy/
--rw-rw-rw-   0        0        0      636 2023-04-07 18:49:36.000000 Urlcut.py-1.0.6/urlcutpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:21:31.399273 Urlcut.py-1.0.7/
+-rw-rw-rw-   0        0        0     1051 2023-04-07 18:51:06.000000 Urlcut.py-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      708 2023-04-07 19:21:31.397272 Urlcut.py-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-04-07 19:08:10.000000 Urlcut.py-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 19:21:31.384212 Urlcut.py-1.0.7/Urlcut.py.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-04-07 19:21:31.000000 Urlcut.py-1.0.7/Urlcut.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-04-07 19:21:31.000000 Urlcut.py-1.0.7/Urlcut.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 19:21:31.000000 Urlcut.py-1.0.7/Urlcut.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-07 19:21:31.000000 Urlcut.py-1.0.7/Urlcut.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-07 19:21:31.000000 Urlcut.py-1.0.7/Urlcut.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 19:21:31.400277 Urlcut.py-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-04-07 19:20:49.000000 Urlcut.py-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:21:31.387212 Urlcut.py-1.0.7/urlcutpy/
+-rw-rw-rw-   0        0        0      613 2023-04-07 19:19:19.000000 Urlcut.py-1.0.7/urlcutpy/__init__.py
```

### Comparing `Urlcut.py-1.0.6/LICENSE.txt` & `Urlcut.py-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Urlcut.py-1.0.6/PKG-INFO` & `Urlcut.py-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Urlcut.py
-Version: 1.0.6
+Version: 1.0.7
 Summary: Official Urlcut Public API package.
 Home-page: https://urlcut.app
 Author: Urlcut
 Author-email: support@urlcut.app
 License: MIT
 Keywords: urlcut
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Urlcut.py-1.0.6/Urlcut.py.egg-info/PKG-INFO` & `Urlcut.py-1.0.7/Urlcut.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Urlcut.py
-Version: 1.0.6
+Version: 1.0.7
 Summary: Official Urlcut Public API package.
 Home-page: https://urlcut.app
 Author: Urlcut
 Author-email: support@urlcut.app
 License: MIT
 Keywords: urlcut
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Urlcut.py-1.0.6/setup.py` & `Urlcut.py-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Urlcut.py',
-    version='1.0.6',
+    version='1.0.7',
     description='Official Urlcut Public API package.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://urlcut.app',
     author='Urlcut',
     author_email='support@urlcut.app',
     license='MIT',
```

### Comparing `Urlcut.py-1.0.6/urlcutpy/__init__.py` & `Urlcut.py-1.0.7/urlcutpy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 Token = ""
 
 def Authenticate(_Authorization_Token):
     global Token 
     if _Authorization_Token:
         token_length = len(_Authorization_Token)
         if token_length < 27:
-            raise UrlcutError("Error")
+            raise UrlcutError("API key is too short to be valid.")
         else:
             Token = _Authorization_Token
     else:
-        raise UrlcutError("No API key provided.")
-
-Authenticate("PCEnv5-POrz4K-OUY8ZR-dgsf5J")
-
+        raise UrlcutError("No API key provided.")
```

