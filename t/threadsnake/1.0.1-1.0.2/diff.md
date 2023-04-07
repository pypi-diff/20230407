# Comparing `tmp/threadsnake-1.0.1.tar.gz` & `tmp/threadsnake-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsnake-1.0.1.tar", last modified: Fri Apr  7 21:09:28 2023, max compression
+gzip compressed data, was "threadsnake-1.0.2.tar", last modified: Fri Apr  7 21:42:03 2023, max compression
```

## Comparing `threadsnake-1.0.1.tar` & `threadsnake-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.931063 threadsnake-1.0.1/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.1/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-04-07 21:09:28.927063 threadsnake-1.0.1/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.1/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-07 21:09:28.931063 threadsnake-1.0.1/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1420 2023-04-07 21:09:21.000000 threadsnake-1.0.1/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.903063 threadsnake-1.0.1/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.911063 threadsnake-1.0.1/src/threadsnake/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.915063 threadsnake-1.0.1/src/threadsnake/html/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/html/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      577 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/html/tools.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.919063 threadsnake-1.0.1/src/threadsnake/http/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/application.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/constants.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httprequest.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httpresponse.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httpserver.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2559 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/server.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/session.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/core/values/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/contenttypes.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/responsecodes.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/middlewares/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/app.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/authorization.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/bodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/cors.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1332 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/defaultheaders.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/jsonbodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/multipartformdataparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/requests.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/session.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/static.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      467 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/timemeassure.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/router.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/tools/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4248 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/routing.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/types.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/turbo/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/turbo/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.915063 threadsnake-1.0.1/src/threadsnake.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1575 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/top_level.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.750516 threadsnake-1.0.2/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.2/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-07 21:41:56.000000 threadsnake-1.0.2/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      863 2023-04-07 21:42:03.750516 threadsnake-1.0.2/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       86 2023-04-07 21:41:56.000000 threadsnake-1.0.2/README.MD
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.2/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-07 21:42:03.750516 threadsnake-1.0.2/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1155 2023-04-07 21:41:56.000000 threadsnake-1.0.2/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.738515 threadsnake-1.0.2/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.742515 threadsnake-1.0.2/src/threadsnake/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.742515 threadsnake-1.0.2/src/threadsnake/html/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/html/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      577 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/html/tools.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.742515 threadsnake-1.0.2/src/threadsnake/http/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/application.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.746516 threadsnake-1.0.2/src/threadsnake/http/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/constants.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/httprequest.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/httpresponse.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/httpserver.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2559 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/server.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/session.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.746516 threadsnake-1.0.2/src/threadsnake/http/core/values/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/values/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/values/contenttypes.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/core/values/responsecodes.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.746516 threadsnake-1.0.2/src/threadsnake/http/middlewares/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/app.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/authorization.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/bodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/cors.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1332 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/defaultheaders.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/jsonbodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/multipartformdataparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/requests.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/session.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/static.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      467 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/middlewares/timemeassure.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/router.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.746516 threadsnake-1.0.2/src/threadsnake/http/tools/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/tools/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/tools/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4248 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/tools/routing.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/http/types.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.750516 threadsnake-1.0.2/src/threadsnake/turbo/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.2/src/threadsnake/turbo/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:42:03.742515 threadsnake-1.0.2/src/threadsnake.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      863 2023-04-07 21:42:03.000000 threadsnake-1.0.2/src/threadsnake.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1609 2023-04-07 21:42:03.000000 threadsnake-1.0.2/src/threadsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-07 21:42:03.000000 threadsnake-1.0.2/src/threadsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-07 21:42:03.000000 threadsnake-1.0.2/src/threadsnake.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-07 21:38:19.000000 threadsnake-1.0.2/version.txt
```

### Comparing `threadsnake-1.0.1/LICENSE` & `threadsnake-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/PKG-INFO` & `threadsnake-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: threadsnake
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tiny experimental server-side express-like library
 Home-page: https://github.com/LostSavannah/threadsnake
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/threadsnake/issues/
 Project-URL: Documentation, https://dev.moradev.dev/threadsnake/documentation/
 Project-URL: Examples, https://dev.moradev.dev/threadsnake/examples/
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# Threadsnake
+
+
+Threadsnake. A yet tiny experimental server-side express-like library.
```

### Comparing `threadsnake-1.0.1/setup.py` & `threadsnake-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 import os
 import setuptools
 
 def readfile(filename):
-    try:
-        with open(filename, 'r', encoding='latin1') as f:
-            return f.read()
-    except:
-        return ''
-
-version_file = os.sep.join([os.path.abspath(os.curdir), 'version.txt'])
-readme_file = os.sep.join([os.path.abspath(os.curdir), 'README.md'])
-
-print(f'version from: {version_file}')
-print(f'readme from: {readme_file}')
+    with open(filename, 'r', encoding='latin1') as f:
+        return f.read()
 
 setuptools.setup(    
     name="threadsnake",
-    version=readfile(version_file),
+    version=readfile('version.txt'),
     author="Erick Fernando Mora Ramirez",
     author_email="erickfernandomoraramirez@gmail.com",
     description="A tiny experimental server-side express-like library",
-    long_description=readfile(readme_file),
+    long_description=readfile('README.MD'),
     long_description_content_type="text/markdown",
     url="https://github.com/LostSavannah/threadsnake",
     project_urls={
         "Bug Tracker": "https://dev.moradev.dev/threadsnake/issues/",
         "Documentation": "https://dev.moradev.dev/threadsnake/documentation/",
         "Examples": "https://dev.moradev.dev/threadsnake/examples/",
     },
```

### Comparing `threadsnake-1.0.1/src/threadsnake/html/tools.py` & `threadsnake-1.0.2/src/threadsnake/html/tools.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/application.py` & `threadsnake-1.0.2/src/threadsnake/http/application.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/common.py` & `threadsnake-1.0.2/src/threadsnake/http/core/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/constants.py` & `threadsnake-1.0.2/src/threadsnake/http/core/constants.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/httprequest.py` & `threadsnake-1.0.2/src/threadsnake/http/core/httprequest.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/httpresponse.py` & `threadsnake-1.0.2/src/threadsnake/http/core/httpresponse.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/httpserver.py` & `threadsnake-1.0.2/src/threadsnake/http/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/server.py` & `threadsnake-1.0.2/src/threadsnake/http/core/server.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/session.py` & `threadsnake-1.0.2/src/threadsnake/http/core/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/core/values/responsecodes.py` & `threadsnake-1.0.2/src/threadsnake/http/core/values/responsecodes.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/authorization.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/authorization.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/bodyparser.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/bodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/defaultheaders.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/jsonbodyparser.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/jsonbodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/multipartformdataparser.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/multipartformdataparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/requests.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/requests.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/session.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/middlewares/static.py` & `threadsnake-1.0.2/src/threadsnake/http/middlewares/static.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/router.py` & `threadsnake-1.0.2/src/threadsnake/http/router.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/tools/common.py` & `threadsnake-1.0.2/src/threadsnake/http/tools/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/tools/routing.py` & `threadsnake-1.0.2/src/threadsnake/http/tools/routing.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake/http/types.py` & `threadsnake-1.0.2/src/threadsnake/http/types.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.1/src/threadsnake.egg-info/PKG-INFO` & `threadsnake-1.0.2/src/threadsnake.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: threadsnake
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tiny experimental server-side express-like library
 Home-page: https://github.com/LostSavannah/threadsnake
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/threadsnake/issues/
 Project-URL: Documentation, https://dev.moradev.dev/threadsnake/documentation/
 Project-URL: Examples, https://dev.moradev.dev/threadsnake/examples/
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# Threadsnake
+
+
+Threadsnake. A yet tiny experimental server-side express-like library.
```

### Comparing `threadsnake-1.0.1/src/threadsnake.egg-info/SOURCES.txt` & `threadsnake-1.0.2/src/threadsnake.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 LICENSE
+MANIFEST.in
+README.MD
 pyproject.toml
 setup.py
+version.txt
 src/threadsnake/__init__.py
 src/threadsnake.egg-info/PKG-INFO
 src/threadsnake.egg-info/SOURCES.txt
 src/threadsnake.egg-info/dependency_links.txt
 src/threadsnake.egg-info/top_level.txt
 src/threadsnake/html/__init__.py
 src/threadsnake/html/tools.py
```

