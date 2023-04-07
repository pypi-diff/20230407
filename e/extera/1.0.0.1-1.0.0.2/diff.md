# Comparing `tmp/extera-1.0.0.1.tar.gz` & `tmp/extera-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extera-1.0.0.1.tar", last modified: Thu Apr  6 22:13:22 2023, max compression
+gzip compressed data, was "extera-1.0.0.2.tar", last modified: Fri Apr  7 18:03:10 2023, max compression
```

## Comparing `extera-1.0.0.1.tar` & `extera-1.0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.507093 extera-1.0.0.1/
--rw-rw-rw-   0        0        0      818 2023-04-06 21:48:44.000000 extera-1.0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1507 2023-04-06 22:13:22.506097 extera-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-04-06 21:40:31.000000 extera-1.0.0.1/README.md
--rw-rw-rw-   0        0        0      869 2023-04-06 22:13:01.000000 extera-1.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 22:13:22.507093 extera-1.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.452535 extera-1.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.461544 extera-1.0.0.1/src/extera/
--rw-rw-rw-   0        0        0        0 2023-03-10 22:35:40.000000 extera-1.0.0.1/src/extera/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.497849 extera-1.0.0.1/src/extera/api/
--rw-rw-rw-   0        0        0        0 2023-03-10 22:35:40.000000 extera-1.0.0.1/src/extera/api/__init__.py
--rw-rw-rw-   0        0        0     2951 2023-04-06 17:23:52.000000 extera-1.0.0.1/src/extera/api/auth.py
--rw-rw-rw-   0        0        0     5456 2023-04-06 17:22:59.000000 extera-1.0.0.1/src/extera/api/base.py
--rw-rw-rw-   0        0        0     5889 2023-04-04 00:27:28.000000 extera-1.0.0.1/src/extera/api/case.py
--rw-rw-rw-   0        0        0       97 2023-04-06 17:31:57.000000 extera-1.0.0.1/src/extera/api/config.py
--rw-rw-rw-   0        0        0     4448 2023-03-30 22:14:28.000000 extera-1.0.0.1/src/extera/api/geometry.py
--rw-rw-rw-   0        0        0     1705 2023-04-06 17:42:53.000000 extera-1.0.0.1/src/extera/api/notificationListener.py
--rw-rw-rw-   0        0        0      114 2023-03-22 22:34:16.000000 extera-1.0.0.1/src/extera/api/paramValue.py
--rw-rw-rw-   0        0        0    13368 2023-04-04 00:40:23.000000 extera-1.0.0.1/src/extera/api/project.py
--rw-rw-rw-   0        0        0     1131 2023-04-06 17:28:30.000000 extera-1.0.0.1/src/extera/api/run.py
--rw-rw-rw-   0        0        0     4056 2023-04-06 17:28:45.000000 extera-1.0.0.1/src/extera/api/study.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.499853 extera-1.0.0.1/src/extera/tools/
--rw-rw-rw-   0        0        0        0 2023-04-06 21:13:20.000000 extera-1.0.0.1/src/extera/tools/__init__.py
--rw-rw-rw-   0        0        0    31098 2023-04-06 21:23:48.000000 extera-1.0.0.1/src/extera/tools/interpret.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.503927 extera-1.0.0.1/src/extera/utils/
--rw-rw-rw-   0        0        0        0 2023-03-10 22:35:40.000000 extera-1.0.0.1/src/extera/utils/__init__.py
--rw-rw-rw-   0        0        0      328 2023-03-10 22:35:40.000000 extera-1.0.0.1/src/extera/utils/excel.py
--rw-rw-rw-   0        0        0     2009 2023-03-10 22:35:40.000000 extera-1.0.0.1/src/extera/utils/range.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:13:22.483664 extera-1.0.0.1/src/extera.egg-info/
--rw-rw-rw-   0        0        0     1507 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-06 22:13:22.000000 extera-1.0.0.1/src/extera.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.164742 extera-1.0.0.2/
+-rw-rw-rw-   0        0        0      818 2023-04-06 21:48:44.000000 extera-1.0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1507 2023-04-07 18:03:10.163733 extera-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-04-06 21:40:31.000000 extera-1.0.0.2/README.md
+-rw-rw-rw-   0        0        0      869 2023-04-07 18:02:46.000000 extera-1.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 18:03:10.164742 extera-1.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.068107 extera-1.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.074635 extera-1.0.0.2/src/extera/
+-rw-rw-rw-   0        0        0        0 2023-03-10 22:35:40.000000 extera-1.0.0.2/src/extera/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.125505 extera-1.0.0.2/src/extera/api/
+-rw-rw-rw-   0        0        0      103 2023-04-07 17:20:55.000000 extera-1.0.0.2/src/extera/api/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-04-07 17:12:04.000000 extera-1.0.0.2/src/extera/api/auth.py
+-rw-rw-rw-   0        0        0     5456 2023-04-06 17:22:59.000000 extera-1.0.0.2/src/extera/api/base.py
+-rw-rw-rw-   0        0        0     6072 2023-04-07 17:22:42.000000 extera-1.0.0.2/src/extera/api/case.py
+-rw-rw-rw-   0        0        0       97 2023-04-06 17:31:57.000000 extera-1.0.0.2/src/extera/api/config.py
+-rw-rw-rw-   0        0        0     4652 2023-04-07 17:23:31.000000 extera-1.0.0.2/src/extera/api/geometry.py
+-rw-rw-rw-   0        0        0     4165 2023-04-07 17:58:21.000000 extera-1.0.0.2/src/extera/api/notificationListener.py
+-rw-rw-rw-   0        0        0      279 2023-04-07 18:00:20.000000 extera-1.0.0.2/src/extera/api/paramValue.py
+-rw-rw-rw-   0        0        0    13669 2023-04-07 17:16:10.000000 extera-1.0.0.2/src/extera/api/project.py
+-rw-rw-rw-   0        0        0     1223 2023-04-07 18:01:06.000000 extera-1.0.0.2/src/extera/api/run.py
+-rw-rw-rw-   0        0        0     4244 2023-04-07 18:01:45.000000 extera-1.0.0.2/src/extera/api/study.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.141970 extera-1.0.0.2/src/extera/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-06 21:13:20.000000 extera-1.0.0.2/src/extera/tools/__init__.py
+-rw-rw-rw-   0        0        0    31082 2023-04-06 22:24:14.000000 extera-1.0.0.2/src/extera/tools/interpret.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.161525 extera-1.0.0.2/src/extera/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-10 22:35:40.000000 extera-1.0.0.2/src/extera/utils/__init__.py
+-rw-rw-rw-   0        0        0      328 2023-03-10 22:35:40.000000 extera-1.0.0.2/src/extera/utils/excel.py
+-rw-rw-rw-   0        0        0     2009 2023-03-10 22:35:40.000000 extera-1.0.0.2/src/extera/utils/range.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:03:10.110775 extera-1.0.0.2/src/extera.egg-info/
+-rw-rw-rw-   0        0        0     1507 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-07 18:03:10.000000 extera-1.0.0.2/src/extera.egg-info/top_level.txt
```

### Comparing `extera-1.0.0.1/LICENSE.txt` & `extera-1.0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extera-1.0.0.1/PKG-INFO` & `extera-1.0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extera
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: Python language binding for Extera Design API
 Author: Extera Design
 License: Copyright (c) 2023 Extera Design. All rights reserved.
         
         Without an explicit agreement, permission is hereby denied to any person
         obtaining a copy of this software and associated documentation files (the
         "Software"), to use, copy, modify, merge, publish, distribute, sublicense,
```

### Comparing `extera-1.0.0.1/pyproject.toml` & `extera-1.0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "extera"
-version = "1.0.0.1"
+version = "1.0.0.2"
 authors = [{name = "Extera Design"}]
 description = "Python language binding for Extera Design API"
 requires-python = ">=3.10"
 dependencies = [
     "requests",
     "websockets",
     "lark",
```

### Comparing `extera-1.0.0.1/src/extera/api/auth.py` & `extera-1.0.0.2/src/extera/api/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,7 +93,10 @@
     r = requests.post(url = '{api}/auth/logout'.format(api = Config.apiUrl), headers = headers, verify = False)
     # print the status
     if r.status_code == 200:
         print('Logout successful')
     else:
         print('Logout failed')
         print(r.content)
+
+
+__all__ = ["login", "logout", "LoginData", "LoginResponse"]
```

### Comparing `extera-1.0.0.1/src/extera/api/base.py` & `extera-1.0.0.2/src/extera/api/base.py`

 * *Files identical despite different names*

### Comparing `extera-1.0.0.1/src/extera/api/case.py` & `extera-1.0.0.2/src/extera/api/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Provides functions to create, access and execute cases from a project or study.
+"""
+
 # imports
 from typing import TypedDict
 from .paramValue import ParameterValue
 from .run import Run
 from .base import *
 
 # case related dictionary types
@@ -143,7 +146,9 @@
         accessToken = accessToken,
         knownErrors =  {
             499: "A previous run is currently queued for execution or running.",
             404: "Failed to create the run.",
             "unknown": "Unknown error. Failed to create the run."
         },
     )
+
+__all__ = ["createCaseInStudy", "createCaseInProject", "getCase", "executeCase", "Case"]
```

### Comparing `extera-1.0.0.1/src/extera/api/geometry.py` & `extera-1.0.0.2/src/extera/api/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Provides functions to add/upload, access, delete and rename geometries.
+"""
+
 # imports
 from os import path
 from typing import TypedDict
 from .base import *
 
 # geometry dictionary types
 class Geometry(TypedDict):
@@ -103,7 +106,9 @@
         data = { "file": newName },
         accessToken = accessToken,
         knownErrors =  {
             404: "The geometry does not exist.",
             "unknown": "Unknown error. Failed to rename the geometry."
         },
     )
+
+__all__ = ["addProjectGeometry", "addProjectGeometries", "getGeometry", "deleteGeometry", "renameGeometry", "Geometry"]
```

### Comparing `extera-1.0.0.1/src/extera/api/project.py` & `extera-1.0.0.2/src/extera/api/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,8 +337,23 @@
     
     casesAsList = list(filter(lambda s: s["name"] == caseName, cases))
     if len(casesAsList) == 0:
         print("Project does not contain a case with name {}".format(caseName))
         return
     if len(casesAsList) == 0:
         return None
-    return casesAsList[0]
+    return casesAsList[0]
+
+__all__ = [
+    "CreateProjectData",
+    "Authorization",
+    "Project",
+    "createProject",
+    "enumAllProjects",
+    "getProject",
+    "getProjectCases",
+    "getProjectStudies",
+    "importXlsx",
+    "getProjectGeometryByName",
+    "getStudyByName",
+    "getProjectCaseByName",
+]
```

### Comparing `extera-1.0.0.1/src/extera/api/run.py` & `extera-1.0.0.2/src/extera/api/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Provides a function to download the run results.
+"""
+
 from typing import TypedDict
 from .paramValue import ParameterValue
 from .base import *
 
 # run related dictionary types
 class Run(TypedDict):
   _id: str
@@ -35,8 +38,8 @@
     accessToken = accessToken,
     knownErrors =  {
       404: "Failed to download the run results.",
       "unknown": "Unknown error: Failed to download the run results.",
     },
   )
 
-    
+__all__ = ["Run", "downloadRunResults"]
```

### Comparing `extera-1.0.0.1/src/extera/api/study.py` & `extera-1.0.0.2/src/extera/api/study.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Provides functions to create, access and access contents of studies.
+"""
+
 # imports
 from typing import TypedDict
 from .case import Case
 from .base import *
 
 # study dictionary types
 class CreateStudyData(TypedDict):
@@ -103,8 +106,10 @@
     casesAsList = list(filter(lambda s: s["name"] == caseName, cases))
     if len(casesAsList) == 0:
         print("Study does not contain a case with name {}".format(caseName))
         return
     
     if len(casesAsList) == 0:
         return None    
-    return casesAsList[0]
+    return casesAsList[0]
+
+__all__ = ["CreateStudyData", "Study", "createStudy", "getStudyCases", "getStudy", "getStudyCaseByName"]
```

### Comparing `extera-1.0.0.1/src/extera/tools/interpret.py` & `extera-1.0.0.2/src/extera/tools/interpret.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     An Extera API script interpreter for a simple and friendly script language
 """
 import urllib3
 import os.path
 import sys
 import re
 import json
-import asyncio
 from shutil import unpack_archive, rmtree
 from threading import Event
 from lark import Lark, Transformer, v_args, lexer, Tree
 from typing import TypedDict, Callable
  
 # adding the folder where the package is located to the system path
 sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
```

### Comparing `extera-1.0.0.1/src/extera/utils/range.py` & `extera-1.0.0.2/src/extera/utils/range.py`

 * *Files identical despite different names*

### Comparing `extera-1.0.0.1/src/extera.egg-info/PKG-INFO` & `extera-1.0.0.2/src/extera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extera
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: Python language binding for Extera Design API
 Author: Extera Design
 License: Copyright (c) 2023 Extera Design. All rights reserved.
         
         Without an explicit agreement, permission is hereby denied to any person
         obtaining a copy of this software and associated documentation files (the
         "Software"), to use, copy, modify, merge, publish, distribute, sublicense,
```

### Comparing `extera-1.0.0.1/src/extera.egg-info/SOURCES.txt` & `extera-1.0.0.2/src/extera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

