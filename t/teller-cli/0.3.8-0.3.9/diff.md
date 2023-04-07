# Comparing `tmp/teller_cli-0.3.8.tar.gz` & `tmp/teller_cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teller_cli-0.3.8.tar", max compression
+gzip compressed data, was "teller_cli-0.3.9.tar", max compression
```

## Comparing `teller_cli-0.3.8.tar` & `teller_cli-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1356 2023-04-02 06:28:41.263825 teller_cli-0.3.8/README.md
--rw-r--r--   0        0        0      562 2023-04-07 17:47:17.624658 teller_cli-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5105 2023-04-07 17:48:12.003483 teller_cli-0.3.8/teller_cli/__init__.py
--rw-r--r--   0        0        0       87 2023-03-10 04:52:35.334095 teller_cli-0.3.8/teller_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-03-10 02:42:44.447116 teller_cli-0.3.8/teller_cli/core/__init__.py
--rw-r--r--   0        0        0     3459 2023-03-31 04:55:21.543518 teller_cli-0.3.8/teller_cli/core/config.py
--rw-r--r--   0        0        0      561 2023-04-02 06:16:14.851429 teller_cli-0.3.8/teller_cli/core/utils/__init__.py
--rw-r--r--   0        0        0    13046 2023-04-07 17:48:12.059487 teller_cli-0.3.8/teller_cli/core/world/__init__.py
--rw-r--r--   0        0        0     6360 2023-04-07 08:52:01.716761 teller_cli-0.3.8/teller_cli/core/world/download.py
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 teller_cli-0.3.8/setup.py
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 teller_cli-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1356 2023-04-02 06:28:41.263825 teller_cli-0.3.9/README.md
+-rw-r--r--   0        0        0      562 2023-04-07 17:51:05.464198 teller_cli-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5129 2023-04-07 17:51:09.017641 teller_cli-0.3.9/teller_cli/__init__.py
+-rw-r--r--   0        0        0       87 2023-03-10 04:52:35.334095 teller_cli-0.3.9/teller_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-10 02:42:44.447116 teller_cli-0.3.9/teller_cli/core/__init__.py
+-rw-r--r--   0        0        0     3459 2023-03-31 04:55:21.543518 teller_cli-0.3.9/teller_cli/core/config.py
+-rw-r--r--   0        0        0      561 2023-04-02 06:16:14.851429 teller_cli-0.3.9/teller_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0    13046 2023-04-07 17:48:12.059487 teller_cli-0.3.9/teller_cli/core/world/__init__.py
+-rw-r--r--   0        0        0     6360 2023-04-07 08:52:01.716761 teller_cli-0.3.9/teller_cli/core/world/download.py
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 teller_cli-0.3.9/setup.py
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 teller_cli-0.3.9/PKG-INFO
```

### Comparing `teller_cli-0.3.8/README.md` & `teller_cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `teller_cli-0.3.8/pyproject.toml` & `teller_cli-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teller-cli"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["JakePIXL <jakewjevans@gmail.com>"]
 readme = "README.md"
 packages = [{include = "teller_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `teller_cli-0.3.8/teller_cli/__init__.py` & `teller_cli-0.3.9/teller_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from teller_cli.core.world import (
     browse_worlds,
     chunk_and_upload,
     compress_folder,
     create_world,
     expand_downloaded,
     get_deep_info,
+    get_folder_size,
     get_info,
     grab_world,
     update_world_size,
 )
 
 from rich import print
 
@@ -50,15 +51,15 @@
     if not world_id:
         world_id = create_world(api_token, api_url, folder_path)
     try:
         zip_file = compress_folder(folder_path)
     except Exception:
         print("> [bold red]Error compressing world.")
 
-    new_file_size = os.path.getsize(zip_file)
+    new_file_size = get_folder_size(folder_path)
 
     if new_file_size > world_size:
         update_world_size(world_id, new_file_size, api_url, api_token)
 
     try:
         chunk_and_upload(zip_file, world_id, api_url, api_token)
     except Exception:
@@ -186,8 +187,8 @@
     except Exception:
         print("> [bold red]Error downloading world.")
 
     if not save:
         os.remove(file_name)
 
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `teller_cli-0.3.8/teller_cli/core/config.py` & `teller_cli-0.3.9/teller_cli/core/config.py`

 * *Files identical despite different names*

### Comparing `teller_cli-0.3.8/teller_cli/core/utils/__init__.py` & `teller_cli-0.3.9/teller_cli/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `teller_cli-0.3.8/teller_cli/core/world/__init__.py` & `teller_cli-0.3.9/teller_cli/core/world/__init__.py`

 * *Files identical despite different names*

### Comparing `teller_cli-0.3.8/teller_cli/core/world/download.py` & `teller_cli-0.3.9/teller_cli/core/world/download.py`

 * *Files identical despite different names*

### Comparing `teller_cli-0.3.8/setup.py` & `teller_cli-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['teller-cli = teller_cli:app']}
 
 setup_kwargs = {
     'name': 'teller-cli',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '',
     'long_description': '# Teller-CLI for ChunkVault-Lite\n\nTeller-CLI is an open source Python/Typer-based CLI tool for uploading Minecraft world backups to ChunkVault-Lite, an open source backup solution provided by Valink Solutions.\n\n## Testing\n\nLimited testing was done on MacOS 13 and Windows 10\n\n## Usage\n\nTo use Teller-CLI, first install the tool:\n\n```bash\n    pip install teller-cli\n```\n\nThen, run the following command to create a snapshot:\n\n```bash\n    teller-cli upload "/path/to/world"\n```\n\nThis will upload the specified backup to ChunkVault-Lite.\n\n### First Launch\n\nOn first launch, Teller-CLI will prompt you to enter the API URL for your ChunkVault-Lite instance. The trailing slash is not necessary, so you can enter the URL without it.\n\nAfter entering the API URL, Teller-CLI will prompt you to enter your API token. You can obtain this token from your ChunkVault-Lite instance. This token is required for authentication purposes and allows Teller-CLI to access your backups.\n\nOnce you have entered the API URL and token, Teller-CLI will store this information locally for future use. You can update this information at any time by running the `teller-cli config` command.\n\n---\n\n## Additional Information\n\nChunkVault-Lite is hosted in a separatly. For more information on ChunkVault-Lite visit the [Repository](https://github.com/Valink-Solutions/ChunkVault-Lite)\n',
     'author': 'JakePIXL',
     'author_email': 'jakewjevans@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `teller_cli-0.3.8/PKG-INFO` & `teller_cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teller-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: JakePIXL
 Author-email: jakewjevans@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

