# Comparing `tmp/dequeai-0.666.tar.gz` & `tmp/dequeai-0.668.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.666.tar", last modified: Fri Apr  7 18:32:01 2023, max compression
+gzip compressed data, was "dequeai-0.668.tar", last modified: Fri Apr  7 18:40:07 2023, max compression
```

## Comparing `dequeai-0.666.tar` & `dequeai-0.668.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:32:01.890736 dequeai-0.666/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:32:01.890736 dequeai-0.666/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:32:01.890736 dequeai-0.666/dequeai/
--rw-r--r--   0 root         (0) root         (0)      228 2023-03-27 20:50:58.000000 dequeai-0.666/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.666/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.666/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.666/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-03-27 20:54:31.000000 dequeai-0.666/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    19322 2023-04-07 17:56:48.000000 dequeai-0.666/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.666/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.666/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.666/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.666/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:32:01.890736 dequeai-0.666/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:32:01.000000 dequeai-0.666/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 18:32:01.000000 dequeai-0.666/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 18:32:01.000000 dequeai-0.666/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 18:32:01.000000 dequeai-0.666/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 18:32:01.000000 dequeai-0.666/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 18:32:01.890736 dequeai-0.666/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 18:31:49.000000 dequeai-0.666/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:40:07.927650 dequeai-0.668/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:40:07.927650 dequeai-0.668/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:40:07.927650 dequeai-0.668/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-03-27 20:50:58.000000 dequeai-0.668/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.668/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.668/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.668/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-04-07 18:39:54.000000 dequeai-0.668/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    19320 2023-04-07 18:39:54.000000 dequeai-0.668/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.668/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.668/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.668/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.668/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:40:07.927650 dequeai-0.668/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:40:07.000000 dequeai-0.668/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 18:40:07.000000 dequeai-0.668/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 18:40:07.000000 dequeai-0.668/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 18:40:07.000000 dequeai-0.668/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 18:40:07.000000 dequeai-0.668/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 18:40:07.927650 dequeai-0.668/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 18:39:54.000000 dequeai-0.668/setup.py
```

### Comparing `dequeai-0.666/dequeai/datatypes.py` & `dequeai-0.668/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.666/dequeai/dequeai_run.py` & `dequeai-0.668/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,19 +403,19 @@
         req_data = {"user_name": self.user_name, "latest": latest, "label": label,
                     "project_name": self._project_name, "run_id": self._run_id, "tags": tags}
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/artifacts/register/",
                              json=req_data)
         res = resp.json()
         print(res)
 
-    def load_artifact(self, user_name, run_id, artifact_type):
+    def load_artifact(self,  artifact_type):
         # Fetch artifact metadata
         req_data = {
-            "user_name": user_name,
-            "run_id": run_id,
+            "user_name": self.user_name,
+            "run_id": self._run_id,
             "artifact_type": artifact_type
         }
         resp = requests.get(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/read/", json=req_data)
         metadata = resp.json()
 
         # Check if metadata exists
         if not metadata:
@@ -423,15 +423,15 @@
             return
 
         artifact_uris = metadata["artifact_uris"]
 
         # Download the artifacts using the artifact URIs
         for artifact_uri in artifact_uris:
             req_data = {
-                "user_name": user_name,
+                "user_name": self.user_name,
                 "artifact_uri": artifact_uri
             }
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/drive/contents/download/presigned_url/read/",
                                  json=req_data)
             res = resp.json()
 
             # Download the artifact using the pre-signed URL
```

### Comparing `dequeai-0.666/dequeai/parsing_service.py` & `dequeai-0.668/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.666/dequeai/rest_connect.py` & `dequeai-0.668/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.666/dequeai/util.py` & `dequeai-0.668/dequeai/util.py`

 * *Files identical despite different names*

