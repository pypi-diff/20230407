# Comparing `tmp/ipywidgets_gallery-0.11.tar.gz` & `tmp/ipywidgets_gallery-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_gallery-0.11.tar", last modified: Fri Apr  7 19:28:34 2023, max compression
+gzip compressed data, was "ipywidgets_gallery-0.12.tar", last modified: Fri Apr  7 20:25:53 2023, max compression
```

## Comparing `ipywidgets_gallery-0.11.tar` & `ipywidgets_gallery-0.12.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)     1551 2023-04-07 19:10:40.000000 ipywidgets_gallery-0.11/README.md
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/ipywidgets_gallery/
--rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 18:40:35.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/checkbox.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      850 2023-04-07 18:41:52.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/colorpicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      825 2023-04-07 18:42:43.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/datepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1190 2023-04-07 18:43:27.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/dropdown.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      911 2023-04-07 18:42:06.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/filepicker.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1421 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/gallery.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      872 2023-04-07 18:41:31.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/intslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      887 2023-04-07 18:41:17.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/radiobuttons.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1486 2023-04-07 18:43:21.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/rangeslider.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      899 2023-04-07 18:42:58.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/selectmultiple.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      836 2023-04-07 18:42:22.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/textarea.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      823 2023-04-07 18:41:01.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/togglebutton.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      889 2023-04-07 18:43:11.000000 ipywidgets_gallery-0.11/ipywidgets_gallery/togglebuttongroup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/
--rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 19:28:34.000000 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/PKG-INFO
--rw-rw-r--   0 leo       (1000) leo       (1000)      727 2023-04-07 19:28:34.000000 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/SOURCES.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 19:28:34.000000 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/dependency_links.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 19:28:34.000000 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/requires.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)       19 2023-04-07 19:28:34.000000 ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/top_level.txt
--rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.11/pyproject.toml
--rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/setup.cfg
--rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 19:27:35.000000 ipywidgets_gallery-0.11/setup.py
-drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 19:28:34.595335 ipywidgets_gallery-0.11/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)      938 2023-04-07 19:24:56.000000 ipywidgets_gallery-0.11/tests/test_all.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1551 2023-04-07 19:10:40.000000 ipywidgets_gallery-0.12/README.md
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/ipywidgets_gallery/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      559 2023-04-07 18:46:08.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      706 2023-04-07 20:03:27.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/checkbox.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      827 2023-04-07 20:04:02.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/colorpicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      743 2023-04-07 20:04:32.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/datepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      932 2023-04-07 20:05:11.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/dropdown.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      812 2023-04-07 20:06:08.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/filepicker.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      880 2023-04-07 20:02:28.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/intslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      810 2023-04-07 20:07:07.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/radiobuttons.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1299 2023-04-07 20:08:02.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/rangeslider.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      822 2023-04-07 20:08:28.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/selectmultiple.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      776 2023-04-07 20:09:21.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/textarea.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      722 2023-04-07 20:10:44.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/togglebutton.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      811 2023-04-07 20:11:04.000000 ipywidgets_gallery-0.12/ipywidgets_gallery/togglebuttongroup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      693 2023-04-07 20:25:53.000000 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/PKG-INFO
+-rw-rw-r--   0 leo       (1000) leo       (1000)      732 2023-04-07 20:25:53.000000 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)        1 2023-04-07 20:25:53.000000 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       18 2023-04-07 20:25:53.000000 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/requires.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       25 2023-04-07 20:25:53.000000 ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/top_level.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)      468 2023-04-07 19:28:13.000000 ipywidgets_gallery-0.12/pyproject.toml
+-rw-rw-r--   0 leo       (1000) leo       (1000)       17 2023-04-07 18:47:25.000000 ipywidgets_gallery-0.12/requirements.txt
+-rw-rw-r--   0 leo       (1000) leo       (1000)       38 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/setup.cfg
+-rw-rw-r--   0 leo       (1000) leo       (1000)      924 2023-04-07 20:25:49.000000 ipywidgets_gallery-0.12/setup.py
+drwxrwxr-x   0 leo       (1000) leo       (1000)        0 2023-04-07 20:25:53.095977 ipywidgets_gallery-0.12/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2023-04-07 20:16:52.000000 ipywidgets_gallery-0.12/tests/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      991 2023-04-07 20:23:52.000000 ipywidgets_gallery-0.12/tests/test_all.py
```

### Comparing `ipywidgets_gallery-0.11/PKG-INFO` & `ipywidgets_gallery-0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets_gallery
-Version: 0.11
+Version: 0.12
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.11/README.md` & `ipywidgets_gallery-0.12/README.md`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/__init__.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/colorpicker.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/colorpicker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import ipywidgets as widgets
 from IPython.display import display
 
+
 class ColorPickerWithOutput:
-    '''ColorPickerWithOutput: A widget that displays a color picker and an output widget that displays the selected color in hexadecimal format.'''
-    def __init__(self, label, message, global_var_name):
-        self.color_picker = widgets.ColorPicker(description=label)
+    """ColorPickerWithOutput: A widget that displays a color picker and an output widget that displays the selected color in hexadecimal format."""
+
+    def __init__(self, label, message, global_var_name, default="#000000"):
+        self.color_picker = widgets.ColorPicker(
+            description=label, value=default
+        )
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = default
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(message.format(change['new']))
-                global_vars = globals()
-                global_vars[self.global_var_name] = change['new']
+                print(message.format(change["new"]))
+                self.value = change["new"]
 
-        self.color_picker.observe(update_output, names='value')
+        self.color_picker.observe(update_output, names="value")
         display(widgets.VBox([self.color_picker, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/dropdown.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/dropdown.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import ipywidgets as widgets
 from IPython.display import display
 
 
 class DropdownWithOutput:
-    def __init__(self, options, global_var_name):
+    def __init__(self, options, default=None):
         self.options = options
-        self.global_var_name = global_var_name
-        
+        self.value = default or options[0]
+
         # Define the dropdown widget
         self.dropdown = widgets.Dropdown(
-            options=options,
-            value=options[0],
-            description='Select an option:'
+            options=options, value=options[0], description="Select an option:"
         )
 
         # Define the output widget
         self.output = widgets.Output()
 
-        # Define the function to update the global variable
-        def update_global_var(change):
-            global_vars = globals()
-            global_vars[self.global_var_name] = change.new
-
         # Define the function to update the output widget
         def update_output(change):
             with self.output:
                 self.output.clear_output()
                 print(change.new)
+                self.value = change.new
 
         # Link the dropdown, the global variable, and the output
-        self.dropdown.observe(update_global_var, names='value')
-        self.dropdown.observe(update_output, names='value')
+        self.dropdown.observe(update_output, names="value")
 
         # Display the dropdown and the output
         display(self.dropdown)
         display(self.output)
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/filepicker.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/filepicker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import ipywidgets as widgets
 from IPython.display import display
 
+
 class FilePickerWithOutput:
-    '''FilePickerWithOutput: A widget that displays a file picker and an output widget that displays the selected file path.'''
-    def __init__(self, label, message, global_var_name):
+    """FilePickerWithOutput: A widget that displays a file picker and an output widget that displays the selected file path."""
+
+    def __init__(self, label, message='Selected file: "{}"'):
         self.file_picker = widgets.FileUpload(description=label)
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = None
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                if len(change['new']) > 0:
-                    print(message.format(list(change['new'].keys())[0]))
-                    global_vars = globals()
-                    global_vars[self.global_var_name] = list(change['new'].keys())[0]
+                if len(change["new"]) > 0:
+                    self.value = list(change["new"].keys())[0]
+                    print(message.format(self.value))
 
-        self.file_picker.observe(update_output, names='value')
-        display(widgets.VBox([self.file_picker, self.output]))
+        self.file_picker.observe(update_output, names="value")
+        display(widgets.VBox([self.file_picker, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/intslider.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/intslider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 import ipywidgets as widgets
 from IPython.display import display
 
+
 class IntSliderWithOutput:
-    '''IntSliderWithOutput: A widget that displays an integer slider and an output widget that displays the current value of the slider.'''
-    def __init__(self, label, min_value, max_value, message, global_var_name):
-        self.slider = widgets.IntSlider(description=label, min=min_value, max=max_value)
+    """IntSliderWithOutput: A widget that displays an integer slider and an output widget that displays the current value of the slider."""
+
+    def __init__(
+        self,
+        label,
+        min_value,
+        max_value,
+        message,
+        default=None,
+    ):
+        self.slider = widgets.IntSlider(
+            description=label, min=min_value, max=max_value
+        )
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = default or min_value
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(message.format(change['new']))
-                global_vars = globals()
-                global_vars[self.global_var_name] = change['new']
+                print(message.format(change["new"]))
+                self.value = change["new"]
 
-        self.slider.observe(update_output, names='value')
+        self.slider.observe(update_output, names="value")
         display(widgets.VBox([self.slider, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/rangeslider.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/rangeslider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import ipywidgets as widgets
 from IPython.display import display
 
 
 class RangeSliderWithOutput:
-    '''RangeSliderWithOutput: A widget that displays an float slider and an output widget that displays the current value of the slider.'''
-    def __init__(self, min_val, max_val, step, global_var_name):
+    """RangeSliderWithOutput: A widget that displays an float slider and an output widget that displays the current value of the slider."""
+
+    def __init__(self, min_val, max_val, step, default=None):
         self.min_val = min_val
         self.max_val = max_val
         self.step = step
-        self.global_var_name = global_var_name
+        self.value = default or min_val
 
         # Define the RangeSlider widget
         self.slider = widgets.FloatRangeSlider(
             value=[min_val, max_val],
             min=min_val,
             max=max_val,
             step=step,
-            description='Range:'
+            description="Range:",
         )
 
         # Define the output widget
         self.output = widgets.Output()
 
-        # Define the function to update the global variable
-        def update_global_var(change):
-            global_vars = globals()
-            global_vars[self.global_var_name] = change.new
-
         # Define the function to update the output widget
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(f"Selected range: {change.new[0]:.2f} - {change.new[1]:.2f}")
+                print(
+                    f"Selected range: {change.new[0]:.2f} - {change.new[1]:.2f}"
+                )
+                self.value = change.new
 
         # Link the slider, the global variable, and the output
-        self.slider.observe(update_global_var, names='value')
-        self.slider.observe(update_output, names='value')
+        self.slider.observe(update_output, names="value")
 
         # Display the slider and the output
         display(widgets.HBox([self.slider, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/selectmultiple.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/datepicker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import ipywidgets as widgets
 from IPython.display import display
 
-class SelectMultipleWithOutput:
-    '''SelectMultipleWithOutput: A widget that displays a list of options and an output widget that displays the selected options when they are changed.'''
-    def __init__(self, label, options, message, global_var_name):
-        self.select_multiple = widgets.SelectMultiple(description=label, options=options)
+
+class DatePickerWithOutput:
+    """DatePickerWithOutput: A widget that displays a date picker and an output widget that displays the selected date."""
+
+    def __init__(self, label, message, default=None):
+        self.date_picker = widgets.DatePicker(description=label)
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = default
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(message.format(change['new']))
-                global_vars = globals()
-                global_vars[self.global_var_name] = change['new']
+                print(message.format(change["new"]))
+                self.value = str(change["new"])
 
-        self.select_multiple.observe(update_output, names='value')
-        display(widgets.VBox([self.select_multiple, self.output]))
+        self.date_picker.observe(update_output, names="value")
+        display(widgets.VBox([self.date_picker, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/textarea.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/textarea.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import ipywidgets as widgets
 from IPython.display import display
 
+
 class TextAreaWithOutput:
-    '''TextAreaWithOutput: A widget that displays a text area and an output widget that displays the contents of the text area when it is changed.'''
-    def __init__(self, label, message, global_var_name):
+    """TextAreaWithOutput: A widget that displays a text area and an output widget that displays the contents of the text area when it is changed."""
+
+    def __init__(self, label, message="Text Area output: {}", default=""):
         self.text_area = widgets.Textarea(description=label)
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = default
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(message.format(change['new']))
-                global_vars = globals()
-                global_vars[self.global_var_name] = change['new']
+                print(message.format(change["new"]))
+                self.value = change["new"]
 
-        self.text_area.observe(update_output, names='value')
-        display(widgets.VBox([self.text_area, self.output]))
+        self.text_area.observe(update_output, names="value")
+        display(widgets.VBox([self.text_area, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery/togglebuttongroup.py` & `ipywidgets_gallery-0.12/ipywidgets_gallery/togglebuttongroup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import ipywidgets as widgets
 from IPython.display import display
 
 
 class ToggleButtonGroupWithOutput:
-    '''ToggleButtonWithOutput: A widget that displays a toggle button and an output widget that displays a message when the button is toggled.'''
-    def __init__(self, label, options, message, global_var_name):
-        self.toggle_buttons = widgets.ToggleButtons(description=label, options=options)
+    """ToggleButtonWithOutput: A widget that displays a toggle button and an output widget that displays a message when the button is toggled."""
+
+    def __init__(self, label, options, message):
+        self.toggle_buttons = widgets.ToggleButtons(
+            description=label, options=options
+        )
         self.output = widgets.Output()
-        self.global_var_name = global_var_name
+        self.value = None
 
         def update_output(change):
             with self.output:
                 self.output.clear_output()
-                print(message.format(change['new']))
-                global_vars = globals()
-                global_vars[self.global_var_name] = change['new']
+                print(message.format(change["new"]))
+                self.value = change["new"]
 
-        self.toggle_buttons.observe(update_output, names='value')
+        self.toggle_buttons.observe(update_output, names="value")
         display(widgets.VBox([self.toggle_buttons, self.output]))
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/PKG-INFO` & `ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipywidgets-gallery
-Version: 0.11
+Version: 0.12
 Summary: A library of interactive widgets for Jupyter notebooks
 Home-page: https://github.com/lsternlicht/ipywidgets_gallery
 Author: Leo Sternlicht
 Author-email: leo@sternlicht.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ipywidgets_gallery-0.11/ipywidgets_gallery.egg-info/SOURCES.txt` & `ipywidgets_gallery-0.12/ipywidgets_gallery.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 ipywidgets_gallery/__init__.py
 ipywidgets_gallery/checkbox.py
 ipywidgets_gallery/colorpicker.py
 ipywidgets_gallery/datepicker.py
 ipywidgets_gallery/dropdown.py
 ipywidgets_gallery/filepicker.py
-ipywidgets_gallery/gallery.py
 ipywidgets_gallery/intslider.py
 ipywidgets_gallery/radiobuttons.py
 ipywidgets_gallery/rangeslider.py
 ipywidgets_gallery/selectmultiple.py
 ipywidgets_gallery/textarea.py
 ipywidgets_gallery/togglebutton.py
 ipywidgets_gallery/togglebuttongroup.py
 ipywidgets_gallery.egg-info/PKG-INFO
 ipywidgets_gallery.egg-info/SOURCES.txt
 ipywidgets_gallery.egg-info/dependency_links.txt
 ipywidgets_gallery.egg-info/requires.txt
 ipywidgets_gallery.egg-info/top_level.txt
+tests/__init__.py
 tests/test_all.py
```

### Comparing `ipywidgets_gallery-0.11/setup.py` & `ipywidgets_gallery-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ipywidgets_gallery",
-    version="0.11",
+    version="0.12",
     description="A library of interactive widgets for Jupyter notebooks",
     url="https://github.com/lsternlicht/ipywidgets_gallery",
     author="Leo Sternlicht",
     author_email="leo@sternlicht.org",
     license="MIT",
     packages=find_packages(),
     install_requires=requirements,
```

### Comparing `ipywidgets_gallery-0.11/tests/test_all.py` & `ipywidgets_gallery-0.12/tests/test_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # test_ipywidgets_gallery.py
 
 from ipywidgets_gallery import (
     CheckboxWithOutput,
     ColorPickerWithOutput,
     DatePickerWithOutput,
     DropdownWithOutput,
-    FilePickerWithOutput,
-    IntSliderWithOutput,
     RadioButtonsWithOutput,
-    RangeSliderWithOutput,
     SelectMultipleWithOutput,
     TextAreaWithOutput,
-    ToggleButtonGroupWithOutput,
     ToggleButtonWithOutput,
 )
+
 import ipywidgets as widgets
 
 
 def test_checkbox_output():
-    checkbox = CheckboxWithOutput("Label", "Checkbox is {}", "checkbox_value")
+    checkbox = CheckboxWithOutput("Label", "Checkbox is {}", True)
     assert isinstance(checkbox.checkbox, widgets.Checkbox)
+    assert checkbox.value == True
 
 
 def test_colorpicker_output():
-    colorpicker = ColorPickerWithOutput("Label", "Color is {}", "color_value")
+    colorpicker = ColorPickerWithOutput("Label", "Color is {}", "#FFFFFF")
     assert isinstance(colorpicker.color_picker, widgets.ColorPicker)
 
 
 def test_datepicker_output():
-    datepicker = DatePickerWithOutput("Label", "Date is {}", "date_value")
+    datepicker = DatePickerWithOutput("Label", "Date is {}", "11/30/1986")
     assert isinstance(datepicker.date_picker, widgets.DatePicker)
+
+
+def test_dropdown_output():
+    dropdown = DropdownWithOutput(["a", "b", "c"], "a")
+    assert isinstance(dropdown.dropdown, widgets.Dropdown)
```

