# Comparing `tmp/codetalk-0.3.0.tar.gz` & `tmp/codetalk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codetalk-0.3.0.tar", last modified: Fri Apr  7 07:36:01 2023, max compression
+gzip compressed data, was "codetalk-0.3.1.tar", last modified: Fri Apr  7 18:32:02 2023, max compression
```

## Comparing `codetalk-0.3.0.tar` & `codetalk-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 07:36:01.391398 codetalk-0.3.0/
--rw-r--r--   0 albert     (501) staff       (20)      557 2023-03-29 20:07:15.000000 codetalk-0.3.0/LICENSE.txt
--rw-r--r--   0 albert     (501) staff       (20)      896 2023-04-07 07:36:01.391276 codetalk-0.3.0/PKG-INFO
--rw-r--r--   0 albert     (501) staff       (20)      749 2023-03-30 03:44:55.000000 codetalk-0.3.0/README.md
--rw-r--r--   0 albert     (501) staff       (20)       38 2023-04-07 07:36:01.391438 codetalk-0.3.0/setup.cfg
--rw-r--r--   0 albert     (501) staff       (20)      897 2023-04-03 05:54:29.000000 codetalk-0.3.0/setup.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 07:36:01.388352 codetalk-0.3.0/src/
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 07:36:01.390271 codetalk-0.3.0/src/codetalk/
--rw-r--r--   0 albert     (501) staff       (20)        0 2023-03-29 20:07:15.000000 codetalk-0.3.0/src/codetalk/__init__.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 07:36:01.391140 codetalk-0.3.0/src/codetalk/assets/
--rw-r--r--   0 albert     (501) staff       (20)      571 2023-03-29 20:07:15.000000 codetalk-0.3.0/src/codetalk/assets/logo.txt
--rw-r--r--   0 albert     (501) staff       (20)        6 2023-04-07 07:35:10.000000 codetalk-0.3.0/src/codetalk/assets/version.txt
--rw-r--r--   0 albert     (501) staff       (20)     5652 2023-04-07 06:59:58.000000 codetalk-0.3.0/src/codetalk/backend.py
--rw-r--r--   0 albert     (501) staff       (20)      624 2023-04-07 02:53:35.000000 codetalk-0.3.0/src/codetalk/config.py
--rw-r--r--   0 albert     (501) staff       (20)     6366 2023-04-05 19:00:00.000000 codetalk-0.3.0/src/codetalk/filtration.py
--rw-r--r--   0 albert     (501) staff       (20)     6126 2023-04-04 06:09:21.000000 codetalk-0.3.0/src/codetalk/formatter.py
--rw-r--r--   0 albert     (501) staff       (20)     2277 2023-04-07 07:32:01.000000 codetalk-0.3.0/src/codetalk/index.py
--rw-r--r--   0 albert     (501) staff       (20)      744 2023-03-29 20:07:15.000000 codetalk-0.3.0/src/codetalk/logconf.py
--rw-r--r--   0 albert     (501) staff       (20)     4325 2023-04-07 07:27:36.000000 codetalk-0.3.0/src/codetalk/main.py
--rw-r--r--   0 albert     (501) staff       (20)     1462 2023-03-29 20:07:15.000000 codetalk-0.3.0/src/codetalk/spinner.py
--rw-r--r--   0 albert     (501) staff       (20)     3774 2023-04-07 07:29:01.000000 codetalk-0.3.0/src/codetalk/subcommand.py
-drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 07:36:01.390941 codetalk-0.3.0/src/codetalk.egg-info/
--rw-r--r--   0 albert     (501) staff       (20)      896 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/PKG-INFO
--rw-r--r--   0 albert     (501) staff       (20)      552 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/SOURCES.txt
--rw-r--r--   0 albert     (501) staff       (20)        1 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/dependency_links.txt
--rw-r--r--   0 albert     (501) staff       (20)       48 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/entry_points.txt
--rw-r--r--   0 albert     (501) staff       (20)       65 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/requires.txt
--rw-r--r--   0 albert     (501) staff       (20)        9 2023-04-07 07:36:01.000000 codetalk-0.3.0/src/codetalk.egg-info/top_level.txt
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 18:32:02.469202 codetalk-0.3.1/
+-rw-r--r--   0 albert     (501) staff       (20)      557 2023-03-29 20:07:15.000000 codetalk-0.3.1/LICENSE.txt
+-rw-r--r--   0 albert     (501) staff       (20)      896 2023-04-07 18:32:02.469081 codetalk-0.3.1/PKG-INFO
+-rw-r--r--   0 albert     (501) staff       (20)      749 2023-03-30 03:44:55.000000 codetalk-0.3.1/README.md
+-rw-r--r--   0 albert     (501) staff       (20)       38 2023-04-07 18:32:02.469236 codetalk-0.3.1/setup.cfg
+-rw-r--r--   0 albert     (501) staff       (20)      897 2023-04-03 05:54:29.000000 codetalk-0.3.1/setup.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 18:32:02.465595 codetalk-0.3.1/src/
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 18:32:02.467852 codetalk-0.3.1/src/codetalk/
+-rw-r--r--   0 albert     (501) staff       (20)        0 2023-03-29 20:07:15.000000 codetalk-0.3.1/src/codetalk/__init__.py
+-rw-r--r--   0 albert     (501) staff       (20)      384 2023-04-07 18:30:53.000000 codetalk-0.3.1/src/codetalk/asset.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 18:32:02.468935 codetalk-0.3.1/src/codetalk/assets/
+-rw-r--r--   0 albert     (501) staff       (20)      571 2023-03-29 20:07:15.000000 codetalk-0.3.1/src/codetalk/assets/logo.txt
+-rw-r--r--   0 albert     (501) staff       (20)        6 2023-04-07 18:31:21.000000 codetalk-0.3.1/src/codetalk/assets/version.txt
+-rw-r--r--   0 albert     (501) staff       (20)     5648 2023-04-07 18:30:36.000000 codetalk-0.3.1/src/codetalk/backend.py
+-rw-r--r--   0 albert     (501) staff       (20)      624 2023-04-07 02:53:35.000000 codetalk-0.3.1/src/codetalk/config.py
+-rw-r--r--   0 albert     (501) staff       (20)     6366 2023-04-05 19:00:00.000000 codetalk-0.3.1/src/codetalk/filtration.py
+-rw-r--r--   0 albert     (501) staff       (20)     6126 2023-04-04 06:09:21.000000 codetalk-0.3.1/src/codetalk/formatter.py
+-rw-r--r--   0 albert     (501) staff       (20)     2277 2023-04-07 07:32:01.000000 codetalk-0.3.1/src/codetalk/index.py
+-rw-r--r--   0 albert     (501) staff       (20)      744 2023-03-29 20:07:15.000000 codetalk-0.3.1/src/codetalk/logconf.py
+-rw-r--r--   0 albert     (501) staff       (20)     3987 2023-04-07 18:27:29.000000 codetalk-0.3.1/src/codetalk/main.py
+-rw-r--r--   0 albert     (501) staff       (20)     1462 2023-03-29 20:07:15.000000 codetalk-0.3.1/src/codetalk/spinner.py
+-rw-r--r--   0 albert     (501) staff       (20)     3774 2023-04-07 07:29:01.000000 codetalk-0.3.1/src/codetalk/subcommand.py
+drwxr-xr-x   0 albert     (501) staff       (20)        0 2023-04-07 18:32:02.468701 codetalk-0.3.1/src/codetalk.egg-info/
+-rw-r--r--   0 albert     (501) staff       (20)      896 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/PKG-INFO
+-rw-r--r--   0 albert     (501) staff       (20)      574 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/SOURCES.txt
+-rw-r--r--   0 albert     (501) staff       (20)        1 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/dependency_links.txt
+-rw-r--r--   0 albert     (501) staff       (20)       48 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/entry_points.txt
+-rw-r--r--   0 albert     (501) staff       (20)       65 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/requires.txt
+-rw-r--r--   0 albert     (501) staff       (20)        9 2023-04-07 18:32:02.000000 codetalk-0.3.1/src/codetalk.egg-info/top_level.txt
```

### Comparing `codetalk-0.3.0/LICENSE.txt` & `codetalk-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/PKG-INFO` & `codetalk-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codetalk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Talk to your code!
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # codetalk
 
 Talk to your code!
```

### Comparing `codetalk-0.3.0/README.md` & `codetalk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/setup.py` & `codetalk-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/assets/logo.txt` & `codetalk-0.3.1/src/codetalk/assets/logo.txt`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/backend.py` & `codetalk-0.3.1/src/codetalk/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import requests
 import sseclient
 import traceback
 
 from . import logconf
 from . import index
+from .asset import get_asset
 from .config import get_config
 from .formatter import TokenFormatter
 from .spinner import spinner
 
 SERVER_ADDRESS = "https://server.codetalk.ai:8000"
 
 def codetalk_api_call(route, payload={}, use_gzip=False):
@@ -164,17 +165,15 @@
     try:
         response = requests.get(addr)
         latest_version = response.json()["version"]
     except Exception as e:
         logging.error(f"Error checking for updates: {e}")
         return
 
-    with open("assets/version.txt") as fp:
-        current_version = fp.read().strip()
-
+    current_version = get_asset('version.txt').strip()
     if current_version != latest_version:
         current_major, current_minor, current_subversion = map(int, current_version.split('.'))
         latest_major, latest_minor, latest_subversion = map(int, latest_version.split('.'))
 
         if current_major < latest_major:
             print_bold_red(f"Major update available! Your version: {current_version}, latest version: {latest_version}")
         elif current_minor < latest_minor or current_subversion < latest_subversion:
```

### Comparing `codetalk-0.3.0/src/codetalk/config.py` & `codetalk-0.3.1/src/codetalk/config.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/filtration.py` & `codetalk-0.3.1/src/codetalk/filtration.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/formatter.py` & `codetalk-0.3.1/src/codetalk/formatter.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/index.py` & `codetalk-0.3.1/src/codetalk/index.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/logconf.py` & `codetalk-0.3.1/src/codetalk/logconf.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/main.py` & `codetalk-0.3.1/src/codetalk/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import logging
 import os
 
 from . import logconf
+from .asset import get_version, print_logo
 from .backend import check_for_updates, create_index, get_response, validate_token
 from .config import get_config, set_config
 from .subcommand import is_chat_command, list_projects
 
 from prompt_toolkit import prompt
 from prompt_toolkit.completion import Completer, PathCompleter
 from prompt_toolkit.document import Document
@@ -21,28 +22,14 @@
         if len(words) > 1 and words[0] in ['delete', 'use', 'index']:
             path = words[-1]
             path_completer = PathCompleter(expanduser=True)
             path_doc = Document(text=path, cursor_position=len(path))
             for completion in path_completer.get_completions(path_doc, complete_event):
                 yield completion
 
-def _get_asset(file_name):
-    dir_path = os.path.dirname(os.path.realpath(__file__))
-    asset_path = os.path.join(dir_path, 'assets', file_name)
-    with open(asset_path) as fp:
-        return fp.read()
-
-def _print_logo():
-    logo = _get_asset('logo.txt')
-    print(logo)
-
-def _get_version():
-    version = _get_asset('version.txt')
-    print(f"codetalk version: {version}")
-
 def _validate():
     fields = ['current_project', 'user_token']
     return all(get_config(f) for f in fields)
 
 def _setup():
     if not get_config('user_token'):
         while True:
@@ -76,15 +63,15 @@
     if wrap_count > 0:
         return " " * (width - 3) + "-> "
     else:
         text = "...: ".rjust(width)
         return HTML("<ansigray>%s</ansigray>") % text
 
 def converse():
-    _print_logo()
+    print_logo()
     messages = []
 
     if not _validate():
         _setup()
     list_projects(truncate=True)
     print("Type `help` to see a list of commands.\n")
 
@@ -122,14 +109,14 @@
 def main():
     parser = argparse.ArgumentParser(description='codetalk')
     parser.add_argument('-v', '--version', action='store_true', help='Display the version information and exit')
 
     args = parser.parse_args()
 
     if args.version:
-        _get_version()
+        get_version()
     else:
         check_for_updates()
         converse()
 
 if __name__ == '__main__':
     main()
```

### Comparing `codetalk-0.3.0/src/codetalk/spinner.py` & `codetalk-0.3.1/src/codetalk/spinner.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk/subcommand.py` & `codetalk-0.3.1/src/codetalk/subcommand.py`

 * *Files identical despite different names*

### Comparing `codetalk-0.3.0/src/codetalk.egg-info/PKG-INFO` & `codetalk-0.3.1/src/codetalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codetalk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Talk to your code!
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # codetalk
 
 Talk to your code!
```

### Comparing `codetalk-0.3.0/src/codetalk.egg-info/SOURCES.txt` & `codetalk-0.3.1/src/codetalk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.txt
 README.md
 setup.py
 src/codetalk/__init__.py
+src/codetalk/asset.py
 src/codetalk/backend.py
 src/codetalk/config.py
 src/codetalk/filtration.py
 src/codetalk/formatter.py
 src/codetalk/index.py
 src/codetalk/logconf.py
 src/codetalk/main.py
```

