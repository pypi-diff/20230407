# Comparing `tmp/phulize-1.0.1.tar.gz` & `tmp/phulize-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phulize-1.0.1.tar", last modified: Fri Apr  7 19:39:25 2023, max compression
+gzip compressed data, was "phulize-1.0.2.tar", last modified: Fri Apr  7 20:04:03 2023, max compression
```

## Comparing `phulize-1.0.1.tar` & `phulize-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 19:39:13.000000 phulize-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 19:39:25.476898 phulize-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-07 19:39:13.000000 phulize-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/phulize/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/bytes_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/folder_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/photo_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/phulize/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/progsettings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:39:25.476898 phulize-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-07 19:39:13.000000 phulize-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.806268 phulize-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 20:03:52.000000 phulize-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 20:04:03.806268 phulize-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-07 20:03:52.000000 phulize-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.802268 phulize-1.0.2/phulize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.806268 phulize-1.0.2/phulize/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.806268 phulize-1.0.2/phulize/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/bytes_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/folder_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/utils/photo_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.806268 phulize-1.0.2/phulize/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 20:03:52.000000 phulize-1.0.2/phulize/version/progsettings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:04:03.802268 phulize-1.0.2/phulize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 20:04:03.000000 phulize-1.0.2/phulize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:04:03.806268 phulize-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-07 20:03:52.000000 phulize-1.0.2/setup.py
```

### Comparing `phulize-1.0.1/LICENSE` & `phulize-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/PKG-INFO` & `phulize-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phulize
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
 Home-page: https://github.com/zaytiri/photos-bulk-resize
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
 Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
 Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
 Classifier: Environment :: Console
```

### Comparing `phulize-1.0.1/README.md` & `phulize-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/app.py` & `phulize-1.0.2/phulize/app.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/output.py` & `phulize-1.0.2/phulize/output.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/resize.py` & `phulize-1.0.2/phulize/resize.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/search.py` & `phulize-1.0.2/phulize/search.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/settings/manager.py` & `phulize-1.0.2/phulize/settings/manager.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/settings/settings.py` & `phulize-1.0.2/phulize/settings/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
                                    metavar="",
                                    to_save=True,
                                    default=[])
 
         self.quality = Argument(name='quality',
                                 abbreviation_name='-q',
                                 full_name='--quality',
-                                help_message='The quality, in percentage, the image should have relative to 100% quality. For instance, '
-                                             'an original image has always 100% quality, if the inserted quality is 50 than the image\'s quality is '
-                                             '50% of the original 100%. Ideal percentage and default value is: between 50-60',
+                                help_message='The quality, in percentage, the image should have relative to 100%% quality. For instance, '
+                                             'an original image has always 100%% quality, if the inserted quality is 50 than the image\'s quality is '
+                                             '50%% of the original 100%%. Ideal percentage and default value is: between 50-60',
                                 metavar="",
                                 to_save=True,
                                 default=50)
 
         self.higher = Argument(name='higher',
                                abbreviation_name='-hi',
                                full_name='--higher',
```

### Comparing `phulize-1.0.1/phulize/utils/bytes_conversion.py` & `phulize-1.0.2/phulize/utils/bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/utils/directory.py` & `phulize-1.0.2/phulize/utils/directory.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/utils/file.py` & `phulize-1.0.2/phulize/utils/file.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/utils/folder_hierarchy.py` & `phulize-1.0.2/phulize/utils/folder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize/utils/photo_file.py` & `phulize-1.0.2/phulize/utils/photo_file.py`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/phulize.egg-info/PKG-INFO` & `phulize-1.0.2/phulize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phulize
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
 Home-page: https://github.com/zaytiri/photos-bulk-resize
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
 Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
 Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
 Classifier: Environment :: Console
```

### Comparing `phulize-1.0.1/phulize.egg-info/SOURCES.txt` & `phulize-1.0.2/phulize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phulize-1.0.1/setup.py` & `phulize-1.0.2/setup.py`

 * *Files identical despite different names*

