# Comparing `tmp/test_rest_api-0.0.0.0.23.tar.gz` & `tmp/test_rest_api-0.0.0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_rest_api-0.0.0.0.23.tar", last modified: Fri Apr  7 17:15:08 2023, max compression
+gzip compressed data, was "test_rest_api-0.0.0.0.24.tar", last modified: Fri Apr  7 17:21:44 2023, max compression
```

## Comparing `test_rest_api-0.0.0.0.23.tar` & `test_rest_api-0.0.0.0.24.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.495660 test_rest_api-0.0.0.0.23/
--rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/LICENSE
--rw-r--r--   0 trjose     (501) staff       (20)    19464 2023-04-07 17:15:08.495065 test_rest_api-0.0.0.0.23/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)    17931 2023-04-07 07:45:37.000000 test_rest_api-0.0.0.0.23/README.md
--rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-07 17:15:08.495867 test_rest_api-0.0.0.0.23/setup.cfg
--rw-r--r--   0 trjose     (501) staff       (20)     2860 2023-04-07 17:13:41.000000 test_rest_api-0.0.0.0.23/setup.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.470161 test_rest_api-0.0.0.0.23/test_rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/__main__.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.475309 test_rest_api-0.0.0.0.23/test_rest_api/global_variables/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/global_variables/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/global_variables/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)     2568 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/global_variables/global_variables.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.477443 test_rest_api-0.0.0.0.23/test_rest_api/logger/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/logger/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/logger/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      848 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/logger/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.480037 test_rest_api-0.0.0.0.23/test_rest_api/reporting/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.23/test_rest_api/reporting/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 16:39:07.000000 test_rest_api-0.0.0.0.23/test_rest_api/reporting/html.py
--rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/reporting/report.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.484032 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/method.py
--rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/response.py
--rw-r--r--   0 trjose     (501) staff       (20)     5987 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/rest_api/rest_api.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.487891 test_rest_api-0.0.0.0.23/test_rest_api/testing/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.23/test_rest_api/testing/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/testing/bug.py
--rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-07 13:46:31.000000 test_rest_api-0.0.0.0.23/test_rest_api/testing/decorator.py
--rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.23/test_rest_api/testing/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 14:33:51.000000 test_rest_api-0.0.0.0.23/test_rest_api/testing/runner.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.493908 test_rest_api-0.0.0.0.23/test_rest_api/utils/
--rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/__init__.py
--rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/aiohttp_session.py
--rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/colors.py
--rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/decorator_hints.py
--rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/error_msg.py
--rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/exception.py
--rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.23/test_rest_api/utils/logger.py
-drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:15:08.473149 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/
--rw-r--r--   0 trjose     (501) staff       (20)    19464 2023-04-07 17:15:08.000000 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-07 17:15:08.000000 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-07 17:15:08.000000 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-07 17:15:08.000000 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/requires.txt
--rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-07 17:15:08.000000 test_rest_api-0.0.0.0.23/test_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.860928 test_rest_api-0.0.0.0.24/
+-rw-r--r--   0 trjose     (501) staff       (20)     1067 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/LICENSE
+-rw-r--r--   0 trjose     (501) staff       (20)    19654 2023-04-07 17:21:44.860291 test_rest_api-0.0.0.0.24/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)    17931 2023-04-07 07:45:37.000000 test_rest_api-0.0.0.0.24/README.md
+-rw-r--r--   0 trjose     (501) staff       (20)       38 2023-04-07 17:21:44.861106 test_rest_api-0.0.0.0.24/setup.cfg
+-rw-r--r--   0 trjose     (501) staff       (20)     2917 2023-04-07 17:21:11.000000 test_rest_api-0.0.0.0.24/setup.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.835726 test_rest_api-0.0.0.0.24/test_rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)      236 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1608 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/__main__.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.840625 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1161 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2568 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/global_variables/global_variables.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.842678 test_rest_api-0.0.0.0.24/test_rest_api/logger/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1237 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      848 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/logger/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.845383 test_rest_api-0.0.0.0.24/test_rest_api/reporting/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-25 09:45:47.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)    34587 2023-04-07 16:39:07.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/html.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5404 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/reporting/report.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.849191 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:34:23.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1824 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      423 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/method.py
+-rw-r--r--   0 trjose     (501) staff       (20)      332 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/response.py
+-rw-r--r--   0 trjose     (501) staff       (20)     5987 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/rest_api/rest_api.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.853036 test_rest_api-0.0.0.0.24/test_rest_api/testing/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-11 07:03:23.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)     3904 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/bug.py
+-rw-r--r--   0 trjose     (501) staff       (20)    14788 2023-04-07 13:46:31.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/decorator.py
+-rw-r--r--   0 trjose     (501) staff       (20)      863 2023-04-04 09:00:40.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)    13772 2023-04-07 14:33:51.000000 test_rest_api-0.0.0.0.24/test_rest_api/testing/runner.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.859166 test_rest_api-0.0.0.0.24/test_rest_api/utils/
+-rw-r--r--   0 trjose     (501) staff       (20)        0 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/__init__.py
+-rw-r--r--   0 trjose     (501) staff       (20)      943 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/aiohttp_session.py
+-rw-r--r--   0 trjose     (501) staff       (20)      546 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/colors.py
+-rw-r--r--   0 trjose     (501) staff       (20)      247 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/decorator_hints.py
+-rw-r--r--   0 trjose     (501) staff       (20)     2027 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/error_msg.py
+-rw-r--r--   0 trjose     (501) staff       (20)     1127 2023-04-03 07:06:15.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/exception.py
+-rw-r--r--   0 trjose     (501) staff       (20)      606 2023-03-24 16:41:57.000000 test_rest_api-0.0.0.0.24/test_rest_api/utils/logger.py
+drwxr-xr-x   0 trjose     (501) staff       (20)        0 2023-04-07 17:21:44.838767 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/
+-rw-r--r--   0 trjose     (501) staff       (20)    19654 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 trjose     (501) staff       (20)     1175 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 trjose     (501) staff       (20)        1 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       29 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/requires.txt
+-rw-r--r--   0 trjose     (501) staff       (20)       14 2023-04-07 17:21:44.000000 test_rest_api-0.0.0.0.24/test_rest_api.egg-info/top_level.txt
```

### Comparing `test_rest_api-0.0.0.0.23/LICENSE` & `test_rest_api-0.0.0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/PKG-INFO` & `test_rest_api-0.0.0.0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: test_rest_api
-Version: 0.0.0.0.23
+Version: 0.0.0.0.24
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
+Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
+Project-URL: Source, https://github.com/troymjose/test_rest_api
+Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_rest_api-0.0.0.0.23/README.md` & `test_rest_api-0.0.0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/setup.py` & `test_rest_api-0.0.0.0.24/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,39 @@
 """
 
 import os
 import codecs
 from setuptools import setup
 
 # Get README.md details
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as f:
-    long_description = "\n" + f.read()
+with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
+    long_description = '\n' + f.read()
 
 # Setup
-setup(name="test_rest_api",
-      version="0.0.0.0.23",
-      author="Troy M Jose",
-      author_email="",
+setup(name='test_rest_api',
+      version='0.0.0.0.24',
+      author='Troy M Jose',
+      author_email='',
+      url='https://github.com/troymjose/test_rest_api',
       bugtrack_url='https://github.com/troymjose/test_rest_api/issues',
-      project_url={
+      project_urls={
           'Source': 'https://github.com/troymjose/test_rest_api',
           'Tracker': 'https://github.com/troymjose/test_rest_api/issues',
       },
-      description="Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests",
+      description='Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests',
       keywords=['test', 'unittest', 'restapi', 'testframework', 'asyncio', 'async', 'asynchronous',
                 'testingframework', 'rest', 'api', 'python', 'python3', 'testing', 'unittesting', 'automation',
                 'automationtest', 'automationtesting',
                 'restapitest', 'restapitesting', 'restapiunittest', 'restapiunittesting', 'restapiautomation',
                 'restapiautomationtest', 'restapiautomationtesting', 'apitest', 'apitesting', 'apiunittest',
                 'apiunittesting', 'apiautomation', 'apiautomationtest', 'apiautomationtesting'],
       packages=['test_rest_api', 'test_rest_api.global_variables', 'test_rest_api.logger', 'test_rest_api.reporting',
                 'test_rest_api.rest_api', 'test_rest_api.testing', 'test_rest_api.utils'],
       install_requires=['aiohttp', 'Jinja2', 'python-dotenv'],
-      long_description_content_type="text/markdown",
+      long_description_content_type='text/markdown',
       long_description=long_description,
       classifiers=['Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
                    'Programming Language :: Python :: 3.11',
                    'Programming Language :: Python :: 3.12',
                    'License :: OSI Approved :: MIT License',
```

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/__main__.py` & `test_rest_api-0.0.0.0.24/test_rest_api/__main__.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/global_variables/exception.py` & `test_rest_api-0.0.0.0.24/test_rest_api/global_variables/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/global_variables/global_variables.py` & `test_rest_api-0.0.0.0.24/test_rest_api/global_variables/global_variables.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/logger/exception.py` & `test_rest_api-0.0.0.0.24/test_rest_api/logger/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/logger/logger.py` & `test_rest_api-0.0.0.0.24/test_rest_api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/reporting/html.py` & `test_rest_api-0.0.0.0.24/test_rest_api/reporting/html.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/reporting/report.py` & `test_rest_api-0.0.0.0.24/test_rest_api/reporting/report.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/rest_api/exception.py` & `test_rest_api-0.0.0.0.24/test_rest_api/rest_api/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/rest_api/rest_api.py` & `test_rest_api-0.0.0.0.24/test_rest_api/rest_api/rest_api.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/testing/bug.py` & `test_rest_api-0.0.0.0.24/test_rest_api/testing/bug.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/testing/decorator.py` & `test_rest_api-0.0.0.0.24/test_rest_api/testing/decorator.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/testing/exception.py` & `test_rest_api-0.0.0.0.24/test_rest_api/testing/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/testing/runner.py` & `test_rest_api-0.0.0.0.24/test_rest_api/testing/runner.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/utils/aiohttp_session.py` & `test_rest_api-0.0.0.0.24/test_rest_api/utils/aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/utils/colors.py` & `test_rest_api-0.0.0.0.24/test_rest_api/utils/colors.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/utils/error_msg.py` & `test_rest_api-0.0.0.0.24/test_rest_api/utils/error_msg.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/utils/exception.py` & `test_rest_api-0.0.0.0.24/test_rest_api/utils/exception.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api/utils/logger.py` & `test_rest_api-0.0.0.0.24/test_rest_api/utils/logger.py`

 * *Files identical despite different names*

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api.egg-info/PKG-INFO` & `test_rest_api-0.0.0.0.24/test_rest_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: test-rest-api
-Version: 0.0.0.0.23
+Version: 0.0.0.0.24
 Summary: Asynchronous Test Framework #HighPerformance #EasyToLearn #FastToCode #AsyncTests
+Home-page: https://github.com/troymjose/test_rest_api
 Author: Troy M Jose
 Author-email: 
+Project-URL: Source, https://github.com/troymjose/test_rest_api
+Project-URL: Tracker, https://github.com/troymjose/test_rest_api/issues
 Keywords: test,unittest,restapi,testframework,asyncio,async,asynchronous,testingframework,rest,api,python,python3,testing,unittesting,automation,automationtest,automationtesting,restapitest,restapitesting,restapiunittest,restapiunittesting,restapiautomation,restapiautomationtest,restapiautomationtesting,apitest,apitesting,apiunittest,apiunittesting,apiautomation,apiautomationtest,apiautomationtesting
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_rest_api-0.0.0.0.23/test_rest_api.egg-info/SOURCES.txt` & `test_rest_api-0.0.0.0.24/test_rest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

