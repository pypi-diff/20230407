# Comparing `tmp/preemo_worker_sdk-0.2.2.tar.gz` & `tmp/preemo_worker_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preemo_worker_sdk-0.2.2.tar", max compression
+gzip compressed data, was "preemo_worker_sdk-0.3.0.tar", max compression
```

## Comparing `preemo_worker_sdk-0.2.2.tar` & `preemo_worker_sdk-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,53 @@
--rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.2.2/LICENSE
--rw-r--r--   0        0        0     2593 2023-03-21 22:01:19.917523 preemo_worker_sdk-0.2.2/README.md
--rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.2.2/preemo/__init__.py
--rw-r--r--   0        0        0      306 2023-03-21 21:58:02.566209 preemo_worker_sdk-0.2.2/preemo/gen/__init__.py
--rw-r--r--   0        0        0      306 2023-03-21 21:58:02.566410 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/__init__.py
--rw-r--r--   0        0        0     4345 2023-03-21 22:01:19.918337 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_part_pb2.py
--rw-r--r--   0        0        0     7822 2023-03-21 22:01:19.918532 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     2637 2023-03-21 22:01:19.918727 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_pb2.py
--rw-r--r--   0        0        0     4633 2023-03-21 22:01:19.918902 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
--rw-r--r--   0        0        0     2683 2023-03-21 22:01:19.919149 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
--rw-r--r--   0        0        0     3994 2023-03-21 22:01:19.919314 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
--rw-r--r--   0        0        0     4212 2023-03-21 22:01:19.919556 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_part_pb2.py
--rw-r--r--   0        0        0     7654 2023-03-21 22:01:19.919777 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     2612 2023-03-21 22:01:19.920004 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_pb2.py
--rw-r--r--   0        0        0     4394 2023-03-21 22:01:19.920227 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
--rw-r--r--   0        0        0     1382 2023-03-21 22:01:19.920385 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/check_function_pb2.py
--rw-r--r--   0        0        0     1811 2023-03-21 22:01:19.920630 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/check_function_pb2.pyi
--rw-r--r--   0        0        0     2544 2023-03-21 22:01:19.920904 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/execute_function_pb2.py
--rw-r--r--   0        0        0     4104 2023-03-21 22:01:19.921062 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/execute_function_pb2.pyi
--rw-r--r--   0        0        0     1128 2023-03-21 22:01:19.921261 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/header_pb2.py
--rw-r--r--   0        0        0     1448 2023-03-21 22:01:19.921565 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/header_pb2.pyi
--rw-r--r--   0        0        0     1403 2023-03-21 22:01:19.921767 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/register_function_pb2.py
--rw-r--r--   0        0        0     1721 2023-03-21 22:01:19.922076 preemo_worker_sdk-0.2.2/preemo/gen/endpoints/register_function_pb2.pyi
--rw-r--r--   0        0        0      306 2023-03-21 21:58:02.566787 preemo_worker_sdk-0.2.2/preemo/gen/models/__init__.py
--rw-r--r--   0        0        0     1135 2023-03-21 22:01:19.922297 preemo_worker_sdk-0.2.2/preemo/gen/models/registered_function_pb2.py
--rw-r--r--   0        0        0     1624 2023-03-21 22:01:19.922595 preemo_worker_sdk-0.2.2/preemo/gen/models/registered_function_pb2.pyi
--rw-r--r--   0        0        0     1174 2023-03-21 22:01:19.922835 preemo_worker_sdk-0.2.2/preemo/gen/models/value_pb2.py
--rw-r--r--   0        0        0     1396 2023-03-21 22:01:19.923183 preemo_worker_sdk-0.2.2/preemo/gen/models/value_pb2.pyi
--rw-r--r--   0        0        0      306 2023-03-21 21:58:02.566970 preemo_worker_sdk-0.2.2/preemo/gen/services/__init__.py
--rw-r--r--   0        0        0    17654 2023-03-21 22:01:19.923516 preemo_worker_sdk-0.2.2/preemo/gen/services/worker_pb2_grpc.py
--rw-r--r--   0        0        0     5213 2023-03-21 22:01:19.923820 preemo_worker_sdk-0.2.2/preemo/gen/services/worker_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.2.2/preemo/py.typed
--rw-r--r--   0        0        0     1158 2023-03-21 22:01:19.924106 preemo_worker_sdk-0.2.2/preemo/worker/__init__.py
--rw-r--r--   0        0        0      192 2023-03-02 18:51:16.182827 preemo_worker_sdk-0.2.2/preemo/worker/__init__.pyi
--rw-r--r--   0        0        0     6594 2023-03-22 21:12:37.699058 preemo_worker_sdk-0.2.2/preemo/worker/_artifact_manager.py
--rw-r--r--   0        0        0      384 2023-03-02 18:51:16.182930 preemo_worker_sdk-0.2.2/preemo/worker/_env.py
--rw-r--r--   0        0        0     1732 2023-03-02 18:51:16.183043 preemo_worker_sdk-0.2.2/preemo/worker/_function_registry.py
--rw-r--r--   0        0        0     7186 2023-03-21 22:01:19.924660 preemo_worker_sdk-0.2.2/preemo/worker/_messaging_client.py
--rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.2.2/preemo/worker/_types.py
--rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.2.2/preemo/worker/_validation.py
--rw-r--r--   0        0        0     6333 2023-03-22 21:27:54.969443 preemo_worker_sdk-0.2.2/preemo/worker/_worker_client.py
--rw-r--r--   0        0        0     1668 2023-03-22 22:51:56.488275 preemo_worker_sdk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.3.0/preemo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-06 00:44:52.196888 preemo_worker_sdk-0.3.0/preemo/gen/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197079 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/__init__.py
+-rw-r--r--   0        0        0     4345 2023-04-06 00:44:52.045784 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7822 2023-04-07 21:20:34.286564 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     2733 2023-04-06 00:44:52.045917 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.py
+-rw-r--r--   0        0        0     5420 2023-04-06 00:44:52.209089 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
+-rw-r--r--   0        0        0     2642 2023-04-06 00:44:52.046026 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.py
+-rw-r--r--   0        0        0     4134 2023-04-06 00:44:52.213421 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi
+-rw-r--r--   0        0        0     2837 2023-04-06 00:44:52.046135 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
+-rw-r--r--   0        0        0     5105 2023-04-06 00:44:52.217891 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4212 2023-04-06 00:44:52.046231 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7654 2023-04-06 00:44:52.222757 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-06 00:44:52.046329 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.py
+-rw-r--r--   0        0        0     5685 2023-04-06 00:44:52.228008 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
+-rw-r--r--   0        0        0     1382 2023-04-06 00:44:52.046428 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.py
+-rw-r--r--   0        0        0     1811 2023-04-06 00:44:52.232051 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.pyi
+-rw-r--r--   0        0        0     1665 2023-04-06 00:44:52.046532 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.py
+-rw-r--r--   0        0        0     3019 2023-04-06 00:44:52.236010 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.pyi
+-rw-r--r--   0        0        0     1128 2023-04-06 00:44:52.046634 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.py
+-rw-r--r--   0        0        0     1515 2023-04-06 00:44:52.239908 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.pyi
+-rw-r--r--   0        0        0     1403 2023-04-06 00:44:52.046746 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.py
+-rw-r--r--   0        0        0     1721 2023-04-06 00:44:52.243919 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.pyi
+-rw-r--r--   0        0        0     1222 2023-04-06 00:44:52.046859 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.py
+-rw-r--r--   0        0        0     1539 2023-04-06 00:44:52.248123 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
+-rw-r--r--   0        0        0     1085 2023-04-06 00:44:52.046972 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.py
+-rw-r--r--   0        0        0      786 2023-04-06 00:44:52.252283 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197557 preemo_worker_sdk-0.3.0/preemo/gen/models/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-06 00:44:52.047113 preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.py
+-rw-r--r--   0        0        0     1624 2023-04-06 00:44:52.256316 preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.pyi
+-rw-r--r--   0        0        0     1174 2023-04-06 00:44:52.047229 preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.py
+-rw-r--r--   0        0        0     1396 2023-04-06 00:44:52.260232 preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197729 preemo_worker_sdk-0.3.0/preemo/gen/services/__init__.py
+-rw-r--r--   0        0        0     4369 2023-04-06 00:44:52.189708 preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.py
+-rw-r--r--   0        0        0     1302 2023-04-06 00:44:52.264181 preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19585 2023-04-06 00:44:52.189860 preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     5787 2023-04-06 00:44:52.268251 preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.3.0/preemo/py.typed
+-rw-r--r--   0        0        0     3310 2023-04-07 21:20:34.286985 preemo_worker_sdk-0.3.0/preemo/worker/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.3.0/preemo/worker/__init__.pyi
+-rw-r--r--   0        0        0    12028 2023-04-07 21:20:34.287528 preemo_worker_sdk-0.3.0/preemo/worker/_artifact_manager.py
+-rw-r--r--   0        0        0      759 2023-04-07 21:20:34.287821 preemo_worker_sdk-0.3.0/preemo/worker/_env.py
+-rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.3.0/preemo/worker/_function_registry.py
+-rw-r--r--   0        0        0     9948 2023-04-07 16:55:48.486452 preemo_worker_sdk-0.3.0/preemo/worker/_messaging_client.py
+-rw-r--r--   0        0        0     2538 2023-04-07 21:20:34.288187 preemo_worker_sdk-0.3.0/preemo/worker/_sdk_server.py
+-rw-r--r--   0        0        0     3229 2023-04-07 21:20:34.288581 preemo_worker_sdk-0.3.0/preemo/worker/_sdk_service.py
+-rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.3.0/preemo/worker/_types.py
+-rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.3.0/preemo/worker/_validation.py
+-rw-r--r--   0        0        0     6887 2023-04-07 21:20:34.288862 preemo_worker_sdk-0.3.0/preemo/worker/_worker_client.py
+-rw-r--r--   0        0        0     1698 2023-04-07 21:20:52.735653 preemo_worker_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3476 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.3.0/PKG-INFO
```

### Comparing `preemo_worker_sdk-0.2.2/LICENSE` & `preemo_worker_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/README.md` & `preemo_worker_sdk-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,78 +17,89 @@
 
 In order to register a function with Preemo workers, you can use `register` to decorate your functions.
 
 ```python
 from preemo.worker import register
 
 @register(name="some_name", namespace="dev")
-def do_something(params: str):
+def do_something(params: bytes):
     ...
 ```
 
 Both parameters, `name` and `namespace`, are optional. If the name isn't specified, it will default to the name of the function. If the namespace isn't specified, it will default to a global namespace.
 
 ```python
 @register
 def do_something(params: str):
     # registers with name do_something in the global namespace
     ...
 ```
 
-At the moment, only functions that take 0 or 1 string arguments will work. These functions should also either return `None` or a string.
+At the moment, only functions that take 0 or 1 bytes arguments will work. These functions should also either return `None` or bytes.
 
 ### Execute Function
 
 In order to execute a function that you have previously registered with Preemo workers, you can use `get_function`.
 
 ```python
 from preemo.worker import get_function
 
 do_something = get_function(name="some_name", namespace="dev")
-result = do_something("params")
+result = do_something(b"params")
 ...
 ```
 
 The second parameter, `namespace`, is optional. If the namespace isn't specified, it will default to a global namespace.
 
 ```python
 # gets the function named do_something in the global namespace
 do_something = get_function("do_something")
-result = do_something("params")
+result = do_something(b"params")
 ...
 ```
 
-### Parallelize Function Execution
+### Parallel Function Execution
 
-In order to execute a function with multiple parameters in parallel, you can use `parallelize`.
+In order to execute a function with multiple parameters at the same time, you can use `parallel`.
 
 ```python
-from preemo.worker import parallelize
+from preemo.worker import get_function, parallel
 
 do_something = get_function(name="some_name", namespace="dev")
-results = parallelize(
+results = parallel(
     do_something,
     params=[
-        "params1",
-        "params2",
+        b"params1",
+        b"params2",
         ...
     ]
 )
 ...
 ```
 
 If your function doesn't take a parameter and you'd like to run multiple instances of it in parallel, you can use the `count` parameter.
 
 ```python
 do_something = get_function(name="some_name", namespace="dev")
-results = parallelize(
+results = parallel(
     do_something,
     count=10
 )
 ...
 ```
 
-<!-- TODO(adrian@preemo.io, 03/20/23): include an explanation of the result objects. They should be objects that give you access to the artifacts. -->
+### Results
+
+In order to view the result of an executed function, you can call `.get()`.
+
+```python
+from preemo.worker import get_function
+
+do_something = get_function(name="some_name", namespace="dev")
+result = do_something(b"params")
+value = result.get()
+...
+```
 
 ## Contributing
 
 [Contribution guidelines for this project](CONTRIBUTING.md)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_part_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     METADATAS_BY_PART_NUMBER_FIELD_NUMBER: builtins.int
     @property
     def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactPartConfigMetadata]:
-        """For an artifact, part numbers must be sequential positive integers starting with 1."""
+        """For an artifact, part numbers must be sequential positive integers starting with 0."""
     def __init__(
         self,
         *,
         metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___CreateArtifactPartConfigMetadata] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas_by_part_number", b"metadatas_by_part_number"]) -> None: ...
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%endpoints/batch_create_artifact.proto\x12\tendpoints\"\x16\n\x14\x43reateArtifactConfig\"\xc9\x01\n\x1a\x42\x61tchCreateArtifactRequest\x12S\n\x10\x63onfigs_by_index\x18\x01 \x03(\x0b\x32\x39.endpoints.BatchCreateArtifactRequest.ConfigsByIndexEntry\x1aV\n\x13\x43onfigsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactConfig:\x02\x38\x01\"@\n\x14\x43reateArtifactResult\x12\x18\n\x0b\x61rtifact_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_artifact_id\"\xcb\x01\n\x1b\x42\x61tchCreateArtifactResponse\x12T\n\x10results_by_index\x18\x01 \x03(\x0b\x32:.endpoints.BatchCreateArtifactResponse.ResultsByIndexEntry\x1aV\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactResult:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%endpoints/batch_create_artifact.proto\x12\tendpoints\"\x16\n\x14\x43reateArtifactConfig\"\xc9\x01\n\x1a\x42\x61tchCreateArtifactRequest\x12S\n\x10\x63onfigs_by_index\x18\x01 \x03(\x0b\x32\x39.endpoints.BatchCreateArtifactRequest.ConfigsByIndexEntry\x1aV\n\x13\x43onfigsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactConfig:\x02\x38\x01\"z\n\x14\x43reateArtifactResult\x12\x18\n\x0b\x61rtifact_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12 \n\x13part_size_threshold\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x0e\n\x0c_artifact_idB\x16\n\x14_part_size_threshold\"\xcb\x01\n\x1b\x42\x61tchCreateArtifactResponse\x12T\n\x10results_by_index\x18\x01 \x03(\x0b\x32:.endpoints.BatchCreateArtifactResponse.ResultsByIndexEntry\x1aV\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactResult:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_create_artifact_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._options = None
@@ -27,13 +27,13 @@
   _CREATEARTIFACTCONFIG._serialized_start=52
   _CREATEARTIFACTCONFIG._serialized_end=74
   _BATCHCREATEARTIFACTREQUEST._serialized_start=77
   _BATCHCREATEARTIFACTREQUEST._serialized_end=278
   _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_start=192
   _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_end=278
   _CREATEARTIFACTRESULT._serialized_start=280
-  _CREATEARTIFACTRESULT._serialized_end=344
-  _BATCHCREATEARTIFACTRESPONSE._serialized_start=347
-  _BATCHCREATEARTIFACTRESPONSE._serialized_end=550
-  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_start=464
-  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_end=550
+  _CREATEARTIFACTRESULT._serialized_end=402
+  _BATCHCREATEARTIFACTRESPONSE._serialized_start=405
+  _BATCHCREATEARTIFACTRESPONSE._serialized_end=608
+  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_start=522
+  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_end=608
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
+import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
@@ -68,23 +69,33 @@
 global___BatchCreateArtifactRequest = BatchCreateArtifactRequest
 
 @typing_extensions.final
 class CreateArtifactResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ARTIFACT_ID_FIELD_NUMBER: builtins.int
+    PART_SIZE_THRESHOLD_FIELD_NUMBER: builtins.int
     artifact_id: builtins.str
+    """Required field representing the unique identifier for a file stored in the cloud."""
+    part_size_threshold: builtins.int
+    """Required field indicating the precise number of bytes a part should
+    reach before creating the next part.
+    """
     def __init__(
         self,
         *,
         artifact_id: builtins.str | None = ...,
+        part_size_threshold: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "artifact_id", b"artifact_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "artifact_id", b"artifact_id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_artifact_id", b"_artifact_id"]) -> typing_extensions.Literal["artifact_id"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_size_threshold", b"_part_size_threshold"]) -> typing_extensions.Literal["part_size_threshold"] | None: ...
 
 global___CreateArtifactResult = CreateArtifactResult
 
 @typing_extensions.final
 class BatchCreateArtifactResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'endpoints/batch_finalize_artifact.proto\x12\tendpoints\"\x18\n\x16\x46inalizeArtifactConfig\"\xdf\x01\n\x1c\x42\x61tchFinalizeArtifactRequest\x12`\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32@.endpoints.BatchFinalizeArtifactRequest.ConfigsByArtifactIdEntry\x1a]\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.endpoints.FinalizeArtifactConfig:\x02\x38\x01\"\x18\n\x16\x46inalizeArtifactResult\"\xe1\x01\n\x1d\x42\x61tchFinalizeArtifactResponse\x12\x61\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32\x41.endpoints.BatchFinalizeArtifactResponse.ResultsByArtifactIdEntry\x1a]\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.endpoints.FinalizeArtifactResult:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'endpoints/batch_finalize_artifact.proto\x12\tendpoints\"h\n\x16\x46inalizeArtifactConfig\x12\x17\n\ntotal_size\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x17\n\npart_count\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\r\n\x0b_total_sizeB\r\n\x0b_part_count\"\xdf\x01\n\x1c\x42\x61tchFinalizeArtifactRequest\x12`\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32@.endpoints.BatchFinalizeArtifactRequest.ConfigsByArtifactIdEntry\x1a]\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.endpoints.FinalizeArtifactConfig:\x02\x38\x01\"\x18\n\x16\x46inalizeArtifactResult\"\xe1\x01\n\x1d\x42\x61tchFinalizeArtifactResponse\x12\x61\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32\x41.endpoints.BatchFinalizeArtifactResponse.ResultsByArtifactIdEntry\x1a]\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.endpoints.FinalizeArtifactResult:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_finalize_artifact_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._options = None
   _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_options = b'8\001'
   _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._options = None
   _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_options = b'8\001'
   _FINALIZEARTIFACTCONFIG._serialized_start=54
-  _FINALIZEARTIFACTCONFIG._serialized_end=78
-  _BATCHFINALIZEARTIFACTREQUEST._serialized_start=81
-  _BATCHFINALIZEARTIFACTREQUEST._serialized_end=304
-  _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_start=211
-  _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_end=304
-  _FINALIZEARTIFACTRESULT._serialized_start=306
-  _FINALIZEARTIFACTRESULT._serialized_end=330
-  _BATCHFINALIZEARTIFACTRESPONSE._serialized_start=333
-  _BATCHFINALIZEARTIFACTRESPONSE._serialized_end=558
-  _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=465
-  _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=558
+  _FINALIZEARTIFACTCONFIG._serialized_end=158
+  _BATCHFINALIZEARTIFACTREQUEST._serialized_start=161
+  _BATCHFINALIZEARTIFACTREQUEST._serialized_end=384
+  _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_start=291
+  _BATCHFINALIZEARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_end=384
+  _FINALIZEARTIFACTRESULT._serialized_start=386
+  _FINALIZEARTIFACTRESULT._serialized_end=410
+  _BATCHFINALIZEARTIFACTRESPONSE._serialized_start=413
+  _BATCHFINALIZEARTIFACTRESPONSE._serialized_end=638
+  _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=545
+  _BATCHFINALIZEARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=638
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_part_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"endpoints/batch_get_artifact.proto\x12\tendpoints\"\x13\n\x11GetArtifactConfig\"\xd0\x01\n\x17\x42\x61tchGetArtifactRequest\x12[\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32;.endpoints.BatchGetArtifactRequest.ConfigsByArtifactIdEntry\x1aX\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.endpoints.GetArtifactConfig:\x02\x38\x01\";\n\x11GetArtifactResult\x12\x17\n\npart_count\x18\x01 \x01(\rH\x00\x88\x01\x01\x42\r\n\x0b_part_count\"\xd2\x01\n\x18\x42\x61tchGetArtifactResponse\x12\\\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32<.endpoints.BatchGetArtifactResponse.ResultsByArtifactIdEntry\x1aX\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.endpoints.GetArtifactResult:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"endpoints/batch_get_artifact.proto\x12\tendpoints\"\x13\n\x11GetArtifactConfig\"\xd0\x01\n\x17\x42\x61tchGetArtifactRequest\x12[\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32;.endpoints.BatchGetArtifactRequest.ConfigsByArtifactIdEntry\x1aX\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.endpoints.GetArtifactConfig:\x02\x38\x01\"\x9d\x01\n\x11GetArtifactResult\x12\x17\n\npart_count\x18\x01 \x01(\rH\x00\x88\x01\x01\x12 \n\x13part_size_threshold\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x17\n\ntotal_size\x18\x03 \x01(\x04H\x02\x88\x01\x01\x42\r\n\x0b_part_countB\x16\n\x14_part_size_thresholdB\r\n\x0b_total_size\"\xd2\x01\n\x18\x42\x61tchGetArtifactResponse\x12\\\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32<.endpoints.BatchGetArtifactResponse.ResultsByArtifactIdEntry\x1aX\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.endpoints.GetArtifactResult:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_get_artifact_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BATCHGETARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._options = None
@@ -26,14 +26,14 @@
   _BATCHGETARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_options = b'8\001'
   _GETARTIFACTCONFIG._serialized_start=49
   _GETARTIFACTCONFIG._serialized_end=68
   _BATCHGETARTIFACTREQUEST._serialized_start=71
   _BATCHGETARTIFACTREQUEST._serialized_end=279
   _BATCHGETARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_start=191
   _BATCHGETARTIFACTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_end=279
-  _GETARTIFACTRESULT._serialized_start=281
-  _GETARTIFACTRESULT._serialized_end=340
-  _BATCHGETARTIFACTRESPONSE._serialized_start=343
-  _BATCHGETARTIFACTRESPONSE._serialized_end=553
-  _BATCHGETARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=465
-  _BATCHGETARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=553
+  _GETARTIFACTRESULT._serialized_start=282
+  _GETARTIFACTRESULT._serialized_end=439
+  _BATCHGETARTIFACTRESPONSE._serialized_start=442
+  _BATCHGETARTIFACTRESPONSE._serialized_end=652
+  _BATCHGETARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=564
+  _BATCHGETARTIFACTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=652
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -4,111 +4,120 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import sys
+import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class GetArtifactConfig(google.protobuf.message.Message):
-    """This config is included for potential future use."""
-
+class FinalizeArtifactConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    TOTAL_SIZE_FIELD_NUMBER: builtins.int
+    PART_COUNT_FIELD_NUMBER: builtins.int
+    total_size: builtins.int
+    """Required field representing the size in bytes of the combined artifact parts."""
+    part_count: builtins.int
+    """Required field indicating the number of parts that were written to."""
     def __init__(
         self,
+        *,
+        total_size: builtins.int | None = ...,
+        part_count: builtins.int | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_size", b"_total_size"]) -> typing_extensions.Literal["total_size"] | None: ...
 
-global___GetArtifactConfig = GetArtifactConfig
+global___FinalizeArtifactConfig = FinalizeArtifactConfig
 
 @typing_extensions.final
-class BatchGetArtifactRequest(google.protobuf.message.Message):
+class BatchFinalizeArtifactRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___GetArtifactConfig: ...
+        def value(self) -> global___FinalizeArtifactConfig: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___GetArtifactConfig | None = ...,
+            value: global___FinalizeArtifactConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactConfig]: ...
+    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactConfig]: ...
     def __init__(
         self,
         *,
-        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactConfig] | None = ...,
+        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactConfig] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
 
-global___BatchGetArtifactRequest = BatchGetArtifactRequest
+global___BatchFinalizeArtifactRequest = BatchFinalizeArtifactRequest
 
 @typing_extensions.final
-class GetArtifactResult(google.protobuf.message.Message):
+class FinalizeArtifactResult(google.protobuf.message.Message):
+    """This result is included for potential future use."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PART_COUNT_FIELD_NUMBER: builtins.int
-    part_count: builtins.int
     def __init__(
         self,
-        *,
-        part_count: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "part_count", b"part_count"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "part_count", b"part_count"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
 
-global___GetArtifactResult = GetArtifactResult
+global___FinalizeArtifactResult = FinalizeArtifactResult
 
 @typing_extensions.final
-class BatchGetArtifactResponse(google.protobuf.message.Message):
+class BatchFinalizeArtifactResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ResultsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___GetArtifactResult: ...
+        def value(self) -> global___FinalizeArtifactResult: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___GetArtifactResult | None = ...,
+            value: global___FinalizeArtifactResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactResult]: ...
+    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactResult]: ...
     def __init__(
         self,
         *,
-        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactResult] | None = ...,
+        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactResult] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
 
-global___BatchGetArtifactResponse = BatchGetArtifactResponse
+global___BatchFinalizeArtifactResponse = BatchFinalizeArtifactResponse
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/check_function_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/check_function_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/execute_function_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: endpoints/execute_function.proto
+# source: endpoints/batch_execute_function.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from models import registered_function_pb2 as models_dot_registered__function__pb2
 from models import value_pb2 as models_dot_value__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n endpoints/execute_function.proto\x12\tendpoints\x1a models/registered_function.proto\x1a\x12models/value.proto\"\x8e\x02\n\x16\x45xecuteFunctionRequest\x12<\n\x13\x66unction_to_execute\x18\x01 \x01(\x0b\x32\x1a.models.RegisteredFunctionH\x00\x88\x01\x01\x12U\n\x13parameters_by_index\x18\x02 \x03(\x0b\x32\x38.endpoints.ExecuteFunctionRequest.ParametersByIndexEntry\x1aG\n\x16ParametersByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.models.Value:\x02\x38\x01\x42\x16\n\x14_function_to_execute\"\xb1\x01\n\x17\x45xecuteFunctionResponse\x12P\n\x10results_by_index\x18\x01 \x03(\x0b\x32\x36.endpoints.ExecuteFunctionResponse.ResultsByIndexEntry\x1a\x44\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.models.Value:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&endpoints/batch_execute_function.proto\x12\tendpoints\x1a models/registered_function.proto\x1a\x12models/value.proto\"\x98\x02\n\x1b\x42\x61tchExecuteFunctionRequest\x12<\n\x13\x66unction_to_execute\x18\x01 \x01(\x0b\x32\x1a.models.RegisteredFunctionH\x00\x88\x01\x01\x12Z\n\x13parameters_by_index\x18\x02 \x03(\x0b\x32=.endpoints.BatchExecuteFunctionRequest.ParametersByIndexEntry\x1aG\n\x16ParametersByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.models.Value:\x02\x38\x01\x42\x16\n\x14_function_to_execute\"\xbb\x01\n\x1c\x42\x61tchExecuteFunctionResponse\x12U\n\x10results_by_index\x18\x01 \x03(\x0b\x32;.endpoints.BatchExecuteFunctionResponse.ResultsByIndexEntry\x1a\x44\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.models.Value:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.execute_function_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_execute_function_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _EXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._options = None
-  _EXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_options = b'8\001'
-  _EXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._options = None
-  _EXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_options = b'8\001'
-  _EXECUTEFUNCTIONREQUEST._serialized_start=102
-  _EXECUTEFUNCTIONREQUEST._serialized_end=372
-  _EXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_start=277
-  _EXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_end=348
-  _EXECUTEFUNCTIONRESPONSE._serialized_start=375
-  _EXECUTEFUNCTIONRESPONSE._serialized_end=552
-  _EXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_start=484
-  _EXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_end=552
+  _BATCHEXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._options = None
+  _BATCHEXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_options = b'8\001'
+  _BATCHEXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._options = None
+  _BATCHEXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_options = b'8\001'
+  _BATCHEXECUTEFUNCTIONREQUEST._serialized_start=108
+  _BATCHEXECUTEFUNCTIONREQUEST._serialized_end=388
+  _BATCHEXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_start=293
+  _BATCHEXECUTEFUNCTIONREQUEST_PARAMETERSBYINDEXENTRY._serialized_end=364
+  _BATCHEXECUTEFUNCTIONRESPONSE._serialized_start=391
+  _BATCHEXECUTEFUNCTIONRESPONSE._serialized_end=578
+  _BATCHEXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_start=510
+  _BATCHEXECUTEFUNCTIONRESPONSE_RESULTSBYINDEXENTRY._serialized_end=578
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/execute_function_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class ExecuteFunctionRequest(google.protobuf.message.Message):
+class BatchExecuteFunctionRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ParametersByIndexEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
@@ -52,18 +52,18 @@
         function_to_execute: preemo.gen.models.registered_function_pb2.RegisteredFunction | None = ...,
         parameters_by_index: collections.abc.Mapping[builtins.int, preemo.gen.models.value_pb2.Value] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_function_to_execute", b"_function_to_execute", "function_to_execute", b"function_to_execute"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_function_to_execute", b"_function_to_execute", "function_to_execute", b"function_to_execute", "parameters_by_index", b"parameters_by_index"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_function_to_execute", b"_function_to_execute"]) -> typing_extensions.Literal["function_to_execute"] | None: ...
 
-global___ExecuteFunctionRequest = ExecuteFunctionRequest
+global___BatchExecuteFunctionRequest = BatchExecuteFunctionRequest
 
 @typing_extensions.final
-class ExecuteFunctionResponse(google.protobuf.message.Message):
+class BatchExecuteFunctionResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ResultsByIndexEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
@@ -86,8 +86,8 @@
     def __init__(
         self,
         *,
         results_by_index: collections.abc.Mapping[builtins.int, preemo.gen.models.value_pb2.Value] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results_by_index", b"results_by_index"]) -> None: ...
 
-global___ExecuteFunctionResponse = ExecuteFunctionResponse
+global___BatchExecuteFunctionResponse = BatchExecuteFunctionResponse
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/header_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/header_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Intended to contain any and all metadata the server might need.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VERSION_FIELD_NUMBER: builtins.int
     version: builtins.str
+    """Required field indicating the version of the Worker SDK."""
     def __init__(
         self,
         *,
         version: builtins.str | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_version", b"_version", "version", b"version"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_version", b"_version", "version", b"version"]) -> None: ...
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/register_function_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/endpoints/register_function_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/models/registered_function_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/models/registered_function_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/models/value_pb2.py` & `preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/models/value_pb2.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/services/worker_pb2_grpc.py` & `preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from endpoints import batch_create_artifact_part_pb2 as endpoints_dot_batch__create__artifact__part__pb2
 from endpoints import batch_create_artifact_pb2 as endpoints_dot_batch__create__artifact__pb2
+from endpoints import batch_execute_function_pb2 as endpoints_dot_batch__execute__function__pb2
 from endpoints import batch_finalize_artifact_pb2 as endpoints_dot_batch__finalize__artifact__pb2
 from endpoints import batch_get_artifact_part_pb2 as endpoints_dot_batch__get__artifact__part__pb2
 from endpoints import batch_get_artifact_pb2 as endpoints_dot_batch__get__artifact__pb2
 from endpoints import check_function_pb2 as endpoints_dot_check__function__pb2
-from endpoints import execute_function_pb2 as endpoints_dot_execute__function__pb2
 from endpoints import header_pb2 as endpoints_dot_header__pb2
 from endpoints import register_function_pb2 as endpoints_dot_register__function__pb2
+from endpoints import sdk_server_ready_pb2 as endpoints_dot_sdk__server__ready__pb2
 
 
 class WorkerServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
@@ -28,14 +29,19 @@
                 response_deserializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.FromString,
                 )
         self.BatchCreateArtifactPart = channel.unary_unary(
                 '/services.WorkerService/BatchCreateArtifactPart',
                 request_serializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.FromString,
                 )
+        self.BatchExecuteFunction = channel.unary_unary(
+                '/services.WorkerService/BatchExecuteFunction',
+                request_serializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionRequest.SerializeToString,
+                response_deserializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionResponse.FromString,
+                )
         self.BatchFinalizeArtifact = channel.unary_unary(
                 '/services.WorkerService/BatchFinalizeArtifact',
                 request_serializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactResponse.FromString,
                 )
         self.BatchGetArtifact = channel.unary_unary(
                 '/services.WorkerService/BatchGetArtifact',
@@ -48,29 +54,29 @@
                 response_deserializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartResponse.FromString,
                 )
         self.CheckFunction = channel.unary_unary(
                 '/services.WorkerService/CheckFunction',
                 request_serializer=endpoints_dot_check__function__pb2.CheckFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_check__function__pb2.CheckFunctionResponse.FromString,
                 )
-        self.ExecuteFunction = channel.unary_unary(
-                '/services.WorkerService/ExecuteFunction',
-                request_serializer=endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.SerializeToString,
-                response_deserializer=endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.FromString,
-                )
         self.Initiate = channel.unary_unary(
                 '/services.WorkerService/Initiate',
                 request_serializer=endpoints_dot_header__pb2.HeaderRequest.SerializeToString,
                 response_deserializer=endpoints_dot_header__pb2.HeaderResponse.FromString,
                 )
         self.RegisterFunction = channel.unary_unary(
                 '/services.WorkerService/RegisterFunction',
                 request_serializer=endpoints_dot_register__function__pb2.RegisterFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_register__function__pb2.RegisterFunctionResponse.FromString,
                 )
+        self.SDKServerReady = channel.unary_unary(
+                '/services.WorkerService/SDKServerReady',
+                request_serializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.SerializeToString,
+                response_deserializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.FromString,
+                )
 
 
 class WorkerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def BatchCreateArtifact(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -80,14 +86,20 @@
 
     def BatchCreateArtifactPart(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def BatchExecuteFunction(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def BatchFinalizeArtifact(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BatchGetArtifact(self, request, context):
@@ -104,27 +116,27 @@
 
     def CheckFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ExecuteFunction(self, request, context):
+    def Initiate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Initiate(self, request, context):
+    def RegisterFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def RegisterFunction(self, request, context):
+    def SDKServerReady(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_WorkerServiceServicer_to_server(servicer, server):
@@ -135,14 +147,19 @@
                     response_serializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.SerializeToString,
             ),
             'BatchCreateArtifactPart': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchCreateArtifactPart,
                     request_deserializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.FromString,
                     response_serializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.SerializeToString,
             ),
+            'BatchExecuteFunction': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchExecuteFunction,
+                    request_deserializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionRequest.FromString,
+                    response_serializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionResponse.SerializeToString,
+            ),
             'BatchFinalizeArtifact': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchFinalizeArtifact,
                     request_deserializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactRequest.FromString,
                     response_serializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactResponse.SerializeToString,
             ),
             'BatchGetArtifact': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchGetArtifact,
@@ -155,29 +172,29 @@
                     response_serializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartResponse.SerializeToString,
             ),
             'CheckFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.CheckFunction,
                     request_deserializer=endpoints_dot_check__function__pb2.CheckFunctionRequest.FromString,
                     response_serializer=endpoints_dot_check__function__pb2.CheckFunctionResponse.SerializeToString,
             ),
-            'ExecuteFunction': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExecuteFunction,
-                    request_deserializer=endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.FromString,
-                    response_serializer=endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.SerializeToString,
-            ),
             'Initiate': grpc.unary_unary_rpc_method_handler(
                     servicer.Initiate,
                     request_deserializer=endpoints_dot_header__pb2.HeaderRequest.FromString,
                     response_serializer=endpoints_dot_header__pb2.HeaderResponse.SerializeToString,
             ),
             'RegisterFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.RegisterFunction,
                     request_deserializer=endpoints_dot_register__function__pb2.RegisterFunctionRequest.FromString,
                     response_serializer=endpoints_dot_register__function__pb2.RegisterFunctionResponse.SerializeToString,
             ),
+            'SDKServerReady': grpc.unary_unary_rpc_method_handler(
+                    servicer.SDKServerReady,
+                    request_deserializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.FromString,
+                    response_serializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'services.WorkerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -215,14 +232,31 @@
         return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchCreateArtifactPart',
             endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.SerializeToString,
             endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def BatchExecuteFunction(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchExecuteFunction',
+            endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionRequest.SerializeToString,
+            endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def BatchFinalizeArtifact(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -283,56 +317,56 @@
         return grpc.experimental.unary_unary(request, target, '/services.WorkerService/CheckFunction',
             endpoints_dot_check__function__pb2.CheckFunctionRequest.SerializeToString,
             endpoints_dot_check__function__pb2.CheckFunctionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ExecuteFunction(request,
+    def Initiate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/ExecuteFunction',
-            endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.SerializeToString,
-            endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/Initiate',
+            endpoints_dot_header__pb2.HeaderRequest.SerializeToString,
+            endpoints_dot_header__pb2.HeaderResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Initiate(request,
+    def RegisterFunction(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/Initiate',
-            endpoints_dot_header__pb2.HeaderRequest.SerializeToString,
-            endpoints_dot_header__pb2.HeaderResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/RegisterFunction',
+            endpoints_dot_register__function__pb2.RegisterFunctionRequest.SerializeToString,
+            endpoints_dot_register__function__pb2.RegisterFunctionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def RegisterFunction(request,
+    def SDKServerReady(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/RegisterFunction',
-            endpoints_dot_register__function__pb2.RegisterFunctionRequest.SerializeToString,
-            endpoints_dot_register__function__pb2.RegisterFunctionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/SDKServerReady',
+            endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.SerializeToString,
+            endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/gen/services/worker_pb2_grpc.pyi` & `preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import preemo.gen.endpoints.batch_create_artifact_part_pb2
 import preemo.gen.endpoints.batch_create_artifact_pb2
+import preemo.gen.endpoints.batch_execute_function_pb2
 import preemo.gen.endpoints.batch_finalize_artifact_pb2
 import preemo.gen.endpoints.batch_get_artifact_part_pb2
 import preemo.gen.endpoints.batch_get_artifact_pb2
 import preemo.gen.endpoints.check_function_pb2
-import preemo.gen.endpoints.execute_function_pb2
 import preemo.gen.endpoints.header_pb2
 import preemo.gen.endpoints.register_function_pb2
+import preemo.gen.endpoints.sdk_server_ready_pb2
 import grpc
 
 class WorkerServiceStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
     BatchCreateArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactRequest,
         preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactResponse,
     ]
     BatchCreateArtifactPart: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartRequest,
         preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartResponse,
     ]
+    BatchExecuteFunction: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionRequest,
+        preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionResponse,
+    ]
     BatchFinalizeArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactRequest,
         preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactResponse,
     ]
     BatchGetArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactRequest,
         preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactResponse,
@@ -36,26 +41,26 @@
         preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartRequest,
         preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartResponse,
     ]
     CheckFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.check_function_pb2.CheckFunctionRequest,
         preemo.gen.endpoints.check_function_pb2.CheckFunctionResponse,
     ]
-    ExecuteFunction: grpc.UnaryUnaryMultiCallable[
-        preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionRequest,
-        preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionResponse,
-    ]
     Initiate: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.header_pb2.HeaderRequest,
         preemo.gen.endpoints.header_pb2.HeaderResponse,
     ]
     RegisterFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.register_function_pb2.RegisterFunctionRequest,
         preemo.gen.endpoints.register_function_pb2.RegisterFunctionResponse,
     ]
+    SDKServerReady: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyRequest,
+        preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyResponse,
+    ]
 
 class WorkerServiceServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def BatchCreateArtifact(
         self,
         request: preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactRequest,
         context: grpc.ServicerContext,
@@ -63,14 +68,20 @@
     @abc.abstractmethod
     def BatchCreateArtifactPart(
         self,
         request: preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartResponse: ...
     @abc.abstractmethod
+    def BatchExecuteFunction(
+        self,
+        request: preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionRequest,
+        context: grpc.ServicerContext,
+    ) -> preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionResponse: ...
+    @abc.abstractmethod
     def BatchFinalizeArtifact(
         self,
         request: preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactResponse: ...
     @abc.abstractmethod
     def BatchGetArtifact(
@@ -87,26 +98,26 @@
     @abc.abstractmethod
     def CheckFunction(
         self,
         request: preemo.gen.endpoints.check_function_pb2.CheckFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.check_function_pb2.CheckFunctionResponse: ...
     @abc.abstractmethod
-    def ExecuteFunction(
-        self,
-        request: preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionRequest,
-        context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionResponse: ...
-    @abc.abstractmethod
     def Initiate(
         self,
         request: preemo.gen.endpoints.header_pb2.HeaderRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.header_pb2.HeaderResponse: ...
     @abc.abstractmethod
     def RegisterFunction(
         self,
         request: preemo.gen.endpoints.register_function_pb2.RegisterFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.register_function_pb2.RegisterFunctionResponse: ...
+    @abc.abstractmethod
+    def SDKServerReady(
+        self,
+        request: preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyRequest,
+        context: grpc.ServicerContext,
+    ) -> preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyResponse: ...
 
 def add_WorkerServiceServicer_to_server(servicer: WorkerServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/worker/_function_registry.py` & `preemo_worker_sdk-0.3.0/preemo/worker/_function_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,22 +24,28 @@
 
         if name in functions_by_name:
             raise Exception(
                 f"must not register multiple functions with the same namespace: {namespace} and name: {name}"
             )
         functions_by_name[name] = function
 
-    def get_function(self, *, name: str, namespace: Optional[str] = None) -> Callable:
+    def get_function(
+        self, *, name: str, namespace: Optional[str] = None
+    ) -> Optional[Callable]:
         if namespace is None:
-            function = self._global_functions_by_name.get(name)
-            if function is None:
-                raise Exception(f"cannot find registered function with name: {name}")
+            return self._global_functions_by_name.get(name)
 
-            return function
+        return self._functions_by_namespace_and_name.get(namespace, {}).get(name)
 
-        function = self._functions_by_namespace_and_name.get(namespace, {}).get(name)
-        if function is None:
-            raise Exception(
-                f"cannot find registered function with namespace: {namespace} and name: {name}"
-            )
+    def get_required_function(
+        self, *, name: str, namespace: Optional[str] = None
+    ) -> Callable:
+        func = self.get_function(name=name, namespace=namespace)
+        if func is not None:
+            return func
+
+        if namespace is None:
+            raise Exception(f"cannot find registered function with name: {name}")
 
-        return function
+        raise Exception(
+            f"cannot find registered function with namespace {namespace} and name: {name}"
+        )
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/worker/_messaging_client.py` & `preemo_worker_sdk-0.3.0/preemo/worker/_messaging_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     BatchCreateArtifactPartRequest,
     BatchCreateArtifactPartResponse,
 )
 from preemo.gen.endpoints.batch_create_artifact_pb2 import (
     BatchCreateArtifactRequest,
     BatchCreateArtifactResponse,
 )
+from preemo.gen.endpoints.batch_execute_function_pb2 import (
+    BatchExecuteFunctionRequest,
+    BatchExecuteFunctionResponse,
+)
 from preemo.gen.endpoints.batch_finalize_artifact_pb2 import (
     BatchFinalizeArtifactRequest,
     BatchFinalizeArtifactResponse,
 )
 from preemo.gen.endpoints.batch_get_artifact_part_pb2 import (
     BatchGetArtifactPartRequest,
     BatchGetArtifactPartResponse,
@@ -23,23 +27,23 @@
     BatchGetArtifactRequest,
     BatchGetArtifactResponse,
 )
 from preemo.gen.endpoints.check_function_pb2 import (
     CheckFunctionRequest,
     CheckFunctionResponse,
 )
-from preemo.gen.endpoints.execute_function_pb2 import (
-    ExecuteFunctionRequest,
-    ExecuteFunctionResponse,
-)
 from preemo.gen.endpoints.header_pb2 import HeaderRequest, HeaderResponse
 from preemo.gen.endpoints.register_function_pb2 import (
     RegisterFunctionRequest,
     RegisterFunctionResponse,
 )
+from preemo.gen.endpoints.sdk_server_ready_pb2 import (
+    SDKServerReadyRequest,
+    SDKServerReadyResponse,
+)
 from preemo.gen.services.worker_pb2_grpc import WorkerServiceStub
 from preemo.worker._validation import ensure_keys_match
 
 
 @runtime_checkable
 class IMessagingClient(Protocol):
     def batch_create_artifact(
@@ -48,14 +52,19 @@
         pass
 
     def batch_create_artifact_part(
         self, request: BatchCreateArtifactPartRequest
     ) -> BatchCreateArtifactPartResponse:
         pass
 
+    def batch_execute_function(
+        self, request: BatchExecuteFunctionRequest
+    ) -> BatchExecuteFunctionResponse:
+        pass
+
     def batch_finalize_artifact(
         self, request: BatchFinalizeArtifactRequest
     ) -> BatchFinalizeArtifactResponse:
         pass
 
     def batch_get_artifact(
         self, request: BatchGetArtifactRequest
@@ -66,24 +75,24 @@
         self, request: BatchGetArtifactPartRequest
     ) -> BatchGetArtifactPartResponse:
         pass
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         pass
 
-    def execute_function(
-        self, request: ExecuteFunctionRequest
-    ) -> ExecuteFunctionResponse:
-        pass
-
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         pass
 
+    def sdk_server_ready(
+        self, request: SDKServerReadyRequest
+    ) -> SDKServerReadyResponse:
+        pass
+
 
 class MessagingClient:
     def __init__(self, *, worker_server_url: str) -> None:
         # TODO(adrian@preemo.io, 03/25/2023): investigate whether it makes sense to use secure_channel instead
         self._channel = grpc.insecure_channel(target=worker_server_url)
         self._worker_service = WorkerServiceStub(self._channel)
 
@@ -96,25 +105,58 @@
         self, request: BatchCreateArtifactRequest
     ) -> BatchCreateArtifactResponse:
         response = self._worker_service.BatchCreateArtifact(request)
         ensure_keys_match(
             expected=request.configs_by_index, actual=response.results_by_index
         )
 
+        for result in response.results_by_index.values():
+            if not result.HasField("artifact_id"):
+                raise Exception("expected CreateArtifactResult to have artifact_id")
+
+            if not result.HasField("part_size_threshold"):
+                raise Exception(
+                    "expected CreateArtifactResult to have part_size_threshold"
+                )
+
         return response
 
     def batch_create_artifact_part(
         self, request: BatchCreateArtifactPartRequest
     ) -> BatchCreateArtifactPartResponse:
         response = self._worker_service.BatchCreateArtifactPart(request)
         ensure_keys_match(
             expected=request.configs_by_artifact_id,
             actual=response.results_by_artifact_id,
         )
 
+        for artifact_id, result in response.results_by_artifact_id.items():
+            config = request.configs_by_artifact_id[artifact_id]
+            ensure_keys_match(
+                expected=config.metadatas_by_part_number,
+                actual=result.metadatas_by_part_number,
+            )
+
+            for metadata in result.metadatas_by_part_number.values():
+                if not metadata.HasField("upload_signed_url"):
+                    raise Exception(
+                        "expected CreateArtifactPartResultMetadata to have upload_signed_url"
+                    )
+
+        return response
+
+    def batch_execute_function(
+        self, request: BatchExecuteFunctionRequest
+    ) -> BatchExecuteFunctionResponse:
+        response = self._worker_service.BatchExecuteFunction(request)
+        ensure_keys_match(
+            expected=request.parameters_by_index,
+            actual=response.results_by_index,
+        )
+
         return response
 
     def batch_finalize_artifact(
         self, request: BatchFinalizeArtifactRequest
     ) -> BatchFinalizeArtifactResponse:
         response = self._worker_service.BatchFinalizeArtifact(request)
         ensure_keys_match(
@@ -129,46 +171,65 @@
     ) -> BatchGetArtifactResponse:
         response = self._worker_service.BatchGetArtifact(request)
         ensure_keys_match(
             expected=request.configs_by_artifact_id,
             actual=response.results_by_artifact_id,
         )
 
+        for result in response.results_by_artifact_id.values():
+            if not result.HasField("part_count"):
+                raise Exception("expected GetArtifactResult to have part_count")
+
+            if not result.HasField("part_size_threshold"):
+                raise Exception(
+                    "expected GetArtifactResult to have part_size_threshold"
+                )
+
+            if not result.HasField("total_size"):
+                raise Exception("expected GetArtifactResult to have total_size")
+
         return response
 
     def batch_get_artifact_part(
         self, request: BatchGetArtifactPartRequest
     ) -> BatchGetArtifactPartResponse:
         response = self._worker_service.BatchGetArtifactPart(request)
         ensure_keys_match(
             expected=request.configs_by_artifact_id,
             actual=response.results_by_artifact_id,
         )
 
+        for artifact_id, result in response.results_by_artifact_id.items():
+            config = request.configs_by_artifact_id[artifact_id]
+            ensure_keys_match(
+                expected=config.metadatas_by_part_number,
+                actual=result.metadatas_by_part_number,
+            )
+
+            for metadata in result.metadatas_by_part_number.values():
+                if not metadata.HasField("download_signed_url"):
+                    raise Exception(
+                        "expected GetArtifactPartResultMetadata to have download_signed_url"
+                    )
+
         return response
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         return self._worker_service.CheckFunction(request)
 
-    def execute_function(
-        self, request: ExecuteFunctionRequest
-    ) -> ExecuteFunctionResponse:
-        response = self._worker_service.ExecuteFunction(request)
-        ensure_keys_match(
-            expected=request.parameters_by_index,
-            actual=response.results_by_index,
-        )
-
-        return response
-
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         return self._worker_service.RegisterFunction(request)
 
+    def sdk_server_ready(
+        self, request: SDKServerReadyRequest
+    ) -> SDKServerReadyResponse:
+        return self._worker_service.SDKServerReady(request)
+
 
 # This class is intended to be used for tests and local development
 class LocalMessagingClient:
     def batch_create_artifact(
         self, request: BatchCreateArtifactRequest
     ) -> BatchCreateArtifactResponse:
         print(f"sending batch create artifact request: {request}")
@@ -176,14 +237,20 @@
 
     def batch_create_artifact_part(
         self, request: BatchCreateArtifactPartRequest
     ) -> BatchCreateArtifactPartResponse:
         print(f"sending batch create artifact part request: {request}")
         return BatchCreateArtifactPartResponse()
 
+    def batch_execute_function(
+        self, request: BatchExecuteFunctionRequest
+    ) -> BatchExecuteFunctionResponse:
+        print(f"sending batch execute function request: {request}")
+        return BatchExecuteFunctionResponse()
+
     def batch_finalize_artifact(
         self, request: BatchFinalizeArtifactRequest
     ) -> BatchFinalizeArtifactResponse:
         print(f"sending batch finalize artifact request: {request}")
         return BatchFinalizeArtifactResponse()
 
     def batch_get_artifact(
@@ -198,18 +265,18 @@
         print(f"sending batch get artifact part request: {request}")
         return BatchGetArtifactPartResponse()
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         print(f"sending check function request: {request}")
         return CheckFunctionResponse()
 
-    def execute_function(
-        self, request: ExecuteFunctionRequest
-    ) -> ExecuteFunctionResponse:
-        print(f"sending execute function request: {request}")
-        return ExecuteFunctionResponse()
-
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         print(f"sending register function request: {request}")
         return RegisterFunctionResponse()
+
+    def sdk_server_ready(
+        self, request: SDKServerReadyRequest
+    ) -> SDKServerReadyResponse:
+        print(f"sending sdk server ready request: {request}")
+        return SDKServerReadyResponse()
```

### Comparing `preemo_worker_sdk-0.2.2/preemo/worker/_types.py` & `preemo_worker_sdk-0.3.0/preemo/worker/_types.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/worker/_validation.py` & `preemo_worker_sdk-0.3.0/preemo/worker/_validation.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.2.2/preemo/worker/_worker_client.py` & `preemo_worker_sdk-0.3.0/preemo/worker/_worker_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 from typing import Callable, List, Optional
 
 from google.protobuf.struct_pb2 import NULL_VALUE
 
+from preemo.gen.endpoints.batch_execute_function_pb2 import BatchExecuteFunctionRequest
 from preemo.gen.endpoints.check_function_pb2 import CheckFunctionRequest
-from preemo.gen.endpoints.execute_function_pb2 import ExecuteFunctionRequest
 from preemo.gen.endpoints.register_function_pb2 import RegisterFunctionRequest
 from preemo.gen.models.registered_function_pb2 import RegisteredFunction
 from preemo.gen.models.value_pb2 import Value
 from preemo.worker._artifact_manager import ArtifactId, IArtifactManager
 from preemo.worker._function_registry import FunctionRegistry
 from preemo.worker._messaging_client import IMessagingClient
 from preemo.worker._types import assert_never
 
 
+class Result:
+    # TODO(adrian@preemo.io, 04/20/2023): need to sort out how this class
+    # can be used when error handling, status checking, etc
+    # Perhaps futures should be used instead
+    def __init__(
+        self, *, artifact_id: ArtifactId, artifact_manager: IArtifactManager
+    ) -> None:
+        self._artifact_id = artifact_id
+        self._artifact_manager = artifact_manager
+
+    def get(self) -> bytes:
+        return self._artifact_manager.get_artifact(self._artifact_id)
+
+
 class Function:
     def __init__(
         self,
         *,
         artifact_manager: IArtifactManager,
         messaging_client: IMessagingClient,
         name: str,
@@ -35,23 +49,23 @@
             CheckFunctionRequest(
                 function_to_check=RegisteredFunction(
                     name=self.name, namespace=self.namespace
                 )
             )
         )
 
-    def __call__(self, params: Optional[str] = None) -> Optional[str]:
+    def __call__(self, params: Optional[bytes] = None) -> Optional[Result]:
         if params is None:
             function_parameter = Value(null_value=NULL_VALUE)
         else:
             artifact_id = self._artifact_manager.create_artifact(params)
             function_parameter = Value(artifact_id=artifact_id.value)
 
-        response = self._messaging_client.execute_function(
-            ExecuteFunctionRequest(
+        response = self._messaging_client.batch_execute_function(
+            BatchExecuteFunctionRequest(
                 function_to_execute=RegisteredFunction(
                     name=self.name, namespace=self.namespace
                 ),
                 parameters_by_index={0: function_parameter},
             )
         )
 
@@ -61,45 +75,49 @@
         if kind is None:
             raise Exception("expected kind to be defined")
 
         if kind == "null_value":
             return None
 
         if kind == "artifact_id":
-            return self._artifact_manager.get_artifact(
-                ArtifactId(value=function_result.artifact_id)
+            return Result(
+                artifact_id=ArtifactId(value=function_result.artifact_id),
+                artifact_manager=self._artifact_manager,
             )
 
         assert_never(kind)
 
 
 class WorkerClient:
     def __init__(
-        self, *, artifact_manager: IArtifactManager, messaging_client: IMessagingClient
+        self,
+        *,
+        artifact_manager: IArtifactManager,
+        function_registry: FunctionRegistry,
+        messaging_client: IMessagingClient,
     ) -> None:
         self._artifact_manager = artifact_manager
         self._messaging_client = messaging_client
-
-        self._function_registry = FunctionRegistry()
+        self._function_registry = function_registry
 
     def get_function(self, name: str, *, namespace: Optional[str] = None) -> Function:
         return Function(
             artifact_manager=self._artifact_manager,
             messaging_client=self._messaging_client,
             name=name,
             namespace=namespace,
         )
 
-    def parallelize(
+    def parallel(
         self,
         function: Function,
         *,
-        params: Optional[List[str]] = None,
+        params: Optional[List[bytes]] = None,
         count: Optional[int] = None,
-    ) -> List[Optional[str]]:
+    ) -> List[Optional[Result]]:
         # TODO(adrian@preemo.io, 03/20/2023): should take an optional config argument includes stuff like max batch size
 
         if params is None:
             if count is None:
                 raise ValueError("either params or count must be specified")
 
             if count <= 0:
@@ -117,38 +135,38 @@
 
             artifact_ids = self._artifact_manager.create_artifacts(params)
             function_parameters_by_index = {
                 i: Value(artifact_id=artifact_id.value)
                 for i, artifact_id in enumerate(artifact_ids)
             }
 
-        response = self._messaging_client.execute_function(
-            ExecuteFunctionRequest(
+        response = self._messaging_client.batch_execute_function(
+            BatchExecuteFunctionRequest(
                 function_to_execute=RegisteredFunction(
                     name=function.name, namespace=function.namespace
                 ),
                 parameters_by_index=function_parameters_by_index,
             )
         )
 
-        # TODO(adrian@preemo.io, 03/20/2023): should download results in parallel or return a handle that allows the user to download result
-        results: List[Optional[str]] = []
+        results: List[Optional[Result]] = []
         for _, function_result in sorted(
             response.results_by_index.items(), key=lambda x: x[0]
         ):
             kind = function_result.WhichOneof("kind")
             if kind is None:
                 raise Exception("expected kind to be defined")
 
             if kind == "null_value":
                 results.append(None)
             elif kind == "artifact_id":
                 results.append(
-                    self._artifact_manager.get_artifact(
-                        ArtifactId(value=function_result.artifact_id)
+                    Result(
+                        artifact_id=ArtifactId(value=function_result.artifact_id),
+                        artifact_manager=self._artifact_manager,
                     )
                 )
             else:
                 assert_never(kind)
 
         return results
```

### Comparing `preemo_worker_sdk-0.2.2/pyproject.toml` & `preemo_worker_sdk-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preemo_worker_sdk"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 license = "MIT"
 authors = [
   "Forrest Moret <forrest@preemo.io>",
   "Adrian Miguel <adrian@preemo.io>",
 ]
 readme = "README.md"
@@ -35,14 +35,15 @@
 isort = "5.10.1"
 mypy = "1.0.0"
 mypy-protobuf = "3.4.0"
 pep8-naming = "0.13.0"
 pytest = "7.2.1"
 twine = "4.0.2"
 types-protobuf = "4.21.0.4"
+types-requests = "2.28.11.17"
 
 [tool.autoflake]
 check = true
 exclude = "preemo/gen"
 ignore-init-module-imports = true
 in-place = true
 recursive = true
```

### Comparing `preemo_worker_sdk-0.2.2/PKG-INFO` & `preemo_worker_sdk-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preemo-worker-sdk
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Home-page: https://www.preemo.io/
 License: MIT
 Author: Forrest Moret
 Author-email: forrest@preemo.io
 Requires-Python: >=3.8.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,79 +39,90 @@
 
 In order to register a function with Preemo workers, you can use `register` to decorate your functions.
 
 ```python
 from preemo.worker import register
 
 @register(name="some_name", namespace="dev")
-def do_something(params: str):
+def do_something(params: bytes):
     ...
 ```
 
 Both parameters, `name` and `namespace`, are optional. If the name isn't specified, it will default to the name of the function. If the namespace isn't specified, it will default to a global namespace.
 
 ```python
 @register
 def do_something(params: str):
     # registers with name do_something in the global namespace
     ...
 ```
 
-At the moment, only functions that take 0 or 1 string arguments will work. These functions should also either return `None` or a string.
+At the moment, only functions that take 0 or 1 bytes arguments will work. These functions should also either return `None` or bytes.
 
 ### Execute Function
 
 In order to execute a function that you have previously registered with Preemo workers, you can use `get_function`.
 
 ```python
 from preemo.worker import get_function
 
 do_something = get_function(name="some_name", namespace="dev")
-result = do_something("params")
+result = do_something(b"params")
 ...
 ```
 
 The second parameter, `namespace`, is optional. If the namespace isn't specified, it will default to a global namespace.
 
 ```python
 # gets the function named do_something in the global namespace
 do_something = get_function("do_something")
-result = do_something("params")
+result = do_something(b"params")
 ...
 ```
 
-### Parallelize Function Execution
+### Parallel Function Execution
 
-In order to execute a function with multiple parameters in parallel, you can use `parallelize`.
+In order to execute a function with multiple parameters at the same time, you can use `parallel`.
 
 ```python
-from preemo.worker import parallelize
+from preemo.worker import get_function, parallel
 
 do_something = get_function(name="some_name", namespace="dev")
-results = parallelize(
+results = parallel(
     do_something,
     params=[
-        "params1",
-        "params2",
+        b"params1",
+        b"params2",
         ...
     ]
 )
 ...
 ```
 
 If your function doesn't take a parameter and you'd like to run multiple instances of it in parallel, you can use the `count` parameter.
 
 ```python
 do_something = get_function(name="some_name", namespace="dev")
-results = parallelize(
+results = parallel(
     do_something,
     count=10
 )
 ...
 ```
 
-<!-- TODO(adrian@preemo.io, 03/20/23): include an explanation of the result objects. They should be objects that give you access to the artifacts. -->
+### Results
+
+In order to view the result of an executed function, you can call `.get()`.
+
+```python
+from preemo.worker import get_function
+
+do_something = get_function(name="some_name", namespace="dev")
+result = do_something(b"params")
+value = result.get()
+...
+```
 
 ## Contributing
 
 [Contribution guidelines for this project](CONTRIBUTING.md)
```

