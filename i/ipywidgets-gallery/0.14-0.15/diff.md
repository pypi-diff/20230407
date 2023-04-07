# Comparing `tmp/ipywidgets_gallery-0.14.tar.gz` & `tmp/ipywidgets_gallery-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_gallery-0.14.tar", last modified: Fri Apr  7 20:31:25 2023, max compression
+gzip compressed data, was "ipywidgets_gallery-0.15.tar", last modified: Fri Apr  7 20:37:45 2023, max compression
```

## Comparing `ipywidgets_gallery-0.14.tar` & `ipywidgets_gallery-0.15.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)     1551 2023-04-07 19:10:40.000000 ipywidgets_gallery-0.14/README.md
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/ipywidgets_gallery/
--rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      779 2023-04-07 20:29:24.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/checkbox.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 20:04:02.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/colorpicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      743 2023-04-07 20:04:32.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/datepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1058 2023-04-07 20:28:49.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/dropdown.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      812 2023-04-07 20:06:08.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/filepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      880 2023-04-07 20:02:28.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/intslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      810 2023-04-07 20:07:07.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/radiobuttons.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1299 2023-04-07 20:08:02.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/rangeslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      822 2023-04-07 20:08:28.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/selectmultiple.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      776 2023-04-07 20:09:21.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/textarea.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      865 2023-04-07 20:29:47.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/togglebutton.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      811 2023-04-07 20:11:04.000000 ipywidgets_gallery-0.14/ipywidgets_gallery/togglebuttongroup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:31:25.000000 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)      732 2023-04-07 20:31:25.000000 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 20:31:25.000000 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 20:31:25.000000 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/requires.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-04-07 20:31:25.000000 ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/top_level.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.14/pyproject.toml
--rw-rw-r--   0 leo       (1000) leo       (1000)       17 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.14/requirements.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/setup.cfg
--rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 20:30:43.000000 ipywidgets_gallery-0.14/setup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:31:25.726803 ipywidgets_gallery-0.14/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2023-04-07 20:16:52.000000 ipywidgets_gallery-0.14/tests/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      991 2023-04-07 20:23:52.000000 ipywidgets_gallery-0.14/tests/test_all.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1551 2023-04-07 19:10:40.000000 ipywidgets_gallery-0.15/README.md
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/ipywidgets_gallery/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      779 2023-04-07 20:29:24.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/checkbox.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 20:04:02.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/colorpicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      743 2023-04-07 20:04:32.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/datepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1058 2023-04-07 20:28:49.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/dropdown.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      842 2023-04-07 20:36:53.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/filepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      880 2023-04-07 20:02:28.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/intslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      810 2023-04-07 20:07:07.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/radiobuttons.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1299 2023-04-07 20:08:02.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/rangeslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      822 2023-04-07 20:08:28.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/selectmultiple.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      776 2023-04-07 20:09:21.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/textarea.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      865 2023-04-07 20:29:47.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/togglebutton.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      811 2023-04-07 20:11:04.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/togglebuttongroup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)      732 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/requires.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/top_level.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.15/pyproject.toml
+-rw-rw-r--   0 leo       (1000) leo       (1000)       17 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.15/requirements.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/setup.cfg
+-rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 20:37:28.000000 ipywidgets_gallery-0.15/setup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2023-04-07 20:16:52.000000 ipywidgets_gallery-0.15/tests/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      991 2023-04-07 20:23:52.000000 ipywidgets_gallery-0.15/tests/test_all.py
```

### Comparing `ipywidgets_gallery-0.14/PKG-INFO` & `ipywidgets_gallery-0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets_gallery
-Version: 0.14
+Version: 0.15
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.14/README.md` & `ipywidgets_gallery-0.15/README.md`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/__init__.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/checkbox.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/checkbox.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/colorpicker.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/colorpicker.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/datepicker.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/datepicker.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/dropdown.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/dropdown.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/filepicker.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/filepicker.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,12 +10,13 @@
         self.output = widgets.Output()
         self.value = None
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
                 if len(change["new"]) > 0:
-                    self.value = list(change["new"].keys())[0]
-                    print(message.format(self.value))
+                    print(change["new"])
+                    self.value = change["new"]
+                    print(message.format(str(self.value)))
 
         self.file_picker.observe(update_output, names="value")
         display(widgets.VBox([self.file_picker, self.output]))
```

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/intslider.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/intslider.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/radiobuttons.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/radiobuttons.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/rangeslider.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/rangeslider.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/selectmultiple.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/selectmultiple.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/textarea.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/textarea.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/togglebutton.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/togglebutton.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery/togglebuttongroup.py` & `ipywidgets_gallery-0.15/ipywidgets_gallery/togglebuttongroup.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/PKG-INFO` & `ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets-gallery
-Version: 0.14
+Version: 0.15
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.14/ipywidgets_gallery.egg-info/SOURCES.txt` & `ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.14/setup.py` & `ipywidgets_gallery-0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ipywidgets_gallery",
-    version="0.14",
+    version="0.15",
     description="A library of interactive widgets for Jupyter notebooks",
     url="https://github.com/lsternlicht/ipywidgets_gallery",
     author="Leo Sternlicht",
     author_email="leo@sternlicht.org",
     license="MIT",
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `ipywidgets_gallery-0.14/tests/test_all.py` & `ipywidgets_gallery-0.15/tests/test_all.py`

 * *Files identical despite different names*

