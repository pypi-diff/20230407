# Comparing `tmp/ipywidgets_gallery-0.15.tar.gz` & `tmp/ipywidgets_gallery-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_gallery-0.15.tar", last modified: Fri Apr  7 20:37:45 2023, max compression
+gzip compressed data, was "ipywidgets_gallery-0.16.tar", last modified: Fri Apr  7 20:44:17 2023, max compression
```

## Comparing `ipywidgets_gallery-0.15.tar` & `ipywidgets_gallery-0.16.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)     1551 2023-04-07 19:10:40.000000 ipywidgets_gallery-0.15/README.md
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/ipywidgets_gallery/
--rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      779 2023-04-07 20:29:24.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/checkbox.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 20:04:02.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/colorpicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      743 2023-04-07 20:04:32.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/datepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1058 2023-04-07 20:28:49.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/dropdown.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      842 2023-04-07 20:36:53.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/filepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      880 2023-04-07 20:02:28.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/intslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      810 2023-04-07 20:07:07.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/radiobuttons.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1299 2023-04-07 20:08:02.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/rangeslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      822 2023-04-07 20:08:28.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/selectmultiple.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      776 2023-04-07 20:09:21.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/textarea.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      865 2023-04-07 20:29:47.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/togglebutton.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      811 2023-04-07 20:11:04.000000 ipywidgets_gallery-0.15/ipywidgets_gallery/togglebuttongroup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)      732 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/requires.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-04-07 20:37:45.000000 ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/top_level.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.15/pyproject.toml
--rw-rw-r--   0 leo       (1000) leo       (1000)       17 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.15/requirements.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/setup.cfg
--rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 20:37:28.000000 ipywidgets_gallery-0.15/setup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:37:45.898898 ipywidgets_gallery-0.15/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2023-04-07 20:16:52.000000 ipywidgets_gallery-0.15/tests/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      991 2023-04-07 20:23:52.000000 ipywidgets_gallery-0.15/tests/test_all.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1883 2023-04-07 20:43:25.000000 ipywidgets_gallery-0.16/README.md
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/ipywidgets_gallery/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      779 2023-04-07 20:29:24.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/checkbox.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 20:04:02.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/colorpicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      743 2023-04-07 20:04:32.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/datepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1058 2023-04-07 20:28:49.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/dropdown.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      842 2023-04-07 20:36:53.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/filepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      880 2023-04-07 20:02:28.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/intslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      810 2023-04-07 20:07:07.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/radiobuttons.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1299 2023-04-07 20:08:02.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/rangeslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      822 2023-04-07 20:08:28.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/selectmultiple.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      776 2023-04-07 20:09:21.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/textarea.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      865 2023-04-07 20:29:47.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/togglebutton.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      811 2023-04-07 20:11:04.000000 ipywidgets_gallery-0.16/ipywidgets_gallery/togglebuttongroup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:44:17.000000 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)      747 2023-04-07 20:44:17.000000 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 20:44:17.000000 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 20:44:17.000000 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/requires.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-04-07 20:44:17.000000 ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/top_level.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.16/pyproject.toml
+-rw-rw-r--   0 leo       (1000) leo       (1000)       17 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.16/requirements.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/setup.cfg
+-rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 20:43:36.000000 ipywidgets_gallery-0.16/setup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:44:17.566328 ipywidgets_gallery-0.16/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2023-04-07 20:16:52.000000 ipywidgets_gallery-0.16/tests/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1102 2023-04-07 20:41:12.000000 ipywidgets_gallery-0.16/tests/test_ipywidgets_gallery.py
```

### Comparing `ipywidgets_gallery-0.15/PKG-INFO` & `ipywidgets_gallery-0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets_gallery
-Version: 0.15
+Version: 0.16
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.15/README.md` & `ipywidgets_gallery-0.16/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -40,13 +40,27 @@
 an output widget that displays the specified message (formatted with the
 selected option) when an option is selected. The global variable named
 `my_global_var` will be set to the selected option when an option is selected.
 
 IPyWidgets Gallery provides a variety of other classes for creating widgets
 with different types of output and global variable assignments. 
 
+## Available widgets
+
+* `CheckboxWithOutput`
+* `ColorPickerWithOutput`
+* `DatePickerWithOutput`
+* `DropdownWithOutput`
+* `FilePickerWithOutput`
+* `IntSliderWithOutput`
+* `RadioButtonsWithOutput`
+* `RangeSliderWithOutput`
+* `SelectMultipleWithOutput`
+* `TextAreaWithOutput`
+* `ToggleButtonWithOutput`
+* `ToggleButtonGroupWithOutput`
 
 
 ## License
 
 IPyWidgets Gallery is released under the MIT License. See the
 [LICENSE](LICENSE) file for details.
```

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/__init__.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/checkbox.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/checkbox.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/colorpicker.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/colorpicker.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/datepicker.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/datepicker.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/dropdown.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/dropdown.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/filepicker.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/filepicker.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/intslider.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/intslider.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/radiobuttons.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/radiobuttons.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/rangeslider.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/rangeslider.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/selectmultiple.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/selectmultiple.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/textarea.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/textarea.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/togglebutton.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/togglebutton.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery/togglebuttongroup.py` & `ipywidgets_gallery-0.16/ipywidgets_gallery/togglebuttongroup.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/PKG-INFO` & `ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets-gallery
-Version: 0.15
+Version: 0.16
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.15/ipywidgets_gallery.egg-info/SOURCES.txt` & `ipywidgets_gallery-0.16/ipywidgets_gallery.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 ipywidgets_gallery/togglebuttongroup.py
 ipywidgets_gallery.egg-info/PKG-INFO
 ipywidgets_gallery.egg-info/SOURCES.txt
 ipywidgets_gallery.egg-info/dependency_links.txt
 ipywidgets_gallery.egg-info/requires.txt
 ipywidgets_gallery.egg-info/top_level.txt
 tests/__init__.py
-tests/test_all.py
+tests/test_ipywidgets_gallery.py
```

### Comparing `ipywidgets_gallery-0.15/setup.py` & `ipywidgets_gallery-0.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ipywidgets_gallery",
-    version="0.15",
+    version="0.16",
     description="A library of interactive widgets for Jupyter notebooks",
     url="https://github.com/lsternlicht/ipywidgets_gallery",
     author="Leo Sternlicht",
     author_email="leo@sternlicht.org",
     license="MIT",
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `ipywidgets_gallery-0.15/tests/test_all.py` & `ipywidgets_gallery-0.16/tests/test_ipywidgets_gallery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # test_ipywidgets_gallery.py
 
 from ipywidgets_gallery import (
     CheckboxWithOutput,
     ColorPickerWithOutput,
     DatePickerWithOutput,
     DropdownWithOutput,
+    FilePickerWithOutput,
+    IntSliderWithOutput,
     RadioButtonsWithOutput,
+    RangeSliderWithOutput,
     SelectMultipleWithOutput,
     TextAreaWithOutput,
     ToggleButtonWithOutput,
+    ToggleButtonGroupWithOutput,
 )
 
 import ipywidgets as widgets
 
 
 def test_checkbox_output():
     checkbox = CheckboxWithOutput("Label", "Checkbox is {}", True)
```

