# Comparing `tmp/hardbrake-0.0.4.tar.gz` & `tmp/hardbrake-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardbrake-0.0.4.tar", last modified: Fri Apr  7 18:38:22 2023, max compression
+gzip compressed data, was "hardbrake-0.0.5.tar", last modified: Fri Apr  7 19:59:10 2023, max compression
```

## Comparing `hardbrake-0.0.4.tar` & `hardbrake-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.550989 hardbrake-0.0.4/
--rw-r--r--   0 tahsin     (501) staff       (20)     1063 2023-04-05 19:04:02.000000 hardbrake-0.0.4/LICENSE
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:38:22.550858 hardbrake-0.0.4/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      892 2023-04-05 19:04:02.000000 hardbrake-0.0.4/README.md
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.549054 hardbrake-0.0.4/hardbrake.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      351 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       43 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)      211 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/requires.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        4 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:38:22.551031 hardbrake-0.0.4/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      759 2023-04-07 18:38:16.000000 hardbrake-0.0.4/setup.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.550636 hardbrake-0.0.4/src/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 18:33:53.000000 hardbrake-0.0.4/src/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       29 2023-04-07 18:26:58.000000 hardbrake-0.0.4/src/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)      757 2023-04-07 18:26:41.000000 hardbrake-0.0.4/src/app.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1370 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/event.py
--rw-r--r--   0 tahsin     (501) staff       (20)      755 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/file.py
--rw-r--r--   0 tahsin     (501) staff       (20)      931 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/loader.py
--rw-r--r--   0 tahsin     (501) staff       (20)      977 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/manager.py
--rw-r--r--   0 tahsin     (501) staff       (20)      364 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/prompts.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1483 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/utils.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.147484 hardbrake-0.0.5/
+-rw-r--r--   0 tahsin     (501) staff       (20)     1063 2023-04-05 19:04:02.000000 hardbrake-0.0.5/LICENSE
+-rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 19:59:10.147341 hardbrake-0.0.5/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      892 2023-04-05 19:04:02.000000 hardbrake-0.0.5/README.md
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.145304 hardbrake-0.0.5/hardbrake.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 19:59:09.000000 hardbrake-0.0.5/hardbrake.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      351 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 19:59:09.000000 hardbrake-0.0.5/hardbrake.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       43 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)      206 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/requires.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        4 2023-04-07 19:59:10.000000 hardbrake-0.0.5/hardbrake.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 19:59:10.147528 hardbrake-0.0.5/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      744 2023-04-07 19:58:59.000000 hardbrake-0.0.5/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 19:59:10.147033 hardbrake-0.0.5/src/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 18:33:53.000000 hardbrake-0.0.5/src/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       29 2023-04-07 18:26:58.000000 hardbrake-0.0.5/src/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      812 2023-04-07 19:56:15.000000 hardbrake-0.0.5/src/app.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1370 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/event.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      755 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/file.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      931 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/loader.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1017 2023-04-07 19:56:42.000000 hardbrake-0.0.5/src/manager.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      364 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/prompts.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1483 2023-04-05 19:04:02.000000 hardbrake-0.0.5/src/utils.py
```

### Comparing `hardbrake-0.0.4/LICENSE` & `hardbrake-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.4/README.md` & `hardbrake-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.4/setup.py` & `hardbrake-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hardbrake",
-    version="0.0.4",
+    version="0.0.5",
     author="Tahsin",
     author_email="hello@tahsin.us",
     description="A wrapper around HandBrake CLI for encoding multiple files with ease.",
     packages=find_packages(),
     install_requires=[
         "autopep8==2.0.1",
         "markdown-it-py==2.1.0",
@@ -16,15 +16,14 @@
         "pyee==9.0.4",
         "Pygments==2.14.0",
         "ranger-fm==1.9.3",
         "rich==13.3.1",
         "tomli==2.0.1",
         "typing_extensions==4.5.0",
         "wcwidth==0.2.6",
-        "file"
     ],
     entry_points={
         'console_scripts': [
             'hardbrake = src.app:main'
         ]
     }
 )
```

### Comparing `hardbrake-0.0.4/src/app.py` & `hardbrake-0.0.5/src/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rich import traceback
 
-import file
-import prompts
-import manager
-import utils
+import src.file as file
+import src.prompts as prompts
+import src.manager as manager
+import src.utils as utils
 
 traceback.install()
 
 utils.verify_installation("HandBrakeCLI")
 
 categories = utils.get_presets()
 category = prompts.multi_select(choices=list(categories.keys()))
```

### Comparing `hardbrake-0.0.4/src/event.py` & `hardbrake-0.0.5/src/event.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.4/src/file.py` & `hardbrake-0.0.5/src/file.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.4/src/loader.py` & `hardbrake-0.0.5/src/loader.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.4/src/manager.py` & `hardbrake-0.0.5/src/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import event
-import loader
-import utils
+import src.event as event
+import src.loader as loader
+import src.utils as utils
 from rich import print
 from rich.panel import Panel
 from rich.syntax import Syntax
 
 
 def manage(cmds: list[str]):
   loader.loader.start()
```

### Comparing `hardbrake-0.0.4/src/utils.py` & `hardbrake-0.0.5/src/utils.py`

 * *Files identical despite different names*

