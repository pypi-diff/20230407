# Comparing `tmp/prelude-sdk-0.9.95.tar.gz` & `tmp/prelude-sdk-0.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-0.9.95.tar", last modified: Wed Mar 29 17:29:33 2023, max compression
+gzip compressed data, was "prelude-sdk-0.9.96.tar", last modified: Fri Apr  7 19:49:45 2023, max compression
```

## Comparing `prelude-sdk-0.9.95.tar` & `prelude-sdk-0.9.96.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:29:33.601547 prelude-sdk-0.9.95/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)      915 2023-03-29 17:29:33.601607 prelude-sdk-0.9.95/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      473 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:29:33.598352 prelude-sdk-0.9.95/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:29:33.600646 prelude-sdk-0.9.95/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2850 2023-03-15 22:01:07.000000 prelude-sdk-0.9.95/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5392 2023-03-20 17:31:16.000000 prelude-sdk-0.9.95/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3628 2023-03-28 21:39:17.000000 prelude-sdk-0.9.95/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      466 2023-02-27 16:46:58.000000 prelude-sdk-0.9.95/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:29:33.601243 prelude-sdk-0.9.95/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2785 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2630 2023-03-16 12:58:31.000000 prelude-sdk-0.9.95/prelude_sdk/models/codes.py
--rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-0.9.95/prelude_sdk/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:29:33.599421 prelude-sdk-0.9.95/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      915 2023-03-29 17:29:33.000000 prelude-sdk-0.9.95/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      563 2023-03-29 17:29:33.000000 prelude-sdk-0.9.95/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-03-29 17:29:33.000000 prelude-sdk-0.9.95/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-03-29 17:29:33.000000 prelude-sdk-0.9.95/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-03-29 17:29:33.000000 prelude-sdk-0.9.95/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-0.9.95/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      533 2023-03-29 17:29:33.601836 prelude-sdk-0.9.95/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152553 prelude-sdk-0.9.96/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2023-04-07 19:49:45.152605 prelude-sdk-0.9.96/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      677 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.149111 prelude-sdk-0.9.96/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.150785 prelude-sdk-0.9.96/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3363 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6411 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4178 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      540 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.151216 prelude-sdk-0.9.96/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2628 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/prelude_sdk/models/codes.py
+-rw-r--r--   0 pack       (501) staff       (20)      867 2023-03-09 20:15:21.000000 prelude-sdk-0.9.96/prelude_sdk/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.149912 prelude-sdk-0.9.96/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      750 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-04-07 19:49:45.000000 prelude-sdk-0.9.96/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-0.9.96/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      533 2023-04-07 19:49:45.152815 prelude-sdk-0.9.96/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152342 prelude-sdk-0.9.96/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1058 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:49:45.152476 prelude-sdk-0.9.96/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2658 2023-04-07 19:45:23.000000 prelude-sdk-0.9.96/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4369 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3462 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-0.9.96/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-0.9.95/LICENSE` & `prelude-sdk-0.9.96/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.95/PKG-INFO` & `prelude-sdk-0.9.96/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.95
+Version: 0.9.96
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,7 +29,16 @@
 ```bash
 pip install prelude-sdk
 ```
 
 ## Documentation 
 
 TBD
+
+## Testing
+
+To test the Python SDK and Probes, run the following commands:
+
+```bash
+pip install -r python/sdk/tests/requirements.txt
+pytest tests --api https://api.preludesecurity.com --email <EMAIL>
+```
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-0.9.96/prelude_sdk/controllers/build_controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,63 +9,93 @@
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
     def create_test(self, test_id, name):
         """ Create or update a test """
         with Spinner():
-            data = dict(name=name)
-            res = requests.post(f'{self.account.hq}/build/tests/{test_id}', json=data, headers=self.account.headers)
+            res = requests.post(
+                f'{self.account.hq}/build/tests/{test_id}', 
+                json=dict(name=name),
+                headers=self.account.headers,
+                timeout=10
+            )
             if not res.status_code == 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def delete_test(self, test_id):
         """ Delete an existing test """
         with Spinner():
-            res = requests.delete(f'{self.account.hq}/build/tests/{test_id}', headers=self.account.headers)
+            res = requests.delete(
+                f'{self.account.hq}/build/tests/{test_id}', 
+                headers=self.account.headers,
+                timeout=10
+            )
             if not res.status_code == 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def get_test(self, test_id):
         """ Get properties of an existing test """
         with Spinner():
-            res = requests.get(f'{self.account.hq}/build/tests/{test_id}', headers=self.account.headers)
+            res = requests.get(
+                f'{self.account.hq}/build/tests/{test_id}',
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def download(self, test_id, filename):
         """ Clone a test file or attachment"""
         with Spinner():
-            res = requests.get(f'{self.account.hq}/build/tests/{test_id}/{filename}', headers=self.account.headers)
+            res = requests.get(
+                f'{self.account.hq}/build/tests/{test_id}/{filename}', 
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.content
             raise Exception(res.text)
 
     @verify_credentials
     def upload(self, test_id, filename, data, binary=False):
         """ Upload a test or attachment """
+        h = self.account.headers | ({'Content-Type': 'application/octet-stream'} if binary else {})
         with Spinner():
-            res = requests.post(f'{self.account.hq}/build/tests/{test_id}/{filename}',
-                                data=data,
-                                headers=self.account.headers | ({'Content-Type': 'application/octet-stream'} if binary else {}))
+            res = requests.post(
+                f'{self.account.hq}/build/tests/{test_id}/{filename}',
+                data=data,
+                headers=h,
+                timeout=10
+            )
             if not res.status_code == 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def map(self, test_id: str, x: str):
         """ Add a classification property to a test """
         with Spinner():
-            res = requests.post(f'{self.account.hq}/build/tests/{test_id}/map/{x}', json=dict(id=test_id), headers=self.account.headers)
+            res = requests.post(
+                f'{self.account.hq}/build/tests/{test_id}/map/{x}', 
+                json=dict(id=test_id),
+                headers=self.account.headers,
+                timeout=10
+            )
             if not res.status_code == 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def unmap(self, test_id: str, x: str):
         """ Remove a classification property from a test """
         with Spinner():
-            res = requests.delete(f'{self.account.hq}/build/tests/{test_id}/map/{x}', json=dict(id=test_id), headers=self.account.headers)
+            res = requests.delete(
+                f'{self.account.hq}/build/tests/{test_id}/map/{x}', 
+                json=dict(id=test_id),
+                headers=self.account.headers,
+                timeout=10
+            )
             if not res.status_code == 200:
                 raise Exception(res.text)
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-0.9.96/prelude_sdk/controllers/detect_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,124 +10,180 @@
         self.account = account
 
     @verify_credentials
     def register_endpoint(self, host, serial_num, edr_id, tags):
         """ Register (or re-register) an endpoint to your account """
         with Spinner():
             params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags)
-            res = requests.post(f'{self.account.hq}/detect/endpoint', headers=self.account.headers, json=params)
+            res = requests.post(
+                f'{self.account.hq}/detect/endpoint',
+                headers=self.account.headers,
+                json=params,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.text
             raise Exception(res.text)
 
     @verify_credentials
     def delete_endpoint(self, ident: str):
         """ Delete an endpoint from your account """
         with Spinner():
             params = dict(id=ident)
-            res = requests.delete(f'{self.account.hq}/detect/endpoint', headers=self.account.headers, json=params)
+            res = requests.delete(
+                f'{self.account.hq}/detect/endpoint',
+                headers=self.account.headers,
+                json=params,
+                timeout=10
+            )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def list_endpoints(self, days: int = 90):
         """ List all endpoints on your account """
         with Spinner():
             params = dict(days=days)
-            res = requests.get(f'{self.account.hq}/detect/endpoint', headers=self.account.headers, params=params)
+            res = requests.get(
+                f'{self.account.hq}/detect/endpoint',
+                headers=self.account.headers,
+                params=params,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
-    
+
     @verify_credentials
     def describe_activity(self, filters: dict, view: str = 'logs'):
         """ Get report for an Account """
         with Spinner():
             params = dict(view=view, **filters)
-            res = requests.get(f'{self.account.hq}/detect/activity', headers=self.account.headers, params=params)
+            res = requests.get(
+                f'{self.account.hq}/detect/activity',
+                headers=self.account.headers,
+                params=params,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def list_queue(self):
+        """ List all tests in the queue """
         with Spinner():
-            res = requests.get(f'{self.account.hq}/detect/queue', headers=self.account.headers)
+            res = requests.get(
+                f'{self.account.hq}/detect/queue',
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def list_tests(self):
         """ List all tests available to an account """
         with Spinner():
-            res = requests.get(f'{self.account.hq}/detect/tests', headers=self.account.headers)
+            res = requests.get(
+                f'{self.account.hq}/detect/tests',
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def enable_test(self, ident: str, run_code: int, tags: str):
         """ Enable a test so endpoints will start running it """
         with Spinner():
             res = requests.post(
                 url=f'{self.account.hq}/detect/queue/{ident}',
                 headers=self.account.headers,
-                json=dict(code=run_code, tags=tags)
+                json=dict(code=run_code, tags=tags),
+                timeout=10
             )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def disable_test(self, ident):
         """ Disable a test so endpoints will stop running it """
         with Spinner():
-            res = requests.delete(f'{self.account.hq}/detect/queue/{ident}', headers=self.account.headers)
+            res = requests.delete(
+                f'{self.account.hq}/detect/queue/{ident}',
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def social_stats(self, ident: str, days: int = 30):
         """ Pull social statistics for a specific test """
         with Spinner():
-            params = dict(days=days)
-            res = requests.get(f'{self.account.hq}/detect/{ident}/social', headers=self.account.headers, params=params)
+            res = requests.get(
+                f'{self.account.hq}/detect/{ident}/social',
+                headers=self.account.headers,
+                params=dict(days=days),
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
-         
+
     @verify_credentials
     def search(self, identifier: str):
         """ Search the NVD for a keyword """
         with Spinner():
-            params = dict(identifier=identifier)
-            res = requests.get(f'{self.account.hq}/detect/search', headers=self.account.headers, params=params)
+            res = requests.get(
+                f'{self.account.hq}/detect/search',
+                headers=self.account.headers,
+                params=dict(identifier=identifier),
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def recommendations(self):
         """ List all security recommendations for your account """
         with Spinner():
-            res = requests.get(f'{self.account.hq}/detect/recommendations', headers=self.account.headers)
+            res = requests.get(
+                f'{self.account.hq}/detect/recommendations',
+                headers=self.account.headers,
+                timeout=10
+            )
             if res.status_code == 200:
                 return res.json()
             raise Exception(res.text)
 
     @verify_credentials
     def create_recommendation(self, title: str, description: str):
         """ Create a new security recommendation """
         with Spinner():
             params = dict(title=title, description=description)
-            res = requests.post(f'{self.account.hq}/detect/recommendations', headers=self.account.headers, json=params)
+            res = requests.post(
+                f'{self.account.hq}/detect/recommendations',
+                headers=self.account.headers,
+                json=params,
+                timeout=10
+            )
             if res.status_code != 200:
                 raise Exception(res.text)
 
     @verify_credentials
     def make_decision(self, id: str, decision: int):
         """ Add a new decision for a security recommendation """
         with Spinner():
             params = dict(decision=decision)
-            res = requests.post(f'{self.account.hq}/detect/recommendations/{id}', headers=self.account.headers, json=params)
+            res = requests.post(
+                f'{self.account.hq}/detect/recommendations/{id}',
+                headers=self.account.headers,
+                json=params,
+                timeout=10
+            )
             if res.status_code != 200:
                 raise Exception(res.text)
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk/models/account.py` & `prelude-sdk-0.9.96/prelude_sdk/models/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             return func(*args, **kwargs)
         except FileNotFoundError:
             raise Exception('Please create a %s file' % args[0].account.keychain_location)
         except KeyError as e:
             raise Exception('Property not found, %s' % e)
         except StopIteration:
             raise Exception('Could not find "%s" profile in %s' % (args[0].account.profile, args[0].account.keychain_location))
+    handler.__wrapped__ = func
     return handler
 
 
 class Account:
 
     def __init__(self, profile='default', hq='https://api.preludesecurity.com', keychain_location=os.path.join(Path.home(), '.prelude', 'keychain.ini')):
         self.profile = profile
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk/models/codes.py` & `prelude-sdk-0.9.96/prelude_sdk/models/codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     UNPROTECTED = 101
     TIMEOUT = 102
     CLEANUP_ERROR = 103
     NOT_RELEVANT = 104
     QUARANTINED_1 = 105
     OUTBOUND_SECURE = 106
     EXPLOIT_PREVENTED = 107
-    INCOMPATIBLE_HOST = 126
+    ENDPOINT_BLOCKED = 126
     QUARANTINED_2 = 127
     UNEXPECTED = 256
 
     @classmethod
     def _missing_(cls, value):
         return ExitCode.MISSING
 
@@ -82,22 +82,22 @@
                 ExitCode.PROTECTED,
                 ExitCode.QUARANTINED_1,
                 ExitCode.QUARANTINED_2,
                 ExitCode.PROCESS_KILLED_1,
                 ExitCode.PROCESS_KILLED_2,
                 ExitCode.NOT_RELEVANT,
                 ExitCode.OUTBOUND_SECURE,
+                ExitCode.ENDPOINT_BLOCKED,
                 ExitCode.EXPLOIT_PREVENTED
             ],
             State.UNPROTECTED: [ExitCode.UNPROTECTED],
             State.ERROR: [
                 ExitCode.ERROR,
                 ExitCode.MALFORMED_VST,
                 ExitCode.TIMEOUT,
-                ExitCode.INCOMPATIBLE_HOST,
                 ExitCode.UNEXPECTED
             ]
         }
 
 
 class Decision(Enum):
     NONE = 0
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk/spinner.py` & `prelude-sdk-0.9.96/prelude_sdk/spinner.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-0.9.95/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-0.9.96/prelude_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 0.9.95
+Version: 0.9.96
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,7 +29,16 @@
 ```bash
 pip install prelude-sdk
 ```
 
 ## Documentation 
 
 TBD
+
+## Testing
+
+To test the Python SDK and Probes, run the following commands:
+
+```bash
+pip install -r python/sdk/tests/requirements.txt
+pytest tests --api https://api.preludesecurity.com --email <EMAIL>
+```
```

### Comparing `prelude-sdk-0.9.95/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-0.9.96/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,15 @@
 prelude_sdk/controllers/__init__.py
 prelude_sdk/controllers/build_controller.py
 prelude_sdk/controllers/detect_controller.py
 prelude_sdk/controllers/iam_controller.py
 prelude_sdk/controllers/probe_controller.py
 prelude_sdk/models/__init__.py
 prelude_sdk/models/account.py
-prelude_sdk/models/codes.py
+prelude_sdk/models/codes.py
+tests/__init__.py
+tests/conftest.py
+tests/test_build_controller.py
+tests/test_detect_controller.py
+tests/test_iam_controller.py
+tests/test_probe_controller.py
+tests/templates/__init__.py
```

### Comparing `prelude-sdk-0.9.95/setup.cfg` & `prelude-sdk-0.9.96/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 0.9.95
+version = 0.9.96
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

