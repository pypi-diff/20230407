# Comparing `tmp/phulize-1.0.0.tar.gz` & `tmp/phulize-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phulize-1.0.0.tar", last modified: Thu Apr  6 22:21:14 2023, max compression
+gzip compressed data, was "phulize-1.0.1.tar", last modified: Fri Apr  7 19:39:25 2023, max compression
```

## Comparing `phulize-1.0.0.tar` & `phulize-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.634310 phulize-1.0.0/
--rw-rw-rw-   0        0        0     1081 2023-03-25 15:21:37.000000 phulize-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    11541 2023-04-06 22:21:14.631318 phulize-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10719 2023-04-06 22:18:06.000000 phulize-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.554529 phulize-1.0.0/phulize/
--rw-rw-rw-   0        0        0        0 2023-03-25 15:21:37.000000 phulize-1.0.0/phulize/__init__.py
--rw-rw-rw-   0        0        0     1589 2023-04-06 22:06:27.000000 phulize-1.0.0/phulize/app.py
--rw-rw-rw-   0        0        0     3475 2023-04-04 19:47:15.000000 phulize-1.0.0/phulize/output.py
--rw-rw-rw-   0        0        0     1459 2023-04-04 20:58:35.000000 phulize-1.0.0/phulize/resize.py
--rw-rw-rw-   0        0        0     2496 2023-04-04 19:38:23.000000 phulize-1.0.0/phulize/search.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.590426 phulize-1.0.0/phulize/settings/
--rw-rw-rw-   0        0        0        0 2023-03-22 18:35:13.000000 phulize-1.0.0/phulize/settings/__init__.py
--rw-rw-rw-   0        0        0      985 2023-03-25 16:29:46.000000 phulize-1.0.0/phulize/settings/manager.py
--rw-rw-rw-   0        0        0     8488 2023-04-06 21:57:28.000000 phulize-1.0.0/phulize/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.621350 phulize-1.0.0/phulize/utils/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:15:01.000000 phulize-1.0.0/phulize/utils/__init__.py
--rw-rw-rw-   0        0        0      622 2023-04-03 21:17:32.000000 phulize-1.0.0/phulize/utils/bytes_conversion.py
--rw-rw-rw-   0        0        0      937 2023-02-28 09:46:50.000000 phulize-1.0.0/phulize/utils/directory.py
--rw-rw-rw-   0        0        0      688 2023-02-28 09:46:50.000000 phulize-1.0.0/phulize/utils/file.py
--rw-rw-rw-   0        0        0      931 2023-04-03 18:26:36.000000 phulize-1.0.0/phulize/utils/folder_hierarchy.py
--rw-rw-rw-   0        0        0      215 2023-04-04 17:49:26.000000 phulize-1.0.0/phulize/utils/log.py
--rw-rw-rw-   0        0        0     1760 2023-04-04 19:10:55.000000 phulize-1.0.0/phulize/utils/photo_file.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.627328 phulize-1.0.0/phulize/version/
--rw-rw-rw-   0        0        0        0 2023-03-25 15:21:37.000000 phulize-1.0.0/phulize/version/__init__.py
--rw-rw-rw-   0        0        0      293 2023-03-25 15:21:37.000000 phulize-1.0.0/phulize/version/progsettings.py
-drwxrwxrwx   0        0        0        0 2023-04-06 22:21:14.581451 phulize-1.0.0/phulize.egg-info/
--rw-rw-rw-   0        0        0    11541 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 22:21:14.000000 phulize-1.0.0/phulize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 22:21:14.635308 phulize-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1540 2023-04-06 22:16:38.000000 phulize-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 19:39:13.000000 phulize-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 19:39:25.476898 phulize-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-07 19:39:13.000000 phulize-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/phulize/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/bytes_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/folder_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/utils/photo_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.476898 phulize-1.0.1/phulize/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 19:39:13.000000 phulize-1.0.1/phulize/version/progsettings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:39:25.472898 phulize-1.0.1/phulize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 19:39:25.000000 phulize-1.0.1/phulize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:39:25.476898 phulize-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-07 19:39:13.000000 phulize-1.0.1/setup.py
```

### Comparing `phulize-1.0.0/LICENSE` & `phulize-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 zay
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 zay
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `phulize-1.0.0/PKG-INFO` & `phulize-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,270 +1,270 @@
-Metadata-Version: 2.1
-Name: phulize
-Version: 1.0.0
-Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
-Home-page: https://github.com/zaytiri/photos-bulk-resize
-Author: zaytiri
-Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
-Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
-Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
-
-# Photo Resizer
-
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
-recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
-organize each photo again.
-
-All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
-resized correctly.
-
-A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
-higher or below the specified. More details below.
-
-All original photos are copied to a different folder which can be configured, also cloning the existent folder
-hierarchy. If any image fails to resize, this photo will remain in the original folder.
-
-At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
-modified. This safety question can be disabled.
-
-An option to shut down the device is also available as it can be useful to leave the process running for a long time
-without worrying.
-
-When all is finished, an output file will be created with statistics and relevant information, such as:
-
-- list of images resized;
-- display original size and resized size of each image;
-- display all photos' original size and resized size;
-- display how much size was resized between all photos;
-- total number of photos resized, increased, unsuccessful and found;
-- warning if the photo size increased instead of decreased;
-
-### Output file example
-
-```txt
-    ... (hidden)
-
-[2023-04-05 17:44:13.979793]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
-	-The original photo size was: 1.98 MB
-	-The resized photo size is: 2.04 MB
-        [WARNING] Size increased!
-
-[2023-04-05 17:44:14.209180]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
-	-The original photo size was: 699.66 KB
-	-The resized photo size is: 258.03 KB
-
-
-[2023-04-05 17:44:14.211177]
-Final Statistics:
-	Size of all original photos: 9.29 MB
-	Size of all resized photos: 4.67 MB
-	Space in disk saved: 4.63 MB
-
-	- Total number of photos with reduced size: 6
-	- Total number of photos with increased size: 1
-	- Total number of photos unsuccessfully reduced: 0
-	- Total number of photos found: 7
-```
-
-### Folder example
-
-The original folder full of images to be resized:
-![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
-
-Content of original folder before resize with pictures' original size:
-![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
-
-Both the original folder and the folder created after all is finished, which contains all original images:
-![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
-
-Display of both folders containing exactly the same hierarchy:
-![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
-
-Content of original folder after resize with pictures' reduced size at 55% quality and the output file:
-![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                              |
-|:-------------------------------------------------------------------------------------|
-| resize photos in bulk conserving folder hierarchy                                    |
-| resize photos depending on specific extension                                        |
-| resize photos recursively  within folders                                            |
-| checking of invalid or corrupted photos                                              |
-| filter photos to resize depending on their size                                      |
-| all original photos are preserved in another folder in case of something going wrong |
-| creation of a final output file containing relevant information about the process    |
-| existence of a safety question                                                       |
-| option of shutting down the device when the resizing process is finished             |
-| configurations provided will be save for easier usage of the command                 |
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```bash
-pip --no-cache-dir install phulize
-```
-
-or,
-
-```bash
-pip3 --no-cache-dir install phulize
-```
-
-## Usage
-
-| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
-|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
-| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
-| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
-| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
-| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
-| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
-| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
-| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
-| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
-| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
-
-<a name="before"></a>
-
-### Before
-- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
-- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
-
-<a name="after"></a>
-
-### After
-- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
-- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
-
-<a name="important"></a>
-
----
-### Important 
-- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
----
-
-Any additional help can be provided if the following command is run:
-```bash
-phulize --help
-```
-
-or,
-```bash
-phulize -h
-```
-Running the previous command is also useful to make sure the package was downloaded correctly.
-
-Example of an initial command, could be:
-```bash
-phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
-```
-This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
-
-Any configuration can also be individually inserted:
-```bash
-phulize -q 50
-```
-```bash
-phulize -f "CONVERTED" 
-```
-
-The following command corresponds to only resizing images that have a size higher than 1MB:
-```bash
-phulize -hi 1048576
-```
-The opposite is also true (resizing images that have a size lower than 1MB):
-```bash
-phulize -b 1048576
-```
-To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
-```bash
-phulize -b 0
-```
-
-The previous configuration can be seen in a file, with the content just like the following:
-```txt
-below: 0
-extensions:
-- .jpg
-- .png
-folder: CONVERTED
-higher: 1048576
-path: C:\Users\<username>\Desktop\example
-quality: 50
-```
-
-
-Usage of boolean arguments:
-```bash
-phulize --safety-question
-phulize --no-safety-question
-```
-```bash
-phulize --shutdown
-phulize --no-shutdown
-```
-
-To run the resizing after all configurations are done:
-```
-phulize --run
-```
-
-<a name="support"></a>
-
-## Support
-
-If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
-Currently maintaining it.
+Metadata-Version: 2.1
+Name: phulize
+Version: 1.0.1
+Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
+Home-page: https://github.com/zaytiri/photos-bulk-resize
+Author: zaytiri
+Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
+Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
+Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
+
+# Photo Resizer
+
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
+recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
+organize each photo again.
+
+All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
+resized correctly.
+
+A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
+higher or below the specified. More details below.
+
+All original photos are copied to a different folder which can be configured, also cloning the existent folder
+hierarchy. If any image fails to resize, this photo will remain in the original folder.
+
+At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
+modified. This safety question can be disabled.
+
+An option to shut down the device is also available as it can be useful to leave the process running for a long time
+without worrying.
+
+When all is finished, an output file will be created with statistics and relevant information, such as:
+
+- list of images resized;
+- display original size and resized size of each image;
+- display all photos' original size and resized size;
+- display how much size was resized between all photos;
+- total number of photos resized, increased, unsuccessful and found;
+- warning if the photo size increased instead of decreased;
+
+### Output file example
+
+```txt
+    ... (hidden)
+
+[2023-04-05 17:44:13.979793]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
+	-The original photo size was: 1.98 MB
+	-The resized photo size is: 2.04 MB
+        [WARNING] Size increased!
+
+[2023-04-05 17:44:14.209180]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
+	-The original photo size was: 699.66 KB
+	-The resized photo size is: 258.03 KB
+
+
+[2023-04-05 17:44:14.211177]
+Final Statistics:
+	Size of all original photos: 9.29 MB
+	Size of all resized photos: 4.67 MB
+	Space in disk saved: 4.63 MB
+
+	- Total number of photos with reduced size: 6
+	- Total number of photos with increased size: 1
+	- Total number of photos unsuccessfully reduced: 0
+	- Total number of photos found: 7
+```
+
+### Folder example
+
+The original folder full of images to be resized:<br>
+![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
+
+Content of original folder before resize with pictures' original size:<br>
+![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
+
+Both the original folder and the folder created after all is finished, which contains all original images:<br>
+![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
+
+Display of both folders containing exactly the same hierarchy:<br>
+![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
+
+Content of original folder after resize with pictures' reduced size at 55% quality and the output file:<br>
+![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                              |
+|:-------------------------------------------------------------------------------------|
+| resize photos in bulk conserving folder hierarchy                                    |
+| resize photos depending on specific extension                                        |
+| resize photos recursively  within folders                                            |
+| checking of invalid or corrupted photos                                              |
+| filter photos to resize depending on their size                                      |
+| all original photos are preserved in another folder in case of something going wrong |
+| creation of a final output file containing relevant information about the process    |
+| existence of a safety question                                                       |
+| option of shutting down the device when the resizing process is finished             |
+| configurations provided will be save for easier usage of the command                 |
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```bash
+pip --no-cache-dir install phulize
+```
+
+or,
+
+```bash
+pip3 --no-cache-dir install phulize
+```
+
+## Usage
+
+| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
+|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
+| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
+| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
+| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
+| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
+| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
+| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
+| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
+| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
+| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
+
+<a name="before"></a>
+
+### Before
+- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
+- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
+
+<a name="after"></a>
+
+### After
+- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
+- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
+
+<a name="important"></a>
+
+---
+### Important 
+- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
+---
+
+Any additional help can be provided if the following command is run:
+```bash
+phulize --help
+```
+
+or,
+```bash
+phulize -h
+```
+Running the previous command is also useful to make sure the package was downloaded correctly.
+
+Example of an initial command, could be:
+```bash
+phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
+```
+This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
+
+Any configuration can also be individually inserted:
+```bash
+phulize -q 50
+```
+```bash
+phulize -f "CONVERTED" 
+```
+
+The following command corresponds to only resizing images that have a size higher than 1MB:
+```bash
+phulize -hi 1048576
+```
+The opposite is also true (resizing images that have a size lower than 1MB):
+```bash
+phulize -b 1048576
+```
+To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
+```bash
+phulize -b 0
+```
+
+The previous configuration can be seen in a file, with the content just like the following:
+```txt
+below: 0
+extensions:
+- .jpg
+- .png
+folder: CONVERTED
+higher: 1048576
+path: C:\Users\<username>\Desktop\example
+quality: 50
+```
+
+
+Usage of boolean arguments:
+```bash
+phulize --safety-question
+phulize --no-safety-question
+```
+```bash
+phulize --shutdown
+phulize --no-shutdown
+```
+
+To run the resizing after all configurations are done:
+```
+phulize --run
+```
+
+<a name="support"></a>
+
+## Support
+
+If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
+Currently maintaining it.
```

### Comparing `phulize-1.0.0/README.md` & `phulize-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
-
-# Photo Resizer
-
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
-recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
-organize each photo again.
-
-All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
-resized correctly.
-
-A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
-higher or below the specified. More details below.
-
-All original photos are copied to a different folder which can be configured, also cloning the existent folder
-hierarchy. If any image fails to resize, this photo will remain in the original folder.
-
-At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
-modified. This safety question can be disabled.
-
-An option to shut down the device is also available as it can be useful to leave the process running for a long time
-without worrying.
-
-When all is finished, an output file will be created with statistics and relevant information, such as:
-
-- list of images resized;
-- display original size and resized size of each image;
-- display all photos' original size and resized size;
-- display how much size was resized between all photos;
-- total number of photos resized, increased, unsuccessful and found;
-- warning if the photo size increased instead of decreased;
-
-### Output file example
-
-```txt
-    ... (hidden)
-
-[2023-04-05 17:44:13.979793]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
-	-The original photo size was: 1.98 MB
-	-The resized photo size is: 2.04 MB
-        [WARNING] Size increased!
-
-[2023-04-05 17:44:14.209180]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
-	-The original photo size was: 699.66 KB
-	-The resized photo size is: 258.03 KB
-
-
-[2023-04-05 17:44:14.211177]
-Final Statistics:
-	Size of all original photos: 9.29 MB
-	Size of all resized photos: 4.67 MB
-	Space in disk saved: 4.63 MB
-
-	- Total number of photos with reduced size: 6
-	- Total number of photos with increased size: 1
-	- Total number of photos unsuccessfully reduced: 0
-	- Total number of photos found: 7
-```
-
-### Folder example
-
-The original folder full of images to be resized:
-![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
-
-Content of original folder before resize with pictures' original size:
-![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
-
-Both the original folder and the folder created after all is finished, which contains all original images:
-![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
-
-Display of both folders containing exactly the same hierarchy:
-![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
-
-Content of original folder after resize with pictures' reduced size at 55% quality and the output file:
-![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                              |
-|:-------------------------------------------------------------------------------------|
-| resize photos in bulk conserving folder hierarchy                                    |
-| resize photos depending on specific extension                                        |
-| resize photos recursively  within folders                                            |
-| checking of invalid or corrupted photos                                              |
-| filter photos to resize depending on their size                                      |
-| all original photos are preserved in another folder in case of something going wrong |
-| creation of a final output file containing relevant information about the process    |
-| existence of a safety question                                                       |
-| option of shutting down the device when the resizing process is finished             |
-| configurations provided will be save for easier usage of the command                 |
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```bash
-pip --no-cache-dir install phulize
-```
-
-or,
-
-```bash
-pip3 --no-cache-dir install phulize
-```
-
-## Usage
-
-| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
-|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
-| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
-| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
-| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
-| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
-| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
-| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
-| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
-| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
-| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
-
-<a name="before"></a>
-
-### Before
-- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
-- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
-
-<a name="after"></a>
-
-### After
-- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
-- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
-
-<a name="important"></a>
-
----
-### Important 
-- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
----
-
-Any additional help can be provided if the following command is run:
-```bash
-phulize --help
-```
-
-or,
-```bash
-phulize -h
-```
-Running the previous command is also useful to make sure the package was downloaded correctly.
-
-Example of an initial command, could be:
-```bash
-phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
-```
-This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
-
-Any configuration can also be individually inserted:
-```bash
-phulize -q 50
-```
-```bash
-phulize -f "CONVERTED" 
-```
-
-The following command corresponds to only resizing images that have a size higher than 1MB:
-```bash
-phulize -hi 1048576
-```
-The opposite is also true (resizing images that have a size lower than 1MB):
-```bash
-phulize -b 1048576
-```
-To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
-```bash
-phulize -b 0
-```
-
-The previous configuration can be seen in a file, with the content just like the following:
-```txt
-below: 0
-extensions:
-- .jpg
-- .png
-folder: CONVERTED
-higher: 1048576
-path: C:\Users\<username>\Desktop\example
-quality: 50
-```
-
-
-Usage of boolean arguments:
-```bash
-phulize --safety-question
-phulize --no-safety-question
-```
-```bash
-phulize --shutdown
-phulize --no-shutdown
-```
-
-To run the resizing after all configurations are done:
-```
-phulize --run
-```
-
-<a name="support"></a>
-
-## Support
-
-If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
+[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
+
+# Photo Resizer
+
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
+recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
+organize each photo again.
+
+All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
+resized correctly.
+
+A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
+higher or below the specified. More details below.
+
+All original photos are copied to a different folder which can be configured, also cloning the existent folder
+hierarchy. If any image fails to resize, this photo will remain in the original folder.
+
+At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
+modified. This safety question can be disabled.
+
+An option to shut down the device is also available as it can be useful to leave the process running for a long time
+without worrying.
+
+When all is finished, an output file will be created with statistics and relevant information, such as:
+
+- list of images resized;
+- display original size and resized size of each image;
+- display all photos' original size and resized size;
+- display how much size was resized between all photos;
+- total number of photos resized, increased, unsuccessful and found;
+- warning if the photo size increased instead of decreased;
+
+### Output file example
+
+```txt
+    ... (hidden)
+
+[2023-04-05 17:44:13.979793]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
+	-The original photo size was: 1.98 MB
+	-The resized photo size is: 2.04 MB
+        [WARNING] Size increased!
+
+[2023-04-05 17:44:14.209180]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
+	-The original photo size was: 699.66 KB
+	-The resized photo size is: 258.03 KB
+
+
+[2023-04-05 17:44:14.211177]
+Final Statistics:
+	Size of all original photos: 9.29 MB
+	Size of all resized photos: 4.67 MB
+	Space in disk saved: 4.63 MB
+
+	- Total number of photos with reduced size: 6
+	- Total number of photos with increased size: 1
+	- Total number of photos unsuccessfully reduced: 0
+	- Total number of photos found: 7
+```
+
+### Folder example
+
+The original folder full of images to be resized:<br>
+![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
+
+Content of original folder before resize with pictures' original size:<br>
+![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
+
+Both the original folder and the folder created after all is finished, which contains all original images:<br>
+![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
+
+Display of both folders containing exactly the same hierarchy:<br>
+![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
+
+Content of original folder after resize with pictures' reduced size at 55% quality and the output file:<br>
+![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                              |
+|:-------------------------------------------------------------------------------------|
+| resize photos in bulk conserving folder hierarchy                                    |
+| resize photos depending on specific extension                                        |
+| resize photos recursively  within folders                                            |
+| checking of invalid or corrupted photos                                              |
+| filter photos to resize depending on their size                                      |
+| all original photos are preserved in another folder in case of something going wrong |
+| creation of a final output file containing relevant information about the process    |
+| existence of a safety question                                                       |
+| option of shutting down the device when the resizing process is finished             |
+| configurations provided will be save for easier usage of the command                 |
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```bash
+pip --no-cache-dir install phulize
+```
+
+or,
+
+```bash
+pip3 --no-cache-dir install phulize
+```
+
+## Usage
+
+| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
+|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
+| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
+| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
+| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
+| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
+| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
+| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
+| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
+| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
+| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
+
+<a name="before"></a>
+
+### Before
+- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
+- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
+
+<a name="after"></a>
+
+### After
+- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
+- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
+
+<a name="important"></a>
+
+---
+### Important 
+- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
+---
+
+Any additional help can be provided if the following command is run:
+```bash
+phulize --help
+```
+
+or,
+```bash
+phulize -h
+```
+Running the previous command is also useful to make sure the package was downloaded correctly.
+
+Example of an initial command, could be:
+```bash
+phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
+```
+This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
+
+Any configuration can also be individually inserted:
+```bash
+phulize -q 50
+```
+```bash
+phulize -f "CONVERTED" 
+```
+
+The following command corresponds to only resizing images that have a size higher than 1MB:
+```bash
+phulize -hi 1048576
+```
+The opposite is also true (resizing images that have a size lower than 1MB):
+```bash
+phulize -b 1048576
+```
+To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
+```bash
+phulize -b 0
+```
+
+The previous configuration can be seen in a file, with the content just like the following:
+```txt
+below: 0
+extensions:
+- .jpg
+- .png
+folder: CONVERTED
+higher: 1048576
+path: C:\Users\<username>\Desktop\example
+quality: 50
+```
+
+
+Usage of boolean arguments:
+```bash
+phulize --safety-question
+phulize --no-safety-question
+```
+```bash
+phulize --shutdown
+phulize --no-shutdown
+```
+
+To run the resizing after all configurations are done:
+```
+phulize --run
+```
+
+<a name="support"></a>
+
+## Support
+
+If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
 Currently maintaining it.
```

### Comparing `phulize-1.0.0/phulize/app.py` & `phulize-1.0.1/phulize/app.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import subprocess
-import sys
-
-from phulize.search import Search
-from phulize.settings.manager import Manager
-from phulize.utils.log import throw
-
-
-def main():
-    arguments = Manager().configure_arguments()
-
-    validate_settings(arguments['Settings'])
-
-    epilogue(arguments['Settings'])
-
-    photos = Search(arguments['Settings'])
-
-    if arguments['Settings'].safety_question.value:
-        response = input(
-            'Are you sure you want to continue? \n [Y/n]')
-        if response == 'n' or response == 'N':
-            sys.exit()
-        elif response == 'Y':
-            photos.search()
-            return
-
-    photos.search()
-
-    if arguments['Settings'].shutdown.value:
-        subprocess.run(["shutdown", "-s"])
-
-
-def validate_settings(arguments):
-    if not arguments.run.value:
-        sys.exit()
-
-    if not arguments.path.value:
-        throw('Path is empty.')
-
-    if arguments.shutdown.value:
-        print('The computer will be shutdown when this program is done.\n')
-
-
-def epilogue(arguments):
-    print('All images found with the a ', end="")
-    first = True
-    for extension in arguments.extensions.value:
-        if first:
-            print(extension, end="")
-            first = False
-            continue
-        print(' or ' + extension, end="")
-    print(
-        ' extension are going to be resized and be kept in the "' +
-        arguments.folder.value + '" folder.')
-    print('\n"' + arguments.path.value + '" is going to be modified permanently.\n')
-
-
-if __name__ == '__main__':
-    main()
+import subprocess
+import sys
+
+from phulize.search import Search
+from phulize.settings.manager import Manager
+from phulize.utils.log import throw
+
+
+def main():
+    arguments = Manager().configure_arguments()
+
+    validate_settings(arguments['Settings'])
+
+    epilogue(arguments['Settings'])
+
+    photos = Search(arguments['Settings'])
+
+    if arguments['Settings'].safety_question.value:
+        response = input(
+            'Are you sure you want to continue? \n [Y/n]')
+        if response == 'n' or response == 'N':
+            sys.exit()
+        elif response == 'Y':
+            photos.search()
+            return
+
+    photos.search()
+
+    if arguments['Settings'].shutdown.value:
+        subprocess.run(["shutdown", "-s"])
+
+
+def validate_settings(arguments):
+    if not arguments.run.value:
+        sys.exit()
+
+    if not arguments.path.value:
+        throw('Path is empty.')
+
+    if arguments.shutdown.value:
+        print('The computer will be shutdown when this program is done.\n')
+
+
+def epilogue(arguments):
+    print('All images found with the a ', end="")
+    first = True
+    for extension in arguments.extensions.value:
+        if first:
+            print(extension, end="")
+            first = False
+            continue
+        print(' or ' + extension, end="")
+    print(
+        ' extension are going to be resized and be kept in the "' +
+        arguments.folder.value + '" folder.')
+    print('\n"' + arguments.path.value + '" is going to be modified permanently.\n')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `phulize-1.0.0/phulize/output.py` & `phulize-1.0.1/phulize/output.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from datetime import date, datetime
-
-from phulize.utils.bytes_conversion import set_converted_bytes_with_label
-from phulize.utils.file import File
-
-
-class Output:
-    original_photos_size = 0.0
-    reduced_photos_size = 0.0
-    photos_not_reduced = []
-    number_photos_increased = 0
-    number_photos_reduced = 0
-    photos = []
-    file = None
-
-    def __add_file_information(self, timestamp, photo):
-        self.__add_line('[' + str(timestamp) + ']\nThe following photo was resized: ' + photo.absolute_path)
-
-        self.__set_message_with_size('\t-The original photo size was: ', photo.size)
-        self.__set_message_with_size('\t-The resized photo size is: ', photo.converted_size)
-
-        space_saved = photo.size - photo.converted_size
-        if space_saved < 0:
-            self.number_photos_increased += 1
-            self.__add_line('\t\t[WARNING] Size increased!')
-        else:
-            self.number_photos_reduced += 1
-
-        self.__add_line('\n')
-        self.original_photos_size += photo.size
-        self.reduced_photos_size += photo.converted_size
-
-    def add_file(self, photo):
-        self.photos.append({
-            'timestamp': datetime.utcnow(),
-            'photo': photo
-        })
-
-    def add_unsuccessful_file(self, unsuccessful_file_path):
-        self.photos_not_reduced.append(unsuccessful_file_path)
-
-    def process(self, absolute_path_parent):
-        date_now = '[' + str(date.today().year) + '-' + str(date.today().month) + '-' + str(date.today().day) + ' ' + str(
-            datetime.utcnow().hour) + '-' + str(
-            datetime.utcnow().minute) + '-' + str(datetime.utcnow().second) + ']'
-        self.file = File(absolute_path_parent + '\\output' + date_now + '.txt')
-        self.file.open('a')
-
-        for photo in self.photos:
-            self.__add_file_information(photo['timestamp'], photo['photo'])
-
-        self.__add_line('[' + str(datetime.utcnow()) + ']\nFinal Statistics:')
-        self.__set_message_with_size('\tSize of all original photos: ', self.original_photos_size)
-        self.__set_message_with_size('\tSize of all resized photos: ', self.reduced_photos_size)
-
-        space_saved = self.original_photos_size - self.reduced_photos_size
-        if space_saved > 0:
-            self.__set_message_with_size('\tSpace in disk saved: ', space_saved)
-
-        self.__add_line('\n\t- Total number of photos with reduced size: ' + str(self.number_photos_reduced))
-        self.__add_line('\t- Total number of photos with increased size: ' + str(self.number_photos_increased))
-        self.__add_line('\t- Total number of photos unsuccessfully reduced: ' + str(len(self.photos_not_reduced)))
-        total = self.number_photos_reduced + len(self.photos_not_reduced) + self.number_photos_increased
-        self.__add_line('\t- Total number of photos found: ' + str(total))
-
-        if len(self.photos_not_reduced) != 0:
-            self.__add_line('\n\tThe following photos were not reduced successfully:')
-            for file in self.photos_not_reduced:
-                self.__add_line('\t--> ' + file)
-
-        self.file.close()
-
-    def __set_message_with_size(self, message, size):
-        size_with_label = set_converted_bytes_with_label(size)
-        self.__add_line(message + '%.2f' % size_with_label['size'] + ' ' + size_with_label['label'])
-
-    def __add_line(self, message):
-        self.file.write(message + '\n')
+from datetime import date, datetime
+
+from phulize.utils.bytes_conversion import set_converted_bytes_with_label
+from phulize.utils.file import File
+
+
+class Output:
+    original_photos_size = 0.0
+    reduced_photos_size = 0.0
+    photos_not_reduced = []
+    number_photos_increased = 0
+    number_photos_reduced = 0
+    photos = []
+    file = None
+
+    def __add_file_information(self, timestamp, photo):
+        self.__add_line('[' + str(timestamp) + ']\nThe following photo was resized: ' + photo.absolute_path)
+
+        self.__set_message_with_size('\t-The original photo size was: ', photo.size)
+        self.__set_message_with_size('\t-The resized photo size is: ', photo.converted_size)
+
+        space_saved = photo.size - photo.converted_size
+        if space_saved < 0:
+            self.number_photos_increased += 1
+            self.__add_line('\t\t[WARNING] Size increased!')
+        else:
+            self.number_photos_reduced += 1
+
+        self.__add_line('\n')
+        self.original_photos_size += photo.size
+        self.reduced_photos_size += photo.converted_size
+
+    def add_file(self, photo):
+        self.photos.append({
+            'timestamp': datetime.utcnow(),
+            'photo': photo
+        })
+
+    def add_unsuccessful_file(self, unsuccessful_file_path):
+        self.photos_not_reduced.append(unsuccessful_file_path)
+
+    def process(self, absolute_path_parent):
+        date_now = '[' + str(date.today().year) + '-' + str(date.today().month) + '-' + str(date.today().day) + ' ' + str(
+            datetime.utcnow().hour) + '-' + str(
+            datetime.utcnow().minute) + '-' + str(datetime.utcnow().second) + ']'
+        self.file = File(absolute_path_parent + '\\output' + date_now + '.txt')
+        self.file.open('a')
+
+        for photo in self.photos:
+            self.__add_file_information(photo['timestamp'], photo['photo'])
+
+        self.__add_line('[' + str(datetime.utcnow()) + ']\nFinal Statistics:')
+        self.__set_message_with_size('\tSize of all original photos: ', self.original_photos_size)
+        self.__set_message_with_size('\tSize of all resized photos: ', self.reduced_photos_size)
+
+        space_saved = self.original_photos_size - self.reduced_photos_size
+        if space_saved > 0:
+            self.__set_message_with_size('\tSpace in disk saved: ', space_saved)
+
+        self.__add_line('\n\t- Total number of photos with reduced size: ' + str(self.number_photos_reduced))
+        self.__add_line('\t- Total number of photos with increased size: ' + str(self.number_photos_increased))
+        self.__add_line('\t- Total number of photos unsuccessfully reduced: ' + str(len(self.photos_not_reduced)))
+        total = self.number_photos_reduced + len(self.photos_not_reduced) + self.number_photos_increased
+        self.__add_line('\t- Total number of photos found: ' + str(total))
+
+        if len(self.photos_not_reduced) != 0:
+            self.__add_line('\n\tThe following photos were not reduced successfully:')
+            for file in self.photos_not_reduced:
+                self.__add_line('\t--> ' + file)
+
+        self.file.close()
+
+    def __set_message_with_size(self, message, size):
+        size_with_label = set_converted_bytes_with_label(size)
+        self.__add_line(message + '%.2f' % size_with_label['size'] + ' ' + size_with_label['label'])
+
+    def __add_line(self, message):
+        self.file.write(message + '\n')
```

### Comparing `phulize-1.0.0/phulize/settings/manager.py` & `phulize-1.0.1/phulize/settings/manager.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os
-
-import argparse
-
-from margument.non_repeatable_settings import NonRepeatableSettings
-from margument.options import Options
-from margument.settings_processor import SettingsProcessor
-from phulize.settings.settings import Settings
-from phulize.version.progsettings import get_version
-
-
-class Manager:
-    def __init__(self):
-        self.args = argparse.ArgumentParser()
-        self.args.add_argument('--version', action='version', version='%(prog)s ' + str(get_version()))
-
-    def configure_arguments(self):
-        # manage generic configurations
-        settings = NonRepeatableSettings(path=os.path.join(os.path.dirname(os.path.realpath(__file__)), 'configs.yaml'),
-                                         program_arguments=Settings(),
-                                         options=Options(show_saved=True, save_different=True))
-
-        settings_processor = SettingsProcessor([settings], self.args)
-
-        return settings_processor.run()
+import os
+
+import argparse
+
+from margument.non_repeatable_settings import NonRepeatableSettings
+from margument.options import Options
+from margument.settings_processor import SettingsProcessor
+from phulize.settings.settings import Settings
+from phulize.version.progsettings import get_version
+
+
+class Manager:
+    def __init__(self):
+        self.args = argparse.ArgumentParser()
+        self.args.add_argument('--version', action='version', version='%(prog)s ' + str(get_version()))
+
+    def configure_arguments(self):
+        # manage generic configurations
+        settings = NonRepeatableSettings(path=os.path.join(os.path.dirname(os.path.realpath(__file__)), 'configs.yaml'),
+                                         program_arguments=Settings(),
+                                         options=Options(show_saved=True, save_different=True))
+
+        settings_processor = SettingsProcessor([settings], self.args)
+
+        return settings_processor.run()
```

### Comparing `phulize-1.0.0/phulize/settings/settings.py` & `phulize-1.0.1/phulize/settings/settings.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-import argparse
-
-from margument.argument import Argument
-from margument.arguments import Arguments
-
-from phulize.utils.directory import Directory
-from phulize.utils.log import throw
-
-
-class Settings(Arguments):
-    def __init__(self):
-        self.path = Argument(name='path',
-                             abbreviation_name='-p',
-                             full_name='--path',
-                             help_message='Folder path containing all photos to be modified.',
-                             metavar="",
-                             to_save=True,
-                             default='')
-
-        self.extensions = Argument(name='extensions',
-                                   abbreviation_name='-e',
-                                   full_name='--extensions',
-                                   help_message='All image extensions to search for and modify.',
-                                   metavar="",
-                                   to_save=True,
-                                   default=[])
-
-        self.quality = Argument(name='quality',
-                                abbreviation_name='-q',
-                                full_name='--quality',
-                                help_message='The quality, in percentage, the image should have relative to 100% quality. For instance, '
-                                             'an original image has always 100% quality, if the inserted quality is 50 than the image\'s quality is '
-                                             '50% of the original 100%. Ideal percentage and default value is: between 50-60',
-                                metavar="",
-                                to_save=True,
-                                default=50)
-
-        self.higher = Argument(name='higher',
-                               abbreviation_name='-hi',
-                               full_name='--higher',
-                               help_message='If different than 0 (zero), any images\' size higher than this value, will be resized using defined '
-                                            'configurations. This value is in Bytes, any size value must be convert into Bytes first.',
-                               metavar="",
-                               to_save=True,
-                               default=0)
-
-        self.below = Argument(name='below',
-                              abbreviation_name='-b',
-                              full_name='--below',
-                              help_message='If different than 0 (zero), any images\' size below this value, will be resized using defined '
-                                           'configurations. This value is in Bytes, any size value must be convert into Bytes first.',
-                              metavar="",
-                              to_save=True,
-                              default=0)
-
-        self.folder = Argument(name='folder',
-                               abbreviation_name='-f',
-                               full_name='--folder',
-                               help_message='Folder name or path to be created. All original photos are copied to this folder with the exact '
-                                            'same original folder hierarchy. Default value is \'_ORIGINAL\'. If value equals \'def\', default value '
-                                            'is set.',
-                               metavar="",
-                               to_save=True,
-                               default='_ORIGINAL')
-
-        self.safety_question = Argument(name='safety_question',
-                                        abbreviation_name='',
-                                        full_name='--safety-question',
-                                        help_message='[WARNING: make sure the path is the correct one] Enable/disable safety question '
-                                                     'regarding modifying all files inside path configured: (default is enabled).'
-                                                     'True: --safety-question | False: --no-safety-question',
-                                        metavar="",
-                                        default=True)
-
-        self.shutdown = Argument(name='shutdown',
-                                 abbreviation_name='',
-                                 full_name='--shutdown',
-                                 help_message='Enable/disable if computer will shutdown when the program has ended: (default is disabled)'
-                                              'True: --shutdown | False: --no-shutdown',
-                                 metavar="",
-                                 default=False)
-
-        self.run = Argument(name='run',
-                            abbreviation_name='-r',
-                            full_name='--run',
-                            help_message='If specified, it will start the resizing process with configured settings.',
-                            metavar="",
-                            default=False)
-
-    def add_arguments(self, args_parser):
-        args_parser.add_argument(self.safety_question.full_name,
-                                 action=argparse.BooleanOptionalAction,
-                                 help=self.safety_question.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.shutdown.full_name,
-                                 action=argparse.BooleanOptionalAction,
-                                 help=self.shutdown.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.path.abbreviation_name, self.path.full_name,
-                                 type=str,
-                                 help=self.path.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.quality.abbreviation_name, self.quality.full_name,
-                                 type=int,
-                                 help=self.quality.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.folder.abbreviation_name, self.folder.full_name,
-                                 type=str,
-                                 help=self.folder.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.higher.abbreviation_name, self.higher.full_name,
-                                 type=int,
-                                 help=self.higher.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.below.abbreviation_name, self.below.full_name,
-                                 type=int,
-                                 help=self.below.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.extensions.abbreviation_name, self.extensions.full_name,
-                                 nargs='*',
-                                 help=self.extensions.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.run.abbreviation_name, self.run.full_name,
-                                 action='store_true',
-                                 help=self.run.help_message,
-                                 default=argparse.SUPPRESS)
-
-    def process_arguments(self, settings):
-        self.process_extensions(settings[0].user_arguments)
-        self.validate_path(settings[0].user_arguments)
-        self.validate_folder_name(settings[0].user_arguments)
-
-    def validate_folder_name(self, user_args):
-        if self.folder.name not in user_args:
-            return
-
-        if user_args.folder == 'def':
-            user_args.folder = self.folder.default
-
-    def process_extensions(self, user_args):
-        if self.extensions.name not in user_args:
-            return
-
-        for extension in user_args.extensions:
-            if not extension.startswith('.'):
-                user_args.extensions[user_args.extensions.index(extension)] = '.' + extension
-
-    def validate_path(self, user_args):
-        if self.path.name in user_args:
-            argument_path = Directory(user_args.path)
-            if not argument_path.exists():
-                throw(user_args.path + ' path does not exist.')
+import argparse
+
+from margument.argument import Argument
+from margument.arguments import Arguments
+
+from phulize.utils.directory import Directory
+from phulize.utils.log import throw
+
+
+class Settings(Arguments):
+    def __init__(self):
+        self.path = Argument(name='path',
+                             abbreviation_name='-p',
+                             full_name='--path',
+                             help_message='Folder path containing all photos to be modified.',
+                             metavar="",
+                             to_save=True,
+                             default='')
+
+        self.extensions = Argument(name='extensions',
+                                   abbreviation_name='-e',
+                                   full_name='--extensions',
+                                   help_message='All image extensions to search for and modify.',
+                                   metavar="",
+                                   to_save=True,
+                                   default=[])
+
+        self.quality = Argument(name='quality',
+                                abbreviation_name='-q',
+                                full_name='--quality',
+                                help_message='The quality, in percentage, the image should have relative to 100% quality. For instance, '
+                                             'an original image has always 100% quality, if the inserted quality is 50 than the image\'s quality is '
+                                             '50% of the original 100%. Ideal percentage and default value is: between 50-60',
+                                metavar="",
+                                to_save=True,
+                                default=50)
+
+        self.higher = Argument(name='higher',
+                               abbreviation_name='-hi',
+                               full_name='--higher',
+                               help_message='If different than 0 (zero), any images\' size higher than this value, will be resized using defined '
+                                            'configurations. This value is in Bytes, any size value must be convert into Bytes first.',
+                               metavar="",
+                               to_save=True,
+                               default=0)
+
+        self.below = Argument(name='below',
+                              abbreviation_name='-b',
+                              full_name='--below',
+                              help_message='If different than 0 (zero), any images\' size below this value, will be resized using defined '
+                                           'configurations. This value is in Bytes, any size value must be convert into Bytes first.',
+                              metavar="",
+                              to_save=True,
+                              default=0)
+
+        self.folder = Argument(name='folder',
+                               abbreviation_name='-f',
+                               full_name='--folder',
+                               help_message='Folder name or path to be created. All original photos are copied to this folder with the exact '
+                                            'same original folder hierarchy. Default value is \'_ORIGINAL\'. If value equals \'def\', default value '
+                                            'is set.',
+                               metavar="",
+                               to_save=True,
+                               default='_ORIGINAL')
+
+        self.safety_question = Argument(name='safety_question',
+                                        abbreviation_name='',
+                                        full_name='--safety-question',
+                                        help_message='[WARNING: make sure the path is the correct one] Enable/disable safety question '
+                                                     'regarding modifying all files inside path configured: (default is enabled).'
+                                                     'True: --safety-question | False: --no-safety-question',
+                                        metavar="",
+                                        default=True)
+
+        self.shutdown = Argument(name='shutdown',
+                                 abbreviation_name='',
+                                 full_name='--shutdown',
+                                 help_message='Enable/disable if computer will shutdown when the program has ended: (default is disabled)'
+                                              'True: --shutdown | False: --no-shutdown',
+                                 metavar="",
+                                 default=False)
+
+        self.run = Argument(name='run',
+                            abbreviation_name='-r',
+                            full_name='--run',
+                            help_message='If specified, it will start the resizing process with configured settings.',
+                            metavar="",
+                            default=False)
+
+    def add_arguments(self, args_parser):
+        args_parser.add_argument(self.safety_question.full_name,
+                                 action=argparse.BooleanOptionalAction,
+                                 help=self.safety_question.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.shutdown.full_name,
+                                 action=argparse.BooleanOptionalAction,
+                                 help=self.shutdown.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.path.abbreviation_name, self.path.full_name,
+                                 type=str,
+                                 help=self.path.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.quality.abbreviation_name, self.quality.full_name,
+                                 type=int,
+                                 help=self.quality.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.folder.abbreviation_name, self.folder.full_name,
+                                 type=str,
+                                 help=self.folder.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.higher.abbreviation_name, self.higher.full_name,
+                                 type=int,
+                                 help=self.higher.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.below.abbreviation_name, self.below.full_name,
+                                 type=int,
+                                 help=self.below.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.extensions.abbreviation_name, self.extensions.full_name,
+                                 nargs='*',
+                                 help=self.extensions.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.run.abbreviation_name, self.run.full_name,
+                                 action='store_true',
+                                 help=self.run.help_message,
+                                 default=argparse.SUPPRESS)
+
+    def process_arguments(self, settings):
+        self.process_extensions(settings[0].user_arguments)
+        self.validate_path(settings[0].user_arguments)
+        self.validate_folder_name(settings[0].user_arguments)
+
+    def validate_folder_name(self, user_args):
+        if self.folder.name not in user_args:
+            return
+
+        if user_args.folder == 'def':
+            user_args.folder = self.folder.default
+
+    def process_extensions(self, user_args):
+        if self.extensions.name not in user_args:
+            return
+
+        for extension in user_args.extensions:
+            if not extension.startswith('.'):
+                user_args.extensions[user_args.extensions.index(extension)] = '.' + extension
+
+    def validate_path(self, user_args):
+        if self.path.name in user_args:
+            argument_path = Directory(user_args.path)
+            if not argument_path.exists():
+                throw(user_args.path + ' path does not exist.')
```

### Comparing `phulize-1.0.0/phulize/utils/directory.py` & `phulize-1.0.1/phulize/utils/directory.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import os.path
-from os.path import exists
-
-
-class Directory:
-    current_folder = ''
-    last_folder_path = ''
-
-    def __init__(self, root):
-        self.root = root
-        self.get_current_folder()
-        self.get_last_directory()
-
-    def get_last_directory(self):
-        self.last_folder_path = os.path.dirname(self.root)
-
-    def get_current_folder(self):
-        self.current_folder = os.path.basename(os.path.normpath(self.root))
-
-    def create(self, new_folder):
-        return os.path.join(self.root, new_folder)
-
-    def create_folder(self, new_folder):
-        new_directory = self.create(new_folder)
-        if not os.path.isdir(new_directory):
-            os.mkdir(new_directory)
-
-        return new_directory
-
-    def search_through(self):
-        return os.walk(self.root)
-
-    def remove(self):
-        os.remove(self.root)
-
-    def exists(self):
-        return exists(self.root)
+import os.path
+from os.path import exists
+
+
+class Directory:
+    current_folder = ''
+    last_folder_path = ''
+
+    def __init__(self, root):
+        self.root = root
+        self.get_current_folder()
+        self.get_last_directory()
+
+    def get_last_directory(self):
+        self.last_folder_path = os.path.dirname(self.root)
+
+    def get_current_folder(self):
+        self.current_folder = os.path.basename(os.path.normpath(self.root))
+
+    def create(self, new_folder):
+        return os.path.join(self.root, new_folder)
+
+    def create_folder(self, new_folder):
+        new_directory = self.create(new_folder)
+        if not os.path.isdir(new_directory):
+            os.mkdir(new_directory)
+
+        return new_directory
+
+    def search_through(self):
+        return os.walk(self.root)
+
+    def remove(self):
+        os.remove(self.root)
+
+    def exists(self):
+        return exists(self.root)
```

### Comparing `phulize-1.0.0/phulize/utils/folder_hierarchy.py` & `phulize-1.0.1/phulize/utils/folder_hierarchy.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from phulize.utils.directory import Directory
-
-
-class FolderHierarchy:
-    def __init__(self, root):
-        self.__root = root
-        self.original = None
-        self.clone = None
-
-    def create_parent(self, new_folder):
-        self.original = Directory(self.__root)
-        new_directory = Directory(self.original.last_folder_path)
-        parent_path = new_directory.create_folder(new_folder)
-        self.clone = Directory(parent_path)
-
-    def duplicate(self, file_root):
-        clone_path = self.clone.root
-
-        path_name_list = file_root.split('\\')
-        pass_main_folder = False
-        for folder in path_name_list:
-            if folder == self.original.current_folder:
-                pass_main_folder = True
-
-            if pass_main_folder:
-                clone_path = clone_path + '\\' + folder
-                self.clone.create_folder(clone_path)
-
-        return clone_path
+from phulize.utils.directory import Directory
+
+
+class FolderHierarchy:
+    def __init__(self, root):
+        self.__root = root
+        self.original = None
+        self.clone = None
+
+    def create_parent(self, new_folder):
+        self.original = Directory(self.__root)
+        new_directory = Directory(self.original.last_folder_path)
+        parent_path = new_directory.create_folder(new_folder)
+        self.clone = Directory(parent_path)
+
+    def duplicate(self, file_root):
+        clone_path = self.clone.root
+
+        path_name_list = file_root.split('\\')
+        pass_main_folder = False
+        for folder in path_name_list:
+            if folder == self.original.current_folder:
+                pass_main_folder = True
+
+            if pass_main_folder:
+                clone_path = clone_path + '\\' + folder
+                self.clone.create_folder(clone_path)
+
+        return clone_path
```

### Comparing `phulize-1.0.0/phulize/utils/photo_file.py` & `phulize-1.0.1/phulize/utils/photo_file.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import os.path
-import shutil
-
-from phulize.utils.directory import Directory
-
-
-class PhotoFile:
-    extension = ''
-    absolute_path = ''
-    name_only = ''
-    size = 0
-    converted_size = 0
-
-    def __init__(self, name, root):
-        self.__name = name
-        self.__root = root
-
-        self.__process_extension_file()
-
-    def process(self):
-        self.__process_file_name()
-        self.__process_absolute_path()
-        self.process_size_before()
-
-    def process_size_before(self):
-        self.size = os.path.getsize(self.absolute_path + self.extension)
-
-    def process_size_after(self):
-        self.converted_size = os.path.getsize(self.absolute_path + self.extension)
-
-    def copy_to(self, new_path, remove_original=True):
-        directory = Directory(new_path)
-        original = r'{}'.format(self.absolute_path) + self.extension
-        target = directory.create(self.__name)
-
-        shutil.copyfile(original, target)
-
-        if remove_original:
-            directory = Directory(self.absolute_path + self.extension)
-            directory.remove()
-
-        copied_photo = PhotoFile(self.__name, new_path)
-        copied_photo.process()
-        return copied_photo
-
-    def exists(self):
-        return Directory(self.absolute_path + self.extension).exists()
-
-    def __process_file_name(self):
-        file_name = self.__name.split('.')
-        file_name.pop()
-        self.name_only = '.'.join(file_name)
-
-    def __process_extension_file(self):
-        self.extension = '.' + self.__name.split('.')[len(self.__name.split('.')) - 1]
-
-    def __process_absolute_path(self):
-        directory = Directory(self.__root)
-        self.absolute_path = directory.create(self.name_only)
+import os.path
+import shutil
+
+from phulize.utils.directory import Directory
+
+
+class PhotoFile:
+    extension = ''
+    absolute_path = ''
+    name_only = ''
+    size = 0
+    converted_size = 0
+
+    def __init__(self, name, root):
+        self.__name = name
+        self.__root = root
+
+        self.__process_extension_file()
+
+    def process(self):
+        self.__process_file_name()
+        self.__process_absolute_path()
+        self.process_size_before()
+
+    def process_size_before(self):
+        self.size = os.path.getsize(self.absolute_path + self.extension)
+
+    def process_size_after(self):
+        self.converted_size = os.path.getsize(self.absolute_path + self.extension)
+
+    def copy_to(self, new_path, remove_original=True):
+        directory = Directory(new_path)
+        original = r'{}'.format(self.absolute_path) + self.extension
+        target = directory.create(self.__name)
+
+        shutil.copyfile(original, target)
+
+        if remove_original:
+            directory = Directory(self.absolute_path + self.extension)
+            directory.remove()
+
+        copied_photo = PhotoFile(self.__name, new_path)
+        copied_photo.process()
+        return copied_photo
+
+    def exists(self):
+        return Directory(self.absolute_path + self.extension).exists()
+
+    def __process_file_name(self):
+        file_name = self.__name.split('.')
+        file_name.pop()
+        self.name_only = '.'.join(file_name)
+
+    def __process_extension_file(self):
+        self.extension = '.' + self.__name.split('.')[len(self.__name.split('.')) - 1]
+
+    def __process_absolute_path(self):
+        directory = Directory(self.__root)
+        self.absolute_path = directory.create(self.name_only)
```

### Comparing `phulize-1.0.0/phulize.egg-info/PKG-INFO` & `phulize-1.0.1/phulize.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,270 +1,270 @@
-Metadata-Version: 2.1
-Name: phulize
-Version: 1.0.0
-Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
-Home-page: https://github.com/zaytiri/photos-bulk-resize
-Author: zaytiri
-Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
-Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
-Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
-
-# Photo Resizer
-
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
-recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
-organize each photo again.
-
-All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
-resized correctly.
-
-A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
-higher or below the specified. More details below.
-
-All original photos are copied to a different folder which can be configured, also cloning the existent folder
-hierarchy. If any image fails to resize, this photo will remain in the original folder.
-
-At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
-modified. This safety question can be disabled.
-
-An option to shut down the device is also available as it can be useful to leave the process running for a long time
-without worrying.
-
-When all is finished, an output file will be created with statistics and relevant information, such as:
-
-- list of images resized;
-- display original size and resized size of each image;
-- display all photos' original size and resized size;
-- display how much size was resized between all photos;
-- total number of photos resized, increased, unsuccessful and found;
-- warning if the photo size increased instead of decreased;
-
-### Output file example
-
-```txt
-    ... (hidden)
-
-[2023-04-05 17:44:13.979793]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
-	-The original photo size was: 1.98 MB
-	-The resized photo size is: 2.04 MB
-        [WARNING] Size increased!
-
-[2023-04-05 17:44:14.209180]
-The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
-	-The original photo size was: 699.66 KB
-	-The resized photo size is: 258.03 KB
-
-
-[2023-04-05 17:44:14.211177]
-Final Statistics:
-	Size of all original photos: 9.29 MB
-	Size of all resized photos: 4.67 MB
-	Space in disk saved: 4.63 MB
-
-	- Total number of photos with reduced size: 6
-	- Total number of photos with increased size: 1
-	- Total number of photos unsuccessfully reduced: 0
-	- Total number of photos found: 7
-```
-
-### Folder example
-
-The original folder full of images to be resized:
-![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
-
-Content of original folder before resize with pictures' original size:
-![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
-
-Both the original folder and the folder created after all is finished, which contains all original images:
-![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
-
-Display of both folders containing exactly the same hierarchy:
-![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
-
-Content of original folder after resize with pictures' reduced size at 55% quality and the output file:
-![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                              |
-|:-------------------------------------------------------------------------------------|
-| resize photos in bulk conserving folder hierarchy                                    |
-| resize photos depending on specific extension                                        |
-| resize photos recursively  within folders                                            |
-| checking of invalid or corrupted photos                                              |
-| filter photos to resize depending on their size                                      |
-| all original photos are preserved in another folder in case of something going wrong |
-| creation of a final output file containing relevant information about the process    |
-| existence of a safety question                                                       |
-| option of shutting down the device when the resizing process is finished             |
-| configurations provided will be save for easier usage of the command                 |
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```bash
-pip --no-cache-dir install phulize
-```
-
-or,
-
-```bash
-pip3 --no-cache-dir install phulize
-```
-
-## Usage
-
-| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
-|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
-| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
-| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
-| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
-| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
-| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
-| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
-| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
-| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
-| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
-
-<a name="before"></a>
-
-### Before
-- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
-- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
-
-<a name="after"></a>
-
-### After
-- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
-- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
-
-<a name="important"></a>
-
----
-### Important 
-- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
----
-
-Any additional help can be provided if the following command is run:
-```bash
-phulize --help
-```
-
-or,
-```bash
-phulize -h
-```
-Running the previous command is also useful to make sure the package was downloaded correctly.
-
-Example of an initial command, could be:
-```bash
-phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
-```
-This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
-
-Any configuration can also be individually inserted:
-```bash
-phulize -q 50
-```
-```bash
-phulize -f "CONVERTED" 
-```
-
-The following command corresponds to only resizing images that have a size higher than 1MB:
-```bash
-phulize -hi 1048576
-```
-The opposite is also true (resizing images that have a size lower than 1MB):
-```bash
-phulize -b 1048576
-```
-To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
-```bash
-phulize -b 0
-```
-
-The previous configuration can be seen in a file, with the content just like the following:
-```txt
-below: 0
-extensions:
-- .jpg
-- .png
-folder: CONVERTED
-higher: 1048576
-path: C:\Users\<username>\Desktop\example
-quality: 50
-```
-
-
-Usage of boolean arguments:
-```bash
-phulize --safety-question
-phulize --no-safety-question
-```
-```bash
-phulize --shutdown
-phulize --no-shutdown
-```
-
-To run the resizing after all configurations are done:
-```
-phulize --run
-```
-
-<a name="support"></a>
-
-## Support
-
-If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
-Currently maintaining it.
+Metadata-Version: 2.1
+Name: phulize
+Version: 1.0.1
+Summary: A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.
+Home-page: https://github.com/zaytiri/photos-bulk-resize
+Author: zaytiri
+Project-URL: GitHub, https://github.com/zaytiri/photos-bulk-resize
+Project-URL: Changelog, https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md
+Keywords: photos,image,processing,resize,reduce,cli,folder,hierarchy,bulk
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Downloads](https://pepy.tech/badge/phulize)](https://pepy.tech/project/phulize)
+
+# Photo Resizer
+
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Photo Resizer is a CLI (command-line interface) tool which takes a folder full of photos and resizes each photo
+recursively depending on the extensions chosen. It does this while conserving folder hierarchy without having to
+organize each photo again.
+
+All photos are checked if they are valid or corrupted before the resizing as well as after, to make sure any photos are
+resized correctly.
+
+A filter is also available for searching for photos, meaning it's possible to only resize photos which the size is
+higher or below the specified. More details below.
+
+All original photos are copied to a different folder which can be configured, also cloning the existent folder
+hierarchy. If any image fails to resize, this photo will remain in the original folder.
+
+At the start, a safety question is displayed to make sure the path inserted is the correct one as it will be permanently
+modified. This safety question can be disabled.
+
+An option to shut down the device is also available as it can be useful to leave the process running for a long time
+without worrying.
+
+When all is finished, an output file will be created with statistics and relevant information, such as:
+
+- list of images resized;
+- display original size and resized size of each image;
+- display all photos' original size and resized size;
+- display how much size was resized between all photos;
+- total number of photos resized, increased, unsuccessful and found;
+- warning if the photo size increased instead of decreased;
+
+### Output file example
+
+```txt
+    ... (hidden)
+
+[2023-04-05 17:44:13.979793]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170906941
+	-The original photo size was: 1.98 MB
+	-The resized photo size is: 2.04 MB
+        [WARNING] Size increased!
+
+[2023-04-05 17:44:14.209180]
+The following photo was resized: C:\Users\<username>\Desktop\example\1subfolder\anothersubfolder\1680170908790
+	-The original photo size was: 699.66 KB
+	-The resized photo size is: 258.03 KB
+
+
+[2023-04-05 17:44:14.211177]
+Final Statistics:
+	Size of all original photos: 9.29 MB
+	Size of all resized photos: 4.67 MB
+	Space in disk saved: 4.63 MB
+
+	- Total number of photos with reduced size: 6
+	- Total number of photos with increased size: 1
+	- Total number of photos unsuccessfully reduced: 0
+	- Total number of photos found: 7
+```
+
+### Folder example
+
+The original folder full of images to be resized:<br>
+![1](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/1.png)
+
+Content of original folder before resize with pictures' original size:<br>
+![5](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/5.png)
+
+Both the original folder and the folder created after all is finished, which contains all original images:<br>
+![2](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/2.png)
+
+Display of both folders containing exactly the same hierarchy:<br>
+![3](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/3.png)
+
+Content of original folder after resize with pictures' reduced size at 55% quality and the output file:<br>
+![4](https://github.com/zaytiri/photos-bulk-resize/blob/main/readme_imgs/4.png)
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                              |
+|:-------------------------------------------------------------------------------------|
+| resize photos in bulk conserving folder hierarchy                                    |
+| resize photos depending on specific extension                                        |
+| resize photos recursively  within folders                                            |
+| checking of invalid or corrupted photos                                              |
+| filter photos to resize depending on their size                                      |
+| all original photos are preserved in another folder in case of something going wrong |
+| creation of a final output file containing relevant information about the process    |
+| existence of a safety question                                                       |
+| option of shutting down the device when the resizing process is finished             |
+| configurations provided will be save for easier usage of the command                 |
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```bash
+pip --no-cache-dir install phulize
+```
+
+or,
+
+```bash
+pip3 --no-cache-dir install phulize
+```
+
+## Usage
+
+| Command (shortcut) | Command (full)                         | Required                             | Default value | Description                                                                                                                                      |
+|:-------------------|----------------------------------------|--------------------------------------|---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
+| -r                 | --run                                  | ***REQUIRED*** to start the resizing | ---           | If specified, the resizing will start running using user-defined configurations.                                                                 |
+| -p                 | --path                                 | ***REQUIRED*** to resize photos      | empty         | Absolute path of the folder containing images to be resized.                                                                                     |
+| -e                 | --extensions                           | ***REQUIRED*** to resize photos      | empty         | Insert the extensions of all the images that should be resized.                                                                                  |
+| -q                 | --quality                              | ***OPTIONAL***                       | 55            | The desired quality of the image. An original image has 100% quality, meaning that anything below this value will reduce the size of the images. |
+| -f                 | --folder                               | ***OPTIONAL***                       | _ORIGINAL     | The name or path of the folder which will contain all original photos resized.                                                                   |
+| -hi                | --higher                               | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size higher than this value will be resized.                            |
+| -b                 | --below                                | ***OPTIONAL***                       | 0             | The size in ***Bytes*** of any image that should be resized. Any images' size below this value will be resized.                                  |
+| ---                | --safety-question/--no-safety-question | ***OPTIONAL***                       | True          | Enable or disable the safety question                                                                                                            |
+| ---                | --shutdown/--no-shutdown               | ***OPTIONAL***                       | False         | Enable or disable the shutting down device when process is finished.                                                                             |
+
+<a name="before"></a>
+
+### Before
+- If possible, **make a backup of the folder to be resized**, in case anything goes wrong. This will ensure no data is lost.
+- It's recommended that a trial is made first (with dummy images), to check the best quality to use.
+
+<a name="after"></a>
+
+### After
+- **Make sure to check the output file for any unexpected outcomes**, regarding if it resized correctly, as expected, or not.
+- **Make sure to check the images resized**, to make sure there is no loss. The program itself checks if an image is or becomes corrupted after resizing, but make sure 
+
+<a name="important"></a>
+
+---
+### Important 
+- The quality of the image to be resized, by default, is 50%, meaning all images to resize will have, approximately, 50% less quality than the original image. This can be change, adding the '--quality' argument with a number between 0 and 100.
+---
+
+Any additional help can be provided if the following command is run:
+```bash
+phulize --help
+```
+
+or,
+```bash
+phulize -h
+```
+Running the previous command is also useful to make sure the package was downloaded correctly.
+
+Example of an initial command, could be:
+```bash
+phulize -p "C:\Users\<username>\Desktop\example" -q 60 -e jpg png
+```
+This will configure the path of the folder containing images to resize, the quality those images should have and the extensions to search for and resize.
+
+Any configuration can also be individually inserted:
+```bash
+phulize -q 50
+```
+```bash
+phulize -f "CONVERTED" 
+```
+
+The following command corresponds to only resizing images that have a size higher than 1MB:
+```bash
+phulize -hi 1048576
+```
+The opposite is also true (resizing images that have a size lower than 1MB):
+```bash
+phulize -b 1048576
+```
+To disable the previous filters ('--hi' or '--b'), one can simply set them to 0 (zero):
+```bash
+phulize -b 0
+```
+
+The previous configuration can be seen in a file, with the content just like the following:
+```txt
+below: 0
+extensions:
+- .jpg
+- .png
+folder: CONVERTED
+higher: 1048576
+path: C:\Users\<username>\Desktop\example
+quality: 50
+```
+
+
+Usage of boolean arguments:
+```bash
+phulize --safety-question
+phulize --no-safety-question
+```
+```bash
+phulize --shutdown
+phulize --no-shutdown
+```
+
+To run the resizing after all configurations are done:
+```
+phulize --run
+```
+
+<a name="support"></a>
+
+## Support
+
+If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
+Currently maintaining it.
```

### Comparing `phulize-1.0.0/phulize.egg-info/SOURCES.txt` & `phulize-1.0.1/phulize.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 phulize/utils/bytes_conversion.py
 phulize/utils/directory.py
 phulize/utils/file.py
 phulize/utils/folder_hierarchy.py
 phulize/utils/log.py
 phulize/utils/photo_file.py
 phulize/version/__init__.py
-phulize/version/progsettings.py
+phulize/version/progsettings.py
+phulize/version/progsettings.yaml
```

### Comparing `phulize-1.0.0/setup.py` & `phulize-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from setuptools import setup
-import pathlib
-
-from phulize.version.progsettings import get_version
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-version = get_version()
-
-setup(
-    name="phulize",
-    version=version,
-    description="A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/zaytiri/photos-bulk-resize",
-    project_urls={
-        'GitHub': 'https://github.com/zaytiri/photos-bulk-resize',
-        'Changelog': 'https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md',
-    },
-    author="zaytiri",
-    classifiers=[
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-    ],
-    keywords="photos, image, processing, resize, reduce, cli, folder, hierarchy, bulk",
-    package_data={'phulize': ['progsettings.yaml']},
-    packages=["phulize", "phulize.settings", "phulize.version", "phulize.utils"],
-    python_requires=">=3.10.6",
-    install_requires=[
-        "PyYAML~=6.0",
-        "margument>=1.0.3",
-        "Pillow~=9.5.0",
-    ],
-    entry_points={
-        "console_scripts": [
-            "phulize=phulize:app.main",
-        ],
-    }
-)
+from setuptools import setup
+import pathlib
+
+from phulize.version.progsettings import get_version
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+version = get_version()
+
+setup(
+    name="phulize",
+    version=version,
+    description="A python CLI tool to resize images while conserving folder hierarchy and preserving original ones in a different folder.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/zaytiri/photos-bulk-resize",
+    project_urls={
+        'GitHub': 'https://github.com/zaytiri/photos-bulk-resize',
+        'Changelog': 'https://github.com/zaytiri/photos-bulk-resize/blob/main/CHANGELOG.md',
+    },
+    author="zaytiri",
+    classifiers=[
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+    ],
+    keywords="photos, image, processing, resize, reduce, cli, folder, hierarchy, bulk",
+    package_data={'phulize': ['version/progsettings.yaml']},
+    packages=["phulize", "phulize.settings", "phulize.version", "phulize.utils"],
+    python_requires=">=3.10.6",
+    install_requires=[
+        "PyYAML~=6.0",
+        "margument>=1.0.3",
+        "Pillow~=9.5.0",
+    ],
+    entry_points={
+        "console_scripts": [
+            "phulize=phulize:app.main",
+        ],
+    }
+)
```

