# Comparing `tmp/irisml-tasks-0.0.8.tar.gz` & `tmp/irisml-tasks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-0.0.8.tar", last modified: Wed Oct 12 06:36:04 2022, max compression
+gzip compressed data, was "irisml-tasks-0.0.9.tar", last modified: Tue Oct 18 17:55:48 2022, max compression
```

## Comparing `irisml-tasks-0.0.8.tar` & `irisml-tasks-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 06:36:04.279043 irisml-tasks-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-10-12 06:36:04.279043 irisml-tasks-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 06:36:04.271042 irisml-tasks-0.0.8/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 06:36:04.275042 irisml-tasks-0.0.8/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/calculate_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/download_azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_current_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_dataset_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_dataset_subset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_fake_image_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_fake_object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_secret_from_azure_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/get_topk.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/join_filepath.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/load_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/run_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/run_sequential.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/save_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/save_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/search_grid_sequential.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/irisml/tasks/upload_azure_blob.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 06:36:04.275042 irisml-tasks-0.0.8/irisml_tasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-10-12 06:36:04.000000 irisml-tasks-0.0.8/irisml_tasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-10-12 06:36:04.000000 irisml-tasks-0.0.8/irisml_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 06:36:04.000000 irisml-tasks-0.0.8/irisml_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-12 06:36:04.000000 irisml-tasks-0.0.8/irisml_tasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-12 06:36:04.000000 irisml-tasks-0.0.8/irisml_tasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-12 06:36:04.279043 irisml-tasks-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 06:36:04.279043 irisml-tasks-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_calculate_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_current_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_dataset_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_dataset_subset.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_fake_image_classification_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_fake_object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_secret_from_azure_keyvault.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_get_topk.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_join_filepath.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_load_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_run_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_run_sequential.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_save_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_save_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-10-12 06:35:04.000000 irisml-tasks-0.0.8/test/test_search_grid_sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:55:48.392162 irisml-tasks-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-10-18 17:55:48.392162 irisml-tasks-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:55:48.384161 irisml-tasks-0.0.9/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:55:48.388161 irisml-tasks-0.0.9/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/calculate_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/download_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_current_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_dataset_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_dataset_subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_fake_image_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_fake_object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_secret_from_azure_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/get_topk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/join_filepath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/load_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/run_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/run_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/save_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/save_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/search_grid_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/irisml/tasks/upload_azure_blob.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:55:48.392162 irisml-tasks-0.0.9/irisml_tasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-10-18 17:55:48.000000 irisml-tasks-0.0.9/irisml_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-18 17:55:48.000000 irisml-tasks-0.0.9/irisml_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 17:55:48.000000 irisml-tasks-0.0.9/irisml_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-18 17:55:48.000000 irisml-tasks-0.0.9/irisml_tasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-18 17:55:48.000000 irisml-tasks-0.0.9/irisml_tasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-18 17:55:48.392162 irisml-tasks-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 17:55:48.392162 irisml-tasks-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_calculate_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_current_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_dataset_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_dataset_subset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_fake_image_classification_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_fake_object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_secret_from_azure_keyvault.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_get_topk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_join_filepath.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_load_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_run_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_run_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_save_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_save_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-10-18 17:54:38.000000 irisml-tasks-0.0.9/test/test_search_grid_sequential.py
```

### Comparing `irisml-tasks-0.0.8/LICENSE` & `irisml-tasks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/PKG-INFO` & `irisml-tasks-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Standard tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,14 +15,17 @@
 
 Visit [irisml](https://github.com/microsoft/irisml) for the detail.
 
 ## tasks
 ### assertion
 This task throws an exception if the given assertion failed for the input object.
 
+## branch
+'If' condition for tasks.
+
 ### calculate_cosine_similarity
 Calculate cosine similarity between two sets of vectors.
 
 ### download_azure_blob
 Download a file from azure blob.
 
 ### get_current_time
```

### Comparing `irisml-tasks-0.0.8/README.md` & `irisml-tasks-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 Visit [irisml](https://github.com/microsoft/irisml) for the detail.
 
 ## tasks
 ### assertion
 This task throws an exception if the given assertion failed for the input object.
 
+## branch
+'If' condition for tasks.
+
 ### calculate_cosine_similarity
 Calculate cosine similarity between two sets of vectors.
 
 ### download_azure_blob
 Download a file from azure blob.
 
 ### get_current_time
```

### Comparing `irisml-tasks-0.0.8/irisml/tasks/assertion.py` & `irisml-tasks-0.0.9/irisml/tasks/assertion.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/calculate_cosine_similarity.py` & `irisml-tasks-0.0.9/irisml/tasks/calculate_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/download_azure_blob.py` & `irisml-tasks-0.0.9/irisml/tasks/download_azure_blob.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_dataset_split.py` & `irisml-tasks-0.0.9/irisml/tasks/get_dataset_split.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_dataset_stats.py` & `irisml-tasks-0.0.9/irisml/tasks/get_dataset_stats.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_dataset_subset.py` & `irisml-tasks-0.0.9/irisml/tasks/get_dataset_subset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_fake_image_classification_dataset.py` & `irisml-tasks-0.0.9/irisml/tasks/get_fake_image_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_fake_object_detection_dataset.py` & `irisml-tasks-0.0.9/irisml/tasks/get_fake_object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_item.py` & `irisml-tasks-0.0.9/irisml/tasks/get_item.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_secret_from_azure_keyvault.py` & `irisml-tasks-0.0.9/irisml/tasks/get_secret_from_azure_keyvault.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/get_topk.py` & `irisml-tasks-0.0.9/irisml/tasks/get_topk.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/join_filepath.py` & `irisml-tasks-0.0.9/irisml/tasks/join_filepath.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/load_state_dict.py` & `irisml-tasks-0.0.9/irisml/tasks/load_state_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,32 @@
     """Load a state_dict from various sources.
 
     Supported sources are:
         1. a dictionary object. Use Inputs.state_dict.
         2. a bytes object. Use Inputs.state_dict_bytes.
         3. a file on local filesystem. Use Config.path.
 
-    If config.strict is False, mismatched or missing parameters will be ignored.
+    Config:
+        path (pathlib.Path): [optional] A file path to the state_dict.
+        strict (bool): Load state_dict in strict mode
+        ignore_shape_mismatch (bool): If True, ignore weights with a wrong shape. 'strict' must be False.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.1.1'
 
     @dataclasses.dataclass
     class Inputs:
         model: torch.nn.Module
         state_dict: typing.Optional[typing.Dict] = None
         state_dict_bytes: typing.Optional[bytes] = None
 
     @dataclasses.dataclass
     class Config:
         path: typing.Optional[pathlib.Path] = None
         strict: bool = True
+        ignore_shape_mismatch: bool = False
 
     @dataclasses.dataclass
     class Outputs:
         model: torch.nn.Module
 
     def execute(self, inputs: Inputs):
         num_sources = len([x for x in [inputs.state_dict, inputs.state_dict_bytes, self.config.path] if x])
@@ -48,22 +52,22 @@
             state_dict = torch.load(io.BytesIO(inputs.state_dict_bytes), map_location='cpu')
         elif self.config.path:
             state_dict = torch.load(self._config.path, map_location='cpu')
 
         if not state_dict:
             raise ValueError("Failed to load the state_dict.")
 
-        if not self.config.strict:
+        if self.config.ignore_shape_mismatch:
             # Filter parameters with different shape.
             existing_state_dict = inputs.model.state_dict()
-            new_state_dict = {k: v for k, v in state_dict.items() if k in existing_state_dict and v.shape == existing_state_dict[k].shape}
+            new_state_dict = {k: v for k, v in state_dict.items() if k not in existing_state_dict or v.shape == existing_state_dict[k].shape}
 
             ignored_keys = set(state_dict) - set(new_state_dict)
-            if ignored_keys:
-                logger.info(f"Ignored {ignored_keys} since they are redundant or they have different shapes.")
+            for key in ignored_keys:
+                logger.info(f"Ignored {key} in the state_dict because it has unexpected shape. Actual: {state_dict[key].shape}, Expected: {existing_state_dict[key].shape}")
 
             state_dict = new_state_dict
 
         model = copy.deepcopy(inputs.model)
         model.load_state_dict(state_dict, strict=self.config.strict)
         return self.Outputs(model)
```

### Comparing `irisml-tasks-0.0.8/irisml/tasks/run_parallel.py` & `irisml-tasks-0.0.9/irisml/tasks/run_parallel.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/run_sequential.py` & `irisml-tasks-0.0.9/irisml/tasks/run_sequential.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/save_file.py` & `irisml-tasks-0.0.9/irisml/tasks/save_file.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/save_state_dict.py` & `irisml-tasks-0.0.9/irisml/tasks/save_state_dict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/search_grid_sequential.py` & `irisml-tasks-0.0.9/irisml/tasks/search_grid_sequential.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml/tasks/upload_azure_blob.py` & `irisml-tasks-0.0.9/irisml/tasks/upload_azure_blob.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/irisml_tasks.egg-info/PKG-INFO` & `irisml-tasks-0.0.9/irisml_tasks.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Standard tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,14 +15,17 @@
 
 Visit [irisml](https://github.com/microsoft/irisml) for the detail.
 
 ## tasks
 ### assertion
 This task throws an exception if the given assertion failed for the input object.
 
+## branch
+'If' condition for tasks.
+
 ### calculate_cosine_similarity
 Calculate cosine similarity between two sets of vectors.
 
 ### download_azure_blob
 Download a file from azure blob.
 
 ### get_current_time
```

### Comparing `irisml-tasks-0.0.8/irisml_tasks.egg-info/SOURCES.txt` & `irisml-tasks-0.0.9/irisml_tasks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 irisml/tasks/assertion.py
+irisml/tasks/branch.py
 irisml/tasks/calculate_cosine_similarity.py
 irisml/tasks/download_azure_blob.py
 irisml/tasks/get_current_time.py
 irisml/tasks/get_dataset_split.py
 irisml/tasks/get_dataset_stats.py
 irisml/tasks/get_dataset_subset.py
 irisml/tasks/get_fake_image_classification_dataset.py
@@ -24,14 +25,15 @@
 irisml/tasks/upload_azure_blob.py
 irisml_tasks.egg-info/PKG-INFO
 irisml_tasks.egg-info/SOURCES.txt
 irisml_tasks.egg-info/dependency_links.txt
 irisml_tasks.egg-info/requires.txt
 irisml_tasks.egg-info/top_level.txt
 test/test_assertion.py
+test/test_branch.py
 test/test_calculate_cosine_similarity.py
 test/test_get_current_time.py
 test/test_get_dataset_split.py
 test/test_get_dataset_stats.py
 test/test_get_dataset_subset.py
 test/test_get_fake_image_classification_dataset.py
 test/test_get_fake_object_detection_dataset.py
```

### Comparing `irisml-tasks-0.0.8/setup.cfg` & `irisml-tasks-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks
-version = 0.0.8
+version = 0.0.9
 url = https://github.com/microsoft/irisml-tasks
 description = Standard tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-0.0.8/test/test_assertion.py` & `irisml-tasks-0.0.9/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_calculate_cosine_similarity.py` & `irisml-tasks-0.0.9/test/test_calculate_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_dataset_split.py` & `irisml-tasks-0.0.9/test/test_get_dataset_split.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_dataset_stats.py` & `irisml-tasks-0.0.9/test/test_get_dataset_stats.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_dataset_subset.py` & `irisml-tasks-0.0.9/test/test_get_dataset_subset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_fake_image_classification_dataset.py` & `irisml-tasks-0.0.9/test/test_get_fake_image_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_fake_object_detection_dataset.py` & `irisml-tasks-0.0.9/test/test_get_fake_object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_secret_from_azure_keyvault.py` & `irisml-tasks-0.0.9/test/test_get_secret_from_azure_keyvault.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_get_topk.py` & `irisml-tasks-0.0.9/test/test_get_topk.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_join_filepath.py` & `irisml-tasks-0.0.9/test/test_join_filepath.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_load_state_dict.py` & `irisml-tasks-0.0.9/test/test_load_state_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         with self.assertRaises(ValueError):
             task.execute(inputs)
 
     def test_different_shape(self):
         fake_model = torch.nn.Conv2d(3, 4, 3)
         fake_model2 = torch.nn.Conv2d(3, 3, 3)
 
-        # It will be ignored if strict == False
-        Task(Task.Config(strict=False)).execute(Task.Inputs(model=fake_model, state_dict=fake_model2.state_dict()))
+        # It will be ignored if ignore_shape_mismatch=True
+        Task(Task.Config(strict=False, ignore_shape_mismatch=True)).execute(Task.Inputs(model=fake_model, state_dict=fake_model2.state_dict()))
 
         with self.assertRaises(RuntimeError):
-            Task(Task.Config(strict=True)).execute(Task.Inputs(model=fake_model, state_dict=fake_model2.state_dict()))
+            Task(Task.Config(strict=False)).execute(Task.Inputs(model=fake_model, state_dict=fake_model2.state_dict()))
 
     def _is_equal_state_dict(self, state_dict1, state_dict2):
         if set(state_dict1) != set(state_dict2):
             return False
 
         for key in state_dict1:
             if not torch.equal(state_dict1[key], state_dict2[key]):
```

### Comparing `irisml-tasks-0.0.8/test/test_run_parallel.py` & `irisml-tasks-0.0.9/test/test_run_parallel.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_run_sequential.py` & `irisml-tasks-0.0.9/test/test_run_sequential.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_save_file.py` & `irisml-tasks-0.0.9/test/test_save_file.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_save_state_dict.py` & `irisml-tasks-0.0.9/test/test_save_state_dict.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-0.0.8/test/test_search_grid_sequential.py` & `irisml-tasks-0.0.9/test/test_search_grid_sequential.py`

 * *Files identical despite different names*

