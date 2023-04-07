# Comparing `tmp/metaseg-0.2.1.tar.gz` & `tmp/metaseg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.2.1.tar", last modified: Fri Apr  7 20:09:30 2023, max compression
+gzip compressed data, was "metaseg-0.2.2.tar", last modified: Fri Apr  7 20:10:36 2023, max compression
```

## Comparing `metaseg-0.2.1.tar` & `metaseg-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:09:30.971795 metaseg-0.2.1/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.2.1/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.2.1/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1349 2023-04-07 20:09:30.971795 metaseg-0.2.1/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1075 2023-04-07 20:09:08.000000 metaseg-0.2.1/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:09:30.968462 metaseg-0.2.1/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-07 20:09:20.000000 metaseg-0.2.1/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.2.1/metaseg/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4502 2023-04-07 20:09:23.000000 metaseg-0.2.1/metaseg/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:09:30.971795 metaseg-0.2.1/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.2.1/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.2.1/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.2.1/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.2.1/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.2.1/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.2.1/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.2.1/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:09:30.971795 metaseg-0.2.1/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      197 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1257 2023-04-07 20:00:15.000000 metaseg-0.2.1/metaseg/utils/file.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.2.1/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:09:30.968462 metaseg-0.2.1/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1349 2023-04-07 20:09:30.000000 metaseg-0.2.1/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      681 2023-04-07 20:09:30.000000 metaseg-0.2.1/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-07 20:09:30.000000 metaseg-0.2.1/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      212 2023-04-07 20:09:30.000000 metaseg-0.2.1/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-07 20:09:30.000000 metaseg-0.2.1/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.2.1/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      125 2023-04-06 18:52:09.000000 metaseg-0.2.1/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-07 20:09:30.975128 metaseg-0.2.1/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.2.1/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:10:36.321794 metaseg-0.2.2/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.2.2/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.2.2/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1349 2023-04-07 20:10:36.321794 metaseg-0.2.2/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1075 2023-04-07 20:09:08.000000 metaseg-0.2.2/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:10:36.318461 metaseg-0.2.2/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-07 20:10:24.000000 metaseg-0.2.2/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.2.2/metaseg/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4502 2023-04-07 20:09:23.000000 metaseg-0.2.2/metaseg/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:10:36.321794 metaseg-0.2.2/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.2.2/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.2.2/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.2.2/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.2.2/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.2.2/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.2.2/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.2.2/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:10:36.321794 metaseg-0.2.2/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      197 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1257 2023-04-07 20:00:15.000000 metaseg-0.2.2/metaseg/utils/file.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.2.2/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:10:36.318461 metaseg-0.2.2/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1349 2023-04-07 20:10:36.000000 metaseg-0.2.2/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      681 2023-04-07 20:10:36.000000 metaseg-0.2.2/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-07 20:10:36.000000 metaseg-0.2.2/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      212 2023-04-07 20:10:36.000000 metaseg-0.2.2/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-07 20:10:36.000000 metaseg-0.2.2/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.2.2/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      125 2023-04-06 18:52:09.000000 metaseg-0.2.2/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-07 20:10:36.321794 metaseg-0.2.2/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.2.2/setup.py
```

### Comparing `metaseg-0.2.1/LICENSE` & `metaseg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/PKG-INFO` & `metaseg-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.2.2 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                                 [pypi_version]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.2.1/README.md` & `metaseg-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/automatic_mask_generator.py` & `metaseg-0.2.2/metaseg/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/build_sam.py` & `metaseg-0.2.2/metaseg/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/demo.py` & `metaseg-0.2.2/metaseg/demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/common.py` & `metaseg-0.2.2/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/image_encoder.py` & `metaseg-0.2.2/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/mask_decoder.py` & `metaseg-0.2.2/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/prompt_encoder.py` & `metaseg-0.2.2/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/sam.py` & `metaseg-0.2.2/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/modeling/transformer.py` & `metaseg-0.2.2/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/predictor.py` & `metaseg-0.2.2/metaseg/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/utils/amg.py` & `metaseg-0.2.2/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/utils/file.py` & `metaseg-0.2.2/metaseg/utils/file.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/utils/onnx.py` & `metaseg-0.2.2/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg/utils/transforms.py` & `metaseg-0.2.2/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/metaseg.egg-info/PKG-INFO` & `metaseg-0.2.2/metaseg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.2.2 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                                 [pypi_version]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.2.1/metaseg.egg-info/SOURCES.txt` & `metaseg-0.2.2/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.2.1/setup.py` & `metaseg-0.2.2/setup.py`

 * *Files identical despite different names*

