# Comparing `tmp/ossapi-3.1.7.tar.gz` & `tmp/ossapi-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.1.7.tar", last modified: Thu Apr  6 23:44:28 2023, max compression
+gzip compressed data, was "ossapi-3.1.8.tar", last modified: Fri Apr  7 18:52:38 2023, max compression
```

## Comparing `ossapi-3.1.7.tar` & `ossapi-3.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-06 23:44:28.183958 ossapi-3.1.7/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.1.7/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-06 23:44:28.183682 ossapi-3.1.7/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-03-28 20:31:37.000000 ossapi-3.1.7/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-06 23:44:28.181352 ossapi-3.1.7/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3864 2023-03-09 02:19:38.000000 ossapi-3.1.7/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-03-31 23:04:14.000000 ossapi-3.1.7/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-06 05:02:02.000000 ossapi-3.1.7/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-01-31 22:30:17.000000 ossapi-3.1.7/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-03-09 05:37:37.000000 ossapi-3.1.7/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-02-01 05:09:38.000000 ossapi-3.1.7/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    84208 2023-04-06 23:44:22.000000 ossapi-3.1.7/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    89202 2023-04-06 23:44:22.000000 ossapi-3.1.7/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-03-08 17:51:25.000000 ossapi-3.1.7/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-01-30 00:39:41.000000 ossapi-3.1.7/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-06 23:44:28.182193 ossapi-3.1.7/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-06 23:44:28.000000 ossapi-3.1.7/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-04-06 23:44:28.000000 ossapi-3.1.7/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-04-06 23:44:28.000000 ossapi-3.1.7/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-04-06 23:44:28.000000 ossapi-3.1.7/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-04-06 23:44:28.000000 ossapi-3.1.7/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-04-06 23:41:32.000000 ossapi-3.1.7/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-04-06 23:44:28.184010 ossapi-3.1.7/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-06 23:44:28.183392 ossapi-3.1.7/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3082 2023-04-06 23:44:22.000000 ossapi-3.1.7/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.1.7/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)     9694 2023-03-09 05:36:41.000000 ossapi-3.1.7/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-06 23:44:22.000000 ossapi-3.1.7/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.1.7/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.609646 ossapi-3.1.8/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.1.8/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-07 18:52:38.609433 ossapi-3.1.8/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-03-28 20:31:37.000000 ossapi-3.1.8/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.607068 ossapi-3.1.8/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3864 2023-03-09 02:19:38.000000 ossapi-3.1.8/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-03-31 23:04:14.000000 ossapi-3.1.8/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-06 05:02:02.000000 ossapi-3.1.8/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-01-31 22:30:17.000000 ossapi-3.1.8/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-03-09 05:37:37.000000 ossapi-3.1.8/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-02-01 05:09:38.000000 ossapi-3.1.8/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    84208 2023-04-07 18:52:33.000000 ossapi-3.1.8/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    89252 2023-04-07 18:52:33.000000 ossapi-3.1.8/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-03-08 17:51:25.000000 ossapi-3.1.8/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-01-30 00:39:41.000000 ossapi-3.1.8/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.607949 ossapi-3.1.8/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-04-07 18:52:11.000000 ossapi-3.1.8/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-04-07 18:52:38.609695 ossapi-3.1.8/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.609130 ossapi-3.1.8/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3082 2023-04-07 18:52:33.000000 ossapi-3.1.8/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.1.8/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)     9694 2023-03-09 05:36:41.000000 ossapi-3.1.8/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-07 18:52:33.000000 ossapi-3.1.8/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.1.8/tests/test_v1.py
```

### Comparing `ossapi-3.1.7/LICENSE` & `ossapi-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/PKG-INFO` & `ossapi-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.7
+Version: 3.1.8
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.7/README.md` & `ossapi-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/__init__.py` & `ossapi-3.1.8/ossapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/encoder.py` & `ossapi-3.1.8/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/enums.py` & `ossapi-3.1.8/ossapi/enums.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/mod.py` & `ossapi-3.1.8/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/models.py` & `ossapi-3.1.8/ossapi/models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/ossapi.py` & `ossapi-3.1.8/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/ossapiv2.py` & `ossapi-3.1.8/ossapi/ossapiv2.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/ossapiv2_async.py` & `ossapi-3.1.8/ossapi/ossapiv2_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,15 +1071,16 @@
 
         Notes
         -----
         Implements the `Get Beatmaps
         <https://osu.ppy.sh/docs/index.html#get-beatmaps>`__ endpoint.
         """
         params = {"ids": beatmap_ids}
-        return await self._get(Beatmaps, "/beatmaps", params).beatmaps
+        beatmaps = await self._get(Beatmaps, "/beatmaps", params)
+        return beatmaps.beatmaps
 
     @request(Scope.PUBLIC, category="beatmaps")
     async def beatmap_attributes(self,
         beatmap_id: int,
         *,
         mods: Optional[ModT] = None,
         ruleset: Optional[GameModeT] = None,
@@ -2421,15 +2422,16 @@
 
         Notes
         -----
         Implements the `Get Users
         <https://osu.ppy.sh/docs/index.html#get-users>`__ endpoint.
         """
         params = {"ids": user_ids}
-        return await self._get(Users, "/users", params).users
+        users = await self._get(Users, "/users", params)
+        return users.users
 
     # /wiki
     # -----
 
     @request(scope=None, category="wiki")
     async def wiki_page(self,
         locale: str,
```

### Comparing `ossapi-3.1.7/ossapi/replay.py` & `ossapi-3.1.8/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi/utils.py` & `ossapi-3.1.8/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/ossapi.egg-info/PKG-INFO` & `ossapi-3.1.8/ossapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.7
+Version: 3.1.8
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.7/pyproject.toml` & `ossapi-3.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.1.7"
+version = "3.1.8"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.1.7/tests/__init__.py` & `ossapi-3.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/tests/test_cursor.py` & `ossapi-3.1.8/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/tests/test_endpoints.py` & `ossapi-3.1.8/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/tests/test_models.py` & `ossapi-3.1.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.7/tests/test_v1.py` & `ossapi-3.1.8/tests/test_v1.py`

 * *Files identical despite different names*

