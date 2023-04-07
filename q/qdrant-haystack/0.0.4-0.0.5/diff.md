# Comparing `tmp/qdrant_haystack-0.0.4.tar.gz` & `tmp/qdrant_haystack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-0.0.4.tar", max compression
+gzip compressed data, was "qdrant_haystack-0.0.5.tar", max compression
```

## Comparing `qdrant_haystack-0.0.4.tar` & `qdrant_haystack-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-20 13:28:56.080807 qdrant_haystack-0.0.4/LICENSE
--rw-r--r--   0        0        0     1696 2023-03-20 13:28:56.080807 qdrant_haystack-0.0.4/README.md
--rw-r--r--   0        0        0      746 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      100 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2285 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    18456 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-03-20 13:28:56.084807 qdrant_haystack-0.0.4/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 qdrant_haystack-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-07 15:46:44.909403 qdrant_haystack-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3160 2023-04-07 15:46:44.909403 qdrant_haystack-0.0.5/README.md
+-rw-r--r--   0        0        0      746 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2285 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    19054 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 qdrant_haystack-0.0.5/PKG-INFO
```

### Comparing `qdrant_haystack-0.0.4/LICENSE` & `qdrant_haystack-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.4/pyproject.toml` & `qdrant_haystack-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "0.0.4"
+version = "0.0.5"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11"
-qdrant-client = "^1.0.2"
+qdrant-client = "^1.1.2"
 farm-haystack = "^1.13.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^3.1.0"
 black = "^23.1.0"
 isort = "^5.12.0"
```

### Comparing `qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.4/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,23 +33,25 @@
         "cosine": rest.Distance.COSINE,
         "dot_product": rest.Distance.DOT,
         "l2": rest.Distance.EUCLID,
     }
 
     def __init__(
         self,
+        location: Optional[str] = None,
         url: Optional[str] = None,
         port: int = 6333,
         grpc_port: int = 6334,
         prefer_grpc: bool = False,
         https: Optional[bool] = None,
         api_key: Optional[str] = None,
         prefix: Optional[str] = None,
         timeout: Optional[float] = None,
         host: Optional[str] = None,
+        path: Optional[str] = None,
         index: str = "Document",
         embedding_dim: int = 768,
         hnsw_config: Optional[Dict] = None,
         content_field: str = "content",
         name_field: str = "name",
         embedding_field: str = "vector",
         similarity: str = "cosine",
@@ -58,23 +60,25 @@
         duplicate_documents: str = "overwrite",
         recreate_index: bool = False,
         **kwargs,
     ):
         super().__init__()
 
         self.client = qdrant_client.QdrantClient(
+            location=location,
             url=url,
             port=port,
             grpc_port=grpc_port,
             prefer_grpc=prefer_grpc,
             https=https,
             api_key=api_key,
             prefix=prefix,
             timeout=timeout,
             host=host,
+            path=path,
             **kwargs,
         )
 
         self._set_up_collection(
             index, embedding_dim, hnsw_config, recreate_index, similarity
         )
 
@@ -161,18 +165,19 @@
     ) -> List[Document]:
         index = index or self.index
 
         documents: List[Document] = []
 
         next_offset = None
         stop_scrolling = False
+        scroll_filter = self.qdrant_filter_converter.convert(None, ids)
         while not stop_scrolling:
             records, next_offset = self.client.scroll(
                 collection_name=index,
-                scroll_filter=self.qdrant_filter_converter.convert(None, ids),
+                scroll_filter=scroll_filter,
                 limit=batch_size,
                 offset=next_offset,
                 with_payload=True,
                 with_vectors=True,
             )
             stop_scrolling = next_offset is None or (
                 isinstance(next_offset, grpc.PointId)
@@ -197,15 +202,18 @@
 
         try:
             response = self.client.count(
                 collection_name=index,
                 count_filter=qdrant_filters,
             )
             return response.count
-        except UnexpectedResponse:
+        except (UnexpectedResponse, ValueError):
+            # Qdrant local raises ValueError if the collection is not found, but
+            # with the remote server UnexpectedResponse is raised. Until that's unified,
+            # we need to catch both.
             return 0
 
     def get_embedding_count(
         self, filters: Optional[FilterType] = None, index: Optional[str] = None
     ) -> int:
         """
         Return the number of embeddings in the document store, which is the same as the
@@ -486,38 +494,44 @@
             )
             return
 
         try:
             # Check if the collection already exists and validate its
             # current configuration with the parameters.
             collection_info = self.client.get_collection(collection_name)
-            current_distance = collection_info.config.params.vectors.distance
-            current_vector_size = collection_info.config.params.vectors.size
-
-            if current_distance != distance:
-                raise ValueError(
-                    f"Collection '{collection_name}' already exists in Qdrant, "
-                    f"but it is configured with a similarity '{current_distance.name}'. "
-                    f"If you want to use that collection, but with a different "
-                    f"similarity, please set `recreate_collection=True` argument."
-                )
-
-            if current_vector_size != embedding_dim:
-                raise ValueError(
-                    f"Collection '{collection_name}' already exists in Qdrant, "
-                    f"but it is configured with a vector size '{current_vector_size}'. "
-                    f"If you want to use that collection, but with a different "
-                    f"vector size, please set `recreate_collection=True` argument."
-                )
-        except (UnexpectedResponse, _InactiveRpcError):
+        except (UnexpectedResponse, _InactiveRpcError, ValueError):
             # That indicates the collection does not exist, so it can be
             # safely created with any configuration.
+            #
+            # Qdrant local raises ValueError if the collection is not found, but
+            # with the remote server UnexpectedResponse / _InactiveRpcError is raised.
+            # Until that's unified, we need to catch both.
             self._recreate_collection(
                 collection_name, distance, embedding_dim, hnsw_config
             )
+            return
+
+        current_distance = collection_info.config.params.vectors.distance
+        current_vector_size = collection_info.config.params.vectors.size
+
+        if current_distance != distance:
+            raise ValueError(
+                f"Collection '{collection_name}' already exists in Qdrant, "
+                f"but it is configured with a similarity '{current_distance.name}'. "
+                f"If you want to use that collection, but with a different "
+                f"similarity, please set `recreate_collection=True` argument."
+            )
+
+        if current_vector_size != embedding_dim:
+            raise ValueError(
+                f"Collection '{collection_name}' already exists in Qdrant, "
+                f"but it is configured with a vector size '{current_vector_size}'. "
+                f"If you want to use that collection, but with a different "
+                f"vector size, please set `recreate_collection=True` argument."
+            )
 
     def _recreate_collection(
         self, collection_name, distance, embedding_dim, hnsw_config
     ):
         self.client.recreate_collection(
             collection_name=collection_name,
             vectors_config=rest.VectorParams(
```

### Comparing `qdrant_haystack-0.0.4/PKG-INFO` & `qdrant_haystack-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: qdrant-haystack
-Version: 0.0.4
-Summary: An integration of Qdrant ANN vector database backend with Haystack
-License: Apache 2.0
-Author: Kacper Łukawski
-Author-email: kacper.lukawski@qdrant.com
-Requires-Python: >=3.8.1,<=3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: farm-haystack (>=1.13.0,<2.0.0)
-Requires-Dist: qdrant-client (>=1.0.2,<2.0.0)
-Description-Content-Type: text/markdown
-
 # qdrant-haystack
 
 An integration of [Qdrant](https://qdrant.tech) vector database with [Haystack](https://haystack.deepset.ai/)
 by [deepset](https://www.deepset.ai).
 
 The library finally allows using Qdrant as a document store, and provides an in-place replacement
 for any other vector embeddings store. Thus, you should expect any kind of application to be working
@@ -41,37 +24,81 @@
 Once installed, you can already start using `QdrantDocumentStore` as any other store that supports
 embeddings.
 
 ```python
 from qdrant_haystack import QdrantDocumentStore
 
 document_store = QdrantDocumentStore(
-    url="localhost",
+    "localhost",
     index="Document",
     embedding_dim=512,
     recreate_index=True,
     hnsw_config={"m": 16, "ef_construct": 64}  # Optional
 )
 ```
 
 The list of parameters accepted by `QdrantDocumentStore` is complementary to those used in the
 official [Python Qdrant client](https://github.com/qdrant/qdrant_client).
 
+### Using local in-memory / disk-persisted mode
+
+Qdrant Python client, from version 1.1.1, supports local in-memory/disk-persisted mode. That's
+a good choice for any test scenarios and quick experiments in which you do not plan to store
+lots of vectors. In such a case spinning a Docker container might be even not required.
+
+The local mode was also implemented in `qdrant-haystack` integration.
+
+#### In-memory storage
+
+In case you want to have a transient storage, for example in case of automated tests launched
+during your CI/CD pipeline, using Qdrant Local mode with in-memory storage might be a preferred
+option. It might be simply enabled by passing `:memory:` as first parameter, while creating an
+instance of `QdrantDocumentStore`.
+
+```python
+from qdrant_haystack import QdrantDocumentStore
+
+document_store = QdrantDocumentStore(
+    ":memory:",
+    index="Document",
+    embedding_dim=512,
+    recreate_index=True,
+    hnsw_config={"m": 16, "ef_construct": 64}  # Optional
+)
+```
+
+#### On disk storage
+
+However, if you prefer to keep the vectors between different runs of your application, it
+might be better to use on disk storage and pass the path that should be used to persist
+the data.
+
+```python
+from qdrant_haystack import QdrantDocumentStore
+
+document_store = QdrantDocumentStore(
+    path="/home/qdrant/storage_local",
+    index="Document",
+    embedding_dim=512,
+    recreate_index=True,
+    hnsw_config={"m": 16, "ef_construct": 64}  # Optional
+)
+```
+
 ### Connecting to Qdrant Cloud cluster
 
 If you prefer not to manage your own Qdrant instance, [Qdrant Cloud](https://cloud.qdrant.io/)
 might be a better option.
 
 ```python
 from qdrant_haystack import QdrantDocumentStore
 
 document_store = QdrantDocumentStore(
-    url="https://YOUR-CLUSTER-URL.aws.cloud.qdrant.io",
+    "https://YOUR-CLUSTER-URL.aws.cloud.qdrant.io",
     index="Document",
     api_key="<< YOUR QDRANT CLOUD API KEY >>",
     embedding_dim=512,
     recreate_index=True,
 )
 ```
 
 There is no difference in terms of functionality between local instances and cloud clusters.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

