# Comparing `tmp/arcanum-newspaper-segmentation-client-1.5.2.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.5.2.tar", last modified: Fri Apr  7 18:17:36 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.5.3.tar", last modified: Fri Apr  7 18:22:30 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.5.2.tar` & `arcanum-newspaper-segmentation-client-1.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 18:17:36.710740 arcanum-newspaper-segmentation-client-1.5.2/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-07 18:17:36.710740 arcanum-newspaper-segmentation-client-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.2/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 18:17:36.710740 arcanum-newspaper-segmentation-client-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-07 18:17:23.000000 arcanum-newspaper-segmentation-client-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 18:17:36.678462 arcanum-newspaper-segmentation-client-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 18:17:36.695083 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-07 18:17:36.000000 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-07 18:17:36.000000 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 18:17:36.000000 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-07 18:17:36.000000 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-07 18:17:36.000000 arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 18:17:36.710740 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    12979 2023-04-07 18:09:27.000000 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0      922 2023-04-07 16:13:39.000000 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     2269 2023-04-04 22:05:29.000000 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:22:30.381074 arcanum-newspaper-segmentation-client-1.5.3/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-07 18:22:30.365381 arcanum-newspaper-segmentation-client-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.3/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 18:22:30.381074 arcanum-newspaper-segmentation-client-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-07 18:22:17.000000 arcanum-newspaper-segmentation-client-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:22:30.334081 arcanum-newspaper-segmentation-client-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 18:22:30.365381 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-07 18:22:30.000000 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-07 18:22:30.000000 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 18:22:30.000000 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-07 18:22:30.000000 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-07 18:22:30.000000 arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 18:22:30.365381 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    12979 2023-04-07 18:09:27.000000 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-07 18:21:52.000000 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     2269 2023-04-04 22:05:29.000000 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/LICENSE` & `arcanum-newspaper-segmentation-client-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.5.2
+Version: 1.5.3
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/setup.py` & `arcanum-newspaper-segmentation-client-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.5.2",
+    version="1.5.3",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.5.2
+Version: 1.5.3
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.5.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 
 def clip_article(image: Image, article: Dict):
     alpha_mask = Image.new('L', image.size, 0)
     alpha_mask_draw = ImageDraw.Draw(alpha_mask)
     scale_boundary(article["boundary"], (image.width, image.height))
     for polygon in article["boundary"]:
-        alpha_mask_draw.polygon(polygon[0], fill=255)
+        alpha_mask_draw.polygon(polygon[0], fill=255, outline=255, width=10)
         for hole in polygon[1:]:
             alpha_mask_draw.polygon(hole, fill=0)
     article_image = image.copy()
     article_image.putalpha(alpha_mask)
     return article_image.crop(alpha_mask.getbbox())
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/pdf.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.2/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.5.3/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

