# Comparing `tmp/pangres-4.1.3.tar.gz` & `tmp/pangres-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangres-4.1.3.tar", last modified: Mon Feb  6 01:00:00 2023, max compression
+gzip compressed data, was "pangres-4.1.4.tar", last modified: Fri Apr  7 19:57:55 2023, max compression
```

## Comparing `pangres-4.1.3.tar` & `pangres-4.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 tibaldo   (1000) tibaldo   (1000)        0 2023-02-06 01:00:00.794152 pangres-4.1.3/
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     1211 2022-08-17 12:14:10.000000 pangres-4.1.3/LICENSE
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)       42 2022-08-17 12:14:10.000000 pangres-4.1.3/MANIFEST.in
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    10867 2023-02-06 01:00:00.794152 pangres-4.1.3/PKG-INFO
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     9907 2023-02-06 00:58:23.000000 pangres-4.1.3/README.md
-drwxrwxr-x   0 tibaldo   (1000) tibaldo   (1000)        0 2023-02-06 01:00:00.794152 pangres-4.1.3/pangres/
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)      642 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/__init__.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)       22 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/_version.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    21965 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/core.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    30344 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/engine.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     7358 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/examples.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     1729 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/exceptions.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     6648 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/executor.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     2680 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/helpers.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     2485 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/logger.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     1485 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/pangres_types.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)        0 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/py.typed
-drwxrwxr-x   0 tibaldo   (1000) tibaldo   (1000)        0 2023-02-06 01:00:00.794152 pangres-4.1.3/pangres/tests/
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)        0 2022-08-17 12:14:10.000000 pangres-4.1.3/pangres/tests/__init__.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    19508 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/conftest.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     6827 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_bad_text.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     2367 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_chunksize.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     9696 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_con_and_trans_control.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    17697 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_core.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)      442 2022-08-17 12:14:10.000000 pangres-4.1.3/pangres/tests/test_helpers.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     6965 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_index.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     2469 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_logging.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    20825 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_pandas_special_engine.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     6121 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_unique_key.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     9600 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_upsert_speed.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     3660 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_utils.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     4793 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/tests/test_yield_chunks.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     7953 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/transaction.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    11139 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/upsert_query.py
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     9311 2023-02-06 00:58:23.000000 pangres-4.1.3/pangres/utils.py
-drwxrwxr-x   0 tibaldo   (1000) tibaldo   (1000)        0 2023-02-06 01:00:00.794152 pangres-4.1.3/pangres.egg-info/
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)    10867 2023-02-06 01:00:00.000000 pangres-4.1.3/pangres.egg-info/PKG-INFO
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)      947 2023-02-06 01:00:00.000000 pangres-4.1.3/pangres.egg-info/SOURCES.txt
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)        1 2023-02-06 01:00:00.000000 pangres-4.1.3/pangres.egg-info/dependency_links.txt
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)       49 2023-02-06 01:00:00.000000 pangres-4.1.3/pangres.egg-info/requires.txt
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)        8 2023-02-06 01:00:00.000000 pangres-4.1.3/pangres.egg-info/top_level.txt
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)       49 2022-11-13 18:38:31.000000 pangres-4.1.3/requirements.txt
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)       79 2023-02-06 01:00:00.794152 pangres-4.1.3/setup.cfg
--rw-rw-r--   0 tibaldo   (1000) tibaldo   (1000)     1721 2023-02-06 00:58:23.000000 pangres-4.1.3/setup.py
+drwxrwxr-x   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2023-04-07 19:57:55.279520 pangres-4.1.4/
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     1211 2022-08-17 12:14:10.000000 pangres-4.1.4/LICENSE
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)       42 2022-08-17 12:14:10.000000 pangres-4.1.4/MANIFEST.in
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    10867 2023-04-07 19:57:55.279520 pangres-4.1.4/PKG-INFO
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     9907 2023-04-07 19:16:40.000000 pangres-4.1.4/README.md
+drwxrwxr-x   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2023-04-07 19:57:55.275520 pangres-4.1.4/pangres/
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)      642 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/__init__.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)       22 2023-04-07 19:47:46.000000 pangres-4.1.4/pangres/_version.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    21965 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/core.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    30337 2023-04-07 19:34:15.000000 pangres-4.1.4/pangres/engine.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     7358 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/examples.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     1729 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/exceptions.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     6648 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/executor.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     2680 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/helpers.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     2485 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/logger.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     1485 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/pangres_types.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/py.typed
+drwxrwxr-x   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2023-04-07 19:57:55.279520 pangres-4.1.4/pangres/tests/
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2022-08-17 12:14:10.000000 pangres-4.1.4/pangres/tests/__init__.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    19508 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/conftest.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     6827 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_bad_text.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     2367 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_chunksize.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    10088 2023-04-07 19:52:03.000000 pangres-4.1.4/pangres/tests/test_con_and_trans_control.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    17697 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_core.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)      442 2022-08-17 12:14:10.000000 pangres-4.1.4/pangres/tests/test_helpers.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     6965 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_index.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     2469 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_logging.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    20825 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_pandas_special_engine.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     6121 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_unique_key.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     9600 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_upsert_speed.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     3660 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_utils.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     4793 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/tests/test_yield_chunks.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     7953 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/transaction.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    11139 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/upsert_query.py
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     9311 2023-04-07 19:16:40.000000 pangres-4.1.4/pangres/utils.py
+drwxrwxr-x   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        0 2023-04-07 19:57:55.275520 pangres-4.1.4/pangres.egg-info/
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)    10867 2023-04-07 19:57:55.000000 pangres-4.1.4/pangres.egg-info/PKG-INFO
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)      947 2023-04-07 19:57:55.000000 pangres-4.1.4/pangres.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        1 2023-04-07 19:57:55.000000 pangres-4.1.4/pangres.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)       49 2023-04-07 19:57:55.000000 pangres-4.1.4/pangres.egg-info/requires.txt
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)        8 2023-04-07 19:57:55.000000 pangres-4.1.4/pangres.egg-info/top_level.txt
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)       49 2023-04-07 19:16:30.000000 pangres-4.1.4/requirements.txt
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)       79 2023-04-07 19:57:55.279520 pangres-4.1.4/setup.cfg
+-rw-rw-r--   0 thibaultbetremieux  (1000) thibaultbetremieux  (1000)     1721 2023-04-07 19:47:30.000000 pangres-4.1.4/setup.py
```

### Comparing `pangres-4.1.3/LICENSE` & `pangres-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/PKG-INFO` & `pangres-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pangres
-Version: 4.1.3
+Version: 4.1.4
 Summary: Postgres insert update with pandas DataFrames.
 Home-page: https://github.com/ThibTrip/pangres
-Download-URL: https://github.com/ThibTrip/pangres/archive/v4.1.3.tar.gz
+Download-URL: https://github.com/ThibTrip/pangres/archive/v4.1.4.tar.gz
 Author: Thibault Bétrémieux
 Author-email: thibault.betremieux@gmail.com
 License: The Unlicense
 Keywords: pandas,postgres,mysql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pangres-4.1.3/README.md` & `pangres-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/__init__.py` & `pangres-4.1.4/pangres/__init__.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/core.py` & `pangres-4.1.4/pangres/core.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/engine.py` & `pangres-4.1.4/pangres/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
         # merge with dtype from user
         new_dtype = {c: JSON for c in json_cols}
         if dtype is not None:
             new_dtype.update(dtype)
 
         # create sqlalchemy table model via pandas
-        pandas_sql_engine = pd.io.sql.SQLDatabase(engine=connection, schema=schema)  # type: ignore  # .sql does exist
+        pandas_sql_engine = pd.io.sql.SQLDatabase(connection, schema=schema)  # type: ignore  # .sql does exist
         pandas_table = pd.io.sql.SQLTable(name=table_name,  # type: ignore  # .sql does exist
                                           pandas_sql_engine=pandas_sql_engine,
                                           frame=df,
                                           dtype=None if new_dtype == {} else new_dtype)  # type: ignore
 
         # turn pandas table into a pure sqlalchemy table
         # inspired from https://github.com/pandas-dev/pandas/blob/main/pandas/io/sql.py#L815-L821
```

### Comparing `pangres-4.1.3/pangres/examples.py` & `pangres-4.1.4/pangres/examples.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/exceptions.py` & `pangres-4.1.4/pangres/exceptions.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/executor.py` & `pangres-4.1.4/pangres/executor.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/helpers.py` & `pangres-4.1.4/pangres/helpers.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/logger.py` & `pangres-4.1.4/pangres/logger.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/pangres_types.py` & `pangres-4.1.4/pangres/pangres_types.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/conftest.py` & `pangres-4.1.4/pangres/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_bad_text.py` & `pangres-4.1.4/pangres/tests/test_bad_text.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_chunksize.py` & `pangres-4.1.4/pangres/tests/test_chunksize.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_con_and_trans_control.py` & `pangres-4.1.4/pangres/tests/test_con_and_trans_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,16 +79,18 @@
 
     # if trans_op=='commit': make sure we have "bar" and "foo" in the index
     # elif trans_op=='rollback': make sure we don't have any data
     # or that the table was not even created (what is rolled back
     # depends on the database type and other factors)
     if trans_op == 'commit':
         df_db = select_table(engine=engine, schema=schema, table_name=table_name, index_col='ix')
-        pd.testing.assert_frame_equal(df_db.sort_index(),
-                                      pd.DataFrame(index=pd.Index(['bar', 'foo'], name='ix')))
+        # this simple check will be enough since we do not have values, only an index
+        assert df_db.index.sort_values().tolist() == ['bar', 'foo']
+        assert df_db.index.name == 'ix'
+
     elif trans_op == 'rollback':
         df_db = select_table(engine=engine, schema=schema, table_name=table_name, error_if_missing=False)
         # no table or an empty table
         assert df_db is None or len(df_db) == 0
 
 
 @adrop_table_between_tests(table_name=TableNames.COMMIT_OR_ROLLBACK_TRANS)
@@ -113,16 +115,18 @@
 
     # if trans_op=='commit': make sure we have "bar" and "foo" in the index
     # elif trans_op=='rollback': make sure we don't have any data
     # or that the table was not even created (what is rolled back
     # depends on the database type and other factors)
     if trans_op == 'commit':
         df_db = await aselect_table(engine=engine, schema=schema, table_name=table_name, index_col='ix')
-        pd.testing.assert_frame_equal(df_db.sort_index(),
-                                      pd.DataFrame(index=pd.Index(['bar', 'foo'], name='ix')))
+        # this simple check will be enough since we do not have values, only an index
+        assert df_db.index.sort_values().tolist() == ['bar', 'foo']
+        assert df_db.index.name == 'ix'
+
     elif trans_op == 'rollback':
         df_db = await aselect_table(engine=engine, schema=schema, table_name=table_name, error_if_missing=False)
         # no table or an empty table
         assert df_db is None or len(df_db) == 0
 
 
 # -
@@ -153,15 +157,17 @@
         # do some other operation that requires commit and then rollback
         upsert(con=connection, df=df.rename(index={'foo': 'bar'}), **common_kwargs)
         connection.rollback()
 
     # the table in the db should be equal to the initial df as the second
     # operation was rolled back
     df_db = select_table(engine=engine, schema=schema, table_name=table_name, index_col='ix')
-    pd.testing.assert_frame_equal(df_db, df)
+    # this simple check will be enough since we do not have values, only an index
+    assert df_db.index.sort_values().tolist() == df.index.sort_values().tolist()
+    assert df_db.index.name == 'ix'
 
 
 @adrop_table_between_tests(table_name=TableNames.COMMIT_AS_YOU_GO)
 async def run_test_commit_as_you_go_async(engine, schema):
     df = pd.DataFrame(index=pd.Index(['foo'], name='ix'))
     table_name = TableNames.COMMIT_AS_YOU_GO
     # common keyword arguments for multiple upsert operations below
@@ -176,15 +182,17 @@
         # do some other operation that requires commit and then rollback
         await aupsert(con=connection, df=df.rename(index={'foo': 'bar'}), **common_kwargs)
         await connection.rollback()
 
     # the table in the db should be equal to the initial df as the second
     # operation was rolled back
     df_db = await aselect_table(engine=engine, schema=schema, table_name=table_name, index_col='ix')
-    pd.testing.assert_frame_equal(df_db, df)
+    # this simple check will be enough since we do not have values, only an index
+    assert df_db.index.sort_values().tolist() == df.index.sort_values().tolist()
+    assert df_db.index.name == 'ix'
 
 
 # -
 
 # ## Errors
 
 # +
```

### Comparing `pangres-4.1.3/pangres/tests/test_core.py` & `pangres-4.1.4/pangres/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_index.py` & `pangres-4.1.4/pangres/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_logging.py` & `pangres-4.1.4/pangres/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_pandas_special_engine.py` & `pangres-4.1.4/pangres/tests/test_pandas_special_engine.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_unique_key.py` & `pangres-4.1.4/pangres/tests/test_unique_key.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_upsert_speed.py` & `pangres-4.1.4/pangres/tests/test_upsert_speed.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_utils.py` & `pangres-4.1.4/pangres/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/tests/test_yield_chunks.py` & `pangres-4.1.4/pangres/tests/test_yield_chunks.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/transaction.py` & `pangres-4.1.4/pangres/transaction.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/upsert_query.py` & `pangres-4.1.4/pangres/upsert_query.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres/utils.py` & `pangres-4.1.4/pangres/utils.py`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/pangres.egg-info/PKG-INFO` & `pangres-4.1.4/pangres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pangres
-Version: 4.1.3
+Version: 4.1.4
 Summary: Postgres insert update with pandas DataFrames.
 Home-page: https://github.com/ThibTrip/pangres
-Download-URL: https://github.com/ThibTrip/pangres/archive/v4.1.3.tar.gz
+Download-URL: https://github.com/ThibTrip/pangres/archive/v4.1.4.tar.gz
 Author: Thibault Bétrémieux
 Author-email: thibault.betremieux@gmail.com
 License: The Unlicense
 Keywords: pandas,postgres,mysql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pangres-4.1.3/pangres.egg-info/SOURCES.txt` & `pangres-4.1.4/pangres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangres-4.1.3/setup.py` & `pangres-4.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 with open(os.path.join(here, "requirements.txt"), "r") as f:
     requirements = [line.strip() for line in f.readlines()]
 
 
 setuptools.setup(
     name="pangres",
-    version="4.1.3",
+    version="4.1.4",
     license='The Unlicense',
     author="Thibault Bétrémieux",
     author_email="thibault.betremieux@gmail.com",
     url='https://github.com/ThibTrip/pangres',
-    download_url='https://github.com/ThibTrip/pangres/archive/v4.1.3.tar.gz',
+    download_url='https://github.com/ThibTrip/pangres/archive/v4.1.4.tar.gz',
     keywords=['pandas', 'postgres', 'mysql', 'sqlite'],
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     package_data={"pangres": ["py.typed"]},
```

