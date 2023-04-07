# Comparing `tmp/fugle-realtime-0.4.1.tar.gz` & `tmp/fugle-realtime-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugle-realtime-0.4.1.tar", max compression
+gzip compressed data, was "fugle-realtime-0.4.2.tar", max compression
```

## Comparing `fugle-realtime-0.4.1.tar` & `fugle-realtime-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1096 2021-10-07 03:13:52.928725 fugle-realtime-0.4.1/LICENSE
--rw-r--r--   0        0        0     1943 2022-12-16 08:40:26.917891 fugle-realtime-0.4.1/README.md
--rw-r--r--   0        0        0      105 2022-12-26 02:27:18.964218 fugle-realtime-0.4.1/fugle_realtime/__init__.py
--rw-r--r--   0        0        0      362 2021-10-07 03:13:52.929111 fugle-realtime-0.4.1/fugle_realtime/base_client.py
--rw-r--r--   0        0        0       35 2021-10-07 03:13:52.929256 fugle-realtime-0.4.1/fugle_realtime/http_client/__init__.py
--rw-r--r--   0        0        0      945 2022-12-08 09:43:37.886064 fugle-realtime-0.4.1/fugle_realtime/http_client/historical.py
--rw-r--r--   0        0        0      481 2022-12-08 09:43:37.887636 fugle-realtime-0.4.1/fugle_realtime/http_client/http_client.py
--rw-r--r--   0        0        0     1094 2022-12-08 09:43:37.888139 fugle-realtime-0.4.1/fugle_realtime/http_client/intraday.py
--rw-r--r--   0        0        0       46 2021-10-07 03:13:52.929597 fugle-realtime-0.4.1/fugle_realtime/websocket_client/__init__.py
--rw-r--r--   0        0        0     1234 2022-11-21 02:35:26.003475 fugle-realtime-0.4.1/fugle_realtime/websocket_client/intraday.py
--rw-r--r--   0        0        0      374 2021-10-07 03:13:52.929791 fugle-realtime-0.4.1/fugle_realtime/websocket_client/websocket_client.py
--rw-r--r--   0        0        0     1359 2021-10-07 03:13:52.929887 fugle-realtime-0.4.1/fugle_realtime/websocket_client/ws.py
--rw-r--r--   0        0        0      719 2022-12-26 02:17:57.903697 fugle-realtime-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2853 2022-12-26 02:31:14.572654 fugle-realtime-0.4.1/setup.py
--rw-r--r--   0        0        0     2775 2022-12-26 02:31:14.572931 fugle-realtime-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2021-10-07 03:13:52.928725 fugle-realtime-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1943 2023-04-07 20:31:10.715430 fugle-realtime-0.4.2/README.md
+-rw-r--r--   0        0        0      105 2023-04-07 20:50:31.717807 fugle-realtime-0.4.2/fugle_realtime/__init__.py
+-rw-r--r--   0        0        0      362 2021-10-07 03:13:52.929111 fugle-realtime-0.4.2/fugle_realtime/base_client.py
+-rw-r--r--   0        0        0       35 2021-10-07 03:13:52.929256 fugle-realtime-0.4.2/fugle_realtime/http_client/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-07 20:47:25.891858 fugle-realtime-0.4.2/fugle_realtime/http_client/historical.py
+-rw-r--r--   0        0        0      481 2023-04-07 20:31:10.716957 fugle-realtime-0.4.2/fugle_realtime/http_client/http_client.py
+-rw-r--r--   0        0        0     1031 2023-04-07 20:47:25.892246 fugle-realtime-0.4.2/fugle_realtime/http_client/intraday.py
+-rw-r--r--   0        0        0       46 2021-10-07 03:13:52.929597 fugle-realtime-0.4.2/fugle_realtime/websocket_client/__init__.py
+-rw-r--r--   0        0        0     1234 2022-11-21 02:35:26.003475 fugle-realtime-0.4.2/fugle_realtime/websocket_client/intraday.py
+-rw-r--r--   0        0        0      374 2021-10-07 03:13:52.929791 fugle-realtime-0.4.2/fugle_realtime/websocket_client/websocket_client.py
+-rw-r--r--   0        0        0     1359 2021-10-07 03:13:52.929887 fugle-realtime-0.4.2/fugle_realtime/websocket_client/ws.py
+-rw-r--r--   0        0        0      719 2023-04-07 20:51:27.792063 fugle-realtime-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2853 2023-04-07 21:00:34.341395 fugle-realtime-0.4.2/setup.py
+-rw-r--r--   0        0        0     2775 2023-04-07 21:00:34.341661 fugle-realtime-0.4.2/PKG-INFO
```

### Comparing `fugle-realtime-0.4.1/LICENSE` & `fugle-realtime-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fugle-realtime-0.4.1/README.md` & `fugle-realtime-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fugle-realtime-0.4.1/fugle_realtime/http_client/historical.py` & `fugle-realtime-0.4.2/fugle_realtime/http_client/historical.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from urllib.parse import urlencode, urljoin
+from urllib.parse import urlencode
 import os
 import requests
 
 
 class Historical:
     def __init__(self, config):
         self.config = config
@@ -14,14 +14,12 @@
         if start is not None: params['from'] = start
         if end is not None: params['to'] = end
         if fields is not None: params['fields'] = fields
 
         return requests.get(self.compile_url('/candles', params)).json()
 
     def compile_url(self, path, params):
-        source = 'marketdata'
         params['apiToken'] = self.config['api_token']
-        base_url = urljoin(self.config['url'], os.path.join(
-            source, self.config['api_version']))
+        base_url = self.config['url'] + '/marketdata/' + self.config['api_version']
         endpoint = path if (path.startswith('/')) else '/' + path
         query = '?' + urlencode(params)
         return base_url + endpoint + query
```

### Comparing `fugle-realtime-0.4.1/fugle_realtime/http_client/intraday.py` & `fugle-realtime-0.4.2/fugle_realtime/http_client/intraday.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from urllib.parse import urlencode, urljoin
+from urllib.parse import urlencode
 import os
 import requests
 
 
 class Intraday:
     def __init__(self, config):
         self.config = config
@@ -19,14 +19,12 @@
     def dealts(self, **params):
         return requests.get(self.compile_url('/intraday/dealts', params)).json()
 
     def volumes(self, **params):
         return requests.get(self.compile_url('/intraday/volumes', params)).json()
 
     def compile_url(self, path, params):
-        source = 'realtime'
         params['apiToken'] = self.config['api_token']
-        baseUrl = urljoin(self.config['url'], os.path.join(
-            source, self.config['api_version']))
+        base_url = self.config['url'] + '/realtime/' + self.config['api_version']
         endpoint = path if (path.startswith('/')) else '/' + path
         query = '?' + urlencode(params)
-        return baseUrl + endpoint + query
+        return base_url + endpoint + query
```

### Comparing `fugle-realtime-0.4.1/fugle_realtime/websocket_client/intraday.py` & `fugle-realtime-0.4.2/fugle_realtime/websocket_client/intraday.py`

 * *Files identical despite different names*

### Comparing `fugle-realtime-0.4.1/fugle_realtime/websocket_client/ws.py` & `fugle-realtime-0.4.2/fugle_realtime/websocket_client/ws.py`

 * *Files identical despite different names*

### Comparing `fugle-realtime-0.4.1/pyproject.toml` & `fugle-realtime-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fugle-realtime"
-version = "0.4.1"
+version = "0.4.2"
 description = "Fugle Realtime API client library for Python"
 authors = ["Fortuna Intelligence Co., Ltd. <development@fugle.tw>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fugle-dev/fugle-realtime-py#readme"
 repository = "https://github.com/fugle-dev/fugle-realtime-py"
 documentation = "https://developer.fugle.tw"
```

### Comparing `fugle-realtime-0.4.1/setup.py` & `fugle-realtime-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.26.0,<3.0.0', 'websocket-client>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'fugle-realtime',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Fugle Realtime API client library for Python',
     'long_description': "# Fugle Realtime\n\n[![PyPI version][pypi-image]][pypi-url]\n[![Python version][python-image]][python-url]\n[![Build Status][action-image]][action-url]\n\n> Fugle Realtime API client library for Python\n\n## Install\n\n```sh\n$ pip install fugle-realtime\n```\n\n## Usage\n\nThe library a Python client that supports HTTP API and WebSocket.\n\n### HTTP API\n\n```py\nfrom fugle_realtime import HttpClient\n\napi_client = HttpClient(api_token='demo')\n```\n\n#### intraday.meta\n\n```py\napi_client.intraday.meta(symbolId='2884')\n```\n\n#### intraday.quote\n\n```py\napi_client.intraday.quote(symbolId='2884')\n```\n\n#### intraday.chart\n\n```py\napi_client.intraday.chart(symbolId='2884')\n```\n\n#### intraday.dealts\n\n```py\napi_client.intraday.dealts(symbolId='2884', limit=50)\n```\n\n#### intraday.volumes\n\n```py\napi_client.intraday.volumes(symbolId='2884')\n```\n\n#### historical.candles\n\n```py\napi_client.historical.candles('2884', '2022-02-07', '2022-02-11', None)\napi_client.historical.candles('2884', None, None, 'open,high,low,close,volume,turnover,change')\n```\n\n### Simple WebSocket Demo\n\n```py\nimport time\nfrom fugle_realtime import WebSocketClient\n\ndef handle_message(message):\n    print(message)\n\ndef main():\n    ws_client = WebSocketClient(api_token='demo')\n    ws = ws_client.intraday.quote(symbolId='2884', on_message=handle_message)\n    ws.run_async()\n    time.sleep(3)\n    ws.close()\n\nif __name__ == '__main__':\n    main()\n```\n\n## Reference\n\n[Fugle Realtime API](https://developer.fugle.tw)\n\n## License\n\n[MIT](LICENSE)\n\n[pypi-image]: https://img.shields.io/pypi/v/fugle-realtime\n[pypi-url]: https://pypi.org/project/fugle-realtime\n[python-image]: https://img.shields.io/pypi/pyversions/fugle-realtime\n[python-url]: https://pypi.org/project/fugle-realtime\n[action-image]: https://img.shields.io/github/actions/workflow/status/fugle-dev/fugle-realtime-python/pytest.yml?branch=master\n[action-url]: https://github.com/fugle-dev/fugle-realtime-py/actions/workflows/pytest.yml\n",
     'author': 'Fortuna Intelligence Co., Ltd.',
     'author_email': 'development@fugle.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fugle-dev/fugle-realtime-py#readme',
```

### Comparing `fugle-realtime-0.4.1/PKG-INFO` & `fugle-realtime-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugle-realtime
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fugle Realtime API client library for Python
 Home-page: https://github.com/fugle-dev/fugle-realtime-py#readme
 License: MIT
 Keywords: fugle,realtime,stock
 Author: Fortuna Intelligence Co., Ltd.
 Author-email: development@fugle.tw
 Requires-Python: >=3.7,<4.0
```

