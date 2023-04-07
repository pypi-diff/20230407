# Comparing `tmp/kizano-1.0.0.tar.gz` & `tmp/kizano-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kizano-1.0.0.tar", last modified: Tue Jul  5 03:32:04 2022, max compression
+gzip compressed data, was "kizano-1.0.1.tar", last modified: Fri Apr  7 21:53:28 2023, max compression
```

## Comparing `kizano-1.0.0.tar` & `kizano-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2022-07-05 03:32:04.356103 kizano-1.0.0/
--rw-r--r--   0 markizano  (1000) kizano    (1006)      242 2022-07-05 03:32:04.356103 kizano-1.0.0/PKG-INFO
--rw-r--r--   0 markizano  (1000) kizano    (1006)      363 2022-06-30 22:20:03.000000 kizano-1.0.0/README.md
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2022-07-05 03:32:04.356103 kizano-1.0.0/kizano.egg-info/
--rw-r--r--   0 markizano  (1000) kizano    (1006)      242 2022-07-05 03:32:04.000000 kizano-1.0.0/kizano.egg-info/PKG-INFO
--rw-r--r--   0 markizano  (1000) kizano    (1006)      221 2022-07-05 03:32:04.000000 kizano-1.0.0/kizano.egg-info/SOURCES.txt
--rw-r--r--   0 markizano  (1000) kizano    (1006)        1 2022-07-05 03:32:04.000000 kizano-1.0.0/kizano.egg-info/dependency_links.txt
--rw-r--r--   0 markizano  (1000) kizano    (1006)        7 2022-07-05 03:32:04.000000 kizano-1.0.0/kizano.egg-info/top_level.txt
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2022-07-05 03:32:04.356103 kizano-1.0.0/lib/
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2022-07-05 03:32:04.356103 kizano-1.0.0/lib/kizano/
--rw-r--r--   0 markizano  (1000) kizano    (1006)       66 2022-06-30 22:20:03.000000 kizano-1.0.0/lib/kizano/__init__.py
-drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2022-07-05 03:32:04.356103 kizano-1.0.0/lib/kizano/logger/
--rw-r--r--   0 markizano  (1000) kizano    (1006)     1863 2022-07-05 02:20:07.000000 kizano-1.0.0/lib/kizano/logger/__init__.py
--rw-r--r--   0 markizano  (1000) kizano    (1006)     3170 2022-06-30 22:20:03.000000 kizano-1.0.0/lib/kizano/utils.py
--rw-r--r--   0 markizano  (1000) kizano    (1006)      265 2022-07-05 03:32:04.364103 kizano-1.0.0/setup.cfg
--rwxr-xr-x   0 markizano  (1000) kizano    (1006)     1202 2022-06-30 22:20:03.000000 kizano-1.0.0/setup.py
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      581 2023-04-07 21:53:28.744200 kizano-1.0.1/PKG-INFO
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      363 2022-06-30 22:20:03.000000 kizano-1.0.1/README.md
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/kizano.egg-info/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      581 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/PKG-INFO
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      221 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/SOURCES.txt
+-rw-r--r--   0 markizano  (1000) kizano    (1006)        1 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/dependency_links.txt
+-rw-r--r--   0 markizano  (1000) kizano    (1006)        7 2023-04-07 21:53:28.000000 kizano-1.0.1/kizano.egg-info/top_level.txt
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/kizano/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     1502 2023-04-07 19:36:24.000000 kizano-1.0.1/lib/kizano/__init__.py
+drwxr-xr-x   0 markizano  (1000) kizano    (1006)        0 2023-04-07 21:53:28.744200 kizano-1.0.1/lib/kizano/logger/
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     1863 2022-07-05 02:20:07.000000 kizano-1.0.1/lib/kizano/logger/__init__.py
+-rw-r--r--   0 markizano  (1000) kizano    (1006)     3346 2023-04-07 19:44:54.000000 kizano-1.0.1/lib/kizano/utils.py
+-rw-r--r--   0 markizano  (1000) kizano    (1006)      313 2023-04-07 21:53:28.744200 kizano-1.0.1/setup.cfg
+-rwxr-xr-x   0 markizano  (1000) kizano    (1006)     1709 2023-04-07 21:53:23.000000 kizano-1.0.1/setup.py
```

### Comparing `kizano-1.0.0/lib/kizano/logger/__init__.py` & `kizano-1.0.1/lib/kizano/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `kizano-1.0.0/lib/kizano/utils.py` & `kizano-1.0.1/lib/kizano/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,11 +82,15 @@
         raise ValueError('\x1b[33mCould not merge\x1b[0m %s(%s) and %s(%s); Error=%s' % (type(target), target, type(obj), obj, e) )
 
     # Recursively merge dicts and set non-dict values
     for k, v in list(obj.items()):
         if k in target and isinstance(v, dict):
             target[k] = dictmerge(target[k], v)
         elif k in target and isinstance(v, (set, tuple, list)):
-            target[k] = target[k] + v
+            oldtype = type(target[k])
+            # Coerce to list so we can add the two reliably
+            target[k] = oldtype( [*target[k]] + [*v] )
+            # Convert back to its original type afterwards.
         else:
             target[k] = v
     return target
+
```

