# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.0.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.0.tar` & `nonebot_plugin_blive_danmaku-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     4464 2023-04-07 08:34:17.540830 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     1859 2023-04-07 09:21:28.528039 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     2645 2023-04-07 06:33:15.900439 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/pusher.py
--rw-r--r--   0        0        0     3383 2023-04-07 06:15:28.649880 nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      976 2023-04-07 15:39:00.337653 nonebot_plugin_blive_danmaku-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1164 2023-04-07 14:28:30.651921 nonebot_plugin_blive_danmaku-0.1.0/README.md
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4464 2023-04-07 08:34:17.540830 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     1859 2023-04-07 09:21:28.528039 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     2645 2023-04-07 06:33:15.900439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/pusher.py
+-rw-r--r--   0        0        0     3383 2023-04-07 06:15:28.649880 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-07 16:47:46.689814 nonebot_plugin_blive_danmaku-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1164 2023-04-07 14:28:30.651921 nonebot_plugin_blive_danmaku-0.1.1/README.md
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/pusher.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/pusher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.0"
+version = "0.1.1"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
-requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 nonebot2 = {extras = ["fastapi"], version = "^2.0.0rc4"}
 nonebot-adapter-onebot = "^2.2.2"
 bilireq = "^0.2.4"
 nonebot_plugin_apscheduler = "^0.2.0"
 tortoise = "^0.1.1"
 tortoise-orm = "^0.19.3"
 aiohttp = "3.7.4"
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/README.md` & `nonebot_plugin_blive_danmaku-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.0/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.1.0
+Version: 0.1.1
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Brotli (==1.0.9)
 Requires-Dist: aiohttp (==3.7.4)
 Requires-Dist: bilireq (>=0.2.4,<0.3.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: tortoise (>=0.1.1,<0.2.0)
```

