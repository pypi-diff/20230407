# Comparing `tmp/elicznik-1.4.0.tar.gz` & `tmp/elicznik-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elicznik-1.4.0.tar", last modified: Fri Apr  7 17:54:58 2023, max compression
+gzip compressed data, was "elicznik-1.4.1.tar", last modified: Fri Apr  7 19:05:44 2023, max compression
```

## Comparing `elicznik-1.4.0.tar` & `elicznik-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 17:54:58.506137 elicznik-1.4.0/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1074 2021-11-24 19:41:45.000000 elicznik-1.4.0/LICENSE
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 17:54:58.506137 elicznik-1.4.0/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     3669 2023-01-10 20:18:36.000000 elicznik-1.4.0/README.md
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       74 2023-04-07 17:54:58.506137 elicznik-1.4.0/setup.cfg
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1158 2023-04-07 17:53:14.000000 elicznik-1.4.0/setup.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 17:54:58.502136 elicznik-1.4.0/src/
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 17:54:58.506137 elicznik-1.4.0/src/elicznik/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       31 2021-11-24 20:04:08.000000 elicznik-1.4.0/src/elicznik/__init__.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     2028 2022-05-29 13:13:33.000000 elicznik-1.4.0/src/elicznik/__main__.py
--rwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)     2227 2023-04-07 17:52:11.000000 elicznik-1.4.0/src/elicznik/elicznik.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      774 2021-11-24 20:12:12.000000 elicznik-1.4.0/src/elicznik/session.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 17:54:58.506137 elicznik-1.4.0/src/elicznik.egg-info/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      353 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/SOURCES.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        1 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/dependency_links.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       53 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/entry_points.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       18 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/requires.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        9 2023-04-07 17:54:58.000000 elicznik-1.4.0/src/elicznik.egg-info/top_level.txt
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1074 2021-11-24 19:41:45.000000 elicznik-1.4.1/LICENSE
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 19:05:44.468745 elicznik-1.4.1/PKG-INFO
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     3669 2023-01-10 20:18:36.000000 elicznik-1.4.1/README.md
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       74 2023-04-07 19:05:44.468745 elicznik-1.4.1/setup.cfg
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1158 2023-04-07 19:05:20.000000 elicznik-1.4.1/setup.py
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.464744 elicznik-1.4.1/src/
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/src/elicznik/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       31 2021-11-24 20:04:08.000000 elicznik-1.4.1/src/elicznik/__init__.py
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     2028 2022-05-29 13:13:33.000000 elicznik-1.4.1/src/elicznik/__main__.py
+-rwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)     2213 2023-04-07 18:07:04.000000 elicznik-1.4.1/src/elicznik/elicznik.py
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      774 2021-11-24 20:12:12.000000 elicznik-1.4.1/src/elicznik/session.py
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/src/elicznik.egg-info/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/PKG-INFO
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      353 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        1 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       53 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/entry_points.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       18 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/requires.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        9 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/top_level.txt
```

### Comparing `elicznik-1.4.0/LICENSE` & `elicznik-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.0/PKG-INFO` & `elicznik-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 1.4.0
+Version: 1.4.1
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 License: UNKNOWN
 Keywords: elicznik,tauron,scrapper
 Platform: UNKNOWN
```

### Comparing `elicznik-1.4.0/README.md` & `elicznik-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.0/setup.py` & `elicznik-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='elicznik',
-    version='1.4.0',
+    version='1.4.1',
     description='Tauron eLicznik scrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mlesniew/elicznik',
     author='Michał Leśniewski',
     author_email='mlesniew@gmail.com',
     classifiers=[
```

### Comparing `elicznik-1.4.0/src/elicznik/__main__.py` & `elicznik-1.4.1/src/elicznik/__main__.py`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.0/src/elicznik/elicznik.py` & `elicznik-1.4.1/src/elicznik/elicznik.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     def get_readings_consumption(self, start_date, end_date=None):
         return dict(self._get_raw_readings("consum", start_date, end_date))
 
     def get_readings(self, start_date, end_date=None):
         consumed = self.get_readings_consumption(start_date, end_date)
         produced = self.get_readings_production(start_date, end_date)
         return sorted(
-            (timestamp, float(consumed.get(timestamp)), float(produced.get(timestamp)))
+            (timestamp, consumed.get(timestamp), produced.get(timestamp))
             for timestamp in set(consumed) | set(produced)
         )
```

### Comparing `elicznik-1.4.0/src/elicznik/session.py` & `elicznik-1.4.1/src/elicznik/session.py`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.0/src/elicznik.egg-info/PKG-INFO` & `elicznik-1.4.1/src/elicznik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 1.4.0
+Version: 1.4.1
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 License: UNKNOWN
 Keywords: elicznik,tauron,scrapper
 Platform: UNKNOWN
```

