# Comparing `tmp/falcon-integration-gateway-3.1.8.tar.gz` & `tmp/falcon-integration-gateway-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon-integration-gateway-3.1.8.tar", last modified: Fri Feb  3 14:43:39 2023, max compression
+gzip compressed data, was "falcon-integration-gateway-3.1.9.tar", last modified: Fri Apr  7 20:07:17 2023, max compression
```

## Comparing `falcon-integration-gateway-3.1.8.tar` & `falcon-integration-gateway-3.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.205124 falcon-integration-gateway-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-02-03 14:43:39.205124 falcon-integration-gateway-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/aws_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/aws_sqs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/chronicle/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/chronicle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/cloudtrail_lake/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/cloudtrail_lake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/cloudtrail_lake/cloudtrail_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/gcp/api/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/gcp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/gcp/api/scc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/workspaceone/
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/workspaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/backends/workspaceone/serverlog/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/backends/workspaceone/serverlog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/config/
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/falcon/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/rtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/falcon_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-02-03 14:43:39.000000 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-03 14:43:39.000000 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:43:39.000000 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-03 14:43:39.000000 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-03 14:43:39.000000 falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.201124 falcon-integration-gateway-3.1.8/fig/log/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.205124 falcon-integration-gateway-3.1.8/fig/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:43:39.205124 falcon-integration-gateway-3.1.8/fig/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/util/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/fig/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-03 14:43:39.205124 falcon-integration-gateway-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-03 14:43:29.000000 falcon-integration-gateway-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/aws_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/aws_sqs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/chronicle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/chronicle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/cloudtrail_lake/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/cloudtrail_lake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/cloudtrail_lake/cloudtrail_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.526381 falcon-integration-gateway-3.1.9/fig/backends/gcp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/gcp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/gcp/api/scc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/backends/workspaceone/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/workspaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/backends/workspaceone/serverlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/backends/workspaceone/serverlog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/rtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/falcon_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-07 20:07:17.000000 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-07 20:07:17.000000 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:07:17.000000 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 20:07:17.000000 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 20:07:17.000000 falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/fig/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/util/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/fig/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-07 20:07:17.530381 falcon-integration-gateway-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-07 20:07:04.000000 falcon-integration-gateway-3.1.9/setup.py
```

### Comparing `falcon-integration-gateway-3.1.8/LICENSE` & `falcon-integration-gateway-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/PKG-INFO` & `falcon-integration-gateway-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-integration-gateway
-Version: 3.1.8
+Version: 3.1.9
 Summary: The CrowdStrike Demo Falcon Integration Gateway for GCP
 Home-page: https://github.com/crowdstrike/falcon-integration-gateway
 Author: CRWD Solution Architects
 Author-email: integrations@crowdstrike.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
```

### Comparing `falcon-integration-gateway-3.1.8/README.md` & `falcon-integration-gateway-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/__main__.py` & `falcon-integration-gateway-3.1.9/fig/__main__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/aws/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/aws_sqs/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/aws_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/azure/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/chronicle/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/chronicle/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/cloudtrail_lake/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/cloudtrail_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/cloudtrail_lake/cloudtrail_offset.py` & `falcon-integration-gateway-3.1.9/fig/backends/cloudtrail_lake/cloudtrail_offset.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/gcp/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/gcp/api/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/gcp/api/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/gcp/api/scc.py` & `falcon-integration-gateway-3.1.9/fig/backends/gcp/api/scc.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/workspaceone/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/workspaceone/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/backends/workspaceone/serverlog/__init__.py` & `falcon-integration-gateway-3.1.9/fig/backends/workspaceone/serverlog/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/config/__init__.py` & `falcon-integration-gateway-3.1.9/fig/config/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon/api.py` & `falcon-integration-gateway-3.1.9/fig/falcon/api.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon/models.py` & `falcon-integration-gateway-3.1.9/fig/falcon/models.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon/rtr.py` & `falcon-integration-gateway-3.1.9/fig/falcon/rtr.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon/stream.py` & `falcon-integration-gateway-3.1.9/fig/falcon/stream.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon_data.py` & `falcon-integration-gateway-3.1.9/fig/falcon_data.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/PKG-INFO` & `falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon-integration-gateway
-Version: 3.1.8
+Version: 3.1.9
 Summary: The CrowdStrike Demo Falcon Integration Gateway for GCP
 Home-page: https://github.com/crowdstrike/falcon-integration-gateway
 Author: CRWD Solution Architects
 Author-email: integrations@crowdstrike.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
```

### Comparing `falcon-integration-gateway-3.1.8/fig/falcon_integration_gateway.egg-info/SOURCES.txt` & `falcon-integration-gateway-3.1.9/fig/falcon_integration_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/queue/__init__.py` & `falcon-integration-gateway-3.1.9/fig/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/fig/worker.py` & `falcon-integration-gateway-3.1.9/fig/worker.py`

 * *Files identical despite different names*

### Comparing `falcon-integration-gateway-3.1.8/setup.py` & `falcon-integration-gateway-3.1.9/setup.py`

 * *Files identical despite different names*

