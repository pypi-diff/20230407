# Comparing `tmp/pixelsort-cli-0.1.3.tar.gz` & `tmp/pixelsort-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelsort-cli-0.1.3.tar", last modified: Fri Apr  7 17:55:16 2023, max compression
+gzip compressed data, was "pixelsort-cli-0.1.4.tar", last modified: Fri Apr  7 19:35:52 2023, max compression
```

## Comparing `pixelsort-cli-0.1.3.tar` & `pixelsort-cli-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1072 2023-04-02 00:49:40.000000 pixelsort-cli-0.1.3/LICENSE
--rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/PKG-INFO
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1490 2023-04-07 16:20:14.000000 pixelsort-cli-0.1.3/README.md
--rw-r--r--   0 dionysus  (1000) wheel      (998)      884 2023-04-07 17:54:45.000000 pixelsort-cli-0.1.3/pyproject.toml
--rw-r--r--   0 dionysus  (1000) wheel      (998)       38 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/setup.cfg
--rw-r--r--   0 dionysus  (1000) wheel      (998)       69 2023-04-07 16:41:27.000000 pixelsort-cli-0.1.3/setup.py
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 17:55:16.033735 pixelsort-cli-0.1.3/src/
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/src/pixelsort/
--rw-r--r--   0 dionysus  (1000) wheel      (998)      115 2023-04-07 16:35:52.000000 pixelsort-cli-0.1.3/src/pixelsort/__init__.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1945 2023-04-07 16:38:22.000000 pixelsort-cli-0.1.3/src/pixelsort/__main__.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1470 2023-04-07 16:36:33.000000 pixelsort-cli-0.1.3/src/pixelsort/cli.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)      231 2023-04-07 16:36:51.000000 pixelsort-cli-0.1.3/src/pixelsort/direction.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     4616 2023-04-07 17:48:37.000000 pixelsort-cli-0.1.3/src/pixelsort/image.py
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/
--rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/PKG-INFO
--rw-r--r--   0 dionysus  (1000) wheel      (998)      431 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)        1 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       54 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/entry_points.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       44 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/requires.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       10 2023-04-07 17:55:16.000000 pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/top_level.txt
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 17:55:16.037069 pixelsort-cli-0.1.3/test/
--rw-r--r--   0 dionysus  (1000) wheel      (998)      384 2023-04-07 17:01:38.000000 pixelsort-cli-0.1.3/test/test_image.py
+drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     1072 2023-04-02 00:49:40.000000 pixelsort-cli-0.1.4/LICENSE
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/PKG-INFO
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     1490 2023-04-07 18:46:29.000000 pixelsort-cli-0.1.4/README.md
+-rw-r--r--   0 dionysus  (1000) wheel      (998)      884 2023-04-07 19:35:30.000000 pixelsort-cli-0.1.4/pyproject.toml
+-rw-r--r--   0 dionysus  (1000) wheel      (998)       38 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/setup.cfg
+-rw-r--r--   0 dionysus  (1000) wheel      (998)       69 2023-04-07 16:41:27.000000 pixelsort-cli-0.1.4/setup.py
+drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/
+drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/pixelsort/
+-rw-r--r--   0 dionysus  (1000) wheel      (998)      115 2023-04-07 16:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort/__init__.py
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     2016 2023-04-07 19:32:19.000000 pixelsort-cli-0.1.4/src/pixelsort/__main__.py
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     1470 2023-04-07 16:36:33.000000 pixelsort-cli-0.1.4/src/pixelsort/cli.py
+-rw-r--r--   0 dionysus  (1000) wheel      (998)      231 2023-04-07 16:36:51.000000 pixelsort-cli-0.1.4/src/pixelsort/direction.py
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     4494 2023-04-07 19:31:41.000000 pixelsort-cli-0.1.4/src/pixelsort/image.py
+drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/
+-rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dionysus  (1000) wheel      (998)      431 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dionysus  (1000) wheel      (998)        1 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dionysus  (1000) wheel      (998)       54 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dionysus  (1000) wheel      (998)       44 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/requires.txt
+-rw-r--r--   0 dionysus  (1000) wheel      (998)       10 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/top_level.txt
+drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/test/
+-rw-r--r--   0 dionysus  (1000) wheel      (998)      384 2023-04-07 17:01:38.000000 pixelsort-cli-0.1.4/test/test_image.py
```

### Comparing `pixelsort-cli-0.1.3/LICENSE` & `pixelsort-cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.3/PKG-INFO` & `pixelsort-cli-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
   --invert INVERT       invert the selected area
   --reverse_sorting REVERSE_SORTING
                         reverse the sorting direction
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 0.7 --invert True --output out.png
+pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

### Comparing `pixelsort-cli-0.1.3/README.md` & `pixelsort-cli-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   --invert INVERT       invert the selected area
   --reverse_sorting REVERSE_SORTING
                         reverse the sorting direction
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 0.7 --invert True --output out.png
+pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

### Comparing `pixelsort-cli-0.1.3/pyproject.toml` & `pixelsort-cli-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelsort-cli"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name = "Ferdinand Theil", email = "f.p.theil@proton.me"},
 ]
 description = "A Python CLI tool for sorting pixels in images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pixelsort-cli-0.1.3/src/pixelsort/__main__.py` & `pixelsort-cli-0.1.4/src/pixelsort/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     image_data: np.ndarray = cv2.imread(str(image_path))
 
     # process image
     image.process_image(image_data, direction, threshold, invert, reversed_direction)
 
     # save image
     if output_path is None:
-        return
+        # show image if no output path is given
+        image.show_image(image_data)
+
     # Parse output path
     output_path = pathlib.Path(output_path)
     if not cli.valid_write_image_path(output_path):
         sys.exit(-1)
 
     cv2.imwrite(str(output_path), image_data)
```

### Comparing `pixelsort-cli-0.1.3/src/pixelsort/cli.py` & `pixelsort-cli-0.1.4/src/pixelsort/cli.py`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.3/src/pixelsort/image.py` & `pixelsort-cli-0.1.4/src/pixelsort/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,18 @@
         reverse_sort (bool): True if the pixels should be sorted in reverse
     """
     is_sort_reverse = direction in [Direction.UP, Direction.LEFT]
     is_vertical = direction in [Direction.UP, Direction.DOWN]
 
     print(f"Processing image with {direction.name} direction, threshold={threshold}, invert={invert}, reverse_sort={reverse_sort}")
 
+    contrast: np.ndarray = create_contrast_mask(image, threshold)
     if invert:  # invert image if sorting in reverse
-        threshold = 1 - threshold
-        contrast: np.ndarray = create_contrast_mask(image, threshold)
         contrast: np.ndarray = cv2.bitwise_not(contrast)
-    else:
-        contrast: np.ndarray = create_contrast_mask(image, threshold)
     # show_image(contrast)
-
     # flip sort direction if sorting in reverse
     if reverse_sort:
         is_sort_reverse = not is_sort_reverse
 
     if is_vertical:
         for x in range(image.shape[1]):
             column_contrast = contrast[:, x]
@@ -41,15 +37,14 @@
     else:
         for y in range(image.shape[0]):
             row_contrast = contrast[y, :]
             row_image = image[y, :]
             process_slice(row_contrast, row_image, is_sort_reverse)
 
     print("Done")
-    # show_image(image)
 
 
 def process_slice(contrast_slice: np.ndarray, image_slice: np.ndarray, is_sort_reverse: bool) -> None:
     """process a slice of the image
 
     Args:
         contrast_slice (np.ndarray): 1d slice of the contrast mask
@@ -114,15 +109,16 @@
     # sort pixels by luminance
     # luminance = (r * 0.3) + (g * 0.59) + (b * 0.11)
     # no point in sorting if there are less than 2 pixels
     if image.size <= 2*3:  # 2 pixels, 3 channels
         return
 
     # sort by luminance
-    luminance = np.sum(image * [0.3, 0.59, 0.11], axis=-1)
+    # numpy is b g r
+    luminance = np.sum(image * [0.11, 0.59, 0.3], axis=-1)
     index = np.argsort(luminance)
 
     if reverse:
         index = index[::-1]
 
     image[:] = image[index]
```

### Comparing `pixelsort-cli-0.1.3/src/pixelsort_cli.egg-info/PKG-INFO` & `pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,15 @@
   --invert INVERT       invert the selected area
   --reverse_sorting REVERSE_SORTING
                         reverse the sorting direction
   --output OUTPUT       path to output file
 ```
 
 ```bash
-pixelsort  data/mountains.jpg right --threshold 0.7 --invert True --output out.png
+pixelsort  data/mountains.jpg right --threshold 1.2 --invert True --output out.png
 ```
 
 ![example 1](https://raw.githubusercontent.com/Blotz/pixelsort-cli/main/data/example1.png)
 
 ---
 
 ## License
```

