# Comparing `tmp/gmap-1.4.4.tar.gz` & `tmp/gmap-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-1.4.4.tar", last modified: Fri Apr  7 17:54:34 2023, max compression
+gzip compressed data, was "gmap-1.4.6.tar", last modified: Fri Apr  7 18:29:59 2023, max compression
```

## Comparing `gmap-1.4.4.tar` & `gmap-1.4.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 17:54:34.008312 gmap-1.4.4/
--rw-r--r--   0 tahsin     (501) staff       (20)      150 2023-04-07 17:54:34.008146 gmap-1.4.4/PKG-INFO
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 17:54:34.006590 gmap-1.4.4/gmap/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.4.4/gmap/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       22 2023-04-07 08:56:10.000000 gmap-1.4.4/gmap/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1360 2023-04-07 08:54:25.000000 gmap-1.4.4/gmap/app.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 17:54:34.007920 gmap-1.4.4/gmap.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      150 2023-04-07 17:54:33.000000 gmap-1.4.4/gmap.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      224 2023-04-07 17:54:34.000000 gmap-1.4.4/gmap.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 17:54:33.000000 gmap-1.4.4/gmap.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 17:54:33.000000 gmap-1.4.4/gmap.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        9 2023-04-07 17:54:33.000000 gmap-1.4.4/gmap.egg-info/requires.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 17:54:33.000000 gmap-1.4.4/gmap.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 17:54:34.008351 gmap-1.4.4/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      394 2023-04-07 17:54:31.000000 gmap-1.4.4/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.173755 gmap-1.4.6/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:29:59.173591 gmap-1.4.6/PKG-INFO
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.171845 gmap-1.4.6/gmap/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.4.6/gmap/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.4.6/gmap/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1360 2023-04-07 18:29:24.000000 gmap-1.4.6/gmap/app.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.173347 gmap-1.4.6/gmap.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      197 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:29:59.173794 gmap-1.4.6/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      341 2023-04-07 18:28:43.000000 gmap-1.4.6/setup.py
```

### Comparing `gmap-1.4.4/gmap/app.py` & `gmap-1.4.6/gmap/app.py`

 * *Files identical despite different names*

