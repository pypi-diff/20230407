# Comparing `tmp/griptape_core-0.1.3.tar.gz` & `tmp/griptape_core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_core-0.1.3.tar", max compression
+gzip compressed data, was "griptape_core-0.2.0.tar", max compression
```

## Comparing `griptape_core-0.1.3.tar` & `griptape_core-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.1.3/LICENSE
--rw-r--r--   0        0        0     2802 2023-04-06 22:24:07.469627 griptape_core-0.1.3/README.md
--rw-r--r--   0        0        0      389 2023-04-06 20:17:23.178444 griptape_core-0.1.3/griptape/__init__.py
--rw-r--r--   0        0        0      184 2023-04-06 20:17:23.178636 griptape_core-0.1.3/griptape/adapters/__init__.py
--rw-r--r--   0        0        0     2379 2023-04-06 20:17:23.178741 griptape_core-0.1.3/griptape/adapters/chatgpt_plugin_adapter.py
--rw-r--r--   0        0        0     1132 2023-04-06 20:17:23.178828 griptape_core-0.1.3/griptape/adapters/langchain_tool_adapter.py
--rw-r--r--   0        0        0      239 2023-04-06 20:17:23.178902 griptape_core-0.1.3/griptape/base_adapter.py
--rw-r--r--   0        0        0      462 2023-04-06 20:17:23.178986 griptape_core-0.1.3/griptape/base_executor.py
--rw-r--r--   0        0        0     3278 2023-04-06 20:17:23.179069 griptape_core-0.1.3/griptape/base_tool.py
--rw-r--r--   0        0        0      358 2023-04-06 20:17:23.179136 griptape_core-0.1.3/griptape/decorators.py
--rw-r--r--   0        0        0      143 2023-04-06 20:17:23.179248 griptape_core-0.1.3/griptape/executors/__init__.py
--rw-r--r--   0        0        0     3013 2023-04-06 22:49:07.290563 griptape_core-0.1.3/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     1882 2023-04-06 20:17:23.179422 griptape_core-0.1.3/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.1.3/griptape/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
--rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.1.3/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.1.3/griptape/utils/__init__.py
--rw-r--r--   0        0        0      892 2023-04-06 20:17:23.179887 griptape_core-0.1.3/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.1.3/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0      708 2023-04-06 22:51:27.564903 griptape_core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 griptape_core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape_core-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-07 15:41:17.241816 griptape_core-0.2.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_core-0.2.0/griptape/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-07 15:43:24.029341 griptape_core-0.2.0/griptape/core/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-07 15:22:12.494258 griptape_core-0.2.0/griptape/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2389 2023-04-07 15:41:17.249886 griptape_core-0.2.0/griptape/core/adapters/chatgpt_plugin_adapter.py
+-rw-r--r--   0        0        0     1137 2023-04-07 15:41:45.232080 griptape_core-0.2.0/griptape/core/adapters/langchain_tool_adapter.py
+-rw-r--r--   0        0        0      249 2023-04-07 15:41:17.253083 griptape_core-0.2.0/griptape/core/base_adapter.py
+-rw-r--r--   0        0        0      467 2023-04-07 15:43:24.032498 griptape_core-0.2.0/griptape/core/base_executor.py
+-rw-r--r--   0        0        0     3283 2023-04-07 15:41:17.246638 griptape_core-0.2.0/griptape/core/base_tool.py
+-rw-r--r--   0        0        0      358 2023-04-06 20:17:23.179136 griptape_core-0.2.0/griptape/core/decorators.py
+-rw-r--r--   0        0        0      143 2023-04-07 15:22:12.494713 griptape_core-0.2.0/griptape/core/executors/__init__.py
+-rw-r--r--   0        0        0     3043 2023-04-07 15:41:17.244366 griptape_core-0.2.0/griptape/core/executors/docker_executor.py
+-rw-r--r--   0        0        0     1887 2023-04-07 15:42:00.394059 griptape_core-0.2.0/griptape/core/executors/local_executor.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape_core-0.2.0/griptape/core/resources/chatgpt_plugin_adapter/ai-plugin.json.j2
+-rw-r--r--   0        0        0      129 2023-04-06 20:17:23.179693 griptape_core-0.2.0/griptape/core/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      233 2023-04-06 20:17:23.179816 griptape_core-0.2.0/griptape/core/utils/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-07 15:43:39.321508 griptape_core-0.2.0/griptape/core/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape_core-0.2.0/griptape/core/utils/manifest_validator.py
+-rw-r--r--   0        0        0      708 2023-04-07 15:45:04.716538 griptape_core-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 griptape_core-0.2.0/PKG-INFO
```

### Comparing `griptape_core-0.1.3/LICENSE` & `griptape_core-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_core-0.1.3/README.md` & `griptape_core-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 pip install griptape-core
 pip install griptape-tools
 ```
 
 Next, initialize an executor and some tools:
 
 ```python
-from griptape.adapters import LangchainToolAdapter, ChatgptPluginAdapter
-from griptape.executors import LocalExecutor
-from griptape_tools import (
+from griptape.core.adapters import LangchainToolAdapter, ChatgptPluginAdapter
+from griptape.core.executors import LocalExecutor
+from griptape.tools import (
     Calculator, GoogleSearch
 )
 
 tool_executor = LocalExecutor()
 
 google_search = GoogleSearch(
     api_search_key="<search key>",
```

### Comparing `griptape_core-0.1.3/griptape/adapters/chatgpt_plugin_adapter.py` & `griptape_core-0.2.0/griptape/core/adapters/chatgpt_plugin_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import json
 import yaml
 from attr import define, field
 from fastapi import FastAPI
-from griptape import BaseAdapter, BaseTool
-from griptape.utils import J2
+from griptape.core import BaseAdapter, BaseTool
+from griptape.core.utils import J2
 import functools
 
 
 @define
 class ChatgptPluginAdapter(BaseAdapter):
     OPENAI_MANIFEST_FILE = "ai-plugin.json"
     OPENAPI_SPEC_FILE = "openapi.yaml"
```

### Comparing `griptape_core-0.1.3/griptape/adapters/langchain_tool_adapter.py` & `griptape_core-0.2.0/griptape/core/adapters/langchain_tool_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import langchain.tools
 from attr import define
-from griptape import BaseAdapter
+from griptape.core import BaseAdapter
 
 
 @define
 class LangchainToolAdapter(BaseAdapter):
     def generate(self, tool_action: callable) -> langchain.tools.BaseTool:
         tool = tool_action.__self__
```

### Comparing `griptape_core-0.1.3/griptape/base_tool.py` & `griptape_core-0.2.0/griptape/core/base_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
             if getattr(method, "is_action", False):
                 methods.append(method)
 
         return methods
 
     def validate(self) -> bool:
-        from griptape.utils import ManifestValidator
+        from griptape.core.utils import ManifestValidator
 
         if not os.path.exists(self.manifest_path):
             raise Exception(f"{self.MANIFEST_FILE} not found")
 
         if not os.path.exists(self.requirements_path):
             raise Exception(f"{self.REQUIREMENTS_FILE} not found")
```

### Comparing `griptape_core-0.1.3/griptape/executors/docker_executor.py` & `griptape_core-0.2.0/griptape/core/executors/docker_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Optional
 from attr import define, field, Factory
 import docker
 from docker.errors import NotFound
 import griptape
-from griptape import BaseExecutor, BaseTool
+from griptape.core import BaseTool
+from griptape.core import BaseExecutor
 import stringcase
 import tempfile
 import shutil
 import os
 
 
 @define
```

### Comparing `griptape_core-0.1.3/griptape/executors/local_executor.py` & `griptape_core-0.2.0/griptape/core/executors/local_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import subprocess
 from attr import define, field
-from griptape import BaseExecutor, BaseTool
+from griptape.core import BaseExecutor, BaseTool
 
 
 @define
 class LocalExecutor(BaseExecutor):
     verbose: int = field(default=False, kw_only=True)
 
     def execute(self, tool_action: callable, value: bytes) -> bytes:
```

### Comparing `griptape_core-0.1.3/griptape/utils/j2.py` & `griptape_core-0.2.0/griptape/core/utils/j2.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 @define(frozen=True)
 class J2:
     import griptape
 
     template_name: Optional[str] = field(default=None)
-    templates_dir: str = field(default=os.path.join(griptape.PACKAGE_ABS_PATH, "resources"), kw_only=True)
+    templates_dir: str = field(default=os.path.join(griptape.core.PACKAGE_ABS_PATH, "resources"), kw_only=True)
     environment: Environment = field(
         default=Factory(
             lambda self: Environment(
                 loader=FileSystemLoader(self.templates_dir),
                 trim_blocks=True,
                 lstrip_blocks=True
             ),
```

### Comparing `griptape_core-0.1.3/pyproject.toml` & `griptape_core-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-core"
-version = "0.1.3"
+version = "0.2.0"
 description = "Python framework for LLM middleware tools. Build once, run anywhere."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-core"
 
 packages = [
```

### Comparing `griptape_core-0.1.3/PKG-INFO` & `griptape_core-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-core
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python framework for LLM middleware tools. Build once, run anywhere.
 Home-page: https://github.com/griptape-ai/griptape-core
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -50,17 +50,17 @@
 pip install griptape-core
 pip install griptape-tools
 ```
 
 Next, initialize an executor and some tools:
 
 ```python
-from griptape.adapters import LangchainToolAdapter, ChatgptPluginAdapter
-from griptape.executors import LocalExecutor
-from griptape_tools import (
+from griptape.core.adapters import LangchainToolAdapter, ChatgptPluginAdapter
+from griptape.core.executors import LocalExecutor
+from griptape.tools import (
     Calculator, GoogleSearch
 )
 
 tool_executor = LocalExecutor()
 
 google_search = GoogleSearch(
     api_search_key="<search key>",
```

