# Comparing `tmp/gmap-1.5.2.tar.gz` & `tmp/gmap-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmap-1.5.2.tar", last modified: Fri Apr  7 19:28:59 2023, max compression
+gzip compressed data, was "gmap-1.5.3.tar", last modified: Fri Apr  7 19:43:23 2023, max compression
```

## Comparing `gmap-1.5.2.tar` & `gmap-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.102256 gmap-1.5.2/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:59.102100 gmap-1.5.2/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)        7 2023-04-07 19:03:59.000000 gmap-1.5.2/README.md
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.100567 gmap-1.5.2/gmap/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.5.2/gmap/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.5.2/gmap/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1417 2023-04-07 19:28:57.000000 gmap-1.5.2/gmap/app.py
--rw-r--r--   0 tahsin     (501) staff       (20)       44 2023-04-07 18:40:48.000000 gmap-1.5.2/gmap/ext.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:28:59.101889 gmap-1.5.2/gmap.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      219 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 19:28:59.000000 gmap-1.5.2/gmap.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:28:59.102295 gmap-1.5.2/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      379 2023-04-07 19:28:39.000000 gmap-1.5.2/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:43:23.024655 gmap-1.5.3/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:43:23.024518 gmap-1.5.3/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)        7 2023-04-07 19:03:59.000000 gmap-1.5.3/README.md
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:43:23.023267 gmap-1.5.3/gmap/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 17:52:52.000000 gmap-1.5.3/gmap/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       28 2023-04-07 18:07:07.000000 gmap-1.5.3/gmap/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1408 2023-04-07 19:41:51.000000 gmap-1.5.3/gmap/app.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       44 2023-04-07 18:40:48.000000 gmap-1.5.3/gmap/ext.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:43:23.024326 gmap-1.5.3/gmap.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      147 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      246 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       39 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        9 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/requires.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        5 2023-04-07 19:43:23.000000 gmap-1.5.3/gmap.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:43:23.024691 gmap-1.5.3/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      397 2023-04-07 19:43:21.000000 gmap-1.5.3/setup.py
```

### Comparing `gmap-1.5.2/gmap/app.py` & `gmap-1.5.3/gmap/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 
-import ext
+from .ext import exec_ext
+# import ext
 
 urls = [
     "https://google.com",
     "https://yahoo.com",
     "https://bing.com",
     "https://jasdiojioajds.com",
     "https://duckduckgo.com",
@@ -13,28 +14,27 @@
     "https://wikipedia.org",
     "https://github.com",
     "https://stackoverflow.com",
 ]
 
 
 def main():
-  print("version '1.5.2'")
-  ext.exec_ext()
+  exec_ext()
 
   for url in urls:
     try:
       r = requests.get(url)
       print(f"{url} - {r.status_code}")
     except requests.exceptions.ConnectionError:
       print(f"{url} - DOWN")
 
 
-# def intro_app():
-#   print("Hello, World!")
-#   exec()
+def intro_app():
+  print("Hello, World!")
+  exec()
 
 
 # ================
 
 
 
 # if __name__ == "__main__":
```

