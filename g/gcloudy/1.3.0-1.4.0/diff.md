# Comparing `tmp/gcloudy-1.3.0.tar.gz` & `tmp/gcloudy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloudy-1.3.0.tar", last modified: Wed Nov 30 22:16:51 2022, max compression
+gzip compressed data, was "gcloudy-1.4.0.tar", last modified: Fri Apr  7 20:54:17 2023, max compression
```

## Comparing `gcloudy-1.3.0.tar` & `gcloudy-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-30 22:16:51.832835 gcloudy-1.3.0/
--rw-r--r--   0 dev        (501) staff       (20)     1117 2022-02-28 20:36:10.000000 gcloudy-1.3.0/LICENSE
--rw-r--r--   0 dev        (501) staff       (20)     6233 2022-11-30 22:16:51.832976 gcloudy-1.3.0/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)     5629 2022-04-20 17:44:26.000000 gcloudy-1.3.0/README.md
--rw-r--r--   0 dev        (501) staff       (20)      151 2022-02-28 20:39:26.000000 gcloudy-1.3.0/pyproject.toml
--rw-r--r--   0 dev        (501) staff       (20)      728 2022-11-30 22:16:51.833599 gcloudy-1.3.0/setup.cfg
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-30 22:16:51.827693 gcloudy-1.3.0/src/
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-30 22:16:51.831112 gcloudy-1.3.0/src/gcloudy/
--rw-r--r--   0 dev        (501) staff       (20)     8237 2022-11-30 20:36:40.000000 gcloudy-1.3.0/src/gcloudy/GoogleCloud.py
--rw-r--r--   0 dev        (501) staff       (20)        0 2022-02-28 20:43:43.000000 gcloudy-1.3.0/src/gcloudy/__init__.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2022-11-30 22:16:51.832576 gcloudy-1.3.0/src/gcloudy.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)     6233 2022-11-30 22:16:51.000000 gcloudy-1.3.0/src/gcloudy.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      233 2022-11-30 22:16:51.000000 gcloudy-1.3.0/src/gcloudy.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2022-11-30 22:16:51.000000 gcloudy-1.3.0/src/gcloudy.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)        8 2022-11-30 22:16:51.000000 gcloudy-1.3.0/src/gcloudy.egg-info/top_level.txt
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-04-07 20:54:17.927907 gcloudy-1.4.0/
+-rw-r--r--   0 dev        (501) staff       (20)     1117 2022-02-28 20:36:10.000000 gcloudy-1.4.0/LICENSE
+-rw-r--r--   0 dev        (501) staff       (20)     6233 2023-04-07 20:54:17.928181 gcloudy-1.4.0/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)     5629 2022-04-20 17:44:26.000000 gcloudy-1.4.0/README.md
+-rw-r--r--   0 dev        (501) staff       (20)      180 2023-04-07 20:48:23.000000 gcloudy-1.4.0/pyproject.toml
+-rw-r--r--   0 dev        (501) staff       (20)      728 2023-04-07 20:54:17.929381 gcloudy-1.4.0/setup.cfg
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-04-07 20:54:17.921367 gcloudy-1.4.0/src/
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-04-07 20:54:17.925315 gcloudy-1.4.0/src/gcloudy/
+-rw-r--r--   0 dev        (501) staff       (20)     8382 2023-04-07 20:52:26.000000 gcloudy-1.4.0/src/gcloudy/GoogleCloud.py
+-rw-r--r--   0 dev        (501) staff       (20)        0 2022-02-28 20:43:43.000000 gcloudy-1.4.0/src/gcloudy/__init__.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2023-04-07 20:54:17.927301 gcloudy-1.4.0/src/gcloudy.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)     6233 2023-04-07 20:54:17.000000 gcloudy-1.4.0/src/gcloudy.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      233 2023-04-07 20:54:17.000000 gcloudy-1.4.0/src/gcloudy.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2023-04-07 20:54:17.000000 gcloudy-1.4.0/src/gcloudy.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)        8 2023-04-07 20:54:17.000000 gcloudy-1.4.0/src/gcloudy.egg-info/top_level.txt
```

### Comparing `gcloudy-1.3.0/LICENSE` & `gcloudy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloudy-1.3.0/PKG-INFO` & `gcloudy-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloudy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A wrapper for google's existing google-cloud python package that aims to make using python inside the Google Cloud framework more intuitive.
 Home-page: https://gitlab.com/tomathon/gcloudy/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/gcloudy/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gcloudy-1.3.0/README.md` & `gcloudy-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gcloudy-1.3.0/setup.cfg` & `gcloudy-1.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gcloudy
-version = 1.3.0
+version = 1.4.0
 author = tomathon
 author_email = tomathon.dev@pm.me
 description = A wrapper for google's existing google-cloud python package that aims to make using python inside the Google Cloud framework more intuitive.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/tomathon/gcloudy/
 project_urls =
```

### Comparing `gcloudy-1.3.0/src/gcloudy/GoogleCloud.py` & `gcloudy-1.4.0/src/gcloudy/GoogleCloud.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 
 
 
 
 
 class BigQuery():
     
-    def __init__(self, project_id):
+    def __init__(self, project_id, use_client = None):
         self.project_id = project_id
+        if use_client is None:
+            self.use_client = bigquery.Client()
+        else:
+            self.use_client = use_client
         
 
     def __repr__(self):
         return(f"|-----|  BigQuery connector instance  |-----|\n -- current Project ID: {self.project_id}")
 
 
     def guess_schema(self, df, bq_type_default = "STRING"):
@@ -52,15 +56,15 @@
             if to_verbose:
                 print(f"-- querying all rows from {bq_path}")
             que = f"SELECT * FROM `{bq_path}`"
         else:
             if to_verbose:
                 print(f"-- querying only top {preview_top} rows from {bq_path}")
             que = f"SELECT * FROM `{bq_path}` LIMIT {preview_top}"
-        client = bigquery.Client()
+        client = self.use_client
         ret = client.query(que).to_dataframe()
         if len(date_cols) != 0:
             for dc in date_cols:
                 ret[dc] = pd.to_datetime(ret[dc])
         if to_verbose:
             print(f"-- returned {ret.shape[0]} rows and {ret.shape[1]} columns")
         return ret
@@ -108,34 +112,34 @@
                 if to_verbose:
                     print("-- using custom user-provided schema")
                 job_config = bigquery.LoadJobConfig(
                     autodetect = False,
                     schema = use_schema,
                     write_disposition = bigquery.WriteDisposition.WRITE_TRUNCATE
                 )
-        client = bigquery.Client()
+        client = self.use_client
         load_job = client.load_table_from_dataframe(df, bq_path, job_config = job_config)
         load_job.result()
         ret = client.get_table(bq_path)
         if to_verbose:
             print(f"-- {ret.num_rows} rows have been successfully written to {bq_path}")
             
             
     def read_custom_query(self, custom_query, to_verbose = True):
-        client = bigquery.Client()
+        client = self.use_client
         ret = client.query(custom_query).to_dataframe()
         if to_verbose:
             print(f"-- returned {ret.shape[0]} rows and {ret.shape[1]} columns")
         return ret
 
 
     def send_query(self, que, to_verbose = True):
         if to_verbose:
             print("-- sending query ...")
-        client = bigquery.Client()
+        client = self.use_client
         qconf = bigquery.QueryJobConfig()
         qjob = client.query(que, job_config = qconf)
         qjob.result()
         if to_verbose:
             print("-- query complete")
```

### Comparing `gcloudy-1.3.0/src/gcloudy.egg-info/PKG-INFO` & `gcloudy-1.4.0/src/gcloudy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloudy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A wrapper for google's existing google-cloud python package that aims to make using python inside the Google Cloud framework more intuitive.
 Home-page: https://gitlab.com/tomathon/gcloudy/
 Author: tomathon
 Author-email: tomathon.dev@pm.me
 Project-URL: Bug Tracker, https://gitlab.com/tomathon/gcloudy/-/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

