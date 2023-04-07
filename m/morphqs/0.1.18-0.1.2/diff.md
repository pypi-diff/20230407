# Comparing `tmp/morphqs-0.1.18.tar.gz` & `tmp/morphqs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphqs-0.1.18.tar", last modified: Fri Apr  7 15:58:17 2023, max compression
+gzip compressed data, was "morphqs-0.1.2.tar", last modified: Thu Mar 30 18:18:59 2023, max compression
```

## Comparing `morphqs-0.1.18.tar` & `morphqs-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 15:58:17.889409 morphqs-0.1.18/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.18/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-07 15:58:17.888148 morphqs-0.1.18/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.18/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 15:58:17.821551 morphqs-0.1.18/morphqs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      226 2023-04-07 14:46:49.000000 morphqs-0.1.18/morphqs/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 15:58:17.876935 morphqs-0.1.18/morphqs/components/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.18/morphqs/components/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.18/morphqs/components/ansible.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6912 2023-04-07 15:57:53.000000 morphqs-0.1.18/morphqs/components/integrations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.18/morphqs/components/uchigheredmsp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6530 2023-04-07 15:50:24.000000 morphqs-0.1.18/morphqs/components/usecasedeployment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 15:58:17.884112 morphqs-0.1.18/morphqs/logging/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.18/morphqs/logging/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.18/morphqs/logging/loghandler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.18/morphqs/morphclass.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-07 15:58:17.850081 morphqs-0.1.18/morphqs.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-07 15:58:17.000000 morphqs-0.1.18/morphqs.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-07 15:58:17.000000 morphqs-0.1.18/morphqs.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-07 15:58:17.000000 morphqs-0.1.18/morphqs.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-07 15:58:17.000000 morphqs-0.1.18/morphqs.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-07 15:58:17.000000 morphqs-0.1.18/morphqs.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-07 15:58:17.890205 morphqs-0.1.18/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-07 15:58:15.000000 morphqs-0.1.18/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.883911 morphqs-0.1.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.2/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      924 2023-03-30 18:18:59.882615 morphqs-0.1.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.826450 morphqs-0.1.2/morphqs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      154 2023-03-29 15:19:51.000000 morphqs-0.1.2/morphqs/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.869945 morphqs-0.1.2/morphqs/components/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.2/morphqs/components/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-03-30 18:18:06.000000 morphqs-0.1.2/morphqs/components/ansible.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5908 2023-03-30 17:03:38.000000 morphqs-0.1.2/morphqs/components/integrations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6361 2023-03-30 18:16:28.000000 morphqs-0.1.2/morphqs/components/uchigheredmsp.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.878601 morphqs-0.1.2/morphqs/logging/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.2/morphqs/logging/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.2/morphqs/logging/loghandler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.2/morphqs/morphclass.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-30 18:18:59.853906 morphqs-0.1.2/morphqs.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      924 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-03-30 18:18:59.000000 morphqs-0.1.2/morphqs.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-03-30 18:18:59.884626 morphqs-0.1.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2023-03-30 18:18:56.000000 morphqs-0.1.2/setup.py
```

### Comparing `morphqs-0.1.18/LICENSE.txt` & `morphqs-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.18/PKG-INFO` & `morphqs-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.18
+Version: 0.1.2
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.18/morphqs/components/integrations.py` & `morphqs-0.1.2/morphqs/components/integrations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ..morphclass import RequestsApi
 import morphqs.logging.loghandler as loghandler
 import json
 import urllib
-import sys
 
 def add_integration(default_branch, repo_url, integration_name):
     """
     The add_integration function is used to create a new integration in Morpheus.
         It takes three arguments: 
             1) default_branch - the branch that will be checked out by default when cloning the repo (defaults to master)
             2) repo_url - The URL of the repository you want to integrate with Morpheus. This can be any valid git url, including SSH and HTTP(S). 
@@ -28,61 +27,40 @@
         intid = intid["integrations"][0]["id"]
     except IndexError as e:
         intid = None
     if intid is not None: 
         logger.info(f"Integration {integration_name} already exists. Skipping.")
         logger.info(f"Integration ID: {intid}")
         logger.debug(intid)
-        coderepoId = cl.get(f"/api/options/codeRepositories?integrationId={intid}").json()
-        logger.debug(coderepoId)
-        logger.debug(f"integration id: {intid}")
-        logger.debug(f"code repo response: {coderepoId}")
-        if coderepoId["data"] != []:
-            repoid = coderepoId["data"][0]["value"]
-            logger.debug(f"repo id {repoid}")
-            return repoid
+        return intid
     else:
         logger.info(f"Integration {integration_name} does not exist. Creating.")
         root_int_payload = {"integration": {
                                 "refresh": True,
                                 "credential": {"type": "local"},
                                 "type": "git",
                                 "config": {
                                     "defaultBranch": default_branch, #"highered",
                                     "cacheEnabled": False
                                 },
                                 "name": integration_name, #"Morpheus Quickshots Base Repo",
                                 "serviceUrl": repo_url #"https://gitlab.com/jaredlutgen/morpheus_quickshots.git"
                             }}
         logger.debug(f"Creating integration {integration_name} with payload {root_int_payload}")
-        cl.post("/api/integrations", data = json.dumps(root_int_payload)).json()
-        intid = cl.get(f"/api/integrations?name={integrationname}").json()
-        try: 
-            intid = intid["integrations"][0]["id"]
-        except IndexError as e:
-            intid = None
-        coderepoId = cl.get(f"/api/options/codeRepositories?integrationId={intid}").json()
-        logger.debug(coderepoId)
-        logger.debug(f"integration id: {intid}")
-        logger.debug(f"code repo response: {coderepoId}")
-        if coderepoId["data"] != []:
-            repoid = coderepoId["data"][0]["value"]
-            logger.debug(f"repo id {repoid}")
-            return repoid
-        # logger.debug(coderepoId)
-        # logger.debug(f"integration id: {intid}")
-        # logger.debug(f"code repo response: {coderepoId}")
-        # if coderepoId["data"] != []:
-        #     repoid = coderepoId["data"][0]["value"]
-        #     logger.debug(f"repo id {repoid}")
-        #     return repoid
-        # else: 
-        #     logger.error("Failed to create integration")
-        #     logger.error(coderepoId)
-        #     sys.exit(1)
+        resp = cl.post("/api/integrations", data = json.dumps(root_int_payload)).json()
+        logger.debug(resp)
+        intid = resp["integration"]["id"]
+        if resp["success"] == True:
+            logger.info(f"Successfully created integration {integration_name}")
+        if resp["success"] == False:
+            logger.error(f"Failed to create integration {integration_name}")
+            logger.error(resp["errors"])
+        logger.debug(intid)
+        logger.debug(resp)
+        return intid
        
 
 
 
 def add_integration_ansible(default_branch, repo_url, integration_name, ansibleplaybooks, ansibleroles, ansiblegroupvars, ansiblehostvars):
     """
     The add_integration_ansible function creates an Ansible integration in Morpheus.
```

### Comparing `morphqs-0.1.18/morphqs/components/uchigheredmsp.py` & `morphqs-0.1.2/morphqs/components/uchigheredmsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
                                     "code": "jythonTask"
                                 },
                                 "visibility": "private",
                                 "labels": [
                                     "higher_ed_msp", "setup", "demo", "poc", "example"
                                 ],
                                 "taskOptions": {
-                                    "pythonAdditionalPackages": "requests morphcp click",
+                                    "pythonAdditionalPackages": "requests morphcp",
                                     "username": None,
                                     "password": None,
                                     "passwordHash": None,
                                     "pythonBinary": None,
                                     "host": None,
                                     "localScriptGitId": None,
                                     "port": None,
-                                    "pythonArgs": "highered",
+                                    "pythonArgs": "higher_ed",
                                     "localScriptGitRef": None
                                 },
                                 "file": {
                                     "sourceType": "repository",
                                     "contentRef": branch,
                                     "contentPath": hchighered_contentPath,
                                     "repository": {
```

### Comparing `morphqs-0.1.18/morphqs/logging/loghandler.py` & `morphqs-0.1.2/morphqs/logging/loghandler.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.18/morphqs/morphclass.py` & `morphqs-0.1.2/morphqs/morphclass.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.18/morphqs.egg-info/PKG-INFO` & `morphqs-0.1.2/morphqs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.18
+Version: 0.1.2
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.18/setup.py` & `morphqs-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Jared Lutgen",
     author_email="jlutgen@morpheusdata.com",
     name='morphqs',
     license="MIT",
     description='Tool utilized to deploy some basic concepts for the Morpheus Data Platform',
-    version='v0.1.18',
+    version='v0.1.2',
     long_description=README,
     url='https://gitlab.com/jaredlutgen/morphqs',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['requests'],
     classifiers=[
         # Trove classifiers
```

