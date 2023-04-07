# Comparing `tmp/fairscape-models-0.1.0.tar.gz` & `tmp/fairscape-models-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape-models-0.1.0.tar", last modified: Wed Apr  5 16:17:29 2023, max compression
+gzip compressed data, was "fairscape-models-0.1.2.tar", last modified: Fri Apr  7 17:16:26 2023, max compression
```

## Comparing `fairscape-models-0.1.0.tar` & `fairscape-models-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/
--rw-r--r--   0 max       (1000) max       (1000)     1066 2023-03-01 20:16:16.000000 fairscape-models-0.1.0/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)     1769 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)       18 2023-02-22 17:11:37.000000 fairscape-models-0.1.0/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/fairscape_models/
--rw-r--r--   0 max       (1000) max       (1000)      270 2023-03-03 21:44:01.000000 fairscape-models-0.1.0/fairscape_models/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      957 2023-04-04 16:22:00.000000 fairscape-models-0.1.0/fairscape_models/base.py
--rw-r--r--   0 max       (1000) max       (1000)      676 2023-04-04 16:21:38.000000 fairscape-models-0.1.0/fairscape_models/computation.py
--rw-r--r--   0 max       (1000) max       (1000)      912 2023-04-04 16:22:39.000000 fairscape-models-0.1.0/fairscape_models/dataset.py
--rw-r--r--   0 max       (1000) max       (1000)      799 2023-03-24 17:21:01.000000 fairscape-models-0.1.0/fairscape_models/ro_crate.py
--rw-r--r--   0 max       (1000) max       (1000)      715 2023-04-04 16:23:08.000000 fairscape-models-0.1.0/fairscape_models/software.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/fairscape_models.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1769 2023-04-05 16:17:29.000000 fairscape-models-0.1.0/fairscape_models.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      497 2023-04-05 16:17:29.000000 fairscape-models-0.1.0/fairscape_models.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-05 16:17:29.000000 fairscape-models-0.1.0/fairscape_models.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)        9 2023-04-05 16:17:29.000000 fairscape-models-0.1.0/fairscape_models.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)       17 2023-04-05 16:17:29.000000 fairscape-models-0.1.0/fairscape_models.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      680 2023-04-05 16:11:28.000000 fairscape-models-0.1.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/setup.cfg
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-05 16:17:29.368324 fairscape-models-0.1.0/tests/
--rw-r--r--   0 max       (1000) max       (1000)     1753 2023-03-08 19:58:36.000000 fairscape-models-0.1.0/tests/test_computation.py
--rw-r--r--   0 max       (1000) max       (1000)     1371 2023-03-13 21:49:23.000000 fairscape-models-0.1.0/tests/test_dataset.py
--rw-r--r--   0 max       (1000) max       (1000)     3828 2023-03-03 21:54:23.000000 fairscape-models-0.1.0/tests/test_ro_crate.py
--rw-r--r--   0 max       (1000) max       (1000)     1128 2023-03-15 15:32:17.000000 fairscape-models-0.1.0/tests/test_software.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-07 17:16:26.470506 fairscape-models-0.1.2/
+-rw-r--r--   0 max       (1000) max       (1000)     1066 2023-03-01 20:16:16.000000 fairscape-models-0.1.2/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     1769 2023-04-07 17:16:26.470506 fairscape-models-0.1.2/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)       18 2023-02-22 17:11:37.000000 fairscape-models-0.1.2/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-07 17:16:26.460506 fairscape-models-0.1.2/fairscape_models/
+-rw-r--r--   0 max       (1000) max       (1000)      270 2023-03-03 21:44:01.000000 fairscape-models-0.1.2/fairscape_models/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      957 2023-04-05 16:20:01.000000 fairscape-models-0.1.2/fairscape_models/base.py
+-rw-r--r--   0 max       (1000) max       (1000)      706 2023-04-05 19:06:00.000000 fairscape-models-0.1.2/fairscape_models/computation.py
+-rw-r--r--   0 max       (1000) max       (1000)      952 2023-04-05 19:10:56.000000 fairscape-models-0.1.2/fairscape_models/dataset.py
+-rw-r--r--   0 max       (1000) max       (1000)      799 2023-03-24 17:21:01.000000 fairscape-models-0.1.2/fairscape_models/ro_crate.py
+-rw-r--r--   0 max       (1000) max       (1000)      735 2023-04-05 19:06:00.000000 fairscape-models-0.1.2/fairscape_models/software.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-07 17:16:26.460506 fairscape-models-0.1.2/fairscape_models.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1769 2023-04-07 17:16:26.000000 fairscape-models-0.1.2/fairscape_models.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      497 2023-04-07 17:16:26.000000 fairscape-models-0.1.2/fairscape_models.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-07 17:16:26.000000 fairscape-models-0.1.2/fairscape_models.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)        9 2023-04-07 17:16:26.000000 fairscape-models-0.1.2/fairscape_models.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       17 2023-04-07 17:16:26.000000 fairscape-models-0.1.2/fairscape_models.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      680 2023-04-07 17:16:20.000000 fairscape-models-0.1.2/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2023-04-07 17:16:26.470506 fairscape-models-0.1.2/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-07 17:16:26.470506 fairscape-models-0.1.2/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     1753 2023-03-08 19:58:36.000000 fairscape-models-0.1.2/tests/test_computation.py
+-rw-r--r--   0 max       (1000) max       (1000)     1371 2023-03-13 21:49:23.000000 fairscape-models-0.1.2/tests/test_dataset.py
+-rw-r--r--   0 max       (1000) max       (1000)     3828 2023-03-03 21:54:23.000000 fairscape-models-0.1.2/tests/test_ro_crate.py
+-rw-r--r--   0 max       (1000) max       (1000)     1128 2023-03-15 15:32:17.000000 fairscape-models-0.1.2/tests/test_software.py
```

### Comparing `fairscape-models-0.1.0/LICENSE` & `fairscape-models-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/PKG-INFO` & `fairscape-models-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-models
-Version: 0.1.0
+Version: 0.1.2
 Summary: Pydantic models for B2AI metadata validation
 Author-email: Max Levinson <mal8ch@virginia.edu>
 License: MIT License
         
         Copyright (c) 2023 fairscape
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fairscape-models-0.1.0/fairscape_models/base.py` & `fairscape-models-0.1.2/fairscape_models/base.py`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/fairscape_models/computation.py` & `fairscape-models-0.1.2/fairscape_models/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,33 @@
 from typing import Optional, Union, Dict, List
 from pydantic import (
     constr,
     AnyUrl
 )
 from datetime import datetime
 
-class Computation(FairscapeBaseModel):
-    metadataType: Optional[str] = "https://w3id.org/EVI#Computation"
-    runBy: str
-    dateCreated: str
-    description: constr(min_length=10, max_length=2056)
-    associatedPublication: Optional[Union[str, AnyUrl]]
-    additionalDocumentation: Optional[Union[str, AnyUrl]]
-    command: Optional[Union[List[str], str]] 
-    usedSoftware: List[str]
-    calledBy: Optional[str]
-    usedDataset: Union[List[str], str]
-    generated: Union[str,List[str]]
-     
+class Dataset(FairscapeBaseModel):
+    metadataType: Optional[str] = "https://w3id.org/EVI#Dataset"
+    author: constr(max_length=64)
+    datePublished: str
+    version: str
+    description: constr(min_length=10)
+    associatedPublication: Optional[str]
+    additionalDocumentation: Optional[str]
+    fileFormat: str
+    dataSchema: Optional[Union[str, dict]]
+    generatedBy: Optional[List[str]]
+    derivedFrom: Optional[List[str]]
+    usedBy: Optional[List[str]]
+    contentUrl: Optional[str]
+
+    class Config:
+        fields={
+            "fileFormat": {
+                "title": "fileFormat",
+                "alias": "format"
+            },
+            "dataSchema": {
+                "title": "dataSchema",
+                "alias": "schema"
+            }
+        }
```

### Comparing `fairscape-models-0.1.0/fairscape_models/ro_crate.py` & `fairscape-models-0.1.2/fairscape_models/ro_crate.py`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/fairscape_models/software.py` & `fairscape-models-0.1.2/fairscape_models/software.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     author: constr(max_length=64)
     dateModified: str
     version: str
     description: constr(min_length=10)
     associatedPublication: Optional[str]
     additionalDocumentation: Optional[str]
     fileFormat: str
-    usedByComputation: List[str]
-    contentUrl: str
+    usedByComputation: Optional[List[str]]
+    contentUrl: Optional[str]
 
     class Config:
        fields={
         "fileFormat":
             {
                 "title": "fileFormat",
                 "alias": "format"
```

### Comparing `fairscape-models-0.1.0/fairscape_models.egg-info/PKG-INFO` & `fairscape-models-0.1.2/fairscape_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-models
-Version: 0.1.0
+Version: 0.1.2
 Summary: Pydantic models for B2AI metadata validation
 Author-email: Max Levinson <mal8ch@virginia.edu>
 License: MIT License
         
         Copyright (c) 2023 fairscape
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fairscape-models-0.1.0/pyproject.toml` & `fairscape-models-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fairscape-models"
-version = "0.1.0"
+version = "0.1.2"
 description = "Pydantic models for B2AI metadata validation"
 readme = "README.md"
 authors = [{ name = "Max Levinson", email="mal8ch@virginia.edu"}]
 license = {file= "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `fairscape-models-0.1.0/tests/test_computation.py` & `fairscape-models-0.1.2/tests/test_computation.py`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/tests/test_dataset.py` & `fairscape-models-0.1.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/tests/test_ro_crate.py` & `fairscape-models-0.1.2/tests/test_ro_crate.py`

 * *Files identical despite different names*

### Comparing `fairscape-models-0.1.0/tests/test_software.py` & `fairscape-models-0.1.2/tests/test_software.py`

 * *Files identical despite different names*

