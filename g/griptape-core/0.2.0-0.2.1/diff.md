# Comparing `tmp/griptape_core-0.2.0.tar.gz` & `tmp/griptape_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.2.0.tar", max compression
+gzip compressed data, was "griptape_core-0.2.1.tar", max compression
```

## Comparing `griptape_core-0.2.0.tar` & `griptape_core-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.2.0/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.2.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.2.0/griptape/__init__.py
--rw-r--r--   0        0        0      349 2023-04-07 15:43:24.029341 griptape_core-0.2.0/griptape/core/__init__.py
--rw-r--r--   0        0        0      184 2023-04-07 15:22:12.494258 griptape_core-0.2.0/griptape/core/adapters/__init__.py
--rw-r--r--   0        0        0     2389 2023-04-07 15:41:17.249886 griptape_core-0.2.0/griptape/core/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1137 2023-04-07 15:41:45.232080 griptape_core-0.2.0/griptape/core/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.2.0/griptape/core/base_adapter.py
--rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.2.0/griptape/core/base_executor.py
--rw-r--r--   0        0        0     3283 2023-04-07 15:41:17.246638 griptape_core-0.2.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0      358 2023-04-06 20:17:23.179136 griptape_core-0.2.0/griptape/core/decorators.py
--rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.2.0/griptape/core/executors/__init__.py
--rw-r--r--   0        0        0     3043 2023-04-07 15:41:17.244366 griptape_core-0.2.0/griptape/core/executors/docker_executor.py
--rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.2.0/griptape/core/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.2.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.2.0/griptape/core/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.2.0/griptape/core/utils/__init__.py
--rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.2.0/griptape/core/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.2.0/griptape/core/utils/manifest_validator.py
--rw-r--r--   0        0        0      708 2023-04-07 15:45:04.716538 griptape_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.2.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.2.1/griptape/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-07 15:43:24.029341 griptape_core-0.2.1/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-07 15:22:12.494258 griptape_core-0.2.1/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2389 2023-04-07 15:41:17.249886 griptape_core-0.2.1/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1137 2023-04-07 15:41:45.232080 griptape_core-0.2.1/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.2.1/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.2.1/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3283 2023-04-07 15:41:17.246638 griptape_core-0.2.1/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      358 2023-04-06 20:17:23.179136 griptape_core-0.2.1/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.2.1/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3048 2023-04-07 15:57:20.791900 griptape_core-0.2.1/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.2.1/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.2.1/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.2.1/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.2.1/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.2.1/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.2.1/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      708 2023-04-07 15:58:04.457023 griptape_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.2.1/PKG-INFO
```

### Comparing `griptape_core-0.2.0/LICENSE` & `griptape_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/README.md` & `griptape_core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/griptape/core/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.2.1/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/griptape/core/adapters/langchain_tool_adapter.py` & `griptape_core-0.2.1/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/griptape/core/base_tool.py` & `griptape_core-0.2.1/griptape/core/base_tool.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/griptape/core/executors/docker_executor.py` & `griptape_core-0.2.1/griptape/core/executors/docker_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def build_image(self, tool: BaseTool) -> None:
         with tempfile.TemporaryDirectory() as temp_dir:
             shutil.rmtree(temp_dir)
             shutil.copytree(self.tool_dir(tool), temp_dir)
 
             if not tool.dockerfile:
-                dockerfile_path = griptape.abs_path(os.path.join(self.DEFAULT_DOCKERFILE_DIR, tool.DOCKERFILE_FILE))
+                dockerfile_path = griptape.core.abs_path(os.path.join(self.DEFAULT_DOCKERFILE_DIR, tool.DOCKERFILE_FILE))
 
                 shutil.copy(dockerfile_path, temp_dir)
 
             image = self.client.images.build(
                 path=temp_dir,
                 tag=self.image_name(tool),
                 rm=True,
```

### Comparing `griptape_core-0.2.0/griptape/core/executors/local_executor.py` & `griptape_core-0.2.1/griptape/core/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/griptape/core/utils/j2.py` & `griptape_core-0.2.1/griptape/core/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape_core-0.2.0/pyproject.toml` & `griptape_core-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.2.0/PKG-INFO` & `griptape_core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

