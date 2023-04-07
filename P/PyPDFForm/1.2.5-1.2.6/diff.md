# Comparing `tmp/PyPDFForm-1.2.5.tar.gz` & `tmp/PyPDFForm-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.5.tar", last modified: Fri Apr  7 18:49:55 2023, max compression
+gzip compressed data, was "PyPDFForm-1.2.6.tar", last modified: Fri Apr  7 19:13:04 2023, max compression
```

## Comparing `PyPDFForm-1.2.5.tar` & `PyPDFForm-1.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:13:04.347535 PyPDFForm-1.2.6/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 19:13:04.000000 PyPDFForm-1.2.6/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:13:04.351535 PyPDFForm-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 19:12:54.000000 PyPDFForm-1.2.6/setup.py
```

### Comparing `PyPDFForm-1.2.5/LICENSE` & `PyPDFForm-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PKG-INFO` & `PyPDFForm-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.5
+Version: 1.2.6
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png"></p>
+<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
 </p>
 
@@ -33,15 +33,15 @@
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
 
-![](https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif)
+![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
 A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.5 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.6 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
-       [https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png]
+       [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif) A sample PDF
+(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
 form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
 master/pdf_samples/sample_template.pdf). Download it and try: ```python import
 os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
 os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
 Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
 = os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
 you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
```

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/constants.py` & `PyPDFForm-1.2.6/PyPDFForm/core/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/filler.py` & `PyPDFForm-1.2.6/PyPDFForm/core/filler.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/font.py` & `PyPDFForm-1.2.6/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/image.py` & `PyPDFForm-1.2.6/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/patterns.py` & `PyPDFForm-1.2.6/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/template.py` & `PyPDFForm-1.2.6/PyPDFForm/core/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/utils.py` & `PyPDFForm-1.2.6/PyPDFForm/core/utils.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/core/watermark.py` & `PyPDFForm-1.2.6/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/element.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/template.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/middleware/text.py` & `PyPDFForm-1.2.6/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm/wrapper.py` & `PyPDFForm-1.2.6/PyPDFForm/wrapper.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.2.6/PyPDFForm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.5
+Version: 1.2.6
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png"></p>
+<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
 </p>
 
@@ -33,15 +33,15 @@
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
 
-![](https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif)
+![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
 A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.5 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.6 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
-       [https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png]
+       [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif) A sample PDF
+(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
 form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
 master/pdf_samples/sample_template.pdf). Download it and try: ```python import
 os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
 os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
 Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
 = os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
 you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
```

### Comparing `PyPDFForm-1.2.5/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.2.6/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.5/README.md` & `PyPDFForm-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png"></p>
+<p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
 </p>
 
@@ -20,15 +20,15 @@
 
 ```shell script
 pip install PyPDFForm
 ```
 
 ## Quick Example
 
-![](https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif)
+![](https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif)
 
 A sample PDF form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/master/pdf_samples/sample_template.pdf). Download it and try:
 
 ```python
 import os
 
 from PyPDFForm import PyPDFForm
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-       [https://github.com/chinapandaman/PyPDFForm/blob/master/logo.png]
+       [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
     chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![]
-(https://github.com/chinapandaman/PyPDFForm/blob/master/demo.gif) A sample PDF
+(https://github.com/chinapandaman/PyPDFForm/raw/master/demo.gif) A sample PDF
 form can be found [here](https://github.com/chinapandaman/PyPDFForm/blob/
 master/pdf_samples/sample_template.pdf). Download it and try: ```python import
 os from PyPDFForm import PyPDFForm PATH_TO_DOWNLOADED_SAMPLE_PDF_FORM =
 os.path.join( os.path.expanduser("~/Downloads"), "sample_template.pdf" ) #
 Change this to where you downloaded the sample PDF form PATH_TO_FILLED_PDF_FORM
 = os.path.join( os.path.expanduser("~"), "output.pdf" ) # Change this to where
 you wish to put your filled PDF form with open(PATH_TO_FILLED_PDF_FORM, "wb+")
```

### Comparing `PyPDFForm-1.2.5/setup.py` & `PyPDFForm-1.2.6/setup.py`

 * *Files identical despite different names*

