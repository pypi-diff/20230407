# Comparing `tmp/feature_engineering_polars-0.3.0.tar.gz` & `tmp/feature_engineering_polars-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_engineering_polars-0.3.0.tar", max compression
+gzip compressed data, was "feature_engineering_polars-0.3.1.tar", max compression
```

## Comparing `feature_engineering_polars-0.3.0.tar` & `feature_engineering_polars-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/LICENSE
--rw-r--r--   0        0        0     1902 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/__init__.py
--rw-r--r--   0        0        0      133 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/encoding/__init__.py
--rw-r--r--   0        0        0     2066 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/encoding/one_hot_encoding.py
--rw-r--r--   0        0        0     4735 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/encoding/target_encoding.py
--rw-r--r--   0        0        0       58 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/imputing/__init__.py
--rw-r--r--   0        0        0     6761 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/fe_polars/imputing/base_imputing.py
--rw-r--r--   0        0        0     1270 2023-04-07 14:19:42.972205 feature_engineering_polars-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 feature_engineering_polars-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1909 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/__init__.py
+-rw-r--r--   0        0        0     2066 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/one_hot_encoding.py
+-rw-r--r--   0        0        0     4735 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/encoding/target_encoding.py
+-rw-r--r--   0        0        0       58 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/imputing/__init__.py
+-rw-r--r--   0        0        0     6948 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/fe_polars/imputing/base_imputing.py
+-rw-r--r--   0        0        0     1270 2023-04-07 16:16:45.718081 feature_engineering_polars-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 feature_engineering_polars-0.3.1/PKG-INFO
```

### Comparing `feature_engineering_polars-0.3.0/LICENSE` & `feature_engineering_polars-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_engineering_polars-0.3.0/README.md` & `feature_engineering_polars-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 - Encoding:
     - Target encoding
     - One hot encoding
 - Imputing:
     - Base imputing:
         - Mean imputing
         - Median imputing
-        - Mode imputing
         - Max imputing
         - Min imputing
+        - Fixed value imputing
```

### Comparing `feature_engineering_polars-0.3.0/fe_polars/encoding/one_hot_encoding.py` & `feature_engineering_polars-0.3.1/fe_polars/encoding/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `feature_engineering_polars-0.3.0/fe_polars/encoding/target_encoding.py` & `feature_engineering_polars-0.3.1/fe_polars/encoding/target_encoding.py`

 * *Files identical despite different names*

### Comparing `feature_engineering_polars-0.3.0/fe_polars/imputing/base_imputing.py` & `feature_engineering_polars-0.3.1/fe_polars/imputing/base_imputing.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,36 @@
 
 import polars
 
 
 class Imputer:
     """Imputer class.
 
-    Impute a value in place of the Null records in the dataframe
+    Impute a value in place of the null records in the dataframe
     depending on the strategy chosen.
 
-    Available strategies:
-
-    - Mean: strategy="mean"
-    - Median: strategy="median"
-    - Maximum: strategy="max"
-    - Minimum: strategy="min"
-    - Fixed value: strategy="fixed_value"
+    Args:
+        feature_to_impute (list): list of features to impute
+        strategy (str): imputation strategy
+        fixed_value (float): specific value to be imputed
+                             (with "fixed_value" strategy)
+        strategy_dict (dict): dictionnary describing strategies to apply
+                              by feature
     """
 
     def __init__(self, **kwargs):
         """Init.
 
         Args:
             kwargs (dict):
                 A dictionnary of optional arguments. Valid arguments include:
                 - features_to_impute
                 - strategy
                 - strategy_dict
+                - fixed_value
         """
         valid_params = {
             "features_to_impute",
             "strategy",
             "strategy_dict",
             "fixed_value",
         }
```

### Comparing `feature_engineering_polars-0.3.0/pyproject.toml` & `feature_engineering_polars-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.poetry]
 name = "feature-engineering-polars"
-version = "0.3.0"
+version = "0.3.1"
 description = "Feature engineering done with Polars"
 authors = ["Jordan Delbar <jordandelbar@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "fe_polars" }]
 
 [tool.poetry.dependencies]
```

### Comparing `feature_engineering_polars-0.3.0/PKG-INFO` & `feature_engineering_polars-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-engineering-polars
-Version: 0.3.0
+Version: 0.3.1
 Summary: Feature engineering done with Polars
 License: MIT
 Author: Jordan Delbar
 Author-email: jordandelbar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -72,11 +72,11 @@
 - Encoding:
     - Target encoding
     - One hot encoding
 - Imputing:
     - Base imputing:
         - Mean imputing
         - Median imputing
-        - Mode imputing
         - Max imputing
         - Min imputing
+        - Fixed value imputing
```

