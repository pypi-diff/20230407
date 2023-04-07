# Comparing `tmp/echostream-node-0.3.7.tar.gz` & `tmp/echostream-node-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echostream-node-0.3.7.tar", last modified: Mon Apr  3 01:04:36 2023, max compression
+gzip compressed data, was "echostream-node-0.3.8.tar", last modified: Fri Apr  7 16:23:31 2023, max compression
```

## Comparing `echostream-node-0.3.7.tar` & `echostream-node-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 01:04:36.446036 echostream-node-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 01:03:58.000000 echostream-node-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-03 01:03:58.000000 echostream-node-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-04-03 01:04:36.446036 echostream-node-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-03 01:03:58.000000 echostream-node-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 01:04:36.446036 echostream-node-0.3.7/echostream_node/
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-04-03 01:03:58.000000 echostream-node-0.3.7/echostream_node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 01:04:36.446036 echostream-node-0.3.7/echostream_node/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)    34186 2023-04-03 01:03:58.000000 echostream-node-0.3.7/echostream_node/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 01:04:36.446036 echostream-node-0.3.7/echostream_node/threading/
--rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-04-03 01:03:58.000000 echostream-node-0.3.7/echostream_node/threading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 01:04:36.446036 echostream-node-0.3.7/echostream_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-04-03 01:04:36.000000 echostream-node-0.3.7/echostream_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-03 01:04:36.000000 echostream-node-0.3.7/echostream_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 01:04:36.000000 echostream-node-0.3.7/echostream_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 01:04:36.000000 echostream-node-0.3.7/echostream_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 01:04:36.000000 echostream-node-0.3.7/echostream_node.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-03 01:03:58.000000 echostream-node-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-03 01:04:36.446036 echostream-node-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 16:22:52.000000 echostream-node-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 16:22:52.000000 echostream-node-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 16:23:31.703426 echostream-node-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-07 16:22:52.000000 echostream-node-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)    34186 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/threading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 16:22:52.000000 echostream-node-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-07 16:23:31.703426 echostream-node-0.3.8/setup.cfg
```

### Comparing `echostream-node-0.3.7/LICENSE` & `echostream-node-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.7/PKG-INFO` & `echostream-node-0.3.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echostream-node
-Version: 0.3.7
+Version: 0.3.8
 Summary: EchoStream library for implementing remote nodes
 Author: EchoStream
 Author-email: pypi@echo.stream
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,23 +28,37 @@
 
 ### AWS Lambda
 
 You may use the publiclally provided layer instead of directly installing `echostream-node` in your lambda package. This layer includes `echostream-node` and all of the Python dependencies *except* those built-in to the AWS Lambda environment for Python.
 
 The Layer arn is:
 ```
-arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-{version}:1
+arn:aws:lambda:{region}:226390263822:layer:echostream-node-{version}:1
 ```
-where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_`. For example, for `echostream-node==0.3.7` the layer arn would be:
+where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_` and `{region}` is the AWS region that your Lambda will run in. Currently, `us-east-1`, `us-east-2`, `us-west-1` and `us-west-2` are supported.
+
+For example, for `echostream-node==0.3.7` in the `us-east-1` region the layer arn would be:
 ```
 arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-0_3_7:1
 ```
 
 ## Usage
 
+### Configuration
+To instantiate a Node a number of variables are required. These can be provided either as environment variables or directly on Node creation:
+
+| Parameter | Environment Variable | Description |
+| --- | --- | --- |
+| `appsync_endpoint` | `APPSYNC_ENDPOINT` | The URL to the EchoStream API endpoint. |
+| `client_id` | `CLIENT_ID` | The Application Client ID for the App's Cognito Client Application. |
+| `name` | `NODE` | The Node's name. |
+| `password` | `PASSWORD` | The password for the App User for the Node's App. |
+| `tenant` | `TENANT` | The name of the Tenant that the Node is a part of. |
+| `username` | `USER_NAME` | The name of the App User for the Node's App. |
+| `user_pool_id` | `USER_POOL_ID` | The User Pool Id for the App's Cognito User Pool. |
 
 ### Threading Application Node
 ```python
 from signal import SIGHUP, SIGINT, SIGTERM, signal, strsignal
 
 from echostream_node import Message
 from echostream_node.threading import AppNode
@@ -135,19 +149,15 @@
 
 However, there are use cases where message ordering is not important but processing speed is.
 In these cases, you may configure your Node upon creation to concurrently process the messages
 that it receives.
 
 ### Making a Threading Application Node Concurrent
 If your Node inherits from the `echostream_node.threading.AppNode` class you can achieve concurrency
-using either threading or multi-processing. The former is appropriate if your processing is IO bound
-or your execution platform does not support shared memory (required for multi-processing). The latter
-is appropriate if your platform supports shared memory *and* your processing is CPU bound.
-
-#### Creating A Concurrent Application Node Using Threading
+using threading.
 
 This will create an AppNode that uses the provided `ThreadPoolExecutor` to concurrently
 process received `Message`s. Note that while you can set the maximum number of workers to
 less than 10, there is no gain to setting it to more than 10 since Nodes will only process
 up to 10 messages at a time.
 
 ```python
@@ -162,36 +172,14 @@
         super().__init__(executor=ThreadPoolExecutor(max_workers=10))
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
 
-#### Creating A Concurrent Application Node Using Multi-Processing
-
-This will create an AppNode that uses the provided `ProcessPoolExecutor` to concurrently
-process received `Message`s. Note that while you can set the maximum number of workers to
-less than 10, there is no gain to setting it to more than 10 since Nodes will only process
-up to 10 messages at a time.
-
-```python
-from concurrent.futures import ProcessPoolExecutor
-
-from echostream_node import Message
-from echostream_node.threading import AppNode
-
-class MyExternalNode(AppNode):
-
-    def __init__(self) -> None:
-        super().__init__(executor=ProcessPoolExecutor(max_workers=10))
-
-    def handle_received_message(self, *, message: Message, source: str) -> None:
-        print(f"Got a message:\n{message.body}")
-        self.audit_message(message, source=source)
-```
 ### Making a Asyncio Application Node Concurrent
 If your Node inherits from the `echostream_node.asyncio.Node` you can set the Node to
 process incoming `Message`s concurrently. There is no setting for the maximum number of tasks;
 a task is created per received `Message`.
 
 ```python
 import asyncio
@@ -246,7 +234,9 @@
     def __init__(self) -> None:
         super().__init__(report_batch_item_failures=True)
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
+
+Full documentation may be found at https://docs.echostream-node.echo.stream.
```

### Comparing `echostream-node-0.3.7/README.md` & `echostream-node-0.3.8/echostream_node.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: echostream-node
+Version: 0.3.8
+Summary: EchoStream library for implementing remote nodes
+Author: EchoStream
+Author-email: pypi@echo.stream
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # echostream-node
 
 EchoStream library for implementing remote nodes that can be used in the echostream system.
 
 This package supports creating External Nodes and Managed Node Types,
 and supports the following EchoStream use cases:
 - An External Node in an External App or Cross Account App that is a stand-alone application or part of another application, using either `threading` or `asyncio`.
@@ -18,23 +28,37 @@
 
 ### AWS Lambda
 
 You may use the publiclally provided layer instead of directly installing `echostream-node` in your lambda package. This layer includes `echostream-node` and all of the Python dependencies *except* those built-in to the AWS Lambda environment for Python.
 
 The Layer arn is:
 ```
-arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-{version}:1
+arn:aws:lambda:{region}:226390263822:layer:echostream-node-{version}:1
 ```
-where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_`. For example, for `echostream-node==0.3.7` the layer arn would be:
+where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_` and `{region}` is the AWS region that your Lambda will run in. Currently, `us-east-1`, `us-east-2`, `us-west-1` and `us-west-2` are supported.
+
+For example, for `echostream-node==0.3.7` in the `us-east-1` region the layer arn would be:
 ```
 arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-0_3_7:1
 ```
 
 ## Usage
 
+### Configuration
+To instantiate a Node a number of variables are required. These can be provided either as environment variables or directly on Node creation:
+
+| Parameter | Environment Variable | Description |
+| --- | --- | --- |
+| `appsync_endpoint` | `APPSYNC_ENDPOINT` | The URL to the EchoStream API endpoint. |
+| `client_id` | `CLIENT_ID` | The Application Client ID for the App's Cognito Client Application. |
+| `name` | `NODE` | The Node's name. |
+| `password` | `PASSWORD` | The password for the App User for the Node's App. |
+| `tenant` | `TENANT` | The name of the Tenant that the Node is a part of. |
+| `username` | `USER_NAME` | The name of the App User for the Node's App. |
+| `user_pool_id` | `USER_POOL_ID` | The User Pool Id for the App's Cognito User Pool. |
 
 ### Threading Application Node
 ```python
 from signal import SIGHUP, SIGINT, SIGTERM, signal, strsignal
 
 from echostream_node import Message
 from echostream_node.threading import AppNode
@@ -125,19 +149,15 @@
 
 However, there are use cases where message ordering is not important but processing speed is.
 In these cases, you may configure your Node upon creation to concurrently process the messages
 that it receives.
 
 ### Making a Threading Application Node Concurrent
 If your Node inherits from the `echostream_node.threading.AppNode` class you can achieve concurrency
-using either threading or multi-processing. The former is appropriate if your processing is IO bound
-or your execution platform does not support shared memory (required for multi-processing). The latter
-is appropriate if your platform supports shared memory *and* your processing is CPU bound.
-
-#### Creating A Concurrent Application Node Using Threading
+using threading.
 
 This will create an AppNode that uses the provided `ThreadPoolExecutor` to concurrently
 process received `Message`s. Note that while you can set the maximum number of workers to
 less than 10, there is no gain to setting it to more than 10 since Nodes will only process
 up to 10 messages at a time.
 
 ```python
@@ -152,36 +172,14 @@
         super().__init__(executor=ThreadPoolExecutor(max_workers=10))
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
 
-#### Creating A Concurrent Application Node Using Multi-Processing
-
-This will create an AppNode that uses the provided `ProcessPoolExecutor` to concurrently
-process received `Message`s. Note that while you can set the maximum number of workers to
-less than 10, there is no gain to setting it to more than 10 since Nodes will only process
-up to 10 messages at a time.
-
-```python
-from concurrent.futures import ProcessPoolExecutor
-
-from echostream_node import Message
-from echostream_node.threading import AppNode
-
-class MyExternalNode(AppNode):
-
-    def __init__(self) -> None:
-        super().__init__(executor=ProcessPoolExecutor(max_workers=10))
-
-    def handle_received_message(self, *, message: Message, source: str) -> None:
-        print(f"Got a message:\n{message.body}")
-        self.audit_message(message, source=source)
-```
 ### Making a Asyncio Application Node Concurrent
 If your Node inherits from the `echostream_node.asyncio.Node` you can set the Node to
 process incoming `Message`s concurrently. There is no setting for the maximum number of tasks;
 a task is created per received `Message`.
 
 ```python
 import asyncio
@@ -236,7 +234,9 @@
     def __init__(self) -> None:
         super().__init__(report_batch_item_failures=True)
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
+
+Full documentation may be found at https://docs.echostream-node.echo.stream.
```

### Comparing `echostream-node-0.3.7/echostream_node/__init__.py` & `echostream-node-0.3.8/echostream_node/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.7/echostream_node/asyncio/__init__.py` & `echostream-node-0.3.8/echostream_node/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.7/echostream_node/threading/__init__.py` & `echostream-node-0.3.8/echostream_node/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.7/echostream_node.egg-info/PKG-INFO` & `echostream-node-0.3.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: echostream-node
-Version: 0.3.7
-Summary: EchoStream library for implementing remote nodes
-Author: EchoStream
-Author-email: pypi@echo.stream
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # echostream-node
 
 EchoStream library for implementing remote nodes that can be used in the echostream system.
 
 This package supports creating External Nodes and Managed Node Types,
 and supports the following EchoStream use cases:
 - An External Node in an External App or Cross Account App that is a stand-alone application or part of another application, using either `threading` or `asyncio`.
@@ -28,23 +18,37 @@
 
 ### AWS Lambda
 
 You may use the publiclally provided layer instead of directly installing `echostream-node` in your lambda package. This layer includes `echostream-node` and all of the Python dependencies *except* those built-in to the AWS Lambda environment for Python.
 
 The Layer arn is:
 ```
-arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-{version}:1
+arn:aws:lambda:{region}:226390263822:layer:echostream-node-{version}:1
 ```
-where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_`. For example, for `echostream-node==0.3.7` the layer arn would be:
+where `{version}` is the version of `echostream-node` that you want, with `.` replaced with `_` and `{region}` is the AWS region that your Lambda will run in. Currently, `us-east-1`, `us-east-2`, `us-west-1` and `us-west-2` are supported.
+
+For example, for `echostream-node==0.3.7` in the `us-east-1` region the layer arn would be:
 ```
 arn:aws:lambda:us-east-1:226390263822:layer:echostream-node-0_3_7:1
 ```
 
 ## Usage
 
+### Configuration
+To instantiate a Node a number of variables are required. These can be provided either as environment variables or directly on Node creation:
+
+| Parameter | Environment Variable | Description |
+| --- | --- | --- |
+| `appsync_endpoint` | `APPSYNC_ENDPOINT` | The URL to the EchoStream API endpoint. |
+| `client_id` | `CLIENT_ID` | The Application Client ID for the App's Cognito Client Application. |
+| `name` | `NODE` | The Node's name. |
+| `password` | `PASSWORD` | The password for the App User for the Node's App. |
+| `tenant` | `TENANT` | The name of the Tenant that the Node is a part of. |
+| `username` | `USER_NAME` | The name of the App User for the Node's App. |
+| `user_pool_id` | `USER_POOL_ID` | The User Pool Id for the App's Cognito User Pool. |
 
 ### Threading Application Node
 ```python
 from signal import SIGHUP, SIGINT, SIGTERM, signal, strsignal
 
 from echostream_node import Message
 from echostream_node.threading import AppNode
@@ -135,19 +139,15 @@
 
 However, there are use cases where message ordering is not important but processing speed is.
 In these cases, you may configure your Node upon creation to concurrently process the messages
 that it receives.
 
 ### Making a Threading Application Node Concurrent
 If your Node inherits from the `echostream_node.threading.AppNode` class you can achieve concurrency
-using either threading or multi-processing. The former is appropriate if your processing is IO bound
-or your execution platform does not support shared memory (required for multi-processing). The latter
-is appropriate if your platform supports shared memory *and* your processing is CPU bound.
-
-#### Creating A Concurrent Application Node Using Threading
+using threading.
 
 This will create an AppNode that uses the provided `ThreadPoolExecutor` to concurrently
 process received `Message`s. Note that while you can set the maximum number of workers to
 less than 10, there is no gain to setting it to more than 10 since Nodes will only process
 up to 10 messages at a time.
 
 ```python
@@ -162,36 +162,14 @@
         super().__init__(executor=ThreadPoolExecutor(max_workers=10))
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
 
-#### Creating A Concurrent Application Node Using Multi-Processing
-
-This will create an AppNode that uses the provided `ProcessPoolExecutor` to concurrently
-process received `Message`s. Note that while you can set the maximum number of workers to
-less than 10, there is no gain to setting it to more than 10 since Nodes will only process
-up to 10 messages at a time.
-
-```python
-from concurrent.futures import ProcessPoolExecutor
-
-from echostream_node import Message
-from echostream_node.threading import AppNode
-
-class MyExternalNode(AppNode):
-
-    def __init__(self) -> None:
-        super().__init__(executor=ProcessPoolExecutor(max_workers=10))
-
-    def handle_received_message(self, *, message: Message, source: str) -> None:
-        print(f"Got a message:\n{message.body}")
-        self.audit_message(message, source=source)
-```
 ### Making a Asyncio Application Node Concurrent
 If your Node inherits from the `echostream_node.asyncio.Node` you can set the Node to
 process incoming `Message`s concurrently. There is no setting for the maximum number of tasks;
 a task is created per received `Message`.
 
 ```python
 import asyncio
@@ -246,7 +224,9 @@
     def __init__(self) -> None:
         super().__init__(report_batch_item_failures=True)
 
     def handle_received_message(self, *, message: Message, source: str) -> None:
         print(f"Got a message:\n{message.body}")
         self.audit_message(message, source=source)
 ```
+
+Full documentation may be found at https://docs.echostream-node.echo.stream.
```

### Comparing `echostream-node-0.3.7/setup.cfg` & `echostream-node-0.3.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = echostream-node
 author = EchoStream
 author_email = pypi@echo.stream
-version = 0.3.7
+version = 0.3.8
 description = EchoStream library for implementing remote nodes
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 include_package_data = true
@@ -16,14 +16,14 @@
 	dynamic-function-loader==0.0.3
 	echostream-botocore==0.0.2
 	gql[aiohttp,requests]==3.4.0
 	gql-appsync-cognito-authentication==0.0.1
 	httpx==0.23.3
 	httpx-auth==0.15.0
 	pycognito==2022.12.0
-	simplejson==3.18.4
+	simplejson==3.19.1
 python_requires = >=3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

