# Comparing `tmp/amarium-0.1.5.tar.gz` & `tmp/amarium-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarium-0.1.5.tar", last modified: Fri Mar 31 13:29:33 2023, max compression
+gzip compressed data, was "amarium-0.1.8.tar", last modified: Fri Apr  7 19:37:36 2023, max compression
```

## Comparing `amarium-0.1.5.tar` & `amarium-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:33.481783 amarium-0.1.5/
--rw-r--r--   0 developer  (1001) developer  (1001)    34475 2023-03-31 13:19:24.000000 amarium-0.1.5/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1001)     3240 2023-03-31 13:29:33.481783 amarium-0.1.5/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     2684 2023-03-31 13:19:24.000000 amarium-0.1.5/README.md
--rw-r--r--   0 developer  (1001) developer  (1001)      671 2023-03-31 13:29:28.000000 amarium-0.1.5/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-03-31 13:29:33.481783 amarium-0.1.5/setup.cfg
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:33.478450 amarium-0.1.5/src/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.5/src/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:33.478450 amarium-0.1.5/src/amarium/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.5/src/amarium/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2528 2023-03-31 13:29:17.000000 amarium-0.1.5/src/amarium/checks.py
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.5/src/amarium/csv_utils.py
--rw-r--r--   0 developer  (1001) developer  (1001)     4608 2023-03-31 13:29:17.000000 amarium-0.1.5/src/amarium/encryption.py
--rw-r--r--   0 developer  (1001) developer  (1001)    10740 2023-03-31 13:29:17.000000 amarium-0.1.5/src/amarium/utils.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:33.481783 amarium-0.1.5/src/amarium.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     3240 2023-03-31 13:29:33.000000 amarium-0.1.5/src/amarium.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      411 2023-03-31 13:29:33.000000 amarium-0.1.5/src/amarium.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-03-31 13:29:33.000000 amarium-0.1.5/src/amarium.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        6 2023-03-31 13:29:33.000000 amarium-0.1.5/src/amarium.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       17 2023-03-31 13:29:33.000000 amarium-0.1.5/src/amarium.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:33.481783 amarium-0.1.5/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)     1992 2023-03-31 13:19:40.000000 amarium-0.1.5/tests/test_checks.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2095 2023-03-31 13:19:40.000000 amarium-0.1.5/tests/test_encryption.py
--rw-r--r--   0 developer  (1001) developer  (1001)     8438 2023-03-31 13:29:13.000000 amarium-0.1.5/tests/test_file_utils.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34475 2023-03-31 13:19:24.000000 amarium-0.1.8/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1001)     3547 2023-04-07 19:37:36.758845 amarium-0.1.8/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     2992 2023-04-07 19:34:55.000000 amarium-0.1.8/README.md
+-rw-r--r--   0 developer  (1001) developer  (1001)      671 2023-04-07 19:37:12.000000 amarium-0.1.8/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-07 19:37:36.758845 amarium-0.1.8/setup.cfg
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/amarium/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2528 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/checks.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-03-31 13:29:17.000000 amarium-0.1.8/src/amarium/csv_utils.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     3431 2023-04-04 20:47:05.000000 amarium-0.1.8/src/amarium/database.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4608 2023-04-07 08:54:09.000000 amarium-0.1.8/src/amarium/encryption.py
+-rw-r--r--   0 developer  (1001) developer  (1001)    10740 2023-04-07 19:32:18.000000 amarium-0.1.8/src/amarium/utils.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/src/amarium.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     3547 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      458 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        6 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       17 2023-04-07 19:37:36.000000 amarium-0.1.8/src/amarium.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-07 19:37:36.758845 amarium-0.1.8/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)     1992 2023-03-31 13:19:40.000000 amarium-0.1.8/tests/test_checks.py
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-04 19:34:02.000000 amarium-0.1.8/tests/test_database.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2095 2023-03-31 13:19:40.000000 amarium-0.1.8/tests/test_encryption.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     8438 2023-04-07 19:32:18.000000 amarium-0.1.8/tests/test_file_utils.py
```

### Comparing `amarium-0.1.5/LICENSE` & `amarium-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amarium-0.1.5/PKG-INFO` & `amarium-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.1.5
+Version: 0.1.8
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,69 +13,80 @@
 License-File: LICENSE
 
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue) 
- 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
+**Table of Content**
 
-# Why 
-We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out. 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Usage](#3-usage)
+- [4. Dev Notes](#4-dev-notes)
+- [5. Stub generation](#5-stub-generation)
+<!-- /TOC -->
 
-# What 
+## 1. Why
 
-Small package with a collection of functions frequently used in handling the filesystem. 
+We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out.
 
-This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why? 
+## 2. What
 
-`Because these functions have to be reliable`
-
-How can you satisfy your craving for perfection with this package? Read the `Dev` section.
+Small package with a collection of functions frequently used in handling the filesystem.
 
+This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why?
 
+`Because these functions have to be reliable`
 
-# Usage 
+How can you satisfy your craving for perfection with this package? Read the `Dev` section.
 
-Please refer to the `tests/` directory for examples of the functions and their usage 
+## 3. Usage
 
+Please refer to the `tests/` directory for examples of the functions and their usage
 
-# Dev Notes
+## 4. Dev Notes
 
 To develop here, we want you to understand that this package is only about creating code of the highest quality.  
 
-Take the download numbers as a reminder for your responsibility. 
+Take the download numbers as a reminder for your responsibility.
 
-For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`. 
+For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`.
 
 Of course, we know it is impossible. To somewhat come close to it, we do:
 
-* No `PEP` violations and checking with linting
-* Automated testing aiming for 100% coverage
-* Usage of CI on the repo and locally!
-* Writing documentation
-* Writing typed code
+- No `PEP` violations and checking with linting
+- Automated testing aiming for 100% coverage
+- Usage of CI on the repo and locally!
+- Writing documentation
+- Writing typed code
 
-Thus, we encourage to use out new package `lia` frequently. 
-Install lia via 
+Thus, we encourage to use out new package `lia` frequently.
+Install lia via
 
 ```bash
 pip install spawn-lia
 ```
+
 `Lia` then helps you to keep your code nice with
+
 ```bash
 lia heal package_name/
 ```
 
-Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you: 
+Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you:
 
 `If you are not having any sense for perfection, this is not a place for you to develop!`
 
+## 5. Stub generation
+
 If you are new to `mypy` and typed Python, please, below are tips on how to get used to it:
 
 Add missing library stubs with `mypy` installed
 
 ```
 stubgen path_to_package
 ```
```

### Comparing `amarium-0.1.5/README.md` & `amarium-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue) 
- 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
+**Table of Content**
 
-# Why 
-We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out. 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Usage](#3-usage)
+- [4. Dev Notes](#4-dev-notes)
+- [5. Stub generation](#5-stub-generation)
+<!-- /TOC -->
 
-# What 
+## 1. Why
 
-Small package with a collection of functions frequently used in handling the filesystem. 
+We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out.
 
-This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why? 
+## 2. What
 
-`Because these functions have to be reliable`
-
-How can you satisfy your craving for perfection with this package? Read the `Dev` section.
+Small package with a collection of functions frequently used in handling the filesystem.
 
+This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why?
 
+`Because these functions have to be reliable`
 
-# Usage 
+How can you satisfy your craving for perfection with this package? Read the `Dev` section.
 
-Please refer to the `tests/` directory for examples of the functions and their usage 
+## 3. Usage
 
+Please refer to the `tests/` directory for examples of the functions and their usage
 
-# Dev Notes
+## 4. Dev Notes
 
 To develop here, we want you to understand that this package is only about creating code of the highest quality.  
 
-Take the download numbers as a reminder for your responsibility. 
+Take the download numbers as a reminder for your responsibility.
 
-For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`. 
+For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`.
 
 Of course, we know it is impossible. To somewhat come close to it, we do:
 
-* No `PEP` violations and checking with linting
-* Automated testing aiming for 100% coverage
-* Usage of CI on the repo and locally!
-* Writing documentation
-* Writing typed code
+- No `PEP` violations and checking with linting
+- Automated testing aiming for 100% coverage
+- Usage of CI on the repo and locally!
+- Writing documentation
+- Writing typed code
 
-Thus, we encourage to use out new package `lia` frequently. 
-Install lia via 
+Thus, we encourage to use out new package `lia` frequently.
+Install lia via
 
 ```bash
 pip install spawn-lia
 ```
+
 `Lia` then helps you to keep your code nice with
+
 ```bash
 lia heal package_name/
 ```
 
-Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you: 
+Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you:
 
 `If you are not having any sense for perfection, this is not a place for you to develop!`
 
+## 5. Stub generation
+
 If you are new to `mypy` and typed Python, please, below are tips on how to get used to it:
 
 Add missing library stubs with `mypy` installed
 
 ```
 stubgen path_to_package
-```
+```
```

### Comparing `amarium-0.1.5/pyproject.toml` & `amarium-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amarium"
-version = "0.1.5"
+version = "0.1.8"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Filesystem handling utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `amarium-0.1.5/src/amarium/checks.py` & `amarium-0.1.8/src/amarium/checks.py`

 * *Files identical despite different names*

### Comparing `amarium-0.1.5/src/amarium/encryption.py` & `amarium-0.1.8/src/amarium/encryption.py`

 * *Files identical despite different names*

### Comparing `amarium-0.1.5/src/amarium/utils.py` & `amarium-0.1.8/src/amarium/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,16 +282,16 @@
     if bool_str == "True":
         bool_str = True
     if bool_str == "False":
         bool_str = False
     return bool_str
 
 
-def attach_slash(raw_string: str) -> str:
-    """The attach_slash function takes a string as input and returns the same
+def append_slash(raw_string: str) -> str:
+    """The append_slash function takes a string as input and returns the same
     string with a slash appended to it. If the input already ends in a slash,
     then no change is made.
 
     :param raw_string:str: Used to Specify the type of data that is being passed into the function.
     :return: A string with a trailing slash.
 
     :doc-author: Julian M. Kleber
```

### Comparing `amarium-0.1.5/src/amarium.egg-info/PKG-INFO` & `amarium-0.1.8/src/amarium.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.1.5
+Version: 0.1.8
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,69 +13,80 @@
 License-File: LICENSE
 
 # Amarium
 
 [![status-badge](https://ci.codeberg.org/api/badges/cap_jmk/amarium/status.svg)](https://ci.codeberg.org/cap_jmk/amarium)
 [![Downloads](https://static.pepy.tech/personalized-badge/amarium?period=total&units=international_system&left_color=orange&right_color=blue&left_text=Downloads)](https://pepy.tech/project/amarium)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue) 
- 
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C-blue)
+[![PyPI - Version](https://img.shields.io/pypi/v/amarium.svg)](https://pypi.org/project/amarium)
 
+**Table of Content**
 
-# Why 
-We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out. 
+<!-- TOC -->
+- [1. Why](#1-why)
+- [2. What](#2-what)
+- [3. Usage](#3-usage)
+- [4. Dev Notes](#4-dev-notes)
+- [5. Stub generation](#5-stub-generation)
+<!-- /TOC -->
 
-# What 
+## 1. Why
 
-Small package with a collection of functions frequently used in handling the filesystem. 
+We found ourselves constantly writing files of some sort, always having to face the same problems and writing the same code to solve these problems. So we decided at some point to seperate the most common function as package out.
 
-This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why? 
+## 2. What
 
-`Because these functions have to be reliable`
-
-How can you satisfy your craving for perfection with this package? Read the `Dev` section.
+Small package with a collection of functions frequently used in handling the filesystem.
 
+This package is really for perfectionists. It is one of the few occasions this bad habit makes sense. `These functions have to be rock-solid!` They are tested, and tested to the bone  - verified over many projects, and evaluated with engineered automated testing. Why?
 
+`Because these functions have to be reliable`
 
-# Usage 
+How can you satisfy your craving for perfection with this package? Read the `Dev` section.
 
-Please refer to the `tests/` directory for examples of the functions and their usage 
+## 3. Usage
 
+Please refer to the `tests/` directory for examples of the functions and their usage
 
-# Dev Notes
+## 4. Dev Notes
 
 To develop here, we want you to understand that this package is only about creating code of the highest quality.  
 
-Take the download numbers as a reminder for your responsibility. 
+Take the download numbers as a reminder for your responsibility.
 
-For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`. 
+For example, in a very early stage we changed the naming in the package and lost users (naturally). Thus here, `no mistakes` are allowed. When we say `no mistakes`, we mean absolutetly `zero`, `nada`.
 
 Of course, we know it is impossible. To somewhat come close to it, we do:
 
-* No `PEP` violations and checking with linting
-* Automated testing aiming for 100% coverage
-* Usage of CI on the repo and locally!
-* Writing documentation
-* Writing typed code
+- No `PEP` violations and checking with linting
+- Automated testing aiming for 100% coverage
+- Usage of CI on the repo and locally!
+- Writing documentation
+- Writing typed code
 
-Thus, we encourage to use out new package `lia` frequently. 
-Install lia via 
+Thus, we encourage to use out new package `lia` frequently.
+Install lia via
 
 ```bash
 pip install spawn-lia
 ```
+
 `Lia` then helps you to keep your code nice with
+
 ```bash
 lia heal package_name/
 ```
 
-Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you: 
+Everytime you write a new function, you should check it locally using `Lia`, to ensure you are not diverging from the quality constraints. Again, we remind you:
 
 `If you are not having any sense for perfection, this is not a place for you to develop!`
 
+## 5. Stub generation
+
 If you are new to `mypy` and typed Python, please, below are tips on how to get used to it:
 
 Add missing library stubs with `mypy` installed
 
 ```
 stubgen path_to_package
 ```
```

### Comparing `amarium-0.1.5/tests/test_checks.py` & `amarium-0.1.8/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `amarium-0.1.5/tests/test_encryption.py` & `amarium-0.1.8/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `amarium-0.1.5/tests/test_file_utils.py` & `amarium-0.1.8/tests/test_file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     prepare_file_name_saving,
     make_date_file_name,
     load_json_from_file,
     convert_str_to_bool,
     make_full_filename,
     save_json_to_file,
     search_subdirs,
-    attach_slash,
+    append_slash,
     delete_file,
     write_tar,
     copy_dir,
 )
 
 from src.amarium.checks import check_make_file_name_suffix, check_make_dir
 
@@ -283,13 +283,13 @@
         date_file_name == time_str
     ), "The time strings do not match, it could be the function is too slow. That means anyways that the system is not suitable for tests."
 
 
 def test_attach_string():
 
     test_string ="test_dir_or_file"
-    test_string_mod = attach_slash(test_string)
+    test_string_mod = append_slash(test_string)
     assert test_string_mod == test_string + "/"
 
     test_string = "test_dir_or_file/"
-    test_string_mod = attach_slash(test_string)
+    test_string_mod = append_slash(test_string)
     assert test_string_mod == test_string
```

