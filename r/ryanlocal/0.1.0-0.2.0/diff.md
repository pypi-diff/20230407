# Comparing `tmp/ryanlocal-0.1.0.tar.gz` & `tmp/ryanlocal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryanlocal-0.1.0.tar", max compression
+gzip compressed data, was "ryanlocal-0.2.0.tar", max compression
```

## Comparing `ryanlocal-0.1.0.tar` & `ryanlocal-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-07 19:41:12.530411 ryanlocal-0.1.0/README.md
--rw-r--r--   0        0        0      446 2023-04-07 20:42:35.563156 ryanlocal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 19:41:12.530077 ryanlocal-0.1.0/ryanlocal/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-07 20:34:52.589516 ryanlocal-0.1.0/ryanlocal/__main__.py
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 ryanlocal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 19:41:12.530411 ryanlocal-0.2.0/README.md
+-rw-r--r--   0        0        0      446 2023-04-07 20:43:46.173938 ryanlocal-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 19:41:12.530077 ryanlocal-0.2.0/ryanlocal/__init__.py
+-rw-r--r--   0        0        0     1228 2023-04-07 20:43:27.470044 ryanlocal-0.2.0/ryanlocal/__main__.py
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 ryanlocal-0.2.0/PKG-INFO
```

### Comparing `ryanlocal-0.1.0/ryanlocal/__main__.py` & `ryanlocal-0.2.0/ryanlocal/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 URL = "https://api.sandbox1.unit21.com/v1/imports/pre-signed-url/create"
 API_KEY = "b361917de20a0c9b18f15f2134dc59ccf45297862f5e80561ae0abdf41"
 STREAM_HAME = "ryanlocal"
 
 
 def get_and_post_presigned_url(file_path):
-    ## get presigned url
+    # get presigned url
     headers = {
         "accept": "application/json",
         "content-type": "application/json",
         "u21-key": API_KEY,
     }
 
     body = {"stream_name": "ryanlocal", "file_name": file_path.name}
     response = requests.post(URL, headers=headers, json=body)
     response.raise_for_status()
     resp_json = response.json()
     print(resp_json)
 
+    # upload file to the presigned url
     upload_response = requests.post(
         # the url from the previous call
         resp_json.get("url"),
         # dictionary from previous call used as form params
         data=resp_json.get("form_fields"),
         # file descriptor dictionary of the actual file
         files={"file": file_path.open("rb")},
```

