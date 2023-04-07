# Comparing `tmp/gmap-1.5.1.tar.gz` & `tmp/gmap-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-1.5.1.tar", last modified: Fri Apr  7 19:28:16 2023, max compression
+gzip compressed data, was "gmap-1.5.2.tar", last modified: Fri Apr  7 19:28:59 2023, max compression
```

## Comparing `gmap-1.5.1.tar` & `gmap-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:16.653453 gmap-1.5.1/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:16.653273 gmap-1.5.1/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)        7 2023-04-07 19:03:59.000000 gmap-1.5.1/README.md
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:16.651296 gmap-1.5.1/gmap/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.5.1/gmap/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.5.1/gmap/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1415 2023-04-07 19:27:23.000000 gmap-1.5.1/gmap/app.py
--rw-r--r--   0 tahsin     (501) staff       (20)       44 2023-04-07 18:40:48.000000 gmap-1.5.1/gmap/ext.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:16.653051 gmap-1.5.1/gmap.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:16.000000 gmap-1.5.1/gmap.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      219 2023-04-07 19:28:16.000000 gmap-1.5.1/gmap.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:28:16.000000 gmap-1.5.1/gmap.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 19:28:16.000000 gmap-1.5.1/gmap.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 19:28:16.000000 gmap-1.5.1/gmap.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:28:16.653496 gmap-1.5.1/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      341 2023-04-07 19:28:14.000000 gmap-1.5.1/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.102256 gmap-1.5.2/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:59.102100 gmap-1.5.2/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)        7 2023-04-07 19:03:59.000000 gmap-1.5.2/README.md
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.100567 gmap-1.5.2/gmap/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.5.2/gmap/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.5.2/gmap/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1417 2023-04-07 19:28:57.000000 gmap-1.5.2/gmap/app.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       44 2023-04-07 18:40:48.000000 gmap-1.5.2/gmap/ext.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.101889 gmap-1.5.2/gmap.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      219 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:28:59.102295 gmap-1.5.2/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      379 2023-04-07 19:28:39.000000 gmap-1.5.2/setup.py
```

### Comparing `gmap-1.5.1/gmap/app.py` & `gmap-1.5.2/gmap/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "https://wikipedia.org",
     "https://github.com",
     "https://stackoverflow.com",
 ]
 
 
 def main():
-  print("version 1.5.0")
+  print("version '1.5.2'")
   ext.exec_ext()
 
   for url in urls:
     try:
       r = requests.get(url)
       print(f"{url} - {r.status_code}")
     except requests.exceptions.ConnectionError:
```

