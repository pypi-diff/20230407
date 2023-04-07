# Comparing `tmp/data_algebra-1.6.6.tar.gz` & `tmp/data_algebra-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_algebra-1.6.6.tar", last modified: Wed Apr  5 01:21:12 2023, max compression
+gzip compressed data, was "data_algebra-1.6.7.tar", last modified: Fri Apr  7 18:24:39 2023, max compression
```

## Comparing `data_algebra-1.6.6.tar` & `data_algebra-1.6.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-05 01:21:12.473884 data_algebra-1.6.6/
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2021-07-26 14:53:15.000000 data_algebra-1.6.6/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)     1830 2023-04-05 01:21:12.473511 data_algebra-1.6.6/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)    23587 2023-02-27 23:31:03.000000 data_algebra-1.6.6/README.md
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-05 01:21:12.470173 data_algebra-1.6.6/data_algebra/
--rw-r--r--   0 johnmount   (501) staff       (20)     9242 2022-12-17 20:59:22.000000 data_algebra-1.6.6/data_algebra/BigQuery.py
--rw-r--r--   0 johnmount   (501) staff       (20)     2683 2022-10-26 22:07:28.000000 data_algebra-1.6.6/data_algebra/MySQL.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3939 2022-10-26 22:07:28.000000 data_algebra-1.6.6/data_algebra/OrderedSet.py
--rw-r--r--   0 johnmount   (501) staff       (20)     2190 2022-10-26 22:07:28.000000 data_algebra-1.6.6/data_algebra/PostgreSQL.py
--rw-r--r--   0 johnmount   (501) staff       (20)    17357 2022-12-04 01:59:41.000000 data_algebra-1.6.6/data_algebra/SQLite.py
--rw-r--r--   0 johnmount   (501) staff       (20)     6895 2023-01-08 20:54:32.000000 data_algebra-1.6.6/data_algebra/SparkSQL.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1122 2023-01-18 01:39:46.000000 data_algebra-1.6.6/data_algebra/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)     6468 2023-01-14 19:51:34.000000 data_algebra-1.6.6/data_algebra/arrow.py
--rw-r--r--   0 johnmount   (501) staff       (20)    29824 2023-01-14 19:52:01.000000 data_algebra-1.6.6/data_algebra/cdata.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1905 2022-01-27 17:07:38.000000 data_algebra-1.6.6/data_algebra/connected_components.py
--rw-r--r--   0 johnmount   (501) staff       (20)     5125 2022-12-31 03:58:02.000000 data_algebra-1.6.6/data_algebra/data_model.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3660 2022-12-17 20:59:22.000000 data_algebra-1.6.6/data_algebra/data_model_space.py
--rw-r--r--   0 johnmount   (501) staff       (20)   109781 2023-01-15 15:30:41.000000 data_algebra-1.6.6/data_algebra/data_ops.py
--rw-r--r--   0 johnmount   (501) staff       (20)    10229 2023-01-12 20:31:50.000000 data_algebra-1.6.6/data_algebra/data_ops_types.py
--rw-r--r--   0 johnmount   (501) staff       (20)     2001 2022-12-09 14:25:28.000000 data_algebra-1.6.6/data_algebra/data_ops_utils.py
--rw-r--r--   0 johnmount   (501) staff       (20)     2081 2023-01-14 23:12:17.000000 data_algebra-1.6.6/data_algebra/data_space.py
--rw-r--r--   0 johnmount   (501) staff       (20)    89431 2023-01-14 19:49:43.000000 data_algebra-1.6.6/data_algebra/db_model.py
--rw-r--r--   0 johnmount   (501) staff       (20)     4820 2022-12-07 00:36:58.000000 data_algebra-1.6.6/data_algebra/db_space.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3189 2022-12-17 20:59:22.000000 data_algebra-1.6.6/data_algebra/eval_cache.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1751 2022-12-09 14:25:28.000000 data_algebra-1.6.6/data_algebra/expr_parse.py
--rw-r--r--   0 johnmount   (501) staff       (20)    41735 2023-01-14 17:28:17.000000 data_algebra-1.6.6/data_algebra/expr_rep.py
--rw-r--r--   0 johnmount   (501) staff       (20)      993 2022-12-21 21:40:26.000000 data_algebra-1.6.6/data_algebra/expression_walker.py
--rw-r--r--   0 johnmount   (501) staff       (20)      828 2022-01-27 17:07:38.000000 data_algebra-1.6.6/data_algebra/flow_text.py
--rw-r--r--   0 johnmount   (501) staff       (20)    19693 2022-10-27 03:02:30.000000 data_algebra-1.6.6/data_algebra/near_sql.py
--rw-r--r--   0 johnmount   (501) staff       (20)    23884 2022-12-17 20:59:22.000000 data_algebra-1.6.6/data_algebra/op_catalog.py
--rw-r--r--   0 johnmount   (501) staff       (20)    52003 2023-04-05 01:00:02.000000 data_algebra-1.6.6/data_algebra/pandas_base.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1140 2022-12-19 15:18:51.000000 data_algebra-1.6.6/data_algebra/pandas_model.py
--rw-r--r--   0 johnmount   (501) staff       (20)    11773 2022-12-09 14:25:28.000000 data_algebra-1.6.6/data_algebra/parse_by_lark.py
--rw-r--r--   0 johnmount   (501) staff       (20)    48407 2023-04-04 22:17:27.000000 data_algebra-1.6.6/data_algebra/polars_model.py
--rw-r--r--   0 johnmount   (501) staff       (20)     7997 2022-10-26 22:07:28.000000 data_algebra-1.6.6/data_algebra/python3_lark.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1493 2023-01-14 20:40:11.000000 data_algebra-1.6.6/data_algebra/shift_pipe_action.py
--rw-r--r--   0 johnmount   (501) staff       (20)    20989 2023-01-07 17:30:55.000000 data_algebra-1.6.6/data_algebra/solutions.py
--rw-r--r--   0 johnmount   (501) staff       (20)     2887 2023-01-11 06:35:53.000000 data_algebra-1.6.6/data_algebra/sql_format_options.py
--rw-r--r--   0 johnmount   (501) staff       (20)    25058 2023-01-15 02:13:29.000000 data_algebra-1.6.6/data_algebra/test_util.py
--rw-r--r--   0 johnmount   (501) staff       (20)     7442 2022-12-18 02:13:01.000000 data_algebra-1.6.6/data_algebra/util.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-05 01:21:12.472932 data_algebra-1.6.6/data_algebra.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)     1830 2023-04-05 01:21:11.000000 data_algebra-1.6.6/data_algebra.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)     1162 2023-04-05 01:21:11.000000 data_algebra-1.6.6/data_algebra.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-05 01:21:11.000000 data_algebra-1.6.6/data_algebra.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)      332 2023-04-05 01:21:11.000000 data_algebra-1.6.6/data_algebra.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       13 2023-04-05 01:21:11.000000 data_algebra-1.6.6/data_algebra.egg-info/top_level.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-05 01:21:12.473976 data_algebra-1.6.6/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     2651 2023-01-18 01:39:39.000000 data_algebra-1.6.6/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:24:39.987996 data_algebra-1.6.7/
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2021-07-26 14:53:15.000000 data_algebra-1.6.7/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)     1830 2023-04-07 18:24:39.987747 data_algebra-1.6.7/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)    23587 2023-02-27 23:31:03.000000 data_algebra-1.6.7/README.md
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:24:39.985937 data_algebra-1.6.7/data_algebra/
+-rw-r--r--   0 johnmount   (501) staff       (20)     9242 2022-12-17 20:59:22.000000 data_algebra-1.6.7/data_algebra/BigQuery.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     2683 2022-10-26 22:07:28.000000 data_algebra-1.6.7/data_algebra/MySQL.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3939 2022-10-26 22:07:28.000000 data_algebra-1.6.7/data_algebra/OrderedSet.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     2190 2022-10-26 22:07:28.000000 data_algebra-1.6.7/data_algebra/PostgreSQL.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    17357 2022-12-04 01:59:41.000000 data_algebra-1.6.7/data_algebra/SQLite.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     6895 2023-01-08 20:54:32.000000 data_algebra-1.6.7/data_algebra/SparkSQL.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1122 2023-04-05 01:23:18.000000 data_algebra-1.6.7/data_algebra/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     6468 2023-01-14 19:51:34.000000 data_algebra-1.6.7/data_algebra/arrow.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    29824 2023-01-14 19:52:01.000000 data_algebra-1.6.7/data_algebra/cdata.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1905 2022-01-27 17:07:38.000000 data_algebra-1.6.7/data_algebra/connected_components.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     5125 2022-12-31 03:58:02.000000 data_algebra-1.6.7/data_algebra/data_model.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3660 2022-12-17 20:59:22.000000 data_algebra-1.6.7/data_algebra/data_model_space.py
+-rw-r--r--   0 johnmount   (501) staff       (20)   109781 2023-01-15 15:30:41.000000 data_algebra-1.6.7/data_algebra/data_ops.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    10229 2023-01-12 20:31:50.000000 data_algebra-1.6.7/data_algebra/data_ops_types.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     2001 2022-12-09 14:25:28.000000 data_algebra-1.6.7/data_algebra/data_ops_utils.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     2081 2023-01-14 23:12:17.000000 data_algebra-1.6.7/data_algebra/data_space.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    89381 2023-04-05 18:01:01.000000 data_algebra-1.6.7/data_algebra/db_model.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     4820 2022-12-07 00:36:58.000000 data_algebra-1.6.7/data_algebra/db_space.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3189 2022-12-17 20:59:22.000000 data_algebra-1.6.7/data_algebra/eval_cache.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1751 2022-12-09 14:25:28.000000 data_algebra-1.6.7/data_algebra/expr_parse.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    41735 2023-01-14 17:28:17.000000 data_algebra-1.6.7/data_algebra/expr_rep.py
+-rw-r--r--   0 johnmount   (501) staff       (20)      993 2022-12-21 21:40:26.000000 data_algebra-1.6.7/data_algebra/expression_walker.py
+-rw-r--r--   0 johnmount   (501) staff       (20)      828 2022-01-27 17:07:38.000000 data_algebra-1.6.7/data_algebra/flow_text.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    19693 2022-10-27 03:02:30.000000 data_algebra-1.6.7/data_algebra/near_sql.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    23884 2022-12-17 20:59:22.000000 data_algebra-1.6.7/data_algebra/op_catalog.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    52114 2023-04-07 17:42:07.000000 data_algebra-1.6.7/data_algebra/pandas_base.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1140 2022-12-19 15:18:51.000000 data_algebra-1.6.7/data_algebra/pandas_model.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    11773 2022-12-09 14:25:28.000000 data_algebra-1.6.7/data_algebra/parse_by_lark.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    48407 2023-04-04 22:17:27.000000 data_algebra-1.6.7/data_algebra/polars_model.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     7997 2022-10-26 22:07:28.000000 data_algebra-1.6.7/data_algebra/python3_lark.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1493 2023-01-14 20:40:11.000000 data_algebra-1.6.7/data_algebra/shift_pipe_action.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    20989 2023-01-07 17:30:55.000000 data_algebra-1.6.7/data_algebra/solutions.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     2887 2023-01-11 06:35:53.000000 data_algebra-1.6.7/data_algebra/sql_format_options.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    25058 2023-01-15 02:13:29.000000 data_algebra-1.6.7/data_algebra/test_util.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     7442 2022-12-18 02:13:01.000000 data_algebra-1.6.7/data_algebra/util.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:24:39.987388 data_algebra-1.6.7/data_algebra.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)     1830 2023-04-07 18:24:39.000000 data_algebra-1.6.7/data_algebra.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)     1162 2023-04-07 18:24:39.000000 data_algebra-1.6.7/data_algebra.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-07 18:24:39.000000 data_algebra-1.6.7/data_algebra.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)      332 2023-04-07 18:24:39.000000 data_algebra-1.6.7/data_algebra.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       13 2023-04-07 18:24:39.000000 data_algebra-1.6.7/data_algebra.egg-info/top_level.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-07 18:24:39.988067 data_algebra-1.6.7/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     2651 2023-04-05 01:23:29.000000 data_algebra-1.6.7/setup.py
```

### Comparing `data_algebra-1.6.6/LICENSE` & `data_algebra-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/PKG-INFO` & `data_algebra-1.6.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_algebra
-Version: 1.6.6
+Version: 1.6.7
 Summary: data_algebra is a data manipulation language that can both generate SQL queries and work on Pandas DataFrames.
 Home-page: https://github.com/WinVector/data_algebra
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `data_algebra-1.6.6/README.md` & `data_algebra-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/BigQuery.py` & `data_algebra-1.6.7/data_algebra/BigQuery.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/MySQL.py` & `data_algebra-1.6.7/data_algebra/MySQL.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/OrderedSet.py` & `data_algebra-1.6.7/data_algebra/OrderedSet.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/PostgreSQL.py` & `data_algebra-1.6.7/data_algebra/PostgreSQL.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/SQLite.py` & `data_algebra-1.6.7/data_algebra/SQLite.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/SparkSQL.py` & `data_algebra-1.6.7/data_algebra/SparkSQL.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/__init__.py` & `data_algebra-1.6.7/data_algebra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Package for data processing in Python: https://github.com/WinVector/data_algebra
 """
 
 __docformat__ = "restructuredtext"
-__version__ = "1.6.6"
+__version__ = "1.6.7"
 
 __doc__ = """
 `data_algebra`<https://github.com/WinVector/data_algebra> is a piped data wrangling system
 based on Codd's relational algebra and experience working with dplyr at scale.  The primary 
 purpose of the package is to support an easy to compose and maintain grammar of data processing
 steps that in turn can be used to generate database specific SQL.  The package also implements
 the same transforms for Pandas and Polars DataFrames.
```

### Comparing `data_algebra-1.6.6/data_algebra/arrow.py` & `data_algebra-1.6.7/data_algebra/arrow.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/cdata.py` & `data_algebra-1.6.7/data_algebra/cdata.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/connected_components.py` & `data_algebra-1.6.7/data_algebra/connected_components.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_model.py` & `data_algebra-1.6.7/data_algebra/data_model.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_model_space.py` & `data_algebra-1.6.7/data_algebra/data_model_space.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_ops.py` & `data_algebra-1.6.7/data_algebra/data_ops.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_ops_types.py` & `data_algebra-1.6.7/data_algebra/data_ops_types.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_ops_utils.py` & `data_algebra-1.6.7/data_algebra/data_ops_utils.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/data_space.py` & `data_algebra-1.6.7/data_algebra/data_space.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/db_model.py` & `data_algebra-1.6.7/data_algebra/db_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -855,29 +855,29 @@
         :param q: sql query
         """
         if isinstance(q, data_algebra.data_ops.ViewRepresentation):
             q = q.to_sql(db_model=self)
         else:
             q = str(q)
         assert isinstance(q, str)
-        data_algebra.data_model.default_data_model().pd.io.sql.execute(q, conn)
+        conn.execute(q)
 
     def read_query(self, conn, q):
         """
 
         :param conn: database connection
         :param q: sql query
         :return: query results as table
         """
         if isinstance(q, data_algebra.data_ops.ViewRepresentation):
             q = q.to_sql(db_model=self)
         else:
             q = str(q)
         assert isinstance(q, str)
-        r = self.local_data_model.pd.io.sql.read_sql(q, conn)
+        r = self.local_data_model.pd.io.sql.read_sql_query(q, conn)
         return r
 
     def table_exists(self, conn, table_name: str) -> bool:
         """
         Return true if table exists.
         """
         assert isinstance(table_name, str)
```

### Comparing `data_algebra-1.6.6/data_algebra/db_space.py` & `data_algebra-1.6.7/data_algebra/db_space.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/eval_cache.py` & `data_algebra-1.6.7/data_algebra/eval_cache.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/expr_parse.py` & `data_algebra-1.6.7/data_algebra/expr_parse.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/expr_rep.py` & `data_algebra-1.6.7/data_algebra/expr_rep.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/expression_walker.py` & `data_algebra-1.6.7/data_algebra/expression_walker.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/flow_text.py` & `data_algebra-1.6.7/data_algebra/flow_text.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/near_sql.py` & `data_algebra-1.6.7/data_algebra/near_sql.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/op_catalog.py` & `data_algebra-1.6.7/data_algebra/op_catalog.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/pandas_base.py` & `data_algebra-1.6.7/data_algebra/pandas_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1104,14 +1104,16 @@
                 "table is not keyed by blocks_in.record_keys + blocks_in.control_table_keys"
             )
         # split on block keys
         if len(blocks_in.control_table_keys) != 1:
             split = [v for k, v in data.groupby(blocks_in.control_table_keys)]
         else:
             split = [v for k, v in data.groupby(blocks_in.control_table_keys[0])]
+        # make sure no row-index bull
+        split = [s.reset_index(drop=True, inplace=False) for s in split]
         # check same number of ids for each block
         # could also double check id columns are identical
         for i in range(1, len(split)):
             assert split[i].shape[0] == split[0].shape[0]
         sk = None
         if (blocks_in.record_keys is not None) and (len(blocks_in.record_keys) > 0):
             # ensure sorted in record order
```

### Comparing `data_algebra-1.6.6/data_algebra/pandas_model.py` & `data_algebra-1.6.7/data_algebra/pandas_model.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/parse_by_lark.py` & `data_algebra-1.6.7/data_algebra/parse_by_lark.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/polars_model.py` & `data_algebra-1.6.7/data_algebra/polars_model.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/python3_lark.py` & `data_algebra-1.6.7/data_algebra/python3_lark.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/shift_pipe_action.py` & `data_algebra-1.6.7/data_algebra/shift_pipe_action.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/solutions.py` & `data_algebra-1.6.7/data_algebra/solutions.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/sql_format_options.py` & `data_algebra-1.6.7/data_algebra/sql_format_options.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/test_util.py` & `data_algebra-1.6.7/data_algebra/test_util.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra/util.py` & `data_algebra-1.6.7/data_algebra/util.py`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/data_algebra.egg-info/PKG-INFO` & `data_algebra-1.6.7/data_algebra.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-algebra
-Version: 1.6.6
+Version: 1.6.7
 Summary: data_algebra is a data manipulation language that can both generate SQL queries and work on Pandas DataFrames.
 Home-page: https://github.com/WinVector/data_algebra
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `data_algebra-1.6.6/data_algebra.egg-info/SOURCES.txt` & `data_algebra-1.6.7/data_algebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_algebra-1.6.6/setup.py` & `data_algebra-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [R](https://www.r-project.org) versions of the system are available as 
 the [rquery](https://github.com/WinVector/rquery) and 
 [rqdatatable](https://github.com/WinVector/rqdatatable) packages.
 """
 
 setuptools.setup(
     name='data_algebra',
-    version='1.6.6',
+    version='1.6.7',
     author='John Mount',
     author_email='jmount@win-vector.com',
     url='https://github.com/WinVector/data_algebra',
     packages=setuptools.find_packages(exclude=['tests', 'Examples']),
     install_requires=[
         "numpy",
         "pandas>=1.0.0",
```

