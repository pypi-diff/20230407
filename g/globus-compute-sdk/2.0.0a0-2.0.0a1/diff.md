# Comparing `tmp/globus-compute-sdk-2.0.0a0.tar.gz` & `tmp/globus-compute-sdk-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.0.0a0.tar", last modified: Tue Mar 21 20:57:46 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.0.0a1.tar", last modified: Mon Apr  3 22:15:05 2023, max compression
```

## Comparing `globus-compute-sdk-2.0.0a0.tar` & `globus-compute-sdk-2.0.0a1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.516166 globus-compute-sdk-2.0.0a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      770 2023-03-21 20:57:46.516239 globus-compute-sdk-2.0.0a0/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.503117 globus-compute-sdk-2.0.0a0/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.504182 globus-compute-sdk-2.0.0a0/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.505985 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      970 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.506787 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      723 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11442 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    27463 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46343 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.508885 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1743 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-03-21 20:31:37.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7544 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      783 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     2476 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/whoami.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/search.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.515197 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8960 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.516007 globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      100 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1680 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7511 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     3737 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-03-21 20:56:51.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-21 20:57:46.503801 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      770 2023-03-21 20:57:46.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1590 2023-03-21 20:57:46.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-03-21 20:57:46.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      379 2023-03-21 20:57:46.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-03-21 20:57:46.000000 globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-03-21 20:57:46.516576 globus-compute-sdk-2.0.0a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2691 2023-03-21 20:00:23.000000 globus-compute-sdk-2.0.0a0/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.923487 globus-compute-sdk-2.0.0a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-03 22:15:05.923533 globus-compute-sdk-2.0.0a1/PKG-INFO
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.919263 globus-compute-sdk-2.0.0a1/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.920152 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.921161 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.921628 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      723 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    27431 2023-04-03 17:23:22.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46343 2023-04-03 17:23:20.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.922695 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7544 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      783 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     2476 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/whoami.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/search.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.922924 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8421 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.923385 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-03 22:12:27.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.919895 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1590 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      379 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-03 22:15:05.923778 globus-compute-sdk-2.0.0a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     2691 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/setup.py
```

### Comparing `globus-compute-sdk-2.0.0a0/LICENSE` & `globus-compute-sdk-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/PKG-INFO` & `globus-compute-sdk-2.0.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,14 @@
         Returns
         -------
         function uuid : str
             UUID identifier for the registered function
         """
         data = FunctionRegistrationData(
             function=function,
-            failover_source="",
             container_uuid=container_uuid,
             entry_point=function_name,
             description=description,
             public=public,
             group=group,
             searchable=searchable,
             serializer=self.fx_serializer,
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 _REGISTERED_FXEXECUTORS: dict[int, t.Any] = {}
 
 
 def __executor_atexit():
     threading.main_thread().join()
     to_shutdown = list(_REGISTERED_FXEXECUTORS.values())
     while to_shutdown:
-        fxe = to_shutdown.pop()
-        fxe.shutdown()
+        gce = to_shutdown.pop()
+        gce.shutdown()
 
 
 threading.Thread(target=__executor_atexit).start()
 
 
 class TaskSubmissionInfo:
     def __init__(
@@ -202,16 +202,16 @@
         """
         The Task Group with which this instance is currently associated.  New tasks will
         be sent to this Task Group upstream, and the result listener will only listen
         for results for this group.
 
         Must be a string.  Set by simple assignment::
 
-            fxe = Executor(endpoint_id="...")
-            fxe.task_group_id = "Some-stored-id"
+            gce = Executor(endpoint_id="...")
+            gce.task_group_id = "Some-stored-id"
 
         This is typically used when reattaching to a previously initiated set of tasks.
         See `reload_tasks()`_ for more information.
 
         [default: ``None``, which translates to the Client task group id]
         """
         return self._task_group_id
@@ -295,16 +295,16 @@
         Schedules the callable to be executed as ``fn(*args, **kwargs)`` and
         returns a ComputeFuture instance representing the execution of the
         callable.
 
         Example use::
 
             >>> def add(a: int, b: int) -> int: return a + b
-            >>> fxe = Executor(endpoint_id="some-ep-id")
-            >>> fut = fxe.submit(add, 1, 2)
+            >>> gce = Executor(endpoint_id="some-ep-id")
+            >>> fut = gce.submit(add, 1, 2)
             >>> fut.result()    # wait (block) until result is received from remote
             3
 
         :param fn: Python function to execute on endpoint
         :param args: positional arguments (if any) as required to execute
             the function
         :param kwargs: keyword arguments (if any) as required to execute
@@ -341,16 +341,16 @@
             # pre_registration.py
             from globus_compute_sdk import Executor
 
             def some_processor(*args, **kwargs):
                 # ... function logic ...
                 return ["some", "result"]
 
-            fxe = Executor()
-            fn_id = fxe.register_function(some_processor)
+            gce = Executor()
+            fn_id = gce.register_function(some_processor)
             print(f"Function registered successfully.\\nFunction ID: {fn_id}")
 
             # Example output:
             #
             # Function registered successfully.
             # Function ID: c407ae80-b31f-447a-9fa6-124098492057
 
@@ -384,16 +384,16 @@
             err_fmt = "%s is shutdown; no new functions may be executed"
             raise RuntimeError(err_fmt % repr(self))
 
         if not self.endpoint_id:
             msg = (
                 "No endpoint_id set.  Did you forget to set it at construction?\n"
                 "  Hint:\n\n"
-                "    fxe = Executor(endpoint_id=<ep_id>)\n"
-                "    fxe.endpoint_id = <ep_id>    # alternative"
+                "    gce = Executor(endpoint_id=<ep_id>)\n"
+                "    gce.endpoint_id = <ep_id>    # alternative"
             )
             self.shutdown(wait=False, cancel_futures=True)
             raise ValueError(msg)
 
         if args is None:
             args = ()
         if kwargs is None:
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,13 +48,14 @@
 
     client_id, client_secret = _get_client_creds_from_env()
 
     try:
         uuid.UUID(client_id)
     except ValueError:
         log.warning(
-            "VERY LIKELY INVALID CLIENT ID (did you copy the username and not the id?"
+            "VERY LIKELY INVALID CLIENT ID (did you copy the username and not the id?)"
+            f"\n  Received: '{client_id}'"
         )
     return globus_sdk.ConfidentialAppAuthClient(
         client_id=str(client_id),
         client_secret=str(client_secret),
     )
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/search.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/search.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/web_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 This module implements a Globus SDK client class suitable for use with the
 Globus Compute web service.
 
 It also implements data helpers for building complex payloads. Most notably,
 `FunctionRegistrationData` which can be constructed from an arbitrary callable.
 """
-import inspect
 import json
 import typing as t
 import uuid
 
 import globus_sdk
 from globus_compute_common.sdk_version_sharing import user_agent_substring
 from globus_compute_sdk.sdk._environments import get_web_service_url
@@ -30,60 +29,47 @@
 class FunctionRegistrationData:
     def __init__(
         self,
         *,
         function: t.Optional[t.Callable] = None,
         function_name: t.Optional[str] = None,
         function_code: t.Optional[str] = None,
-        function_source: t.Optional[str] = None,
-        failover_source: t.Optional[str] = None,
         container_uuid: t.Optional[ID_PARAM_T] = None,
         entry_point: t.Optional[str] = None,
         description: t.Optional[str] = None,
         public: bool = False,
         group: t.Optional[str] = None,
         searchable: bool = True,
         serializer: t.Optional[ComputeSerializer] = None,
     ):
         if function is not None:
             function_name = function.__name__
             function_code = _get_packed_code(function, serializer=serializer)
 
-            if function_source is None:
-                try:
-                    function_source = inspect.getsource(function)
-                except OSError:
-                    if failover_source is not None:
-                        function_source = failover_source
-                    else:
-                        raise
-
         if function_name is None or function_code is None:
             raise ValueError(
                 "Either 'function' must be provided, or "
                 "both of 'function_name' and 'function_code'"
             )
 
         self.function_name = function_name
         self.function_code = function_code
-        self.function_source = function_source
         self.container_uuid = (
             str(container_uuid) if container_uuid is not None else container_uuid
         )
         self.entry_point = entry_point if entry_point is not None else function_name
         self.description = description
         self.public = public
         self.group = group
         self.searchable = searchable
 
     def to_dict(self):
         return {
             "function_name": self.function_name,
             "function_code": self.function_code,
-            "function_source": self.function_source,
             "container_uuid": self.container_uuid,
             "entry_point": self.entry_point,
             "description": self.description,
             "public": self.public,
             "group": self.group,
             "searchable": self.searchable,
         }
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk/version.py` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.0a0"
+__version__ = "2.0.0a1"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-sdk-2.0.0a0/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a0/setup.py` & `globus-compute-sdk-2.0.0a1/setup.py`

 * *Files identical despite different names*

