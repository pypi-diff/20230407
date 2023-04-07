# Comparing `tmp/isdn-1.0.1.tar.gz` & `tmp/isdn-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isdn-1.0.1.tar", max compression
+gzip compressed data, was "isdn-1.1.0.tar", max compression
```

## Comparing `isdn-1.0.1.tar` & `isdn-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-04-02 19:25:05.189791 isdn-1.0.1/LICENSE
--rw-r--r--   0        0        0     1429 2023-04-02 19:25:05.189791 isdn-1.0.1/README.md
--rw-r--r--   0        0        0     4315 2023-04-02 19:25:05.189791 isdn-1.0.1/isdn/__init__.py
--rw-r--r--   0        0        0     1777 2023-04-02 19:25:05.189791 isdn-1.0.1/isdn/client.py
--rw-r--r--   0        0        0     3025 2023-04-02 19:25:05.189791 isdn-1.0.1/isdn/command.py
--rw-r--r--   0        0        0     1912 2023-04-02 19:25:05.189791 isdn-1.0.1/isdn/parser.py
--rw-r--r--   0        0        0     1036 2023-04-02 19:25:05.189791 isdn-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2316 1970-01-01 00:00:00.000000 isdn-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-07 19:20:09.800680 isdn-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3236 2023-04-07 19:20:09.800680 isdn-1.1.0/README.md
+-rw-r--r--   0        0        0      192 2023-04-07 19:20:09.800680 isdn-1.1.0/isdn/__init__.py
+-rw-r--r--   0        0        0     1814 2023-04-07 19:20:09.800680 isdn-1.1.0/isdn/client.py
+-rw-r--r--   0        0        0     2980 2023-04-07 19:20:09.800680 isdn-1.1.0/isdn/command.py
+-rw-r--r--   0        0        0     6172 2023-04-07 19:20:09.800680 isdn-1.1.0/isdn/model.py
+-rw-r--r--   0        0        0      535 2023-04-07 19:20:09.800680 isdn-1.1.0/isdn/parser.py
+-rw-r--r--   0        0        0     1091 2023-04-07 19:20:09.804680 isdn-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 isdn-1.1.0/PKG-INFO
```

### Comparing `isdn-1.0.1/LICENSE` & `isdn-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isdn-1.0.1/isdn/client.py` & `isdn-1.1.0/isdn/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterator
 
 import requests
 
-from . import ISDNRecord, __version__
-from .parser import ISDNJpXMLParser
+from . import __version__
+from .model import ISDNRecord, ISDNRoot
+from .parser import ISDNJpSitemapXMLParser
 
 ISDN_XML_ENDPOINT = "https://isdn.jp/xml/{isdn}"
 ISDN_IMAGE_ENDPOINT = "https://isdn.jp/images/thumbs/{isdn}.png"
 ISDN_SITEMAP = "https://isdn.jp/sitemap.xml"
 
 
 class ISDNClient:
@@ -33,15 +34,15 @@
     def _get(self, isdn: str, endpoint_url: str) -> requests.Response:
         r = self.s.get(endpoint_url.format(isdn=self.normalize_isdn(isdn)))
         r.raise_for_status()
         return r
 
     def get(self, isdn: str) -> ISDNRecord:
         r = self._get(isdn, self.xml_endpoint_url)
-        return ISDNJpXMLParser.parse_record(r.content)
+        return ISDNRoot.from_xml_first(r.content)
 
     def get_raw(self, isdn: str) -> bytes:
         r = self._get(isdn, self.xml_endpoint_url)
         return r.content
 
     def get_image(self, isdn: str) -> bytes:
         r = self._get(isdn, self.image_endpoint_url)
@@ -50,8 +51,8 @@
     def _list(self) -> requests.Response:
         r = self.s.get(self.sitemap_url, stream=True)
         r.raise_for_status()
         return r
 
     def list(self) -> Iterator[str]:
         r = self._list()
-        return ISDNJpXMLParser.parse_list(r.raw)
+        return ISDNJpSitemapXMLParser.parse_list(r.raw)
```

### Comparing `isdn-1.0.1/isdn/command.py` & `isdn-1.1.0/isdn/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import json
 import os
 import time
 
 import click
 from requests.exceptions import HTTPError
 
-from . import ISDN, __version__
+from . import __version__
 from .client import ISDNClient
-from .parser import ISDNJpXMLParser
+from .model import ISDN, ISDNRoot
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -25,17 +24,17 @@
 @click.option("--format", "-f", type=click.Choice(["xml", "dict", "json"]), default="xml")
 def get_isdn(isdn: str, format: str):
     c = ISDNClient()
     match format:
         case "xml":
             res = c.get_raw(isdn)
         case "dict":
-            res = c.get(isdn).to_dict()
+            res = c.get(isdn).dict()
         case "json":
-            res = json.dumps(c.get(isdn).to_dict(), ensure_ascii=False)
+            res = c.get(isdn).json(ensure_ascii=False)
         case _:
             raise NotImplementedError
     click.echo(res)
 
 
 @cli.command("list", help="List all ISDNs from isdn.jp")
 def list_isdns():
@@ -68,15 +67,15 @@
 
             try:
                 res = c.get_raw(isdn)
                 with open(path, "wb") as out:
                     out.write(res)
 
                 if write_image:
-                    record = ISDNJpXMLParser.parse_record(res)
+                    record = ISDNRoot.from_xml_first(res)
                     if record.sample_image_uri:
                         img = c.get_image(isdn)
                         with open(image_path, "wb") as out:
                             out.write(img)
             except HTTPError as err:
                 if stop_on_error:
                     raise err
```

