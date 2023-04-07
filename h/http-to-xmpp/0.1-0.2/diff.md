# Comparing `tmp/http-to-xmpp-0.1.tar.gz` & `tmp/http-to-xmpp-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http-to-xmpp-0.1.tar", last modified: Wed Apr  5 21:18:18 2023, max compression
+gzip compressed data, was "http-to-xmpp-0.2.tar", last modified: Fri Apr  7 20:26:08 2023, max compression
```

## Comparing `http-to-xmpp-0.1.tar` & `http-to-xmpp-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-04-05 21:18:18.713419 http-to-xmpp-0.1/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1297 2023-04-05 21:18:18.713419 http-to-xmpp-0.1/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      999 2023-04-05 21:08:25.000000 http-to-xmpp-0.1/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-04-05 21:18:18.713419 http-to-xmpp-0.1/http_to_xmpp.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1297 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      258 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       51 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/entry_points.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       16 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       13 2023-04-05 21:18:18.000000 http-to-xmpp-0.1/http_to_xmpp.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3317 2023-04-05 21:16:25.000000 http-to-xmpp-0.1/http_to_xmpp.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)      694 2023-04-05 21:08:06.000000 http-to-xmpp-0.1/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-04-05 21:18:18.713419 http-to-xmpp-0.1/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-04-07 20:26:08.714040 http-to-xmpp-0.2/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1256 2023-04-07 20:26:08.714040 http-to-xmpp-0.2/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      958 2023-04-07 20:24:20.000000 http-to-xmpp-0.2/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-04-07 20:26:08.710040 http-to-xmpp-0.2/http_to_xmpp.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1256 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      258 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       51 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/entry_points.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       16 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       13 2023-04-07 20:26:08.000000 http-to-xmpp-0.2/http_to_xmpp.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3490 2023-04-07 20:25:05.000000 http-to-xmpp-0.2/http_to_xmpp.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      694 2023-04-05 21:08:06.000000 http-to-xmpp-0.2/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-04-07 20:26:08.714040 http-to-xmpp-0.2/setup.cfg
```

### Comparing `http-to-xmpp-0.1/README.md` & `http-to-xmpp-0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 ```bash
 $ export XMPP_DEST_JID=the_human_receiving_messages@the_server.org
 $ export XMPP_JID=the_bot_account@the_server.org
 $ export XMPP_PASSWORD=the_bot_password
 $ http-to-xmpp
 ```
 
-or via arguments, but beware of `ps` showing your password!
+or via arguments:
 
 ```bash
-$ http-to-xmpp --xmpp-jid the_bot_account@the_server.org --xmpp-password the_bot_password --xmpp-dest-jid the_human_receiving_messages@the_server.org
+$ http-to-xmpp --xmpp-jid bot_account@the_server.org --xmpp-password "$(pass bot_account@the_server.org)" --xmpp-dest-jid human_account@the_server.org
 ```
 
 HTTP host and port to listen to can be changed using `--http-host` and `--http-port`, they default to `localhost:1985`.
 
 
 ## Usage
```

### Comparing `http-to-xmpp-0.1/http_to_xmpp.py` & `http-to-xmpp-0.2/http_to_xmpp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """HTTP to XMPP gateway."""
 
 import argparse
 import asyncio
 import os
 import signal
 import socket
+import json
 import sys
 
 import aioxmpp
 import aioxmpp.dispatcher
 from aiohttp import web
 
-__version__ = "0.1"
+__version__ = "0.2"
 
 
 class XMPPClient:
     def __init__(self, jid, password):
         self.jid = jid
         self.password = password
 
@@ -51,15 +52,19 @@
     def forward_to(self, to_jid, xmpp_client):
         self.to_jid = to_jid
         self.xmpp_client = xmpp_client
 
     async def on_post(self, request):
         if not self.xmpp_client:
             return
-        self.xmpp_client.send(await request.text(), self.to_jid)
+        data = await request.text()
+        try:
+            self.xmpp_client.send(json.dumps(json.loads(data), indent=4), self.to_jid)
+        except json.JSONDecodeError:
+            self.xmpp_client.send(data, self.to_jid)
         return web.Response(text="")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("--http-host", default="localhost")
     parser.add_argument("--http-port", default=1985, type=int)
```

### Comparing `http-to-xmpp-0.1/pyproject.toml` & `http-to-xmpp-0.2/pyproject.toml`

 * *Files identical despite different names*

