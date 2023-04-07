# Comparing `tmp/textscribe-0.1.6.tar.gz` & `tmp/textscribe-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textscribe-0.1.6.tar", last modified: Wed Apr  5 17:39:37 2023, max compression
+gzip compressed data, was "textscribe-0.1.7.tar", last modified: Fri Apr  7 18:27:26 2023, max compression
```

## Comparing `textscribe-0.1.6.tar` & `textscribe-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 17:39:37.625107 textscribe-0.1.6/
--rw-rw-rw-   0        0        0       81 2023-03-26 04:27:30.000000 textscribe-0.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-03-26 04:31:13.000000 textscribe-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       31 2023-03-26 04:28:38.000000 textscribe-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6135 2023-04-05 17:39:37.625107 textscribe-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5572 2023-04-05 17:39:16.000000 textscribe-0.1.6/README.md
--rw-rw-rw-   0        0        0      108 2023-03-26 05:09:04.000000 textscribe-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      448 2023-04-05 17:39:37.627108 textscribe-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      810 2023-04-05 17:39:26.000000 textscribe-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 17:39:37.611105 textscribe-0.1.6/textscribe/
--rw-rw-rw-   0        0        0        0 2023-03-26 05:21:58.000000 textscribe-0.1.6/textscribe/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-03-28 00:48:52.000000 textscribe-0.1.6/textscribe/scribe.py
-drwxrwxrwx   0        0        0        0 2023-04-05 17:39:37.624107 textscribe-0.1.6/textscribe.egg-info/
--rw-rw-rw-   0        0        0     6135 2023-04-05 17:39:37.000000 textscribe-0.1.6/textscribe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-05 17:39:37.000000 textscribe-0.1.6/textscribe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 17:39:37.000000 textscribe-0.1.6/textscribe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-05 17:39:37.000000 textscribe-0.1.6/textscribe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 18:27:26.827777 textscribe-0.1.7/
+-rw-rw-rw-   0        0        0       81 2023-03-26 04:27:30.000000 textscribe-0.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-03-26 04:31:13.000000 textscribe-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-03-26 04:28:38.000000 textscribe-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6110 2023-04-07 18:27:26.826778 textscribe-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5571 2023-04-06 01:07:56.000000 textscribe-0.1.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-26 05:09:04.000000 textscribe-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 18:27:26.827777 textscribe-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      810 2023-04-07 18:27:24.000000 textscribe-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:27:26.808776 textscribe-0.1.7/textscribe/
+-rw-rw-rw-   0        0        0        0 2023-03-26 05:21:58.000000 textscribe-0.1.7/textscribe/__init__.py
+-rw-rw-rw-   0        0        0     4806 2023-04-07 18:26:58.000000 textscribe-0.1.7/textscribe/scribe.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:27:26.825778 textscribe-0.1.7/textscribe.egg-info/
+-rw-rw-rw-   0        0        0     6110 2023-04-07 18:27:26.000000 textscribe-0.1.7/textscribe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-07 18:27:26.000000 textscribe-0.1.7/textscribe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 18:27:26.000000 textscribe-0.1.7/textscribe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-07 18:27:26.000000 textscribe-0.1.7/textscribe.egg-info/top_level.txt
```

### Comparing `textscribe-0.1.6/LICENSE` & `textscribe-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `textscribe-0.1.6/PKG-INFO` & `textscribe-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: textscribe
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easily Structuring Data
 Home-page: 
 Author: Hunter Thomas
 Author-email: waidai2027@gmail.com
 License: MIT
 Keywords: Structure data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CSV, JSON and TXT Reader and Writer Library
 
 This library offers streamlined and efficient methods for reading and writing data to CSV, JSON and TXT files, enabling faster and more convenient data processing.
 
@@ -196,13 +195,13 @@
 name_values = get_json_values(file_name, label)
 print(name_values)
 
 ```
 
 ## Github Repo
 
--https://github.com/huntert1004/textscribe
+https://github.com/huntert1004/textscribe
```

### Comparing `textscribe-0.1.6/README.md` & `textscribe-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,13 +178,13 @@
 name_values = get_json_values(file_name, label)
 print(name_values)
 
 ```
 
 ## Github Repo
 
--https://github.com/huntert1004/textscribe
+https://github.com/huntert1004/textscribe
```

### Comparing `textscribe-0.1.6/setup.py` & `textscribe-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='textscribe',
-  version='0.1.6',
+  version='0.1.7',
   description='Easily Structuring Data',
   long_description=long_description,
   url='',  
   author='Hunter Thomas',
   author_email='waidai2027@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `textscribe-0.1.6/textscribe.egg-info/PKG-INFO` & `textscribe-0.1.7/textscribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: textscribe
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easily Structuring Data
 Home-page: 
 Author: Hunter Thomas
 Author-email: waidai2027@gmail.com
 License: MIT
 Keywords: Structure data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CSV, JSON and TXT Reader and Writer Library
 
 This library offers streamlined and efficient methods for reading and writing data to CSV, JSON and TXT files, enabling faster and more convenient data processing.
 
@@ -196,13 +195,13 @@
 name_values = get_json_values(file_name, label)
 print(name_values)
 
 ```
 
 ## Github Repo
 
--https://github.com/huntert1004/textscribe
+https://github.com/huntert1004/textscribe
```

