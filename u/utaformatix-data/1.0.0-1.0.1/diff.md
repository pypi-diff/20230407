# Comparing `tmp/utaformatix-data-1.0.0.tar.gz` & `tmp/utaformatix-data-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utaformatix-data-1.0.0.tar", last modified: Fri Apr  7 17:20:24 2023, max compression
+gzip compressed data, was "utaformatix-data-1.0.1.tar", last modified: Fri Apr  7 17:29:06 2023, max compression
```

## Comparing `utaformatix-data-1.0.0.tar` & `utaformatix-data-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:20:24.033200 utaformatix-data-1.0.0/
--rw-r--r--   0 sdercolin   (501) staff       (20)       24 2023-04-07 17:17:40.000000 utaformatix-data-1.0.0/MANIFEST.in
--rw-r--r--   0 sdercolin   (501) staff       (20)      290 2023-04-07 17:20:24.033058 utaformatix-data-1.0.0/PKG-INFO
--rw-r--r--   0 sdercolin   (501) staff       (20)      739 2023-04-07 16:47:37.000000 utaformatix-data-1.0.0/README.md
--rw-r--r--   0 sdercolin   (501) staff       (20)       15 2023-04-07 17:01:47.000000 utaformatix-data-1.0.0/requirements.txt
--rw-r--r--   0 sdercolin   (501) staff       (20)       38 2023-04-07 17:20:24.033239 utaformatix-data-1.0.0/setup.cfg
--rw-r--r--   0 sdercolin   (501) staff       (20)      562 2023-04-07 17:20:11.000000 utaformatix-data-1.0.0/setup.py
-drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:20:24.032031 utaformatix-data-1.0.0/ufdata/
--rw-r--r--   0 sdercolin   (501) staff       (20)      272 2023-04-07 14:57:59.000000 utaformatix-data-1.0.0/ufdata/__init__.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1485 2023-04-07 15:01:51.000000 utaformatix-data-1.0.0/ufdata/document.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1227 2023-04-07 15:01:42.000000 utaformatix-data-1.0.0/ufdata/note.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1146 2023-04-07 15:01:36.000000 utaformatix-data-1.0.0/ufdata/pitch.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1896 2023-04-07 15:01:28.000000 utaformatix-data-1.0.0/ufdata/project.py
--rw-r--r--   0 sdercolin   (501) staff       (20)      664 2023-04-07 15:01:22.000000 utaformatix-data-1.0.0/ufdata/tempo.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1002 2023-04-07 15:01:13.000000 utaformatix-data-1.0.0/ufdata/time_signature.py
--rw-r--r--   0 sdercolin   (501) staff       (20)     1037 2023-04-07 15:01:42.000000 utaformatix-data-1.0.0/ufdata/track.py
-drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:20:24.032839 utaformatix-data-1.0.0/utaformatix_data.egg-info/
--rw-r--r--   0 sdercolin   (501) staff       (20)      290 2023-04-07 17:20:24.000000 utaformatix-data-1.0.0/utaformatix_data.egg-info/PKG-INFO
--rw-r--r--   0 sdercolin   (501) staff       (20)      390 2023-04-07 17:20:24.000000 utaformatix-data-1.0.0/utaformatix_data.egg-info/SOURCES.txt
--rw-r--r--   0 sdercolin   (501) staff       (20)        1 2023-04-07 17:20:24.000000 utaformatix-data-1.0.0/utaformatix_data.egg-info/dependency_links.txt
--rw-r--r--   0 sdercolin   (501) staff       (20)       15 2023-04-07 17:20:24.000000 utaformatix-data-1.0.0/utaformatix_data.egg-info/requires.txt
--rw-r--r--   0 sdercolin   (501) staff       (20)        7 2023-04-07 17:20:24.000000 utaformatix-data-1.0.0/utaformatix_data.egg-info/top_level.txt
+drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:29:06.003269 utaformatix-data-1.0.1/
+-rw-r--r--   0 sdercolin   (501) staff       (20)       24 2023-04-07 17:17:40.000000 utaformatix-data-1.0.1/MANIFEST.in
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1062 2023-04-07 17:29:06.003102 utaformatix-data-1.0.1/PKG-INFO
+-rw-r--r--   0 sdercolin   (501) staff       (20)      739 2023-04-07 16:47:37.000000 utaformatix-data-1.0.1/README.md
+-rw-r--r--   0 sdercolin   (501) staff       (20)       15 2023-04-07 17:01:47.000000 utaformatix-data-1.0.1/requirements.txt
+-rw-r--r--   0 sdercolin   (501) staff       (20)       38 2023-04-07 17:29:06.003311 utaformatix-data-1.0.1/setup.cfg
+-rw-r--r--   0 sdercolin   (501) staff       (20)      660 2023-04-07 17:28:25.000000 utaformatix-data-1.0.1/setup.py
+drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:29:06.002190 utaformatix-data-1.0.1/ufdata/
+-rw-r--r--   0 sdercolin   (501) staff       (20)      272 2023-04-07 14:57:59.000000 utaformatix-data-1.0.1/ufdata/__init__.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1485 2023-04-07 15:01:51.000000 utaformatix-data-1.0.1/ufdata/document.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1227 2023-04-07 15:01:42.000000 utaformatix-data-1.0.1/ufdata/note.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1146 2023-04-07 15:01:36.000000 utaformatix-data-1.0.1/ufdata/pitch.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1896 2023-04-07 15:01:28.000000 utaformatix-data-1.0.1/ufdata/project.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)      664 2023-04-07 15:01:22.000000 utaformatix-data-1.0.1/ufdata/tempo.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1002 2023-04-07 15:01:13.000000 utaformatix-data-1.0.1/ufdata/time_signature.py
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1037 2023-04-07 15:01:42.000000 utaformatix-data-1.0.1/ufdata/track.py
+drwxr-xr-x   0 sdercolin   (501) staff       (20)        0 2023-04-07 17:29:06.002759 utaformatix-data-1.0.1/utaformatix_data.egg-info/
+-rw-r--r--   0 sdercolin   (501) staff       (20)     1062 2023-04-07 17:29:05.000000 utaformatix-data-1.0.1/utaformatix_data.egg-info/PKG-INFO
+-rw-r--r--   0 sdercolin   (501) staff       (20)      390 2023-04-07 17:29:05.000000 utaformatix-data-1.0.1/utaformatix_data.egg-info/SOURCES.txt
+-rw-r--r--   0 sdercolin   (501) staff       (20)        1 2023-04-07 17:29:05.000000 utaformatix-data-1.0.1/utaformatix_data.egg-info/dependency_links.txt
+-rw-r--r--   0 sdercolin   (501) staff       (20)       15 2023-04-07 17:29:05.000000 utaformatix-data-1.0.1/utaformatix_data.egg-info/requires.txt
+-rw-r--r--   0 sdercolin   (501) staff       (20)        7 2023-04-07 17:29:05.000000 utaformatix-data-1.0.1/utaformatix_data.egg-info/top_level.txt
```

### Comparing `utaformatix-data-1.0.0/README.md` & `utaformatix-data-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/document.py` & `utaformatix-data-1.0.1/ufdata/document.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/note.py` & `utaformatix-data-1.0.1/ufdata/note.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/pitch.py` & `utaformatix-data-1.0.1/ufdata/pitch.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/project.py` & `utaformatix-data-1.0.1/ufdata/project.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/tempo.py` & `utaformatix-data-1.0.1/ufdata/tempo.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/time_signature.py` & `utaformatix-data-1.0.1/ufdata/time_signature.py`

 * *Files identical despite different names*

### Comparing `utaformatix-data-1.0.0/ufdata/track.py` & `utaformatix-data-1.0.1/ufdata/track.py`

 * *Files identical despite different names*

