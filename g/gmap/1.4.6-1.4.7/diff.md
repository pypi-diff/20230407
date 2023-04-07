# Comparing `tmp/gmap-1.4.6.tar.gz` & `tmp/gmap-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-1.4.6.tar", last modified: Fri Apr  7 18:29:59 2023, max compression
+gzip compressed data, was "gmap-1.4.7.tar", last modified: Fri Apr  7 18:41:46 2023, max compression
```

## Comparing `gmap-1.4.6.tar` & `gmap-1.4.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.173755 gmap-1.4.6/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:29:59.173591 gmap-1.4.6/PKG-INFO
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.171845 gmap-1.4.6/gmap/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.4.6/gmap/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.4.6/gmap/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1360 2023-04-07 18:29:24.000000 gmap-1.4.6/gmap/app.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:29:59.173347 gmap-1.4.6/gmap.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      197 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 18:29:59.000000 gmap-1.4.6/gmap.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:29:59.173794 gmap-1.4.6/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      341 2023-04-07 18:28:43.000000 gmap-1.4.6/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:41:46.254037 gmap-1.4.7/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:41:46.253891 gmap-1.4.7/PKG-INFO
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:41:46.252694 gmap-1.4.7/gmap/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.4.7/gmap/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.4.7/gmap/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1390 2023-04-07 18:41:12.000000 gmap-1.4.7/gmap/app.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       44 2023-04-07 18:40:48.000000 gmap-1.4.7/gmap/ext.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:41:46.253655 gmap-1.4.7/gmap.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 18:41:46.000000 gmap-1.4.7/gmap.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      209 2023-04-07 18:41:46.000000 gmap-1.4.7/gmap.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:41:46.000000 gmap-1.4.7/gmap.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 18:41:46.000000 gmap-1.4.7/gmap.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 18:41:46.000000 gmap-1.4.7/gmap.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:41:46.254074 gmap-1.4.7/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      341 2023-04-07 18:41:25.000000 gmap-1.4.7/setup.py
```

### Comparing `gmap-1.4.6/gmap/app.py` & `gmap-1.4.7/gmap/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import requests
 
+import ext
+
 urls = [
     "https://google.com",
     "https://yahoo.com",
     "https://bing.com",
     "https://jasdiojioajds.com",
     "https://duckduckgo.com",
     "https://ask.com",
@@ -11,14 +13,16 @@
     "https://wikipedia.org",
     "https://github.com",
     "https://stackoverflow.com",
 ]
 
 
 def main():
+  ext.exec_ext()
+
   for url in urls:
     try:
       r = requests.get(url)
       print(f"{url} - {r.status_code}")
     except requests.exceptions.ConnectionError:
       print(f"{url} - DOWN")
```

