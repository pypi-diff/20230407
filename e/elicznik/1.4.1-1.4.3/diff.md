# Comparing `tmp/elicznik-1.4.1.tar.gz` & `tmp/elicznik-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elicznik-1.4.1.tar", last modified: Fri Apr  7 19:05:44 2023, max compression
+gzip compressed data, was "elicznik-1.4.3.tar", last modified: Fri Apr  7 19:30:19 2023, max compression
```

## Comparing `elicznik-1.4.1.tar` & `elicznik-1.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1074 2021-11-24 19:41:45.000000 elicznik-1.4.1/LICENSE
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 19:05:44.468745 elicznik-1.4.1/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     3669 2023-01-10 20:18:36.000000 elicznik-1.4.1/README.md
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       74 2023-04-07 19:05:44.468745 elicznik-1.4.1/setup.cfg
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1158 2023-04-07 19:05:20.000000 elicznik-1.4.1/setup.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.464744 elicznik-1.4.1/src/
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/src/elicznik/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       31 2021-11-24 20:04:08.000000 elicznik-1.4.1/src/elicznik/__init__.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     2028 2022-05-29 13:13:33.000000 elicznik-1.4.1/src/elicznik/__main__.py
--rwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)     2213 2023-04-07 18:07:04.000000 elicznik-1.4.1/src/elicznik/elicznik.py
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      774 2021-11-24 20:12:12.000000 elicznik-1.4.1/src/elicznik/session.py
-drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:05:44.468745 elicznik-1.4.1/src/elicznik.egg-info/
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4377 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/PKG-INFO
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      353 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/SOURCES.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        1 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/dependency_links.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       53 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/entry_points.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       18 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/requires.txt
--rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        9 2023-04-07 19:05:44.000000 elicznik-1.4.1/src/elicznik.egg-info/top_level.txt
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:30:19.727174 elicznik-1.4.3/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1074 2021-11-24 19:41:45.000000 elicznik-1.4.3/LICENSE
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4401 2023-04-07 19:30:19.727174 elicznik-1.4.3/PKG-INFO
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     3669 2023-01-10 20:18:36.000000 elicznik-1.4.3/README.md
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       74 2023-04-07 19:30:19.727174 elicznik-1.4.3/setup.cfg
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1180 2023-04-07 19:29:18.000000 elicznik-1.4.3/setup.py
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:30:19.723174 elicznik-1.4.3/src/
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:30:19.727174 elicznik-1.4.3/src/elicznik/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       31 2021-11-24 20:04:08.000000 elicznik-1.4.3/src/elicznik/__init__.py
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     1684 2023-04-07 19:17:28.000000 elicznik-1.4.3/src/elicznik/__main__.py
+-rwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)     2213 2023-04-07 19:18:13.000000 elicznik-1.4.3/src/elicznik/elicznik.py
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      774 2021-11-24 20:12:12.000000 elicznik-1.4.3/src/elicznik/session.py
+drwxrwxr-x   0 mlesniew  (1000) mlesniew  (1000)        0 2023-04-07 19:30:19.727174 elicznik-1.4.3/src/elicznik.egg-info/
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)     4401 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/PKG-INFO
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)      353 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        1 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       53 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/entry_points.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)       18 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/requires.txt
+-rw-rw-r--   0 mlesniew  (1000) mlesniew  (1000)        9 2023-04-07 19:30:19.000000 elicznik-1.4.3/src/elicznik.egg-info/top_level.txt
```

### Comparing `elicznik-1.4.1/LICENSE` & `elicznik-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.1/PKG-INFO` & `elicznik-1.4.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 1.4.1
+Version: 1.4.3
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 License: UNKNOWN
 Keywords: elicznik,tauron,scrapper
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Home Automation
+Classifier: Topic :: Internet
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tauron eLicznik Scraper
 
 This Python 3 package allows to read electric energy meter reading history from the
```

### Comparing `elicznik-1.4.1/README.md` & `elicznik-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.1/setup.py` & `elicznik-1.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='elicznik',
-    version='1.4.1',
+    version='1.4.3',
     description='Tauron eLicznik scrapper',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mlesniew/elicznik',
     author='Michał Leśniewski',
     author_email='mlesniew@gmail.com',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
+        'Environment :: Console',
         'Intended Audience :: Developers',
-        'Intended Audience :: End Users/Desktop',
-        'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3',
+        'Topic :: Home Automation',
+        'Topic :: Internet',
+        'Topic :: Utilities',
     ],
     keywords='elicznik, tauron, scrapper',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.6, <4',
     install_requires=['requests', 'tabulate'],
     entry_points={
```

### Comparing `elicznik-1.4.1/src/elicznik/__main__.py` & `elicznik-1.4.3/src/elicznik/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import argparse
 import csv
 import datetime
-import json
 import sys
 
 import tabulate
 
 from .elicznik import ELicznik
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--format",
-        choices=["raw", "table", "csv"],
+        choices=["table", "csv"],
         default="table",
         help="Specify the output format",
     )
     parser.add_argument("username", help="tauron-dystrybucja.pl user name")
     parser.add_argument("password", help="tauron-dystrybucja.pl password")
     parser.add_argument(
         "start_date",
@@ -37,32 +36,19 @@
         "in ISO8601 format.  Can be omitted to only retrieve a single "
         "day's measurements.",
     )
 
     args = parser.parse_args()
 
     with ELicznik(args.username, args.password) as elicznik:
-        if args.format == "raw":
-            print(
-                json.dumps(
-                    elicznik.get_raw_readings(
-                        args.start_date, args.end_date
-                    ),
-                    indent=4,
-                )
-            )
-            return
-
         result = elicznik.get_readings(args.start_date, args.end_date)
 
         if args.format == "table":
             print(
-                tabulate.tabulate(
-                    result, headers=["timestamp", "consumed", "produced"]
-                )
+                tabulate.tabulate(result, headers=["timestamp", "consumed", "produced"])
             )
         else:
             writer = csv.writer(sys.stdout)
             for timestamp, consumed, produced in result:
                 writer.writerow((timestamp.isoformat(), consumed, produced))
```

### Comparing `elicznik-1.4.1/src/elicznik/elicznik.py` & `elicznik-1.4.3/src/elicznik/elicznik.py`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.1/src/elicznik/session.py` & `elicznik-1.4.3/src/elicznik/session.py`

 * *Files identical despite different names*

### Comparing `elicznik-1.4.1/src/elicznik.egg-info/PKG-INFO` & `elicznik-1.4.3/src/elicznik.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: elicznik
-Version: 1.4.1
+Version: 1.4.3
 Summary: Tauron eLicznik scrapper
 Home-page: https://github.com/mlesniew/elicznik
 Author: Michał Leśniewski
 Author-email: mlesniew@gmail.com
 License: UNKNOWN
 Keywords: elicznik,tauron,scrapper
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Home Automation
+Classifier: Topic :: Internet
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tauron eLicznik Scraper
 
 This Python 3 package allows to read electric energy meter reading history from the
```

