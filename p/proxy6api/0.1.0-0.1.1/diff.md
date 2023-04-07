# Comparing `tmp/proxy6api-0.1.0.tar.gz` & `tmp/proxy6api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxy6api-0.1.0.tar", max compression
+gzip compressed data, was "proxy6api-0.1.1.tar", max compression
```

## Comparing `proxy6api-0.1.0.tar` & `proxy6api-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-0.1.0/LICENSE
--rw-r--r--   0        0        0       71 2023-03-31 20:13:38.586324 proxy6api-0.1.0/README.md
--rw-r--r--   0        0        0      319 2023-04-07 16:03:25.967425 proxy6api-0.1.0/proxy6api/__init__.py
--rw-r--r--   0        0        0     9548 2023-04-07 16:02:07.433705 proxy6api-0.1.0/proxy6api/client.py
--rw-r--r--   0        0        0        0 2023-04-07 15:43:29.731085 proxy6api-0.1.0/proxy6api/settings/__init__.py
--rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-0.1.0/proxy6api/settings/bases.py
--rw-r--r--   0        0        0     2269 2023-04-03 17:09:54.155879 proxy6api-0.1.0/proxy6api/settings/errors.py
--rw-r--r--   0        0        0      457 2023-04-07 16:04:25.122129 proxy6api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 proxy6api-0.1.0/setup.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 proxy6api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-03-31 20:13:38.586324 proxy6api-0.1.1/LICENSE
+-rw-r--r--   0        0        0       71 2023-03-31 20:13:38.586324 proxy6api-0.1.1/README.md
+-rw-r--r--   0        0        0      132 2023-04-07 16:14:29.038118 proxy6api-0.1.1/proxy6api/__init__.py
+-rw-r--r--   0        0        0     9548 2023-04-07 16:02:07.433705 proxy6api-0.1.1/proxy6api/client.py
+-rw-r--r--   0        0        0        0 2023-04-07 15:43:29.731085 proxy6api-0.1.1/proxy6api/settings/__init__.py
+-rw-r--r--   0        0        0     3885 2023-04-03 17:00:42.211299 proxy6api-0.1.1/proxy6api/settings/bases.py
+-rw-r--r--   0        0        0     2269 2023-04-03 17:09:54.155879 proxy6api-0.1.1/proxy6api/settings/errors.py
+-rw-r--r--   0        0        0      457 2023-04-07 16:14:52.154425 proxy6api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 proxy6api-0.1.1/setup.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 proxy6api-0.1.1/PKG-INFO
```

### Comparing `proxy6api-0.1.0/LICENSE` & `proxy6api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.0/proxy6api/client.py` & `proxy6api-0.1.1/proxy6api/client.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.0/proxy6api/settings/bases.py` & `proxy6api-0.1.1/proxy6api/settings/bases.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.0/proxy6api/settings/errors.py` & `proxy6api-0.1.1/proxy6api/settings/errors.py`

 * *Files identical despite different names*

### Comparing `proxy6api-0.1.0/setup.py` & `proxy6api-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'proxy6api',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'This is unofficial software for using api with proxy 6.net',
     'long_description': '# Proxy6API\nThis is unofficial software for using api with proxy 6.net\n',
     'author': 'Konstantin Raikhert',
     'author_email': 'raikhert13@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `proxy6api-0.1.0/PKG-INFO` & `proxy6api-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxy6api
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is unofficial software for using api with proxy 6.net
 License: MIT
 Author: Konstantin Raikhert
 Author-email: raikhert13@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

