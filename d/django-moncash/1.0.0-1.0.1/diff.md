# Comparing `tmp/django_moncash-1.0.0.tar.gz` & `tmp/django_moncash-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-1.0.0.tar", last modified: Fri Apr  7 20:29:54 2023, max compression
+gzip compressed data, was "django_moncash-1.0.1.tar", last modified: Fri Apr  7 20:44:35 2023, max compression
```

## Comparing `django_moncash-1.0.0.tar` & `django_moncash-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:29:54.989371 django_moncash-1.0.0/
--rw-r--r--   0 macbook    (501) staff       (20)      771 2023-04-07 20:29:54.989466 django_moncash-1.0.0/PKG-INFO
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:29:54.988662 django_moncash-1.0.0/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)      771 2023-04-07 20:29:54.000000 django_moncash-1.0.0/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 20:29:54.000000 django_moncash-1.0.0/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 20:29:54.000000 django_moncash-1.0.0/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 20:29:54.000000 django_moncash-1.0.0/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 20:29:54.000000 django_moncash-1.0.0/django_moncash.egg-info/top_level.txt
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:29:54.989228 django_moncash-1.0.0/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.0.0/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.0.0/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 20:29:54.989863 django_moncash-1.0.0/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)       94 2023-04-07 16:31:17.000000 django_moncash-1.0.0/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205953 django_moncash-1.0.1/
+-rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 20:44:35.206048 django_moncash-1.0.1/PKG-INFO
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205166 django_moncash-1.0.1/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      257 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       27 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-07 20:44:35.000000 django_moncash-1.0.1/django_moncash.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-07 20:44:35.205764 django_moncash-1.0.1/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-1.0.1/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-1.0.1/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-07 20:44:35.206445 django_moncash-1.0.1/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)      415 2023-04-07 20:38:55.000000 django_moncash-1.0.1/setup.py
```

### Comparing `django_moncash-1.0.0/migrations/0001_initial.py` & `django_moncash-1.0.1/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-1.0.0/setup.cfg` & `django_moncash-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 1.0.0
+version = 1.0.1
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

