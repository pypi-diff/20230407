# Comparing `tmp/nonebot_plugin_genshinuid-4.0.1.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.0.2.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.0.1.tar` & `nonebot_plugin_genshinuid-4.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14037 2023-04-06 16:10:41.216594 nonebot_plugin_genshinuid-4.0.1/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-06 14:38:25.709357 nonebot_plugin_genshinuid-4.0.1/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    22427 2023-04-07 17:32:00.585344 nonebot_plugin_genshinuid-4.0.1/GenshinUID/client.py
--rw-r--r--   0        0        0     1004 2023-04-02 16:27:11.522237 nonebot_plugin_genshinuid-4.0.1/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-04-06 14:38:25.734782 nonebot_plugin_genshinuid-4.0.1/GenshinUID/path.py
--rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.1/LICENSE
--rw-r--r--   0        0        0     1588 2023-04-07 17:45:52.922030 nonebot_plugin_genshinuid-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-03-25 16:39:34.235973 nonebot_plugin_genshinuid-4.0.1/README.md
--rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    14037 2023-04-06 16:10:41.216594 nonebot_plugin_genshinuid-4.0.2/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-06 14:38:25.709357 nonebot_plugin_genshinuid-4.0.2/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    22427 2023-04-07 17:32:00.585344 nonebot_plugin_genshinuid-4.0.2/GenshinUID/client.py
+-rw-r--r--   0        0        0     1004 2023-04-02 16:27:11.522237 nonebot_plugin_genshinuid-4.0.2/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-04-06 14:38:25.734782 nonebot_plugin_genshinuid-4.0.2/GenshinUID/path.py
+-rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.2/LICENSE
+-rw-r--r--   0        0        0     1613 2023-04-07 18:29:47.524391 nonebot_plugin_genshinuid-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-03-25 16:39:34.235973 nonebot_plugin_genshinuid-4.0.2/README.md
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.0.1/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.0.2/GenshinUID/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.0.2/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.0.2/GenshinUID/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.0.2/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/LICENSE` & `nonebot_plugin_genshinuid-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/pyproject.toml` & `nonebot_plugin_genshinuid-4.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.0.1"
+version = "4.0.2"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
@@ -42,14 +42,15 @@
 [tool.poetry.dependencies]
 python = "^3.8.1"
 nonebot2 = ">=2.0.0b4"
 pillow = ">=9.2.0"
 gitpython = ">=3.1.27"
 msgspec = ">=0.13.1"
 aiofiles = ">=23.1.0"
+websockets = ">=11.0.1"
 
 [[tool.poetry.source]]
 name = "USTC"
 url = "https://pypi.mirrors.ustc.edu.cn/simple"
 default = false
 secondary = true
```

### Comparing `nonebot_plugin_genshinuid-4.0.1/README.md` & `nonebot_plugin_genshinuid-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.1/PKG-INFO` & `nonebot_plugin_genshinuid-4.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.0.1
+Version: 4.0.2
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0)
 Requires-Dist: gitpython (>=3.1.27)
 Requires-Dist: msgspec (>=0.13.1)
 Requires-Dist: nonebot2 (>=2.0.0b4)
 Requires-Dist: pillow (>=9.2.0)
+Requires-Dist: websockets (>=11.0.1)
 Project-URL: Bug Tracker, https://github.com/KimigaiiWuyi/GenshinUID/issues
 Project-URL: Documentation, https://docs.gsuid.gbots.work/#/
 Project-URL: Repository, https://github.com/KimigaiiWuyi/GenshinUID
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/KimigaiiWuyi/GenshinUID/"><img src="https://s2.loli.net/2023/03/25/bareSdYcsmRPOyZ.png" width="256" height="256" alt="GenshinUID"></a>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.2 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼çå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0) Requires-Dist: gitpython
 (>=3.1.27) Requires-Dist: msgspec (>=0.13.1) Requires-Dist: nonebot2
-(>=2.0.0b4) Requires-Dist: pillow (>=9.2.0) Project-URL: Bug Tracker, https://
-github.com/KimigaiiWuyi/GenshinUID/issues Project-URL: Documentation, https://
-docs.gsuid.gbots.work/#/ Project-URL: Repository, https://github.com/
-KimigaiiWuyi/GenshinUID Description-Content-Type: text/markdown
+(>=2.0.0b4) Requires-Dist: pillow (>=9.2.0) Requires-Dist: websockets
+(>=11.0.1) Project-URL: Bug Tracker, https://github.com/KimigaiiWuyi/
+GenshinUID/issues Project-URL: Documentation, https://docs.gsuid.gbots.work/#/
+Project-URL: Repository, https://github.com/KimigaiiWuyi/GenshinUID
+Description-Content-Type: text/markdown
                                  [GenshinUID]
                          ****** GenshinUID 4.0 ******
                               *** â¨æ¯æOneBot
  (QQ)ãQQé¢éãå¾®ä¿¡ãå¼é»å¦ãTelegramçå¨åè½åç¥Botæä»¶â¨
                                       ***
              å®è£ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
              [https://s2.loli.net/2023/03/26/76oWuYJwg18aXL2.jpg]
```

