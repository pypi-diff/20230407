# Comparing `tmp/responsibleai_tabular_automl-0.2.2.tar.gz` & `tmp/responsibleai_tabular_automl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_tabular_automl-0.2.2.tar", last modified: Mon Mar 20 18:32:18 2023, max compression
+gzip compressed data, was "responsibleai_tabular_automl-0.2.3.tar", last modified: Fri Apr  7 16:26:17 2023, max compression
```

## Comparing `responsibleai_tabular_automl-0.2.2.tar` & `responsibleai_tabular_automl-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 18:32:18.620057 responsibleai_tabular_automl-0.2.2/
--rw-rw-rw-   0        0        0      778 2023-03-20 18:32:18.620057 responsibleai_tabular_automl-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 18:32:18.573548 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/
--rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/__init__.py
--rw-rw-rw-   0        0        0     6104 2023-03-11 03:45:17.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/_loggerfactory.py
--rw-rw-rw-   0        0        0    11682 2023-03-20 18:12:19.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/automl_inference_run.py
--rw-rw-rw-   0        0        0    10000 2023-03-20 18:11:43.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/rai_automl.py
--rw-rw-rw-   0        0        0      210 2023-03-20 18:16:58.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/version.py
-drwxrwxrwx   0        0        0        0 2023-03-20 18:32:18.604388 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/
--rw-rw-rw-   0        0        0      778 2023-03-20 18:32:18.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-03-20 18:32:18.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 18:32:18.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-03-20 18:32:18.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-03-20 18:32:18.000000 responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 18:32:18.620057 responsibleai_tabular_automl-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 18:32:18.620057 responsibleai_tabular_automl-0.2.2/tests/
--rw-rw-rw-   0        0        0     1654 2023-03-10 18:46:03.000000 responsibleai_tabular_automl-0.2.2/tests/test_rai_automl.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/
+-rw-rw-rw-   0        0        0      778 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.462535 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/
+-rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/__init__.py
+-rw-rw-rw-   0        0        0     6104 2023-03-11 03:45:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/_loggerfactory.py
+-rw-rw-rw-   0        0        0    11682 2023-03-28 18:22:08.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/automl_inference_run.py
+-rw-rw-rw-   0        0        0    10433 2023-04-07 16:22:59.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/rai_automl.py
+-rw-rw-rw-   0        0        0      210 2023-04-07 16:23:50.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/version.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.510432 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/
+-rw-rw-rw-   0        0        0      778 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/tests/
+-rw-rw-rw-   0        0        0     1654 2023-03-30 17:25:44.000000 responsibleai_tabular_automl-0.2.3/tests/test_rai_automl.py
```

### Comparing `responsibleai_tabular_automl-0.2.2/PKG-INFO` & `responsibleai_tabular_automl-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_tabular_automl
-Version: 0.2.2
+Version: 0.2.3
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/_loggerfactory.py` & `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/_loggerfactory.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/automl_inference_run.py` & `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/automl_inference_run.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl/rai_automl.py` & `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/rai_automl.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 @track(_get_logger)
 def _compute_and_upload_rai_insights_internal(
     current_run: Run, automl_child_run: Run
 ):
     automl_child_run.download_files("outputs/rai")
 
+    print("Generating RAI insights for AutoML child run")
     _ai_logger.info("Generating RAI insights for AutoML child run")
 
     metadata = None
     with open("outputs/rai/metadata.json", "r") as fp:
         metadata = json.load(fp)
 
     train = pd.read_parquet("outputs/rai/train.df.parquet")
@@ -122,27 +123,29 @@
             test=test,
             target_column=target_column_name,
             categorical_features=categorical_features,
             task_type=task_type,
             classes=classes,
         )
         rai_insights.explainer.add()
+        rai_insights.error_analysis.add()
         rai_insights.compute()
         rai_insights.save("dashboard")
         current_run.upload_folder("dashboard", "dashboard")
 
         rai_data = rai_insights.get_data()
         rai_dict = serialize_json_safe(rai_data)
         ux_json_path = Path("ux_json")
         ux_json_path.mkdir(parents=True, exist_ok=True)
         json_filename = ux_json_path / "dashboard.json"
         with open(json_filename, "w") as json_file:
             json.dump(rai_dict, json_file)
         current_run.upload_folder("ux_json", "ux_json")
         automl_child_run.tag("model_rai", "True")
+        print("Successfully generated and uploaded the RAI insights")
         _ai_logger.info("Successfully generated and uploaded the RAI insights")
     else:
         warnings.warn("Currently RAI is not supported for "
                       "text and datetime features")
         _ai_logger.info("Currently RAI is not supported for "
                         "text and datetime features")
     current_run.complete()
@@ -202,14 +205,16 @@
         output = str(e)
     return (success, output)
 
 
 @track(_get_logger)
 def execute_automl_inference_script(automl_child_run_id, ws):
     automl_run = ws.get_run(automl_child_run_id)
+    print("Generating predictions for AutoML model")
+    _ai_logger.info("Generating predictions for AutoML model")
 
     command = ["pip", "list"]
     success, output = call_with_output(command)
 
     automl_run.download_file("outputs/mlflow-model/conda.yaml", "conda.yaml")
     automl_env_name = "automl_env_" + str(time.time())
     command = [
@@ -249,14 +254,16 @@
         "env",
         "remove",
         "--name",
         automl_env_name,
         "-y"
     ]
     success, output = call_with_output(command)
+    print("Successfully generated predictions for AutoML model")
+    _ai_logger.info("Successfully generated predictions for AutoML model")
 
 
 @track(_get_logger)
 def compute_and_upload_rai_insights(
     automl_parent_run_id: Optional[str] = None,
     automl_child_run_id: Optional[str] = None
 ):
```

### Comparing `responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/PKG-INFO` & `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-tabular-automl
-Version: 0.2.2
+Version: 0.2.3
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.2.2/responsibleai_tabular_automl.egg-info/SOURCES.txt` & `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.2/setup.py` & `responsibleai_tabular_automl-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.2/tests/test_rai_automl.py` & `responsibleai_tabular_automl-0.2.3/tests/test_rai_automl.py`

 * *Files identical despite different names*

