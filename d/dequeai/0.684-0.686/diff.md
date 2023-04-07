# Comparing `tmp/dequeai-0.684.tar.gz` & `tmp/dequeai-0.686.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.684.tar", last modified: Fri Apr  7 18:57:01 2023, max compression
+gzip compressed data, was "dequeai-0.686.tar", last modified: Fri Apr  7 19:00:13 2023, max compression
```

## Comparing `dequeai-0.684.tar` & `dequeai-0.686.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:57:01.378002 dequeai-0.684/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:57:01.378002 dequeai-0.684/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:57:01.374002 dequeai-0.684/dequeai/
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-07 18:40:49.000000 dequeai-0.684/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.684/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.684/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.684/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-07 18:51:21.000000 dequeai-0.684/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    19325 2023-04-07 18:56:38.000000 dequeai-0.684/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.684/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.684/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.684/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.684/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 18:57:01.378002 dequeai-0.684/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 18:57:00.000000 dequeai-0.684/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 18:57:01.000000 dequeai-0.684/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 18:57:00.000000 dequeai-0.684/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 18:57:01.000000 dequeai-0.684/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 18:57:01.000000 dequeai-0.684/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 18:57:01.378002 dequeai-0.684/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 18:56:47.000000 dequeai-0.684/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 19:00:13.598715 dequeai-0.686/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-04-07 18:40:49.000000 dequeai-0.686/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.686/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.686/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-04-07 18:51:21.000000 dequeai-0.686/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    19333 2023-04-07 18:59:51.000000 dequeai-0.686/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.686/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.686/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 19:00:13.598715 dequeai-0.686/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 19:00:00.000000 dequeai-0.686/setup.py
```

### Comparing `dequeai-0.684/dequeai/datatypes.py` & `dequeai-0.686/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.684/dequeai/dequeai.py` & `dequeai-0.686/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.684/dequeai/dequeai_run.py` & `dequeai-0.686/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
         artifact_uris = metadata["artifact_uris"]
 
         # Download the artifacts using the artifact URIs
         for artifact_uri in artifact_uris:
             req_data = {
                 "user_name": self.user_name,
-                "artifact_uri": artifact_uri
+                "complete_object_path": artifact_uri
             }
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/drive/contents/download/presigned_url/read/",
                                  json=req_data)
             res = resp.json()
 
             # Download the artifact using the pre-signed URL
             http_response = requests.get(url=res["url"])
```

### Comparing `dequeai-0.684/dequeai/parsing_service.py` & `dequeai-0.686/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.684/dequeai/rest_connect.py` & `dequeai-0.686/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.684/dequeai/util.py` & `dequeai-0.686/dequeai/util.py`

 * *Files identical despite different names*

