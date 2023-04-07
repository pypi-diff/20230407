# Comparing `tmp/mlopspython-extraction-70337926846377927701164.tar.gz` & `tmp/mlopspython-extraction-74126878396677081493445.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlopspython-extraction-70337926846377927701164.tar", last modified: Fri Mar 17 20:28:04 2023, max compression
+gzip compressed data, was "mlopspython-extraction-74126878396677081493445.tar", last modified: Fri Apr  7 20:15:49 2023, max compression
```

## Comparing `mlopspython-extraction-70337926846377927701164.tar` & `mlopspython-extraction-74126878396677081493445.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-17 20:27:42.000000 mlopspython-extraction-70337926846377927701164/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 20:27:42.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-17 20:27:42.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 20:28:04.179875 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-17 20:28:04.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-17 20:28:04.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 20:28:04.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-17 20:28:04.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 20:28:04.000000 mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/top_level.txt
```

### Comparing `mlopspython-extraction-70337926846377927701164/src/mlopspython_extraction/extraction.py` & `mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/extraction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 from dataclasses import dataclass
 from io import BytesIO
 from pathlib import Path
+from typing import Iterable
 
 import fitz
 from fitz import Pixmap
 
 
 def convert_pixmap_to_rgb(pixmap) -> Pixmap:
     """Convert to rgb in order to write on png"""
     # check if it is already on rgb
     if pixmap.n < 4:
         return pixmap
     else:
         return fitz.Pixmap(fitz.csRGB, pixmap)
 
+@dataclass
+class ImageResult:
+    image_bytes_io: BytesIO
+    index_page: int
+    index_image: int
+
+def extract_images_stream(pdf_bytes) -> Iterable[ImageResult]:
+    with fitz.open(stream=pdf_bytes, filetype="pdf") as document:
+        number_pages = len(document) - 1
+        for index_page in range(number_pages):
+            images = document.get_page_images(index_page)
+            for index_image, image in enumerate(images):
+                xref = image[0]
+                image_pix = fitz.Pixmap(document, xref)
+                image_bytes_io = BytesIO(convert_pixmap_to_rgb(image_pix).tobytes())
+                yield ImageResult(image_bytes_io, index_page, index_image)
 
 @dataclass
 class ExtractImagesResult:
     number_files_input: int
     number_images_output: int
 
 
 def extract_images(pdfs_directory_path: str, images_directory_path: str) -> ExtractImagesResult:
-    pdfs = [p for p in Path(pdfs_directory_path).iterdir() if p.is_file()]
+    pdfs = [p for p in Path(pdfs_directory_path).iterdir() if p.is_file() and p.suffix == ".pdf"]
     Path(images_directory_path).mkdir(parents=True, exist_ok=True)
     number_images_output = 0
     for pdf_path in pdfs:
         with open(pdf_path, "rb") as pdf_stream:
             pdf_bytes = pdf_stream.read()
-        with fitz.open(stream=pdf_bytes, filetype="pdf") as document:
-            number_pages = len(document) - 1
-            for index in range(number_pages):
-                images = document.get_page_images(index)
-                for index_image, image in enumerate(images):
-                    xref = image[0]
-                    image_pix = fitz.Pixmap(document, xref)
-                    image_bytes_io = BytesIO(convert_pixmap_to_rgb(image_pix).tobytes())
-                    filename = "{0}_page{1}_index{2}.png".format(pdf_path.stem, str(index), str(index_image))
-                    number_images_output = number_images_output + 1
-                    with open(Path(images_directory_path) / filename, "wb") as file_stream:
-                        file_stream.write(image_bytes_io.getbuffer())
+        for image_stream in extract_images_stream(pdf_bytes):
+            filename = "{0}_page{1}_index{2}.png".format(pdf_path.stem, str(image_stream.index_page), str(image_stream.index_image))
+            number_images_output = number_images_output + 1
+            with open(Path(images_directory_path) / filename, "wb") as file_stream:
+                file_stream.write(image_stream.image_bytes_io.getbuffer())
 
     return ExtractImagesResult(number_files_input=len(pdfs), number_images_output=number_images_output)
 
+
 if __name__ == "__main__":
-    pdfs_directory_path = ".\dataset-cats-dogs-others"
-    images_directory_path = ".\extracted_images"
+    pdfs_directory_path = ".\\dataset-cats-dogs-others"
+    images_directory_path = ".\\extracted_images"
     extract_images(pdfs_directory_path, images_directory_path)
```

