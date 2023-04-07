# Comparing `tmp/wrds2pg-1.0.8.tar.gz` & `tmp/wrds2pg-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrds2pg-1.0.8.tar", last modified: Wed Jul 14 16:15:34 2021, max compression
+gzip compressed data, was "wrds2pg-1.0.9.tar", last modified: Thu Jul 22 13:53:37 2021, max compression
```

## Comparing `wrds2pg-1.0.8.tar` & `wrds2pg-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2021-07-14 16:15:34.176353 wrds2pg-1.0.8/
--rw-r--r--   0 iangow     (501) staff       (20)     1073 2021-06-18 12:49:59.000000 wrds2pg-1.0.8/LICENCE
--rw-r--r--   0 iangow     (501) staff       (20)     4843 2021-07-14 16:15:34.176222 wrds2pg-1.0.8/PKG-INFO
--rw-r--r--   0 iangow     (501) staff       (20)     4374 2021-06-18 12:49:59.000000 wrds2pg-1.0.8/README.md
--rw-r--r--   0 iangow     (501) staff       (20)       38 2021-07-14 16:15:34.176406 wrds2pg-1.0.8/setup.cfg
--rw-r--r--   0 iangow     (501) staff       (20)      745 2021-07-14 16:09:44.000000 wrds2pg-1.0.8/setup.py
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2021-07-14 16:15:34.175198 wrds2pg-1.0.8/wrds2pg/
--rw-r--r--   0 iangow     (501) staff       (20)      233 2021-06-18 12:49:59.000000 wrds2pg-1.0.8/wrds2pg/__init__.py
--rw-r--r--   0 iangow     (501) staff       (20)    18679 2021-07-14 16:09:44.000000 wrds2pg-1.0.8/wrds2pg/wrds2pg.py
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2021-07-14 16:15:34.176081 wrds2pg-1.0.8/wrds2pg.egg-info/
--rw-r--r--   0 iangow     (501) staff       (20)     4843 2021-07-14 16:15:34.000000 wrds2pg-1.0.8/wrds2pg.egg-info/PKG-INFO
--rw-r--r--   0 iangow     (501) staff       (20)      219 2021-07-14 16:15:34.000000 wrds2pg-1.0.8/wrds2pg.egg-info/SOURCES.txt
--rw-r--r--   0 iangow     (501) staff       (20)        1 2021-07-14 16:15:34.000000 wrds2pg-1.0.8/wrds2pg.egg-info/dependency_links.txt
--rw-r--r--   0 iangow     (501) staff       (20)       36 2021-07-14 16:15:34.000000 wrds2pg-1.0.8/wrds2pg.egg-info/requires.txt
--rw-r--r--   0 iangow     (501) staff       (20)        8 2021-07-14 16:15:34.000000 wrds2pg-1.0.8/wrds2pg.egg-info/top_level.txt
+drwxr-xr-x   0 igow      (1000) igow      (1000)        0 2021-07-22 13:53:37.725203 wrds2pg-1.0.9/
+-rw-r--r--   0 igow      (1000) igow      (1000)     1073 2020-04-29 19:50:05.000000 wrds2pg-1.0.9/LICENCE
+-rw-r--r--   0 igow      (1000) igow      (1000)     4843 2021-07-22 13:53:37.725203 wrds2pg-1.0.9/PKG-INFO
+-rw-r--r--   0 igow      (1000) igow      (1000)     4374 2021-07-22 13:50:44.000000 wrds2pg-1.0.9/README.md
+-rw-r--r--   0 igow      (1000) igow      (1000)       38 2021-07-22 13:53:37.725203 wrds2pg-1.0.9/setup.cfg
+-rw-r--r--   0 igow      (1000) igow      (1000)      745 2021-07-22 13:51:32.000000 wrds2pg-1.0.9/setup.py
+drwxr-xr-x   0 igow      (1000) igow      (1000)        0 2021-07-22 13:53:37.725203 wrds2pg-1.0.9/wrds2pg/
+-rw-r--r--   0 igow      (1000) igow      (1000)      233 2020-12-08 21:03:04.000000 wrds2pg-1.0.9/wrds2pg/__init__.py
+-rw-r--r--   0 igow      (1000) igow      (1000)    18678 2021-07-22 13:51:20.000000 wrds2pg-1.0.9/wrds2pg/wrds2pg.py
+drwxr-xr-x   0 igow      (1000) igow      (1000)        0 2021-07-22 13:53:37.725203 wrds2pg-1.0.9/wrds2pg.egg-info/
+-rw-r--r--   0 igow      (1000) igow      (1000)     4843 2021-07-22 13:53:37.000000 wrds2pg-1.0.9/wrds2pg.egg-info/PKG-INFO
+-rw-r--r--   0 igow      (1000) igow      (1000)      219 2021-07-22 13:53:37.000000 wrds2pg-1.0.9/wrds2pg.egg-info/SOURCES.txt
+-rw-r--r--   0 igow      (1000) igow      (1000)        1 2021-07-22 13:53:37.000000 wrds2pg-1.0.9/wrds2pg.egg-info/dependency_links.txt
+-rw-r--r--   0 igow      (1000) igow      (1000)       36 2021-07-22 13:53:37.000000 wrds2pg-1.0.9/wrds2pg.egg-info/requires.txt
+-rw-r--r--   0 igow      (1000) igow      (1000)        8 2021-07-22 13:53:37.000000 wrds2pg-1.0.9/wrds2pg.egg-info/top_level.txt
```

### Comparing `wrds2pg-1.0.8/LICENCE` & `wrds2pg-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `wrds2pg-1.0.8/PKG-INFO` & `wrds2pg-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrds2pg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Import WRDS tables or SAS data into PostgreSQL.
 Home-page: https://github.com/iangow/wrds2pg/
 Author: Ian Gow
 Author-email: iandgow@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wrds2pg-1.0.8/README.md` & `wrds2pg-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wrds2pg-1.0.8/setup.py` & `wrds2pg-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
     print(long_description)
 
 setuptools.setup(
     name="wrds2pg",
-    version="1.0.8",
+    version="1.0.9",
     author="Ian Gow",
     author_email="iandgow@gmail.com",
     description="Import WRDS tables or SAS data into PostgreSQL.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iangow/wrds2pg/",
     packages=setuptools.find_packages(),
```

### Comparing `wrds2pg-1.0.8/wrds2pg/wrds2pg.py` & `wrds2pg-1.0.9/wrds2pg/wrds2pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
     finally:
         connection.close()
         p.close()
     return True
 
 def wrds_update(table_name, schema, host=os.getenv("PGHOST"), dbname=os.getenv("PGDATABASE"), engine=None, 
         wrds_id=os.getenv("WRDS_ID"), rpath=None, fpath=None, force=False, fix_missing=False, fix_cr=False, drop="", keep="", 
-        obs="", rename="", alt_table_name=None, encoding=None, col_types=None, create_roles=False):
+        obs="", rename="", alt_table_name=None, encoding=None, col_types=None, create_roles=True):
           
     if not alt_table_name:
         alt_table_name = table_name
           
     if rpath:
         force = True
```

### Comparing `wrds2pg-1.0.8/wrds2pg.egg-info/PKG-INFO` & `wrds2pg-1.0.9/wrds2pg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrds2pg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Import WRDS tables or SAS data into PostgreSQL.
 Home-page: https://github.com/iangow/wrds2pg/
 Author: Ian Gow
 Author-email: iandgow@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

