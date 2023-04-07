# Comparing `tmp/dequeai-0.680.tar.gz` & `tmp/dequeai-0.682.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.680.tar", last modified: Fri Apr  7 18:46:48 2023, max compression
+gzip compressed data, was "dequeai-0.682.tar", last modified: Fri Apr  7 18:51:47 2023, max compression
```

## Comparing `dequeai-0.680.tar` & `dequeai-0.682.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:46:47.992131 dequeai-0.680/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:46:47.992131 dequeai-0.680/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:46:47.992131 dequeai-0.680/dequeai/
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-07 18:40:49.000000 dequeai-0.680/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.680/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.680/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.680/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-04-07 18:46:13.000000 dequeai-0.680/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    19389 2023-04-07 18:46:33.000000 dequeai-0.680/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.680/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.680/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.680/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.680/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:46:47.992131 dequeai-0.680/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:46:47.000000 dequeai-0.680/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 18:46:47.000000 dequeai-0.680/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 18:46:47.000000 dequeai-0.680/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 18:46:47.000000 dequeai-0.680/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 18:46:47.000000 dequeai-0.680/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 18:46:47.992131 dequeai-0.680/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 18:46:33.000000 dequeai-0.680/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:51:47.208940 dequeai-0.682/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:51:47.208940 dequeai-0.682/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:51:47.208940 dequeai-0.682/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-07 18:40:49.000000 dequeai-0.682/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.682/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.682/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.682/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-04-07 18:51:21.000000 dequeai-0.682/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    19324 2023-04-07 18:51:21.000000 dequeai-0.682/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.682/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.682/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.682/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.682/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:51:47.208940 dequeai-0.682/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:51:46.000000 dequeai-0.682/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 18:51:47.000000 dequeai-0.682/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 18:51:46.000000 dequeai-0.682/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 18:51:47.000000 dequeai-0.682/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 18:51:47.000000 dequeai-0.682/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 18:51:47.208940 dequeai-0.682/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 18:51:33.000000 dequeai-0.682/setup.py
```

### Comparing `dequeai-0.680/dequeai/datatypes.py` & `dequeai-0.682/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.680/dequeai/dequeai.py` & `dequeai-0.682/dequeai/dequeai.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 
 def log( data, step=None, commit=True):
     run.log(data, step, commit)
 
 def log_artifact(artifact_type, path):
     run.log_artifact(artifact_type, path)
 
-def load_artifact(artifact_type, run_id=None):
+def load_artifact(artifact_type, run_id):
     run.load_artifact(artifact_type, run_id)
 
 
 def register_artifacts(latest=True, label=None, tags=None):
     run.register_artifacts(latest, label, tags)
```

### Comparing `dequeai-0.680/dequeai/dequeai_run.py` & `dequeai-0.682/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,18 +403,17 @@
         req_data = {"user_name": self.user_name, "latest": latest, "label": label,
                     "project_name": self._project_name, "run_id": self._run_id, "tags": tags}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/artifacts/register/",
                              json=req_data)
         res = resp.json()
         print(res)
 
-    def load_artifact(self,  artifact_type, run_id=None):
+    def load_artifact(self,  artifact_type, run_id):
         # Fetch artifact metadata
-        if run_id is None:
-            run_id = self._run_id
+
 
         req_data = {
             "user_name": self.user_name,
             "run_id": run_id,
             "artifact_type": artifact_type
         }
         resp = requests.get(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/read/", json=req_data)
```

### Comparing `dequeai-0.680/dequeai/parsing_service.py` & `dequeai-0.682/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.680/dequeai/rest_connect.py` & `dequeai-0.682/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.680/dequeai/util.py` & `dequeai-0.682/dequeai/util.py`

 * *Files identical despite different names*

