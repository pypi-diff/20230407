# Comparing `tmp/arcanum-newspaper-segmentation-client-1.4.1.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f:\repos\arcanum-main\products\newspaper_segmentation\newspaper_segmentation_client\dist\tmp2dgu4bbk\arcanum-newspaper-segmenta", last modified: Fri Jun  3 09:48:18 2022, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.5.0.tar", last modified: Fri Apr  7 16:27:31 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.4.1.tar` & `arcanum-newspaper-segmentation-client-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      716 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2022-06-03 09:46:48.000000 arcanum-newspaper-segmentation-client-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/
-drwxrwxrwx   0        0        0        0 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0        1 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      716 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       28 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       30 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-03 09:48:18.000000 arcanum-newspaper-segmentation-client-1.4.1/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    16873 2022-06-03 09:44:28.000000 arcanum-newspaper-segmentation-client-1.4.1/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0    12514 2022-02-15 14:40:04.000000 arcanum-newspaper-segmentation-client-1.4.1/src/newspaper_segmentation_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:27:31.276939 arcanum-newspaper-segmentation-client-1.5.0/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-07 16:27:31.276939 arcanum-newspaper-segmentation-client-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.0/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 16:27:31.276939 arcanum-newspaper-segmentation-client-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-07 16:25:04.000000 arcanum-newspaper-segmentation-client-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:27:31.230060 arcanum-newspaper-segmentation-client-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 16:27:31.245684 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-07 16:27:31.000000 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-07 16:27:31.000000 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:27:31.000000 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-07 16:27:31.000000 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-07 16:27:31.000000 arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 16:27:31.276939 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    12514 2023-04-04 17:58:06.000000 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0      922 2023-04-07 16:13:39.000000 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     2269 2023-04-04 22:05:29.000000 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      691 2023-04-04 22:05:29.000000 arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/text.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/LICENSE` & `arcanum-newspaper-segmentation-client-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.4.1
+Version: 1.5.0
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arcanum Newspaper Segmentation client
 
 Client for Arcanum Newspaper Segmentation API.
 [Read more](https://www.arcanum.com/en/newspaper-segmentation/)
-
-
```

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/setup.py` & `arcanum-newspaper-segmentation-client-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.4.1",
+    version="1.5.0",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
@@ -17,13 +17,14 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'pillow',
         'boto3',
         'requests',
-        'numpy'
+        'numpy',
+        'pymupdf<=1.21.1'
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.5.0/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.4.1
+Version: 1.5.0
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Arcanum Newspaper Segmentation client
 
 Client for Arcanum Newspaper Segmentation API.
 [Read more](https://www.arcanum.com/en/newspaper-segmentation/)
-
-
```

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.4.1/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.5.0/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

