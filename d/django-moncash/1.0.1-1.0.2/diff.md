# Comparing `tmp/django_moncash-1.0.1.tar.gz` & `tmp/django_moncash-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-1.0.1.tar", last modified: Fri Apr  7 20:44:35 2023, max compression
+gzip compressed data, was "django_moncash-1.0.2.tar", last modified: Fri Apr  7 21:07:45 2023, max compression
```

## Comparing `django_moncash-1.0.1.tar` & `django_moncash-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205953 django_moncash-1.0.1/
--rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 20:44:35.206048 django_moncash-1.0.1/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205166 django_moncash-1.0.1/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205764 django_moncash-1.0.1/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.0.1/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.0.1/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 20:44:35.206445 django_moncash-1.0.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-07 20:38:55.000000 django_moncash-1.0.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:07:45.724715 django_moncash-1.0.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     8254 2023-04-07 21:07:45.724838 django_moncash-1.0.2/PKG-INFO
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:07:45.723989 django_moncash-1.0.2/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     8254 2023-04-07 21:07:45.000000 django_moncash-1.0.2/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 21:07:45.000000 django_moncash-1.0.2/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 21:07:45.000000 django_moncash-1.0.2/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 21:07:45.000000 django_moncash-1.0.2/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 21:07:45.000000 django_moncash-1.0.2/django_moncash.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:07:45.724554 django_moncash-1.0.2/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.0.2/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.0.2/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 21:07:45.725382 django_moncash-1.0.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-07 20:38:55.000000 django_moncash-1.0.2/setup.py
```

### Comparing `django_moncash-1.0.1/PKG-INFO` & `django_moncash-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 1.0.1
+Version: 1.0.2
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 License: GNU
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -267,14 +267,23 @@
 
 ## Development
 Run all tests.
 ```sh
     python load_tests.py
 ```
 
+## Donate to support us
+
+Scan and donate using the Moncash App
+
+![Moncash_QR](https://pypi.org/project/django_moncash/assets/gr.jpg)  
+
+Or send to 
+(+509) 48-02-0151
+
 ## License
 [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.txt)
 _Version 3, 29 June 2007_
 
 ## Useful links
 - [Pypi package link](https://pypi.org/project/django_moncash/)
 - [Digicel Moncash API Dashboard](https://sandbox.moncashbutton.digicelgroup.com)
```

### Comparing `django_moncash-1.0.1/django_moncash.egg-info/PKG-INFO` & `django_moncash-1.0.2/django_moncash.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moncash
-Version: 1.0.1
+Version: 1.0.2
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 License: GNU
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -267,14 +267,23 @@
 
 ## Development
 Run all tests.
 ```sh
     python load_tests.py
 ```
 
+## Donate to support us
+
+Scan and donate using the Moncash App
+
+![Moncash_QR](https://pypi.org/project/django_moncash/assets/gr.jpg)  
+
+Or send to 
+(+509) 48-02-0151
+
 ## License
 [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.txt)
 _Version 3, 29 June 2007_
 
 ## Useful links
 - [Pypi package link](https://pypi.org/project/django_moncash/)
 - [Digicel Moncash API Dashboard](https://sandbox.moncashbutton.digicelgroup.com)
```

### Comparing `django_moncash-1.0.1/migrations/0001_initial.py` & `django_moncash-1.0.2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-1.0.1/setup.cfg` & `django_moncash-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 1.0.1
+version = 1.0.2
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

