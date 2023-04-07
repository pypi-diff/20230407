# Comparing `tmp/hubmap-clt-1.1.2.tar.gz` & `tmp/hubmap-clt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubmap-clt-1.1.2.tar", last modified: Tue May 24 17:56:12 2022, max compression
+gzip compressed data, was "hubmap-clt-1.1.3.tar", last modified: Fri Apr  7 17:21:24 2023, max compression
```

## Comparing `hubmap-clt-1.1.2.tar` & `hubmap-clt-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-05-24 17:56:12.953052 hubmap-clt-1.1.2/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       34 2022-05-23 19:06:31.000000 hubmap-clt-1.1.2/MANIFEST.in
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     3323 2022-05-24 17:56:12.953052 hubmap-clt-1.1.2/PKG-INFO
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     2285 2022-03-02 20:07:39.000000 hubmap-clt-1.1.2/README.md
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-05-24 17:56:12.953052 hubmap-clt-1.1.2/hubmap_clt/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)        0 2022-03-02 20:07:39.000000 hubmap-clt-1.1.2/hubmap_clt/__init__.py
--rwxrwxr-x   0 drf57     (1000) drf57     (1000)    11110 2022-05-24 17:52:21.000000 hubmap-clt-1.1.2/hubmap_clt/__main__.py
--rwxrwxr-x   0 drf57     (1000) drf57     (1000)     2314 2022-05-23 19:30:36.000000 hubmap-clt-1.1.2/hubmap_clt/clt-help.txt
-drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2022-05-24 17:56:12.953052 hubmap-clt-1.1.2/hubmap_clt.egg-info/
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     3323 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/PKG-INFO
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      306 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/SOURCES.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)        1 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/dependency_links.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       75 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/entry_points.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)      107 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/requires.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       11 2022-05-24 17:56:12.000000 hubmap-clt-1.1.2/hubmap_clt.egg-info/top_level.txt
--rw-rw-r--   0 drf57     (1000) drf57     (1000)       38 2022-05-24 17:56:12.953052 hubmap-clt-1.1.2/setup.cfg
--rw-rw-r--   0 drf57     (1000) drf57     (1000)     1158 2022-05-24 17:52:21.000000 hubmap-clt-1.1.2/setup.py
+drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2023-04-07 17:21:24.317968 hubmap-clt-1.1.3/
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)       34 2022-05-23 19:06:31.000000 hubmap-clt-1.1.3/MANIFEST.in
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)     3323 2023-04-07 17:21:24.317968 hubmap-clt-1.1.3/PKG-INFO
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)     2285 2022-03-02 20:07:39.000000 hubmap-clt-1.1.3/README.md
+drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2023-04-07 17:21:24.313967 hubmap-clt-1.1.3/hubmap_clt/
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)        0 2022-03-02 20:07:39.000000 hubmap-clt-1.1.3/hubmap_clt/__init__.py
+-rwxrwxr-x   0 drf57     (1000) drf57     (1000)    11089 2023-04-07 16:55:49.000000 hubmap-clt-1.1.3/hubmap_clt/__main__.py
+-rwxrwxr-x   0 drf57     (1000) drf57     (1000)     2314 2023-04-06 15:20:40.000000 hubmap-clt-1.1.3/hubmap_clt/clt-help.txt
+drwxrwxr-x   0 drf57     (1000) drf57     (1000)        0 2023-04-07 17:21:24.313967 hubmap-clt-1.1.3/hubmap_clt.egg-info/
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)     3323 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/PKG-INFO
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)      306 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/SOURCES.txt
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)        1 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/dependency_links.txt
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)       75 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/entry_points.txt
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)      107 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/requires.txt
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)       11 2023-04-07 17:21:24.000000 hubmap-clt-1.1.3/hubmap_clt.egg-info/top_level.txt
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)       38 2023-04-07 17:21:24.317968 hubmap-clt-1.1.3/setup.cfg
+-rw-rw-r--   0 drf57     (1000) drf57     (1000)     1158 2023-04-07 16:59:22.000000 hubmap-clt-1.1.3/setup.py
```

### Comparing `hubmap-clt-1.1.2/PKG-INFO` & `hubmap-clt-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-clt
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command line interface to download multiple files and directories from Globus file transfer service using a manifest file.
 Home-page: UNKNOWN
 Author: Hubmap
 Author-email: api-developers@hubmapconsortium.org
 License: UNKNOWN
 Description: # hubmap-clt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hubmap-clt Version: 1.1.2 Summary: A command line
+Metadata-Version: 2.1 Name: hubmap-clt Version: 1.1.3 Summary: A command line
 interface to download multiple files and directories from Globus file transfer
 service using a manifest file. Home-page: UNKNOWN Author: Hubmap Author-email:
 api-developers@hubmapconsortium.org License: UNKNOWN Description: # hubmap-clt
 --- A command line interface to download multiple files and directories from
 the Globus file transfer service. ### Overview The HuBMAP Command-Line Transfer
 uses the Globus cli to transfer files from a manifest file. This file contains
 the ID (UUID or HuBMAP ID) and the path to the specific file or directory to be
```

### Comparing `hubmap-clt-1.1.2/README.md` & `hubmap-clt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hubmap-clt-1.1.2/hubmap_clt/__main__.py` & `hubmap-clt-1.1.3/hubmap_clt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     unique_globus_endpoint_ids = []
     # Add the particular path from manifest_dict into path_dict
     for each in path_json:
         each_dict = {}
         for item in manifest_list:
             if each['id'] in item.keys():
                 each_dict = item
-                manifest_list.remove(item)
+                break
         each["specific_path"] = each_dict[each['id']].strip('"').strip()
         if each["globus_endpoint_uuid"] not in unique_globus_endpoint_ids:
             unique_globus_endpoint_ids.append(each["globus_endpoint_uuid"])
     at_least_one_success = []
     for each in unique_globus_endpoint_ids:
         endpoint_list = []
         for item in path_json:
```

### Comparing `hubmap-clt-1.1.2/hubmap_clt/clt-help.txt` & `hubmap-clt-1.1.3/hubmap_clt/clt-help.txt`

 * *Files identical despite different names*

### Comparing `hubmap-clt-1.1.2/hubmap_clt.egg-info/PKG-INFO` & `hubmap-clt-1.1.3/hubmap_clt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-clt
-Version: 1.1.2
+Version: 1.1.3
 Summary: A command line interface to download multiple files and directories from Globus file transfer service using a manifest file.
 Home-page: UNKNOWN
 Author: Hubmap
 Author-email: api-developers@hubmapconsortium.org
 License: UNKNOWN
 Description: # hubmap-clt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hubmap-clt Version: 1.1.2 Summary: A command line
+Metadata-Version: 2.1 Name: hubmap-clt Version: 1.1.3 Summary: A command line
 interface to download multiple files and directories from Globus file transfer
 service using a manifest file. Home-page: UNKNOWN Author: Hubmap Author-email:
 api-developers@hubmapconsortium.org License: UNKNOWN Description: # hubmap-clt
 --- A command line interface to download multiple files and directories from
 the Globus file transfer service. ### Overview The HuBMAP Command-Line Transfer
 uses the Globus cli to transfer files from a manifest file. This file contains
 the ID (UUID or HuBMAP ID) and the path to the specific file or directory to be
```

### Comparing `hubmap-clt-1.1.2/setup.py` & `hubmap-clt-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name='hubmap-clt',
     description='A command line interface to download multiple files and directories from Globus file transfer '
                 'service using a manifest file.',
-    version='1.1.2',
+    version='1.1.3',
     packages=['hubmap_clt'],
     python_requires='>=3.6',
     entry_points='''
         [console_scripts]
         hubmap-clt=hubmap_clt.__main__:main
     ''',
     author="Hubmap",
```

