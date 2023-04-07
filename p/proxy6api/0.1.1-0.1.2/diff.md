# Comparing `tmp/proxy6api-0.1.1.tar.gz` & `tmp/proxy6api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy6api-0.1.1.tar", max compression
+gzip compressed data, was "proxy6api-0.1.2.tar", max compression
```

## Comparing `proxy6api-0.1.1.tar` & `proxy6api-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-0.1.1/LICENSE
--rw-r--r--   0        0        0       71 2023-03-31 20:13:38.586324 proxy6api-0.1.1/README.md
--rw-r--r--   0        0        0      132 2023-04-07 16:14:29.038118 proxy6api-0.1.1/proxy6api/__init__.py
--rw-r--r--   0        0        0     9548 2023-04-07 16:02:07.433705 proxy6api-0.1.1/proxy6api/client.py
--rw-r--r--   0        0        0        0 2023-04-07 15:43:29.731085 proxy6api-0.1.1/proxy6api/settings/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-0.1.1/proxy6api/settings/bases.py
--rw-r--r--   0        0        0     2269 2023-04-03 17:09:54.155879 proxy6api-0.1.1/proxy6api/settings/errors.py
--rw-r--r--   0        0        0      457 2023-04-07 16:14:52.154425 proxy6api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 proxy6api-0.1.1/setup.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 proxy6api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-0.1.2/LICENSE
+-rw-r--r--   0        0        0       71 2023-03-31 20:13:38.586324 proxy6api-0.1.2/README.md
+-rw-r--r--   0        0        0      337 2023-04-07 17:04:48.246253 proxy6api-0.1.2/proxy6api/__init__.py
+-rw-r--r--   0        0        0     8516 2023-04-07 17:00:12.854973 proxy6api-0.1.2/proxy6api/client.py
+-rw-r--r--   0        0        0      185 2023-04-07 17:03:32.320244 proxy6api-0.1.2/proxy6api/settings/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-0.1.2/proxy6api/settings/bases.py
+-rw-r--r--   0        0        0     2269 2023-04-03 17:09:54.155879 proxy6api-0.1.2/proxy6api/settings/errors.py
+-rw-r--r--   0        0        0      457 2023-04-07 16:54:45.074343 proxy6api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 proxy6api-0.1.2/setup.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 proxy6api-0.1.2/PKG-INFO
```

### Comparing `proxy6api-0.1.1/LICENSE` & `proxy6api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.1/proxy6api/client.py` & `proxy6api-0.1.2/proxy6api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,14 @@
     api_key: api_key
     """
 
     url: str = "https://proxy6.net/api"
     api_key: str = None
 
 
-"""
-Traceback (most recent call last):
-  File "/home/konstantin/Dev/Proxy6API/proxy6/client.py", line 214, in <module>
-    print(client.get_proxy())
-  File "/home/konstantin/Dev/Proxy6API/proxy6/client.py", line 111, in get_proxy
-    return self.request(method="getproxy", state=state, descr=descr, nokey=nokey, page=page, limit=limit)
-  File "/home/konstantin/Dev/Proxy6API/proxy6/client.py", line 48, in request
-    response_json = requests.get(url=url).json()
-  File "/usr/lib/python3/dist-packages/requests/models.py", line 900, in json
-    return complexjson.loads(self.text, **kwargs)
-  File "/usr/lib/python3.10/json/__init__.py", line 346, in loads
-    return _default_decoder.decode(s)
-  File "/usr/lib/python3.10/json/decoder.py", line 337, in decode
-    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python3.10/json/decoder.py", line 355, in raw_decode
-    raise JSONDecodeError("Expecting value", s, err.value) from None
-json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)
-"""
-
-
 class Proxy_6_Client:
     def __init__(self, api_url: Proxy_6_API_URL) -> None:
         self.url = api_url.url
         self.api_key = api_url.api_key
 
     @staticmethod
     def _query_params_of_method(**query_params) -> str:
```

### Comparing `proxy6api-0.1.1/proxy6api/settings/bases.py` & `proxy6api-0.1.2/proxy6api/settings/bases.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.1/proxy6api/settings/errors.py` & `proxy6api-0.1.2/proxy6api/settings/errors.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.1/setup.py` & `proxy6api-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'proxy6api',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'This is unofficial software for using api with proxy 6.net',
     'long_description': '# Proxy6API\nThis is unofficial software for using api with proxy 6.net\n',
     'author': 'Konstantin Raikhert',
     'author_email': 'raikhert13@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `proxy6api-0.1.1/PKG-INFO` & `proxy6api-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy6api
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is unofficial software for using api with proxy 6.net
 License: MIT
 Author: Konstantin Raikhert
 Author-email: raikhert13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

