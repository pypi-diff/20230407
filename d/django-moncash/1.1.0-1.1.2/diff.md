# Comparing `tmp/django_moncash-1.1.0.tar.gz` & `tmp/django_moncash-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-1.1.0.tar", last modified: Fri Apr  7 21:16:33 2023, max compression
+gzip compressed data, was "django_moncash-1.1.2.tar", last modified: Fri Apr  7 21:20:14 2023, max compression
```

## Comparing `django_moncash-1.1.0.tar` & `django_moncash-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:16:33.949224 django_moncash-1.1.0/
--rw-r--r--   0 macbook    (501) staff       (20)     8232 2023-04-07 21:16:33.949341 django_moncash-1.1.0/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:16:33.948374 django_moncash-1.1.0/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     8232 2023-04-07 21:16:33.000000 django_moncash-1.1.0/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 21:16:33.000000 django_moncash-1.1.0/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 21:16:33.000000 django_moncash-1.1.0/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 21:16:33.000000 django_moncash-1.1.0/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 21:16:33.000000 django_moncash-1.1.0/django_moncash.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:16:33.949066 django_moncash-1.1.0/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.1.0/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.1.0/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 21:16:33.949778 django_moncash-1.1.0/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-07 20:38:55.000000 django_moncash-1.1.0/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:20:14.026362 django_moncash-1.1.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     8232 2023-04-07 21:20:14.026480 django_moncash-1.1.2/PKG-INFO
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:20:14.025686 django_moncash-1.1.2/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     8232 2023-04-07 21:20:13.000000 django_moncash-1.1.2/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 21:20:13.000000 django_moncash-1.1.2/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 21:20:13.000000 django_moncash-1.1.2/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 21:20:13.000000 django_moncash-1.1.2/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 21:20:13.000000 django_moncash-1.1.2/django_moncash.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 21:20:14.026223 django_moncash-1.1.2/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.1.2/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.1.2/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 21:20:14.027108 django_moncash-1.1.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-07 20:38:55.000000 django_moncash-1.1.2/setup.py
```

### Comparing `django_moncash-1.1.0/PKG-INFO` & `django_moncash-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 1.1.0
+Version: 1.1.2
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 License: GNU
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -281,11 +281,11 @@
 (+509) 48-02-0151
 
 ## License
 [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.txt)
 _Version 3, 29 June 2007_
 
 ## Useful links
-- [Pypi package link](https://pypi.org/project/django_moncash/)
+- [Pypi package link](https://pypi.org/project/django-moncash/)
 - [Digicel Moncash API Dashboard](https://sandbox.moncashbutton.digicelgroup.com)
 - [RestAPI_MonCash_doc.pdf](https://sandbox.moncashbutton.digicelgroup.com/Moncash-business/resources/doc/RestAPI_MonCash_doc.pdf)
 - [Low level SDK for python](https://github.com/dokla/moncash_python)
```

### Comparing `django_moncash-1.1.0/django_moncash.egg-info/PKG-INFO` & `django_moncash-1.1.2/django_moncash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moncash
-Version: 1.1.0
+Version: 1.1.2
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 License: GNU
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -281,11 +281,11 @@
 (+509) 48-02-0151
 
 ## License
 [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.txt)
 _Version 3, 29 June 2007_
 
 ## Useful links
-- [Pypi package link](https://pypi.org/project/django_moncash/)
+- [Pypi package link](https://pypi.org/project/django-moncash/)
 - [Digicel Moncash API Dashboard](https://sandbox.moncashbutton.digicelgroup.com)
 - [RestAPI_MonCash_doc.pdf](https://sandbox.moncashbutton.digicelgroup.com/Moncash-business/resources/doc/RestAPI_MonCash_doc.pdf)
 - [Low level SDK for python](https://github.com/dokla/moncash_python)
```

### Comparing `django_moncash-1.1.0/migrations/0001_initial.py` & `django_moncash-1.1.2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-1.1.0/setup.cfg` & `django_moncash-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 1.1.0
+version = 1.1.2
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

