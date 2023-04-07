# Comparing `tmp/rompt-1.0.0.tar.gz` & `tmp/rompt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rompt-1.0.0.tar", last modified: Fri Apr  7 02:53:54 2023, max compression
+gzip compressed data, was "rompt-1.0.1.tar", last modified: Fri Apr  7 15:20:35 2023, max compression
```

## Comparing `rompt-1.0.0.tar` & `rompt-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 02:53:54.499690 rompt-1.0.0/
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1064 2023-04-06 19:58:39.000000 rompt-1.0.0/LICENSE
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2083 2023-04-07 02:53:54.499774 rompt-1.0.0/PKG-INFO
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1776 2023-04-07 02:42:57.000000 rompt-1.0.0/README.md
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)      548 2023-04-07 02:53:54.500067 rompt-1.0.0/setup.cfg
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)       38 2023-04-06 16:56:40.000000 rompt-1.0.0/setup.py
-drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 02:53:54.496406 rompt-1.0.0/src/
-drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 02:53:54.498463 rompt-1.0.0/src/rompt/
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)       97 2023-04-07 02:33:18.000000 rompt-1.0.0/src/rompt/__init__.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)       85 2023-04-06 16:58:13.000000 rompt-1.0.0/src/rompt/__main__.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)      646 2023-04-06 18:18:47.000000 rompt-1.0.0/src/rompt/bindings.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)      993 2023-04-06 19:56:44.000000 rompt-1.0.0/src/rompt/common.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2830 2023-04-06 19:56:09.000000 rompt-1.0.0/src/rompt/generate.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)      966 2023-04-07 02:47:11.000000 rompt-1.0.0/src/rompt/main.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1906 2023-04-06 19:28:50.000000 rompt-1.0.0/src/rompt/pull.py
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2511 2023-04-06 19:33:46.000000 rompt-1.0.0/src/rompt/track.py
-drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 02:53:54.499385 rompt-1.0.0/src/rompt.egg-info/
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2083 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/PKG-INFO
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)      417 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/SOURCES.txt
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)        1 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/dependency_links.txt
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)       42 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/entry_points.txt
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)       17 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/requires.txt
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)        6 2023-04-07 02:53:54.000000 rompt-1.0.0/src/rompt.egg-info/top_level.txt
-drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 02:53:54.499544 rompt-1.0.0/test/
--rw-r--r--   0 dilanozkaynak   (501) staff       (20)     3695 2023-04-07 02:46:10.000000 rompt-1.0.0/test/test_main.py
+drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 15:20:35.342042 rompt-1.0.1/
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1064 2023-04-06 19:58:39.000000 rompt-1.0.1/LICENSE
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2083 2023-04-07 15:20:35.342133 rompt-1.0.1/PKG-INFO
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1776 2023-04-07 02:42:57.000000 rompt-1.0.1/README.md
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)      548 2023-04-07 15:20:35.342447 rompt-1.0.1/setup.cfg
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)       38 2023-04-06 16:56:40.000000 rompt-1.0.1/setup.py
+drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 15:20:35.338562 rompt-1.0.1/src/
+drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 15:20:35.340853 rompt-1.0.1/src/rompt/
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)       97 2023-04-07 02:33:18.000000 rompt-1.0.1/src/rompt/__init__.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)       85 2023-04-06 16:58:13.000000 rompt-1.0.1/src/rompt/__main__.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)      646 2023-04-06 18:18:47.000000 rompt-1.0.1/src/rompt/bindings.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)      993 2023-04-06 19:56:44.000000 rompt-1.0.1/src/rompt/common.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2830 2023-04-06 19:56:09.000000 rompt-1.0.1/src/rompt/generate.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     1181 2023-04-07 15:19:15.000000 rompt-1.0.1/src/rompt/main.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2083 2023-04-07 15:16:13.000000 rompt-1.0.1/src/rompt/pull.py
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2511 2023-04-06 19:33:46.000000 rompt-1.0.1/src/rompt/track.py
+drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 15:20:35.341755 rompt-1.0.1/src/rompt.egg-info/
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     2083 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/PKG-INFO
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)      417 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/SOURCES.txt
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)        1 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/dependency_links.txt
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)       42 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/entry_points.txt
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)       17 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/requires.txt
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)        6 2023-04-07 15:20:35.000000 rompt-1.0.1/src/rompt.egg-info/top_level.txt
+drwxr-xr-x   0 dilanozkaynak   (501) staff       (20)        0 2023-04-07 15:20:35.341917 rompt-1.0.1/test/
+-rw-r--r--   0 dilanozkaynak   (501) staff       (20)     3695 2023-04-07 02:46:10.000000 rompt-1.0.1/test/test_main.py
```

### Comparing `rompt-1.0.0/LICENSE` & `rompt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/PKG-INFO` & `rompt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rompt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to interact with the Rompt API and CLI.
 Home-page: https://github.com/rompt-ai/rompt-py
 Author: Rompt.ai
 Author-email: admin@rompt.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rompt-1.0.0/README.md` & `rompt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/setup.cfg` & `rompt-1.0.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rompt
-version = 1.0.0
+version = 1.0.1
 author = Rompt.ai
 author_email = admin@rompt.ai
 license = MIT
 description = Python library to interact with the Rompt API and CLI.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rompt-ai/rompt-py
```

### Comparing `rompt-1.0.0/src/rompt/bindings.py` & `rompt-1.0.1/src/rompt/bindings.py`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/src/rompt/common.py` & `rompt-1.0.1/src/rompt/common.py`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/src/rompt/generate.py` & `rompt-1.0.1/src/rompt/generate.py`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/src/rompt/main.py` & `rompt-1.0.1/src/rompt/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import argparse
 from .pull import pull
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument(
+    subparser = parser.add_subparsers(dest="command")
+    subparser.required = True
+    pull_parser = subparser.add_parser("pull")
+
+    pull_parser.add_argument(
         "-b", "--branch", type=str, help="Branch", required=False, default=None
     )
-    parser.add_argument(
+    pull_parser.add_argument(
         "-d",
         "--destination",
         type=str,
         help="Destination",
         required=False,
         default="prompts.json",
     )
-    parser.add_argument(
+    pull_parser.add_argument(
         "-t", "--token", type=str, help="API token", required=False, default=None
     )
-    parser.add_argument(
-        "--_env", type=str, help=argparse.SUPPRESS, required=False, default="prod"
+    pull_parser.add_argument(
+        "--_env", type=str, help=argparse.SUPPRESS, required=False, default=None
     )
-    parser.add_argument(
+    pull_parser.add_argument(
         "--_dry", type=bool, help=argparse.SUPPRESS, required=False, default=False
     )
 
     args = parser.parse_args()
-    pull(
-        branch=args.branch,
-        destination=args.destination,
-        api_token=args.token,
-        _dry=args._dry,
-        _env=args._env,
-    )
+
+    if args.command == "pull":
+        pull(
+            branch=args.branch,
+            destination=args.destination,
+            api_token=args.token,
+            _dry=args._dry,
+            _env=args._env,
+        )
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
```

### Comparing `rompt-1.0.0/src/rompt/pull.py` & `rompt-1.0.1/src/rompt/pull.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rompt.common import get_api_token, debug_log
 
 
 def pull(
     branch: Optional[str],
     destination: str,
     api_token: Optional[str],
-    _env: str,
+    _env: Optional[str],
     _dry: bool,
 ):
     root_api = f"api-{_env}.aws.rompt.ai" if _env else "api.aws.rompt.ai"
     api_token = api_token or get_api_token()
 
     debug_log(
         _env,
@@ -27,14 +27,19 @@
                 "rootApi": root_api,
                 "cwd": os.getcwd(),
             },
             indent=2,
         ),
     )
 
+    if not api_token:
+        raise Exception(
+            "You must provide an API token in your env or `--token`. You can get one from https://rompt.ai."
+        )
+
     response = requests.post(
         f"https://{root_api}/pull",
         json=(
             {
                 "apiToken": api_token,
                 "branch": branch,
             }
```

### Comparing `rompt-1.0.0/src/rompt/track.py` & `rompt-1.0.1/src/rompt/track.py`

 * *Files identical despite different names*

### Comparing `rompt-1.0.0/src/rompt.egg-info/PKG-INFO` & `rompt-1.0.1/src/rompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rompt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to interact with the Rompt API and CLI.
 Home-page: https://github.com/rompt-ai/rompt-py
 Author: Rompt.ai
 Author-email: admin@rompt.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `rompt-1.0.0/test/test_main.py` & `rompt-1.0.1/test/test_main.py`

 * *Files identical despite different names*

