# Comparing `tmp/hapdoc-1.9.4.tar.gz` & `tmp/hapdoc-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapdoc-1.9.4.tar", last modified: Fri Apr  7 16:11:40 2023, max compression
+gzip compressed data, was "hapdoc-1.9.5.tar", last modified: Fri Apr  7 16:24:13 2023, max compression
```

## Comparing `hapdoc-1.9.4.tar` & `hapdoc-1.9.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.467656 hapdoc-1.9.4/
--rw-rw-rw-   0        0        0     1085 2023-02-05 04:11:14.000000 hapdoc-1.9.4/LICENSE
--rw-rw-rw-   0        0        0       33 2023-03-26 12:25:42.000000 hapdoc-1.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3386 2023-04-07 16:11:40.467656 hapdoc-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2023-04-05 05:08:04.000000 hapdoc-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.431823 hapdoc-1.9.4/hapdoc/
--rw-rw-rw-   0        0        0     1552 2023-04-07 03:20:08.000000 hapdoc-1.9.4/hapdoc/__init__.py
--rw-rw-rw-   0        0        0      143 2023-03-24 08:02:32.000000 hapdoc-1.9.4/hapdoc/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.459632 hapdoc-1.9.4/hapdoc/autodocker/
--rw-rw-rw-   0        0        0     3445 2023-04-05 12:30:09.000000 hapdoc-1.9.4/hapdoc/autodocker/__init__.py
--rw-rw-rw-   0        0        0     1802 2023-04-04 15:32:08.000000 hapdoc-1.9.4/hapdoc/autodocker/abc.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.463656 hapdoc-1.9.4/hapdoc/autodocker/filetypes/
--rw-rw-rw-   0        0        0      141 2023-04-04 15:28:59.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-04-04 15:28:21.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/fastapi.py
--rw-rw-rw-   0        0        0     3499 2023-04-05 04:49:11.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/js.py
--rw-rw-rw-   0        0        0     4955 2023-04-02 09:14:56.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/py.py
--rw-rw-rw-   0        0        0    13119 2023-04-07 16:11:06.000000 hapdoc-1.9.4/hapdoc/hapdoc.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.465645 hapdoc-1.9.4/hapdoc/md/
--rw-rw-rw-   0        0        0     3936 2023-04-05 14:12:12.000000 hapdoc-1.9.4/hapdoc/md/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.424741 hapdoc-1.9.4/hapdoc/templates/
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.466645 hapdoc-1.9.4/hapdoc/templates/vitepress/
--rw-rw-rw-   0        0        0    18129 2023-04-07 03:35:17.000000 hapdoc-1.9.4/hapdoc/templates/vitepress/index.html
--rw-rw-rw-   0        0        0     4982 2023-04-05 12:43:48.000000 hapdoc-1.9.4/hapdoc/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.457988 hapdoc-1.9.4/hapdoc.egg-info/
--rw-rw-rw-   0        0        0     3386 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 16:11:40.467656 hapdoc-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1878 2023-04-07 16:11:13.000000 hapdoc-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.124104 hapdoc-1.9.5/
+-rw-rw-rw-   0        0        0     1085 2023-02-05 04:11:14.000000 hapdoc-1.9.5/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-03-26 12:25:42.000000 hapdoc-1.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3386 2023-04-07 16:24:13.124104 hapdoc-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2023-04-05 05:08:04.000000 hapdoc-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.098104 hapdoc-1.9.5/hapdoc/
+-rw-rw-rw-   0        0        0     1552 2023-04-07 03:20:08.000000 hapdoc-1.9.5/hapdoc/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-03-24 08:02:32.000000 hapdoc-1.9.5/hapdoc/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.118105 hapdoc-1.9.5/hapdoc/autodocker/
+-rw-rw-rw-   0        0        0     3445 2023-04-05 12:30:09.000000 hapdoc-1.9.5/hapdoc/autodocker/__init__.py
+-rw-rw-rw-   0        0        0     1802 2023-04-04 15:32:08.000000 hapdoc-1.9.5/hapdoc/autodocker/abc.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.121104 hapdoc-1.9.5/hapdoc/autodocker/filetypes/
+-rw-rw-rw-   0        0        0      141 2023-04-04 15:28:59.000000 hapdoc-1.9.5/hapdoc/autodocker/filetypes/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-04-04 15:28:21.000000 hapdoc-1.9.5/hapdoc/autodocker/filetypes/fastapi.py
+-rw-rw-rw-   0        0        0     3499 2023-04-05 04:49:11.000000 hapdoc-1.9.5/hapdoc/autodocker/filetypes/js.py
+-rw-rw-rw-   0        0        0     4991 2023-04-07 16:22:07.000000 hapdoc-1.9.5/hapdoc/autodocker/filetypes/py.py
+-rw-rw-rw-   0        0        0    13119 2023-04-07 16:11:06.000000 hapdoc-1.9.5/hapdoc/hapdoc.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.122104 hapdoc-1.9.5/hapdoc/md/
+-rw-rw-rw-   0        0        0     3936 2023-04-05 14:12:12.000000 hapdoc-1.9.5/hapdoc/md/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.091109 hapdoc-1.9.5/hapdoc/templates/
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.123103 hapdoc-1.9.5/hapdoc/templates/vitepress/
+-rw-rw-rw-   0        0        0    18129 2023-04-07 03:35:17.000000 hapdoc-1.9.5/hapdoc/templates/vitepress/index.html
+-rw-rw-rw-   0        0        0     4982 2023-04-05 12:43:48.000000 hapdoc-1.9.5/hapdoc/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:24:13.117106 hapdoc-1.9.5/hapdoc.egg-info/
+-rw-rw-rw-   0        0        0     3386 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-07 16:24:13.000000 hapdoc-1.9.5/hapdoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 16:24:13.124104 hapdoc-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2023-04-07 16:23:41.000000 hapdoc-1.9.5/setup.py
```

### Comparing `hapdoc-1.9.4/LICENSE` & `hapdoc-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/PKG-INFO` & `hapdoc-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapdoc
-Version: 1.9.4
+Version: 1.9.5
 Summary: autodoc tool for everything
 Home-page: https://github.com/HapticX/hapdoc
 Author: Ethosa
 Author-email: social.ethosa@gmail.com
 Maintainer: HapticX
 Maintainer-email: hapticx.company@gmail.com
 License: MIT
```

### Comparing `hapdoc-1.9.4/README.md` & `hapdoc-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/__init__.py` & `hapdoc-1.9.5/hapdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/autodocker/__init__.py` & `hapdoc-1.9.5/hapdoc/autodocker/__init__.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/autodocker/abc.py` & `hapdoc-1.9.5/hapdoc/autodocker/abc.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/autodocker/filetypes/fastapi.py` & `hapdoc-1.9.5/hapdoc/autodocker/filetypes/fastapi.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/autodocker/filetypes/js.py` & `hapdoc-1.9.5/hapdoc/autodocker/filetypes/js.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/autodocker/filetypes/py.py` & `hapdoc-1.9.5/hapdoc/autodocker/filetypes/py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 Describes Python file type
 """
-from re import findall, split, sub, MULTILINE
+from re import findall, compile, sub, MULTILINE
 from typing import Iterable
 
 from ..abc import ABCFileType
 
 
 class Py(ABCFileType):
     """
@@ -81,20 +81,20 @@
         :param output: output directory
         :param one_file: True when file flag is True
         :return:
         """
         source, end_path, filename = cls.pre(filepath, output, one_file)
         data = f'# {filename}\n'
 
-        description = findall(r'^"{3}\s*([\s\S]+?)\s*"{3}', source, MULTILINE)
+        description = findall(compile(r'^"{3}\s*([\s\S]+?)\s*"{3}', MULTILINE), source)
         if description:
             data += f'\n{description[0].strip()}'
 
         # Handle classes
-        classes = findall(r'class +([^:]+):\n(\s+)([^\n]+(\n+\2[ \S]*)+)', source)
+        classes = findall(compile(r'^\s*class +([^:]+?):\n(\s+)([^\n]+(\n+\2[ \S]*)+)', MULTILINE), source)
         classes_text = []
         for class_data in classes:
             name = class_data[0]
             doc = findall(r'"{3}\s*([\s\S]+?)"{3}', class_data[2])
             doc = f'{doc[0]}' if doc else ''
             class_text = f'\n### `{name}`\n{doc}'
             # Handle class methods
```

### Comparing `hapdoc-1.9.4/hapdoc/hapdoc.py` & `hapdoc-1.9.5/hapdoc/hapdoc.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/md/__init__.py` & `hapdoc-1.9.5/hapdoc/md/__init__.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/templates/vitepress/index.html` & `hapdoc-1.9.5/hapdoc/templates/vitepress/index.html`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc/utils.py` & `hapdoc-1.9.5/hapdoc/utils.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/hapdoc.egg-info/PKG-INFO` & `hapdoc-1.9.5/hapdoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapdoc
-Version: 1.9.4
+Version: 1.9.5
 Summary: autodoc tool for everything
 Home-page: https://github.com/HapticX/hapdoc
 Author: Ethosa
 Author-email: social.ethosa@gmail.com
 Maintainer: HapticX
 Maintainer-email: hapticx.company@gmail.com
 License: MIT
```

### Comparing `hapdoc-1.9.4/hapdoc.egg-info/SOURCES.txt` & `hapdoc-1.9.5/hapdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.4/setup.py` & `hapdoc-1.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ethosa',
     author_email='social.ethosa@gmail.com',
     maintainer='HapticX',
     maintainer_email='hapticx.company@gmail.com',
     url='https://github.com/HapticX/hapdoc',
-    version='1.9.4',
+    version='1.9.5',
     packages=find_packages(),
     py_modules=['hapdoc'],
     install_requires=['click', 'fastapi', 'uvicorn', 'jinja2'],
     package_data={
         'hapdoc': ['*.html']
     },
     include_package_data=True,
```

