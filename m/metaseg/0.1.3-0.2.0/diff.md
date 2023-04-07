# Comparing `tmp/metaseg-0.1.3.tar.gz` & `tmp/metaseg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.1.3.tar", last modified: Fri Apr  7 13:29:34 2023, max compression
+gzip compressed data, was "metaseg-0.2.0.tar", last modified: Fri Apr  7 20:00:20 2023, max compression
```

## Comparing `metaseg-0.1.3.tar` & `metaseg-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 13:29:34.264477 metaseg-0.1.3/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.1.3/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.1.3/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1066 2023-04-07 13:29:34.264477 metaseg-0.1.3/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      792 2023-04-07 13:27:02.000000 metaseg-0.1.3/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 13:29:34.257811 metaseg-0.1.3/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-07 13:29:03.000000 metaseg-0.1.3/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.1.3/metaseg/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1839 2023-04-07 13:29:29.000000 metaseg-0.1.3/metaseg/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 13:29:34.261144 metaseg-0.1.3/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 13:29:34.264477 metaseg-0.1.3/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      197 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.1.3/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 13:29:34.261144 metaseg-0.1.3/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1066 2023-04-07 13:29:34.000000 metaseg-0.1.3/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      659 2023-04-07 13:29:34.000000 metaseg-0.1.3/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-07 13:29:34.000000 metaseg-0.1.3/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      212 2023-04-07 13:29:34.000000 metaseg-0.1.3/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-07 13:29:34.000000 metaseg-0.1.3/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.1.3/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      125 2023-04-06 18:52:09.000000 metaseg-0.1.3/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-07 13:29:34.264477 metaseg-0.1.3/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.1.3/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:00:19.998468 metaseg-0.2.0/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.2.0/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.2.0/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1054 2023-04-07 20:00:19.998468 metaseg-0.2.0/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      780 2023-04-07 19:59:53.000000 metaseg-0.2.0/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:00:19.995134 metaseg-0.2.0/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-07 18:10:55.000000 metaseg-0.2.0/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.2.0/metaseg/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4179 2023-04-07 20:00:15.000000 metaseg-0.2.0/metaseg/demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:00:19.998468 metaseg-0.2.0/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.2.0/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.2.0/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.2.0/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.2.0/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.2.0/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.2.0/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.2.0/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:00:19.998468 metaseg-0.2.0/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      197 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1257 2023-04-07 20:00:15.000000 metaseg-0.2.0/metaseg/utils/file.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.2.0/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-07 20:00:19.995134 metaseg-0.2.0/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1054 2023-04-07 20:00:19.000000 metaseg-0.2.0/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      681 2023-04-07 20:00:19.000000 metaseg-0.2.0/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-07 20:00:19.000000 metaseg-0.2.0/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      212 2023-04-07 20:00:19.000000 metaseg-0.2.0/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-07 20:00:19.000000 metaseg-0.2.0/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.2.0/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      125 2023-04-06 18:52:09.000000 metaseg-0.2.0/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-07 20:00:19.998468 metaseg-0.2.0/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.2.0/setup.py
```

### Comparing `metaseg-0.1.3/LICENSE` & `metaseg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/PKG-INFO` & `metaseg-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.1.3
+Version: 0.2.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -30,14 +30,13 @@
 ```
 
 ### Usage
 ```python
 from metaseg import SegAutoMaskGenerator
 
 SegAutoMaskGenerator(
-        model_type="default", 
-        checkpoint_path="sam_vit_h_4b8939.pth",
-        image_path= "test.png",
-        device="cuda",
-        show_mask=True, 
+        model_type="vit_h", # "vit_l", "vit_b"
+        source= "test.png", # test.mp4
+        device="cuda", # "cpu" or "cuda"
+        show=True, 
 )
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.1.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.2.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                                 [pypi_version]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator
-SegAutoMaskGenerator( model_type="default",
-checkpoint_path="sam_vit_h_4b8939.pth", image_path= "test.png", device="cuda",
-show_mask=True, ) ```
+SegAutoMaskGenerator( model_type="vit_h", # "vit_l", "vit_b" source=
+"test.png", # test.mp4 device="cuda", # "cpu" or "cuda" show=True, ) ```
```

### Comparing `metaseg-0.1.3/README.md` & `metaseg-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,13 @@
 ```
 
 ### Usage
 ```python
 from metaseg import SegAutoMaskGenerator
 
 SegAutoMaskGenerator(
-        model_type="default", 
-        checkpoint_path="sam_vit_h_4b8939.pth",
-        image_path= "test.png",
-        device="cuda",
-        show_mask=True, 
+        model_type="vit_h", # "vit_l", "vit_b"
+        source= "test.png", # test.mp4
+        device="cuda", # "cpu" or "cuda"
+        show=True, 
 )
 ```
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                                 [pypi_version]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator
-SegAutoMaskGenerator( model_type="default",
-checkpoint_path="sam_vit_h_4b8939.pth", image_path= "test.png", device="cuda",
-show_mask=True, ) ```
+SegAutoMaskGenerator( model_type="vit_h", # "vit_l", "vit_b" source=
+"test.png", # test.mp4 device="cuda", # "cpu" or "cuda" show=True, ) ```
```

### Comparing `metaseg-0.1.3/metaseg/automatic_mask_generator.py` & `metaseg-0.2.0/metaseg/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/build_sam.py` & `metaseg-0.2.0/metaseg/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/common.py` & `metaseg-0.2.0/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/image_encoder.py` & `metaseg-0.2.0/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/mask_decoder.py` & `metaseg-0.2.0/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/prompt_encoder.py` & `metaseg-0.2.0/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/sam.py` & `metaseg-0.2.0/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/modeling/transformer.py` & `metaseg-0.2.0/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/predictor.py` & `metaseg-0.2.0/metaseg/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/utils/amg.py` & `metaseg-0.2.0/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/utils/onnx.py` & `metaseg-0.2.0/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg/utils/transforms.py` & `metaseg-0.2.0/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.1.3/metaseg.egg-info/PKG-INFO` & `metaseg-0.2.0/metaseg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.1.3
+Version: 0.2.0
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -30,14 +30,13 @@
 ```
 
 ### Usage
 ```python
 from metaseg import SegAutoMaskGenerator
 
 SegAutoMaskGenerator(
-        model_type="default", 
-        checkpoint_path="sam_vit_h_4b8939.pth",
-        image_path= "test.png",
-        device="cuda",
-        show_mask=True, 
+        model_type="vit_h", # "vit_l", "vit_b"
+        source= "test.png", # test.mp4
+        device="cuda", # "cpu" or "cuda"
+        show=True, 
 )
 ```
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.1.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.2.0 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                                 [pypi_version]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator
-SegAutoMaskGenerator( model_type="default",
-checkpoint_path="sam_vit_h_4b8939.pth", image_path= "test.png", device="cuda",
-show_mask=True, ) ```
+SegAutoMaskGenerator( model_type="vit_h", # "vit_l", "vit_b" source=
+"test.png", # test.mp4 device="cuda", # "cpu" or "cuda" show=True, ) ```
```

### Comparing `metaseg-0.1.3/metaseg.egg-info/SOURCES.txt` & `metaseg-0.2.0/metaseg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 metaseg/modeling/image_encoder.py
 metaseg/modeling/mask_decoder.py
 metaseg/modeling/prompt_encoder.py
 metaseg/modeling/sam.py
 metaseg/modeling/transformer.py
 metaseg/utils/__init__.py
 metaseg/utils/amg.py
+metaseg/utils/file.py
 metaseg/utils/onnx.py
 metaseg/utils/transforms.py
```

### Comparing `metaseg-0.1.3/setup.py` & `metaseg-0.2.0/setup.py`

 * *Files identical despite different names*

