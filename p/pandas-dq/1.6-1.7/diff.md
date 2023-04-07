# Comparing `tmp/pandas_dq-1.6.tar.gz` & `tmp/pandas_dq-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_dq-1.6.tar", last modified: Fri Apr  7 14:23:55 2023, max compression
+gzip compressed data, was "pandas_dq-1.7.tar", last modified: Fri Apr  7 17:03:29 2023, max compression
```

## Comparing `pandas_dq-1.6.tar` & `pandas_dq-1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 14:23:55.323599 pandas_dq-1.6/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.6/LICENSE
--rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.6/MANIFEST.in
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9758 2023-04-07 14:23:55.323599 pandas_dq-1.6/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)     8087 2023-04-07 13:15:32.000000 pandas_dq-1.6/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 14:23:55.307973 pandas_dq-1.6/pandas_dq.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9758 2023-04-07 14:23:54.000000 pandas_dq-1.6/pandas_dq.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-07 14:23:54.000000 pandas_dq-1.6/pandas_dq.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-07 14:23:54.000000 pandas_dq-1.6/pandas_dq.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-07 14:23:54.000000 pandas_dq-1.6/pandas_dq.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-07 14:23:54.000000 pandas_dq-1.6/pandas_dq.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)    40289 2023-04-07 14:20:58.000000 pandas_dq-1.6/pandas_dq.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.6/requirements.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-07 14:23:55.323599 pandas_dq-1.6/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-07 14:13:10.000000 pandas_dq-1.6/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 17:03:29.818100 pandas_dq-1.7/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.7/LICENSE
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.7/MANIFEST.in
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11030 2023-04-07 17:03:29.818100 pandas_dq-1.7/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     9215 2023-04-07 16:58:41.000000 pandas_dq-1.7/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 17:03:29.802470 pandas_dq-1.7/pandas_dq.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11030 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    43639 2023-04-07 16:46:41.000000 pandas_dq-1.7/pandas_dq.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.7/requirements.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-07 17:03:29.833721 pandas_dq-1.7/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-07 16:47:57.000000 pandas_dq-1.7/setup.py
```

### Comparing `pandas_dq-1.6/LICENSE` & `pandas_dq-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.6/MANIFEST.in` & `pandas_dq-1.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.6/PKG-INFO` & `pandas_dq-1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas_dq
-Version: 1.6
+Version: 1.7
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -32,33 +32,51 @@
         
         ### 1.  dq_report function
         
         ![dq_report_code](./images/find_dq_screenshot.png)
         
         <p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
         <ol>
-        <li>It detects missing values and suggests to impute them with mean, median, mode, or a constant value.</li>
-        <li>It identifies rare categories and suggests to group them into a single category or drop them.</li>
-        <li>It finds infinite values and suggests to replace them with NaN or a large value.</li>
-        <li>It detects mixed data types and suggests to convert them to a single type or split them into multiple columns.</li>
-        <li>It detects outliers and suggests to remove them or use robust statistics.</li>
-        <li>It detects high cardinality features and suggests to reduce them using encoding techniques or feature selection methods.</li>
-        <li>It detects highly correlated features and suggests to drop one of them or use dimensionality reduction techniques.</li>
-        <li>It detects duplicate rows and columns and suggests to drop them or keep only one copy.</li>
-        <li>It detects skewed distributions and suggests to apply transformations or scaling techniques. </li>
-        <li>It detects imbalanced classes and suggests to use resampling techniques or class weights. </li>
-        <li>It detects feature leakage and suggests to avoid using features that are not available at prediction time. </li>
+        <li>It detects ID columns</li>
+        <li>It detects zero-variance columns </li>
+        <li>It identifies rare categories (less than 5% of categories in a column)</li>
+        <li>It finds infinite values in a column</li>
+        <li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
+        <li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
+        <li>It detects high cardinality features (i.e. a feature that has more than 100 categories)</li>
+        <li>It detects highly correlated features (i.e. two features that have an absolute correlation higher than 0.8)</li>
+        <li>It detects duplicate rows (i.e. the same row occurs more than once in the dataset)</li>
+        <li>It detects duplicate columns (i.e. the same column occurs twice or more in the dataset)</li>
+        <li>It detects skewed distributions (i.e. a feature that has a skew more than 1.0) </li>
+        <li>It detects imbalanced classes (i.e. target variable has one class more than other in a significant way) </li>
+        <li>It detects feature leakage (i.e. a feature that is highly correlated to target with correlation > 0.8)</li>
         </ol>
         Notice that for large datasets, this report generation may take time. So please be patient while it analyzes your dataset!
         
         ### 2.  Fix_DQ class: a scikit_learn transformer which can detect data quality issues and clean them all in one line of code
         
         ![fix_dq](./images/fix_dq_screenshot.png)
         
         <p>`Fix_DQ` is a great way to clean an entire train data set and apply the same steps in an MLOps pipeline to a test dataset.  `Fix_DQ` can be used to detect most issues in your data (similar to dq_report but without the target related steps) in one step (during `fit` method). This transformer can then be saved (or "pickled") for applying the same steps on test data either at the same time or later.<br>
+        <p>Fix_DQ will perform following data quality cleaning steps:
+        <ol>
+        <li>It removes ID columns from further processing</li>
+        <li>It removes zero-variance columns from further processing</li>
+        <li>It identifies rare categories and groups them into a single category called "Rare"</li>
+        <li>It finds infinite values and replaces them with an upper bound based on Inter Quartile Range</li>
+        <li>It detects mixed data types and drops those mixed-type columns from further processing</li>
+        <li>It detects outliers and suggests to remove them or use robust statistics.</li>
+        <li>It detects high cardinality features but leaves them as it is.</li>
+        <li>It detects highly correlated features and drops one of them (whichever comes first in the column sequence)</li>
+        <li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
+        <li>It detects duplicate columns and drops one of them or keeps only one copy</li>
+        <li>It detects skewed distributions and applies log or box-cox transformations on them </li>
+        <li>It detects imbalanced classes and leaves them as it is </li>
+        <li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
+        </ol>
         
         
         ###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
         <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
         
         ## Install
         <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas_dq Version: 1.6 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas_dq Version: 1.7 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
@@ -15,45 +15,67 @@
 automatically cleaning your dirty dataset using pandas scikit_learn functions.
 You can analyze your dataset and fix them - all in a single line of code! !
 [pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
 modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
 (./images/find_dq_screenshot.png)
 `dq_report` is a function that is the most popular way to use pandas_dq and it
 performs following data quality analysis steps:
-   1. It detects missing values and suggests to impute them with mean, median,
-      mode, or a constant value.
-   2. It identifies rare categories and suggests to group them into a single
-      category or drop them.
-   3. It finds infinite values and suggests to replace them with NaN or a large
-      value.
-   4. It detects mixed data types and suggests to convert them to a single type
-      or split them into multiple columns.
-   5. It detects outliers and suggests to remove them or use robust statistics.
-   6. It detects high cardinality features and suggests to reduce them using
-      encoding techniques or feature selection methods.
-   7. It detects highly correlated features and suggests to drop one of them or
-      use dimensionality reduction techniques.
-   8. It detects duplicate rows and columns and suggests to drop them or keep
-      only one copy.
-   9. It detects skewed distributions and suggests to apply transformations or
-      scaling techniques.
-  10. It detects imbalanced classes and suggests to use resampling techniques
-      or class weights.
-  11. It detects feature leakage and suggests to avoid using features that are
-      not available at prediction time.
+   1. It detects ID columns
+   2. It detects zero-variance columns
+   3. It identifies rare categories (less than 5% of categories in a column)
+   4. It finds infinite values in a column
+   5. It detects mixed data types (i.e. a column that has more than a single
+      data type)
+   6. It detects outliers (i.e. a float column that is beyond the Inter
+      Quartile Range)
+   7. It detects high cardinality features (i.e. a feature that has more than
+      100 categories)
+   8. It detects highly correlated features (i.e. two features that have an
+      absolute correlation higher than 0.8)
+   9. It detects duplicate rows (i.e. the same row occurs more than once in the
+      dataset)
+  10. It detects duplicate columns (i.e. the same column occurs twice or more
+      in the dataset)
+  11. It detects skewed distributions (i.e. a feature that has a skew more than
+      1.0)
+  12. It detects imbalanced classes (i.e. target variable has one class more
+      than other in a significant way)
+  13. It detects feature leakage (i.e. a feature that is highly correlated to
+      target with correlation > 0.8)
 Notice that for large datasets, this report generation may take time. So please
 be patient while it analyzes your dataset! ### 2. Fix_DQ class: a scikit_learn
 transformer which can detect data quality issues and clean them all in one line
 of code ![fix_dq](./images/fix_dq_screenshot.png)
 `Fix_DQ` is a great way to clean an entire train data set and apply the same
 steps in an MLOps pipeline to a test dataset. `Fix_DQ` can be used to detect
 most issues in your data (similar to dq_report but without the target related
 steps) in one step (during `fit` method). This transformer can then be saved
 (or "pickled") for applying the same steps on test data either at the same time
 or later.
+Fix_DQ will perform following data quality cleaning steps:
+   1. It removes ID columns from further processing
+   2. It removes zero-variance columns from further processing
+   3. It identifies rare categories and groups them into a single category
+      called "Rare"
+   4. It finds infinite values and replaces them with an upper bound based on
+      Inter Quartile Range
+   5. It detects mixed data types and drops those mixed-type columns from
+      further processing
+   6. It detects outliers and suggests to remove them or use robust statistics.
+   7. It detects high cardinality features but leaves them as it is.
+   8. It detects highly correlated features and drops one of them (whichever
+      comes first in the column sequence)
+   9. It detects duplicate rows and drops one of them or keeps only one copy of
+      duplicate rows
+  10. It detects duplicate columns and drops one of them or keeps only one copy
+  11. It detects skewed distributions and applies log or box-cox
+      transformations on them
+  12. It detects imbalanced classes and leaves them as it is
+  13. It detects feature leakage and drops one of those features if they are
+      highly correlated to target
 ### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
 ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
```

### Comparing `pandas_dq-1.6/README.md` & `pandas_dq-1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,33 +25,51 @@
 
 ### 1.  dq_report function
 
 ![dq_report_code](./images/find_dq_screenshot.png)
 
 <p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
 <ol>
-<li>It detects missing values and suggests to impute them with mean, median, mode, or a constant value.</li>
-<li>It identifies rare categories and suggests to group them into a single category or drop them.</li>
-<li>It finds infinite values and suggests to replace them with NaN or a large value.</li>
-<li>It detects mixed data types and suggests to convert them to a single type or split them into multiple columns.</li>
-<li>It detects outliers and suggests to remove them or use robust statistics.</li>
-<li>It detects high cardinality features and suggests to reduce them using encoding techniques or feature selection methods.</li>
-<li>It detects highly correlated features and suggests to drop one of them or use dimensionality reduction techniques.</li>
-<li>It detects duplicate rows and columns and suggests to drop them or keep only one copy.</li>
-<li>It detects skewed distributions and suggests to apply transformations or scaling techniques. </li>
-<li>It detects imbalanced classes and suggests to use resampling techniques or class weights. </li>
-<li>It detects feature leakage and suggests to avoid using features that are not available at prediction time. </li>
+<li>It detects ID columns</li>
+<li>It detects zero-variance columns </li>
+<li>It identifies rare categories (less than 5% of categories in a column)</li>
+<li>It finds infinite values in a column</li>
+<li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
+<li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
+<li>It detects high cardinality features (i.e. a feature that has more than 100 categories)</li>
+<li>It detects highly correlated features (i.e. two features that have an absolute correlation higher than 0.8)</li>
+<li>It detects duplicate rows (i.e. the same row occurs more than once in the dataset)</li>
+<li>It detects duplicate columns (i.e. the same column occurs twice or more in the dataset)</li>
+<li>It detects skewed distributions (i.e. a feature that has a skew more than 1.0) </li>
+<li>It detects imbalanced classes (i.e. target variable has one class more than other in a significant way) </li>
+<li>It detects feature leakage (i.e. a feature that is highly correlated to target with correlation > 0.8)</li>
 </ol>
 Notice that for large datasets, this report generation may take time. So please be patient while it analyzes your dataset!
 
 ### 2.  Fix_DQ class: a scikit_learn transformer which can detect data quality issues and clean them all in one line of code
 
 ![fix_dq](./images/fix_dq_screenshot.png)
 
 <p>`Fix_DQ` is a great way to clean an entire train data set and apply the same steps in an MLOps pipeline to a test dataset.  `Fix_DQ` can be used to detect most issues in your data (similar to dq_report but without the target related steps) in one step (during `fit` method). This transformer can then be saved (or "pickled") for applying the same steps on test data either at the same time or later.<br>
+<p>Fix_DQ will perform following data quality cleaning steps:
+<ol>
+<li>It removes ID columns from further processing</li>
+<li>It removes zero-variance columns from further processing</li>
+<li>It identifies rare categories and groups them into a single category called "Rare"</li>
+<li>It finds infinite values and replaces them with an upper bound based on Inter Quartile Range</li>
+<li>It detects mixed data types and drops those mixed-type columns from further processing</li>
+<li>It detects outliers and suggests to remove them or use robust statistics.</li>
+<li>It detects high cardinality features but leaves them as it is.</li>
+<li>It detects highly correlated features and drops one of them (whichever comes first in the column sequence)</li>
+<li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
+<li>It detects duplicate columns and drops one of them or keeps only one copy</li>
+<li>It detects skewed distributions and applies log or box-cox transformations on them </li>
+<li>It detects imbalanced classes and leaves them as it is </li>
+<li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
+</ol>
 
 
 ###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
 
 ## Install
 <p>
```

#### html2text {}

```diff
@@ -12,45 +12,67 @@
 automatically cleaning your dirty dataset using pandas scikit_learn functions.
 You can analyze your dataset and fix them - all in a single line of code! !
 [pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
 modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
 (./images/find_dq_screenshot.png)
 `dq_report` is a function that is the most popular way to use pandas_dq and it
 performs following data quality analysis steps:
-   1. It detects missing values and suggests to impute them with mean, median,
-      mode, or a constant value.
-   2. It identifies rare categories and suggests to group them into a single
-      category or drop them.
-   3. It finds infinite values and suggests to replace them with NaN or a large
-      value.
-   4. It detects mixed data types and suggests to convert them to a single type
-      or split them into multiple columns.
-   5. It detects outliers and suggests to remove them or use robust statistics.
-   6. It detects high cardinality features and suggests to reduce them using
-      encoding techniques or feature selection methods.
-   7. It detects highly correlated features and suggests to drop one of them or
-      use dimensionality reduction techniques.
-   8. It detects duplicate rows and columns and suggests to drop them or keep
-      only one copy.
-   9. It detects skewed distributions and suggests to apply transformations or
-      scaling techniques.
-  10. It detects imbalanced classes and suggests to use resampling techniques
-      or class weights.
-  11. It detects feature leakage and suggests to avoid using features that are
-      not available at prediction time.
+   1. It detects ID columns
+   2. It detects zero-variance columns
+   3. It identifies rare categories (less than 5% of categories in a column)
+   4. It finds infinite values in a column
+   5. It detects mixed data types (i.e. a column that has more than a single
+      data type)
+   6. It detects outliers (i.e. a float column that is beyond the Inter
+      Quartile Range)
+   7. It detects high cardinality features (i.e. a feature that has more than
+      100 categories)
+   8. It detects highly correlated features (i.e. two features that have an
+      absolute correlation higher than 0.8)
+   9. It detects duplicate rows (i.e. the same row occurs more than once in the
+      dataset)
+  10. It detects duplicate columns (i.e. the same column occurs twice or more
+      in the dataset)
+  11. It detects skewed distributions (i.e. a feature that has a skew more than
+      1.0)
+  12. It detects imbalanced classes (i.e. target variable has one class more
+      than other in a significant way)
+  13. It detects feature leakage (i.e. a feature that is highly correlated to
+      target with correlation > 0.8)
 Notice that for large datasets, this report generation may take time. So please
 be patient while it analyzes your dataset! ### 2. Fix_DQ class: a scikit_learn
 transformer which can detect data quality issues and clean them all in one line
 of code ![fix_dq](./images/fix_dq_screenshot.png)
 `Fix_DQ` is a great way to clean an entire train data set and apply the same
 steps in an MLOps pipeline to a test dataset. `Fix_DQ` can be used to detect
 most issues in your data (similar to dq_report but without the target related
 steps) in one step (during `fit` method). This transformer can then be saved
 (or "pickled") for applying the same steps on test data either at the same time
 or later.
+Fix_DQ will perform following data quality cleaning steps:
+   1. It removes ID columns from further processing
+   2. It removes zero-variance columns from further processing
+   3. It identifies rare categories and groups them into a single category
+      called "Rare"
+   4. It finds infinite values and replaces them with an upper bound based on
+      Inter Quartile Range
+   5. It detects mixed data types and drops those mixed-type columns from
+      further processing
+   6. It detects outliers and suggests to remove them or use robust statistics.
+   7. It detects high cardinality features but leaves them as it is.
+   8. It detects highly correlated features and drops one of them (whichever
+      comes first in the column sequence)
+   9. It detects duplicate rows and drops one of them or keeps only one copy of
+      duplicate rows
+  10. It detects duplicate columns and drops one of them or keeps only one copy
+  11. It detects skewed distributions and applies log or box-cox
+      transformations on them
+  12. It detects imbalanced classes and leaves them as it is
+  13. It detects feature leakage and drops one of those features if they are
+      highly correlated to target
 ### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
 ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
```

### Comparing `pandas_dq-1.6/pandas_dq.egg-info/PKG-INFO` & `pandas_dq-1.7/pandas_dq.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-dq
-Version: 1.6
+Version: 1.7
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -32,33 +32,51 @@
         
         ### 1.  dq_report function
         
         ![dq_report_code](./images/find_dq_screenshot.png)
         
         <p>`dq_report` is a function that is the most popular way to use pandas_dq and it performs following data quality analysis steps:
         <ol>
-        <li>It detects missing values and suggests to impute them with mean, median, mode, or a constant value.</li>
-        <li>It identifies rare categories and suggests to group them into a single category or drop them.</li>
-        <li>It finds infinite values and suggests to replace them with NaN or a large value.</li>
-        <li>It detects mixed data types and suggests to convert them to a single type or split them into multiple columns.</li>
-        <li>It detects outliers and suggests to remove them or use robust statistics.</li>
-        <li>It detects high cardinality features and suggests to reduce them using encoding techniques or feature selection methods.</li>
-        <li>It detects highly correlated features and suggests to drop one of them or use dimensionality reduction techniques.</li>
-        <li>It detects duplicate rows and columns and suggests to drop them or keep only one copy.</li>
-        <li>It detects skewed distributions and suggests to apply transformations or scaling techniques. </li>
-        <li>It detects imbalanced classes and suggests to use resampling techniques or class weights. </li>
-        <li>It detects feature leakage and suggests to avoid using features that are not available at prediction time. </li>
+        <li>It detects ID columns</li>
+        <li>It detects zero-variance columns </li>
+        <li>It identifies rare categories (less than 5% of categories in a column)</li>
+        <li>It finds infinite values in a column</li>
+        <li>It detects mixed data types (i.e. a column that has more than a single data type)</li>
+        <li>It detects outliers (i.e. a float column that is beyond the Inter Quartile Range)</li>
+        <li>It detects high cardinality features (i.e. a feature that has more than 100 categories)</li>
+        <li>It detects highly correlated features (i.e. two features that have an absolute correlation higher than 0.8)</li>
+        <li>It detects duplicate rows (i.e. the same row occurs more than once in the dataset)</li>
+        <li>It detects duplicate columns (i.e. the same column occurs twice or more in the dataset)</li>
+        <li>It detects skewed distributions (i.e. a feature that has a skew more than 1.0) </li>
+        <li>It detects imbalanced classes (i.e. target variable has one class more than other in a significant way) </li>
+        <li>It detects feature leakage (i.e. a feature that is highly correlated to target with correlation > 0.8)</li>
         </ol>
         Notice that for large datasets, this report generation may take time. So please be patient while it analyzes your dataset!
         
         ### 2.  Fix_DQ class: a scikit_learn transformer which can detect data quality issues and clean them all in one line of code
         
         ![fix_dq](./images/fix_dq_screenshot.png)
         
         <p>`Fix_DQ` is a great way to clean an entire train data set and apply the same steps in an MLOps pipeline to a test dataset.  `Fix_DQ` can be used to detect most issues in your data (similar to dq_report but without the target related steps) in one step (during `fit` method). This transformer can then be saved (or "pickled") for applying the same steps on test data either at the same time or later.<br>
+        <p>Fix_DQ will perform following data quality cleaning steps:
+        <ol>
+        <li>It removes ID columns from further processing</li>
+        <li>It removes zero-variance columns from further processing</li>
+        <li>It identifies rare categories and groups them into a single category called "Rare"</li>
+        <li>It finds infinite values and replaces them with an upper bound based on Inter Quartile Range</li>
+        <li>It detects mixed data types and drops those mixed-type columns from further processing</li>
+        <li>It detects outliers and suggests to remove them or use robust statistics.</li>
+        <li>It detects high cardinality features but leaves them as it is.</li>
+        <li>It detects highly correlated features and drops one of them (whichever comes first in the column sequence)</li>
+        <li>It detects duplicate rows and drops one of them or keeps only one copy of duplicate rows</li>
+        <li>It detects duplicate columns and drops one of them or keeps only one copy</li>
+        <li>It detects skewed distributions and applies log or box-cox transformations on them </li>
+        <li>It detects imbalanced classes and leaves them as it is </li>
+        <li>It detects feature leakage and drops one of those features if they are highly correlated to target </li>
+        </ol>
         
         
         ###  How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
         <p>This is another way to find the best data cleaning steps for your train data and then use the cleaned data in hyper parameter tuning using GridSearchCV or RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.<br>
         
         ## Install
         <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas-dq Version: 1.6 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas-dq Version: 1.7 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
@@ -15,45 +15,67 @@
 automatically cleaning your dirty dataset using pandas scikit_learn functions.
 You can analyze your dataset and fix them - all in a single line of code! !
 [pandas_dq](./images/pandas_dq_logo.png) ## Uses `pandas_dq` has two important
 modules: `dq_report` and `Fix_DQ`. ### 1. dq_report function ![dq_report_code]
 (./images/find_dq_screenshot.png)
 `dq_report` is a function that is the most popular way to use pandas_dq and it
 performs following data quality analysis steps:
-   1. It detects missing values and suggests to impute them with mean, median,
-      mode, or a constant value.
-   2. It identifies rare categories and suggests to group them into a single
-      category or drop them.
-   3. It finds infinite values and suggests to replace them with NaN or a large
-      value.
-   4. It detects mixed data types and suggests to convert them to a single type
-      or split them into multiple columns.
-   5. It detects outliers and suggests to remove them or use robust statistics.
-   6. It detects high cardinality features and suggests to reduce them using
-      encoding techniques or feature selection methods.
-   7. It detects highly correlated features and suggests to drop one of them or
-      use dimensionality reduction techniques.
-   8. It detects duplicate rows and columns and suggests to drop them or keep
-      only one copy.
-   9. It detects skewed distributions and suggests to apply transformations or
-      scaling techniques.
-  10. It detects imbalanced classes and suggests to use resampling techniques
-      or class weights.
-  11. It detects feature leakage and suggests to avoid using features that are
-      not available at prediction time.
+   1. It detects ID columns
+   2. It detects zero-variance columns
+   3. It identifies rare categories (less than 5% of categories in a column)
+   4. It finds infinite values in a column
+   5. It detects mixed data types (i.e. a column that has more than a single
+      data type)
+   6. It detects outliers (i.e. a float column that is beyond the Inter
+      Quartile Range)
+   7. It detects high cardinality features (i.e. a feature that has more than
+      100 categories)
+   8. It detects highly correlated features (i.e. two features that have an
+      absolute correlation higher than 0.8)
+   9. It detects duplicate rows (i.e. the same row occurs more than once in the
+      dataset)
+  10. It detects duplicate columns (i.e. the same column occurs twice or more
+      in the dataset)
+  11. It detects skewed distributions (i.e. a feature that has a skew more than
+      1.0)
+  12. It detects imbalanced classes (i.e. target variable has one class more
+      than other in a significant way)
+  13. It detects feature leakage (i.e. a feature that is highly correlated to
+      target with correlation > 0.8)
 Notice that for large datasets, this report generation may take time. So please
 be patient while it analyzes your dataset! ### 2. Fix_DQ class: a scikit_learn
 transformer which can detect data quality issues and clean them all in one line
 of code ![fix_dq](./images/fix_dq_screenshot.png)
 `Fix_DQ` is a great way to clean an entire train data set and apply the same
 steps in an MLOps pipeline to a test dataset. `Fix_DQ` can be used to detect
 most issues in your data (similar to dq_report but without the target related
 steps) in one step (during `fit` method). This transformer can then be saved
 (or "pickled") for applying the same steps on test data either at the same time
 or later.
+Fix_DQ will perform following data quality cleaning steps:
+   1. It removes ID columns from further processing
+   2. It removes zero-variance columns from further processing
+   3. It identifies rare categories and groups them into a single category
+      called "Rare"
+   4. It finds infinite values and replaces them with an upper bound based on
+      Inter Quartile Range
+   5. It detects mixed data types and drops those mixed-type columns from
+      further processing
+   6. It detects outliers and suggests to remove them or use robust statistics.
+   7. It detects high cardinality features but leaves them as it is.
+   8. It detects highly correlated features and drops one of them (whichever
+      comes first in the column sequence)
+   9. It detects duplicate rows and drops one of them or keeps only one copy of
+      duplicate rows
+  10. It detects duplicate columns and drops one of them or keeps only one copy
+  11. It detects skewed distributions and applies log or box-cox
+      transformations on them
+  12. It detects imbalanced classes and leaves them as it is
+  13. It detects feature leakage and drops one of those features if they are
+      highly correlated to target
 ### How can we use Fix_DQ in GridSearchCV to find the best model pipeline?
 This is another way to find the best data cleaning steps for your train data
 and then use the cleaned data in hyper parameter tuning using GridSearchCV or
 RandomizedSearchCV along with a LightGBM or an XGBoost or a scikit-learn model.
 ## Install
 **Prerequsites:**
    1. pandas_dq is built using pandas, numpy and scikit-learn - that's all. It
```

### Comparing `pandas_dq-1.6/pandas_dq.py` & `pandas_dq-1.7/pandas_dq.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,27 +111,33 @@
         columns=['Data Type']
     )
 
     missing_values = df.isnull().sum()
     missing_cols = missing_values[missing_values > 0].index.tolist()
     number_cols = df.select_dtypes(include=["integer", "float"]).columns.tolist() # Get numerical columns
     float_cols = df.select_dtypes(include=[ "float"]).columns.tolist() # Get float columns
+    id_cols = []
+    zero_var_cols = []
 
     missing_data = pd.DataFrame(
         missing_values,
         columns=['Missing Values']
     )
     unique_values = pd.DataFrame(
         columns=['Unique Values']
     )
     for row in list(df.columns.values):
         if row in float_cols:
             unique_values.loc[row] = ["NA"]
         else:
             unique_values.loc[row] = [df[row].nunique()]
+            if df[row].nunique() == df.shape[0]:
+                id_cols.append(row)
+            elif df[row].nunique() == 1:
+                zero_var_cols.append(row)
         
     maximum_values = pd.DataFrame(
         columns=['Maximum Value']
     )
     minimum_values = pd.DataFrame(
         columns=['Minimum Value']
     )
@@ -149,14 +155,44 @@
     ### now generate the data quality starter dataframe
     dq_df2 = data_types.join(missing_data).join(unique_values).join(minimum_values).join(maximum_values)
 
     ### set up additional columns    
     dq_df2["first_comma"] = ""
     dq_df2[new_col] = f""
     
+    # Detect ID columns in dataset and recommend removing them
+    if len(id_cols) > 0:
+        new_string = f"There are ID columns in the dataset. Recommend removing them before modeling."
+        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
+        dq_df1.loc[bad_col,'first_comma'] = ', '
+        for col in id_cols:
+            # Append a row to the dq_df1 with the column name and the issue only if the column has a missing value
+            new_string = f"Possible ID colum: drop before modeling process."
+            dq_df2.loc[col,new_col] += dq_df2.loc[col,'first_comma'] + new_string
+            dq_df2.loc[col,'first_comma'] = ', '
+    else:
+        new_string = f"There are no ID columns in the dataset. So no ID columns to remove before modeling."
+        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
+        dq_df1.loc[good_col,'first_comma'] = ', '
+
+    # Detect ID columns in dataset and recommend removing them
+    if len(zero_var_cols) > 0:
+        new_string = f"There are zero-variance columns in the dataset. Recommend removing them before modeling."
+        dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
+        dq_df1.loc[bad_col,'first_comma'] = ', '
+        for col in zero_var_cols:
+            # Append a row to the dq_df1 with the column name and the issue only if the column has a missing value
+            new_string = f"Zero-variance colum: drop before modeling process."
+            dq_df2.loc[col,new_col] += dq_df2.loc[col,'first_comma'] + new_string
+            dq_df2.loc[col,'first_comma'] = ', '
+    else:
+        new_string = f"There are no zero-variance columns in the dataset. So no zero-variance columns to remove before modeling."
+        dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
+        dq_df1.loc[good_col,'first_comma'] = ', '
+
     # Detect missing values and suggests to impute them with mean, median, mode, or a constant value123
     #missing_values = df.isnull().sum()
     #missing_cols = missing_values[missing_values > 0].index.tolist()
     if len(missing_cols) > 0:
         for col in missing_cols:
             # Append a row to the dq_df1 with the column name and the issue only if the column has a missing value
             if missing_values[col] > 0:
@@ -562,45 +598,41 @@
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
         
         # Drop duplicate rows
         dup_rows = X.duplicated().sum()
         if dup_rows > 0:
-            print(f'Alert: Dropping {dup_rows} rows can sometimes cause column data types to change to object. Double-check!')
+            print(f'Alert: Dropping {dup_rows} duplicate rows can sometimes cause column data types to change to object. Double-check!')
             X = X.drop_duplicates()
         
         # Drop duplicate columns
         dup_cols = X.T.duplicated().sum()
         if dup_cols > 0:
-            print(f'Alert: Dropping {dup_cols} cols can sometimes cause column data types to change to object. Double-check!')
+            print(f'Alert: Dropping {dup_cols} duplicate cols can sometimes cause column data types to change to object. Double-check!')
             X = X.T.drop_duplicates().T
         
         # Return the DataFrame with no duplicates
         return X
     
     # Define a function to detect skewed distributions and apply a proper transformation to the column
     def transform_skewed(self, X):
         # Check if X is a pandas DataFrame
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
         
         # Get the numerical columns
         num_cols = X.select_dtypes(include=["float"]).columns.tolist()
-        
-        # Define a threshold for skewness
-        skew_threshold = 0.5
-        
+                
         # Loop through each numerical column
         for col in num_cols:
             # Find if a column transformer exists for this column
             if col in self.col_transformers_:
                 # Cap the outliers using the upper bound
-                # Check if the skewness is above the threshold
                 if str(self.col_transformers_[col]).split("(")[0] == "PowerTransformer":
                     ### power transformer expects Pandas DataFrame
                     pt = self.col_transformers_[col]
                     X[col] = pt.transform(X[[col]])
                 else:
                     ### function transformer expects pandas series
                     ft = self.col_transformers_[col]
@@ -615,14 +647,25 @@
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
         
         # Get the numerical columns
         num_cols = X.select_dtypes(include=["int", "float"]).columns.tolist()
         float_cols = X.select_dtypes(include=["float"]).columns.tolist()
+        non_float_cols = left_subtract(X.columns, float_cols)
+
+        # Detect ID columns
+        self.id_cols_ = [column for column in non_float_cols if X[column].nunique() == X.shape[0]]
+        if len(self.id_cols_) > 0:
+            print(f"{len(self.id_cols_)} ID cols will be dropped from further processing: {self.id_cols_}")
+
+        # Detect zero-variance columns
+        self.zero_var_cols_ = [column for column in non_float_cols if X[column].nunique() == 1]
+        if len(self.zero_var_cols_) > 0:
+            print(f"    {len(self.zero_var_cols_)} zero-variance cols will be dropped from further processing: {self.zero_var_cols_}")
         
         # Detect highly correlated features
         self.drop_corr_cols_ = []
         correlation_matrix = X.corr().abs() # Get the absolute correlation matrix of numerical columns
         upper_triangle = correlation_matrix.where(np.triu(np.ones(correlation_matrix.shape), k=1).astype(bool)) # Get the upper triangle of the matrix
         high_corr_cols = [column for column in upper_triangle.columns if any(upper_triangle[column] > self.correlation_threshold)] # Get the columns with high correlation
         if len(high_corr_cols) > 0:
@@ -660,15 +703,15 @@
                 # Store the upper bound in the dictionary
                 self.upper_bounds_[col] = upper_bound
 
         # Initialize an empty dictionary to store the column transformers
         self.col_transformers_ = {}
         
         # Define a threshold for skewness
-        skew_threshold = 0.5
+        skew_threshold = 1.0
         
         # Loop through each float column
         for col in float_cols:
             # Calculate the skewness of the column
             skewness = X[col].skew()
             # Check if the skewness is above the threshold
             if abs(skewness) > skew_threshold:
@@ -706,16 +749,30 @@
     def transform(self, X):
         # Check if X is a pandas DataFrame
         if not isinstance(X, pd.DataFrame):
             # Convert X to a pandas DataFrame
             X = pd.DataFrame(X)
         
         ### drop mixed data type columns from further processing ##
+        if len(self.id_cols_) > 0:
+            X = X.drop(self.id_cols_, axis=1)
+
+        ### drop mixed data type columns from further processing ##
+        if len(self.zero_var_cols_) > 0:
+            X = X.drop(self.zero_var_cols_, axis=1)
+
+        ### drop mixed data type columns from further processing ##
         if len(self.mixed_type_cols_) > 0:
-            X = X.drop(self.mixed_type_cols_, axis=1)
+            drop_cols = left_subtract(self.mixed_type_cols_, self.zero_var_cols_+self.id_cols_)
+            if len(drop_cols) > 0:
+                X = X.drop(drop_cols, axis=1)
+            else:
+                drop_cols = left_subtract(self.zero_var_cols_+self.id_cols_, self.mixed_type_cols_)
+                if len(drop_cols) > 0:
+                    X = X.drop(drop_cols, axis=1)
             
         ### drop highly correlated columns from further processing ##
         if len(self.drop_corr_cols_) > 0:
             if len(left_subtract(self.drop_corr_cols_,self.mixed_type_cols_)) > 0:
                 extra_cols = left_subtract(self.drop_corr_cols_,self.mixed_type_cols_)
             elif len(left_subtract(self.mixed_type_cols_,drop_corr_cols_)) > 0:
                 extra_cols = left_subtract(self.mixed_type_cols_, self.drop_corr_cols_)
@@ -745,12 +802,12 @@
         transformed_X = self.transform_skewed(rare_X)
                 
         # Return the transformed DataFrame
         return transformed_X
 
 ############################################################################################
 module_type = 'Running' if  __name__ == "__main__" else 'Imported'
-version_number =  '1.6'
+version_number =  '1.7'
 print(f"""{module_type} pandas_dq ({version_number}). Always upgrade to get latest version.
 from pandas_dq import dq_report, Fix_DQ
 """)
 #################################################################################
```

### Comparing `pandas_dq-1.6/setup.py` & `pandas_dq-1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandas_dq",
-    version="1.6",
+    version="1.7",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Clean your data using a scikit-learn transformer in a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/pandas_dq",
```

