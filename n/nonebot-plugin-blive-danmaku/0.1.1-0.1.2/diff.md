# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.1.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.1.tar` & `nonebot_plugin_blive_danmaku-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.1/LICENSE
--rw-r--r--   0        0        0     4464 2023-04-07 08:34:17.540830 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     1859 2023-04-07 09:21:28.528039 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     2645 2023-04-07 06:33:15.900439 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/pusher.py
--rw-r--r--   0        0        0     3383 2023-04-07 06:15:28.649880 nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      950 2023-04-07 16:47:46.689814 nonebot_plugin_blive_danmaku-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1164 2023-04-07 14:28:30.651921 nonebot_plugin_blive_danmaku-0.1.1/README.md
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.2/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       67 2023-04-07 19:00:18.585303 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0     2837 2023-04-07 19:41:42.478829 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/pusher.py
+-rw-r--r--   0        0        0     1407 2023-04-07 18:48:25.619184 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_add.py
+-rw-r--r--   0        0        0     1396 2023-04-07 18:49:55.897456 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_delete.py
+-rw-r--r--   0        0        0      916 2023-04-07 18:53:16.447915 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_list.py
+-rw-r--r--   0        0        0      829 2023-04-07 18:52:14.308552 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_off.py
+-rw-r--r--   0        0        0      820 2023-04-07 18:50:57.288389 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/sub_on.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     1953 2023-04-07 19:33:48.683619 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1330 2023-04-07 05:20:29.198527 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3289 2023-04-07 19:01:53.281128 nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-07 19:51:23.975973 nonebot_plugin_blive_danmaku-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    59274 2023-04-07 19:51:27.937112 nonebot_plugin_blive_danmaku-0.1.2/README.md
+-rw-r--r--   0        0        0    60383 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from nonebot import get_driver
 from tortoise import Tortoise
 from tortoise.connection import connections
 
 from ..utils import get_path
 from .model import Sub
+from nonebot.log import logger
 
-sub_list = []
+sub_dict = {"list":[]}
 
 class Db:
     @classmethod
     async def init(cls):
         config={
             "connections":{"danmaku_bot":f"sqlite://{get_path('danmakuBot.sqlite3')}"},
             "apps":{
@@ -30,14 +31,15 @@
         await cls.update_sub_list()
         return True
     
     @classmethod
     async def delete_sub(cls, **kwargs) -> bool:
         if not await Sub.delete(**kwargs):
             return False
+        await cls.update_sub_list()
         return True
     
     @classmethod
     async def update_sub(cls, conf, switch, **kwargs):
         res = await Sub.update(kwargs, **{conf: switch})
         if res:
             await cls.update_sub_list()
@@ -51,17 +53,17 @@
     @classmethod
     async def get_sub(cls, **kwargs):
         res = await Sub.get(**kwargs).first()
         return res
 
     @classmethod
     def get_sub_list(cls):
-        return sub_list
+        return sub_dict["list"]
 
     @classmethod
     async def update_sub_list(cls):
         subs = Sub.all()
-        sub_list = list(set([sub.uid async for sub in subs if sub.street_lamp]))
+        sub_dict["list"] = list(set([sub.uid async for sub in subs if sub.street_lamp]))
 
 
 get_driver().on_startup(Db.init)
 get_driver().on_shutdown(connections.close_all)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/pusher.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/command/pusher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import time
 import asyncio
 from bilireq.live import get_rooms_info_by_uids
-from .utils import send_msg, scheduler
-from .blivedm import blivedm
-from .database import Db as db
+from ..utils import send_msg
+from ..blivedm import blivedm
+from ..database import Db as db
 from nonebot.log import logger
+from nonebot import require
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
+
 
 class ClientModel:
-    def __init__(self, uid, name, room_id):
-        self.uid=uid
-        self.name=name
+    def __init__(self, room_id):
+        self.uid=""
+        self.name=""
         self.client=blivedm.BLiveClient(room_id)
 
 
 clients = []
 
 
 @scheduler.scheduled_job(
@@ -34,17 +38,19 @@
     for uid, info in res.items():
         new_status = 0 if info["live_status"] == 2 else info["live_status"]
         index = [x for x in clients if x.uid == uid]
         if not index:
             if new_status:
                 logger.info(f'{info["uname"]}开播了，连接直播间')
                 room_id = info["short_id"] if info["short_id"] else info["room_id"]
-                model = ClientModel(uid, info["uname"], room_id)
+                model = ClientModel(room_id)
                 model.client.add_handler(handler)
                 model.client.start()
+                model.uid=uid
+                model.name=info["uname"]
                 clients.append(model)
         else:
             if new_status == 0:
                 model = index[0]
                 client = model.client
                 try:
                     asyncio.gather(client.join())
@@ -57,13 +63,14 @@
 class MsgHandler(blivedm.BaseHandler):
     async def _on_danmaku(self, client: blivedm.BLiveClient, message: blivedm.DanmakuMessage):
         if(message.msg.startswith("#路灯")):
             subs = await db.get_subs(uid=client.room_owner_uid)
             if not subs:
                 return
             for sub in subs:
-                index = [x for x in clients if x.uid == sub.uid]
+                index = [x for x in clients if x.uid == str(sub.uid)]
+                logger.info(index)
                 model = index[0]
                 logger.info(f'{model.name}的直播间收到路灯：{message.uname} -> {message.msg}')
                 datetime = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
                 msg = f'【{model.name}】 在 {datetime} 收到了 {message.uname} 发来的路灯【{message.msg.replace("#路灯","", 1).strip()}】'
                 await send_msg(bot_id=sub.bot_id,send_type=sub.type,type_id=sub.type_id,message=msg)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.2/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,11 +88,7 @@
     return event.group_id if isinstance(event, GroupMessageEvent) else event.user_id
 
 
 def on_startup():
     if not Path(get_path()).is_dir():
             Path(get_path()).mkdir(parents=True)
 
-
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler 
-
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.1/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.1"
+version = "0.1.2"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

