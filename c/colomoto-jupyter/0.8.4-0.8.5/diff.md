# Comparing `tmp/colomoto_jupyter-0.8.4.tar.gz` & `tmp/colomoto_jupyter-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colomoto_jupyter-0.8.4.tar", last modified: Wed Jun  8 08:43:59 2022, max compression
+gzip compressed data, was "colomoto_jupyter-0.8.5.tar", last modified: Fri Apr  7 21:52:20 2023, max compression
```

## Comparing `colomoto_jupyter-0.8.4.tar` & `colomoto_jupyter-0.8.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 08:43:59.622727 colomoto_jupyter-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-08 08:43:59.618726 colomoto_jupyter-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/cellcollective.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 08:43:59.618726 colomoto_jupyter-0.8.4/colomoto/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    26247 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/minibn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/modelchecking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/setup_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/temporal_logics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 08:43:59.618726 colomoto_jupyter-0.8.4/colomoto_jupyter/
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    11789 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/jupyter_ext.js
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/sessionfiles.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/widget_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/colomoto_jupyter/wui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 08:43:59.618726 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-08 08:43:59.000000 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-06-08 08:43:59.000000 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 08:43:59.000000 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-08 08:43:59.000000 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-06-08 08:43:59.000000 colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/espresso_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/itstools.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/itstools_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/nusmv.py
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/nusmv_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 08:43:59.622727 colomoto_jupyter-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-08 08:43:46.000000 colomoto_jupyter-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/cellcollective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/minibn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/modelchecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/setup_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/temporal_logics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/jupyter_ext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/sessionfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/widget_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/wui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/espresso_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/itstools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/itstools_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/nusmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/nusmv_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 21:52:13.000000 colomoto_jupyter-0.8.5/setup.py
```

### Comparing `colomoto_jupyter-0.8.4/PKG-INFO` & `colomoto_jupyter-0.8.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: colomoto_jupyter
-Version: 0.8.4
+Version: 0.8.5
 Summary: CoLoMoTo helper functions for Juypter integration
 Home-page: https://github.com/colomoto/colomoto-jupyter
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: LGPL v3+/CeCILL-C
 Keywords: jupyter,computational systems biology
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 
 
 Provides helper functions for integration in the CoLoMoTo Jupyter notebook.
 
 See https://github.com/colomoto/colomoto-jupyter
-
-
```

### Comparing `colomoto_jupyter-0.8.4/README.md` & `colomoto_jupyter-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/cellcollective.py` & `colomoto_jupyter-0.8.5/cellcollective.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto/helpers.py` & `colomoto_jupyter-0.8.5/colomoto/helpers.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto/minibn.py` & `colomoto_jupyter-0.8.5/colomoto/minibn.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,20 +26,33 @@
     jupyter_setup("minibn", label="miniBN")
 
 class NOT(boolean.NOT):
     def __init__(self, *args):
         super().__init__(*args)
         self.operator = "!"
 
+import boolean.boolean as bpy
+
+class _TRUE(bpy._TRUE):
+    def __call__(self, **kw):
+        return self if not kw else True
+
+
+class _FALSE(bpy._FALSE):
+    def __call__(self, **kw):
+        return self if not kw else False
+
 
 class BaseNetwork(dict):
     def __init__(self, data=None, Symbol_class=boolean.Symbol,
             allowed_in_name=('.','_',':','-'), **kwargs):
         super().__init__()
         self.ba = boolean.BooleanAlgebra(NOT_class=NOT,
+            TRUE_class=_TRUE,
+            FALSE_class=_FALSE,
             Symbol_class=Symbol_class,
             allowed_in_token=allowed_in_name)
         if data:
             if isinstance(data, str):
                 if "\n" in data or not os.path.exists(data):
                     self.import_data(data.splitlines())
                 else:
```

### Comparing `colomoto_jupyter-0.8.4/colomoto/modelchecking.py` & `colomoto_jupyter-0.8.5/colomoto/modelchecking.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto/setup_helper.py` & `colomoto_jupyter-0.8.5/colomoto/setup_helper.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto/temporal_logics.py` & `colomoto_jupyter-0.8.5/colomoto/temporal_logics.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto/types.py` & `colomoto_jupyter-0.8.5/colomoto/types.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/__init__.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/formatters.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/formatters.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/io.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/io.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/jupyter_ext.js` & `colomoto_jupyter-0.8.5/colomoto_jupyter/jupyter_ext.js`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/sessionfiles.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/sessionfiles.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/upload.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/upload.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/widget_utils.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/widget_utils.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter/wui.py` & `colomoto_jupyter-0.8.5/colomoto_jupyter/wui.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/PKG-INFO` & `colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: colomoto-jupyter
-Version: 0.8.4
+Version: 0.8.5
 Summary: CoLoMoTo helper functions for Juypter integration
 Home-page: https://github.com/colomoto/colomoto-jupyter
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: LGPL v3+/CeCILL-C
 Keywords: jupyter,computational systems biology
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 
 
 Provides helper functions for integration in the CoLoMoTo Jupyter notebook.
 
 See https://github.com/colomoto/colomoto-jupyter
-
-
```

### Comparing `colomoto_jupyter-0.8.4/colomoto_jupyter.egg-info/SOURCES.txt` & `colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/itstools.py` & `colomoto_jupyter-0.8.5/itstools.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/nusmv.py` & `colomoto_jupyter-0.8.5/nusmv.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.4/setup.py` & `colomoto_jupyter-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf8 -*-
 
 from setuptools import setup, find_packages
 
 NAME = "colomoto_jupyter"
 
 setup(name=NAME,
-    version='0.8.4',
+    version='0.8.5',
     author = "Loïc Paulevé",
     author_email = "loic.pauleve@ens-cachan.org",
     url = "https://github.com/colomoto/colomoto-jupyter",
     description = "CoLoMoTo helper functions for Juypter integration",
     long_description = """
 Provides helper functions for integration in the CoLoMoTo Jupyter notebook.
```

