# Comparing `tmp/xia_token_flask-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_token_flask-0.1.8-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 163096 bytes, number of entries: 7
--rw-r--r--  2.0 unx      102 b- defN 23-Apr-06 21:03 xia_token_flask/__init__.py
--rw-r--r--  2.0 unx   431616 b- defN 23-Apr-07 06:08 xia_token_flask/token.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-07 06:08 xia_token_flask-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      700 b- defN 23-Apr-07 06:08 xia_token_flask-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-07 06:08 xia_token_flask-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-07 06:08 xia_token_flask-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      610 b- defN 23-Apr-07 06:08 xia_token_flask-0.1.7.dist-info/RECORD
-7 files, 433295 bytes uncompressed, 162002 bytes compressed:  62.6%
+Zip file size: 130105 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      102 b- defN 23-Apr-07 16:08 xia_token_flask/__init__.py
+-rw-r--r--  2.0 unx   357408 b- defN 23-Apr-07 16:09 xia_token_flask/token.cpython-310-darwin.so
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-07 16:09 xia_token_flask-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      663 b- defN 23-Apr-07 16:09 xia_token_flask-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Apr-07 16:09 xia_token_flask-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-07 16:09 xia_token_flask-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      614 b- defN 23-Apr-07 16:09 xia_token_flask-0.1.8.dist-info/RECORD
+7 files, 359063 bytes uncompressed, 129005 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_token_flask/__init__.py
 Comment: 
 
-Filename: xia_token_flask/token.cp39-win_amd64.pyd
+Filename: xia_token_flask/token.cpython-310-darwin.so
 Comment: 
 
-Filename: xia_token_flask-0.1.7.dist-info/LICENSE.txt
+Filename: xia_token_flask-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.7.dist-info/METADATA
+Filename: xia_token_flask-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_token_flask-0.1.7.dist-info/WHEEL
+Filename: xia_token_flask-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_token_flask-0.1.7.dist-info/top_level.txt
+Filename: xia_token_flask-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.7.dist-info/RECORD
+Filename: xia_token_flask-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_token_flask/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_token_flask.token import FlaskToken
 
 
 __all__ = [
     "FlaskToken",
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_token_flask-0.1.7.dist-info/METADATA` & `xia_token_flask-0.1.8.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xia-token-flask
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Flask
 Requires-Dist: PyJWT
 Requires-Dist: xia-engine
 
@@ -28,9 +26,7 @@
 =============================
 
 Install the package::
 
     pip install
 
 
-
-
```

