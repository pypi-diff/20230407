# Comparing `tmp/hardbrake-0.0.3.tar.gz` & `tmp/hardbrake-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardbrake-0.0.3.tar", last modified: Fri Apr  7 18:37:08 2023, max compression
+gzip compressed data, was "hardbrake-0.0.4.tar", last modified: Fri Apr  7 18:38:22 2023, max compression
```

## Comparing `hardbrake-0.0.3.tar` & `hardbrake-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:37:08.027220 hardbrake-0.0.3/
--rw-r--r--   0 tahsin     (501) staff       (20)     1063 2023-04-05 19:04:02.000000 hardbrake-0.0.3/LICENSE
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:37:08.027080 hardbrake-0.0.3/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      892 2023-04-05 19:04:02.000000 hardbrake-0.0.3/README.md
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:37:08.024984 hardbrake-0.0.3/hardbrake.egg-info/
--rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:37:07.000000 hardbrake-0.0.3/hardbrake.egg-info/PKG-INFO
--rw-r--r--   0 tahsin     (501) staff       (20)      351 2023-04-07 18:37:08.000000 hardbrake-0.0.3/hardbrake.egg-info/SOURCES.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:37:07.000000 hardbrake-0.0.3/hardbrake.egg-info/dependency_links.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       43 2023-04-07 18:37:07.000000 hardbrake-0.0.3/hardbrake.egg-info/entry_points.txt
--rw-r--r--   0 tahsin     (501) staff       (20)      206 2023-04-07 18:37:07.000000 hardbrake-0.0.3/hardbrake.egg-info/requires.txt
--rw-r--r--   0 tahsin     (501) staff       (20)        4 2023-04-07 18:37:07.000000 hardbrake-0.0.3/hardbrake.egg-info/top_level.txt
--rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:37:08.027263 hardbrake-0.0.3/setup.cfg
--rw-r--r--   0 tahsin     (501) staff       (20)      744 2023-04-07 18:37:05.000000 hardbrake-0.0.3/setup.py
-drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:37:08.026831 hardbrake-0.0.3/src/
--rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 18:33:53.000000 hardbrake-0.0.3/src/__init__.py
--rw-r--r--   0 tahsin     (501) staff       (20)       29 2023-04-07 18:26:58.000000 hardbrake-0.0.3/src/__main__.py
--rw-r--r--   0 tahsin     (501) staff       (20)      757 2023-04-07 18:26:41.000000 hardbrake-0.0.3/src/app.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1370 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/event.py
--rw-r--r--   0 tahsin     (501) staff       (20)      755 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/file.py
--rw-r--r--   0 tahsin     (501) staff       (20)      931 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/loader.py
--rw-r--r--   0 tahsin     (501) staff       (20)      977 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/manager.py
--rw-r--r--   0 tahsin     (501) staff       (20)      364 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/prompts.py
--rw-r--r--   0 tahsin     (501) staff       (20)     1483 2023-04-05 19:04:02.000000 hardbrake-0.0.3/src/utils.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.550989 hardbrake-0.0.4/
+-rw-r--r--   0 tahsin     (501) staff       (20)     1063 2023-04-05 19:04:02.000000 hardbrake-0.0.4/LICENSE
+-rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:38:22.550858 hardbrake-0.0.4/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      892 2023-04-05 19:04:02.000000 hardbrake-0.0.4/README.md
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.549054 hardbrake-0.0.4/hardbrake.egg-info/
+-rw-r--r--   0 tahsin     (501) staff       (20)      199 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/PKG-INFO
+-rw-r--r--   0 tahsin     (501) staff       (20)      351 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/SOURCES.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        1 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/dependency_links.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       43 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/entry_points.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)      211 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/requires.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)        4 2023-04-07 18:38:22.000000 hardbrake-0.0.4/hardbrake.egg-info/top_level.txt
+-rw-r--r--   0 tahsin     (501) staff       (20)       38 2023-04-07 18:38:22.551031 hardbrake-0.0.4/setup.cfg
+-rw-r--r--   0 tahsin     (501) staff       (20)      759 2023-04-07 18:38:16.000000 hardbrake-0.0.4/setup.py
+drwxr-xr-x   0 tahsin     (501) staff       (20)        0 2023-04-07 18:38:22.550636 hardbrake-0.0.4/src/
+-rw-r--r--   0 tahsin     (501) staff       (20)        0 2023-04-07 18:33:53.000000 hardbrake-0.0.4/src/__init__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)       29 2023-04-07 18:26:58.000000 hardbrake-0.0.4/src/__main__.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      757 2023-04-07 18:26:41.000000 hardbrake-0.0.4/src/app.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1370 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/event.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      755 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/file.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      931 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/loader.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      977 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/manager.py
+-rw-r--r--   0 tahsin     (501) staff       (20)      364 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/prompts.py
+-rw-r--r--   0 tahsin     (501) staff       (20)     1483 2023-04-05 19:04:02.000000 hardbrake-0.0.4/src/utils.py
```

### Comparing `hardbrake-0.0.3/LICENSE` & `hardbrake-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/README.md` & `hardbrake-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/setup.py` & `hardbrake-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hardbrake",
-    version="0.0.3",
+    version="0.0.4",
     author="Tahsin",
     author_email="hello@tahsin.us",
     description="A wrapper around HandBrake CLI for encoding multiple files with ease.",
     packages=find_packages(),
     install_requires=[
         "autopep8==2.0.1",
         "markdown-it-py==2.1.0",
@@ -16,14 +16,15 @@
         "pyee==9.0.4",
         "Pygments==2.14.0",
         "ranger-fm==1.9.3",
         "rich==13.3.1",
         "tomli==2.0.1",
         "typing_extensions==4.5.0",
         "wcwidth==0.2.6",
+        "file"
     ],
     entry_points={
         'console_scripts': [
             'hardbrake = src.app:main'
         ]
     }
 )
```

### Comparing `hardbrake-0.0.3/src/app.py` & `hardbrake-0.0.4/src/app.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/src/event.py` & `hardbrake-0.0.4/src/event.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/src/file.py` & `hardbrake-0.0.4/src/file.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/src/loader.py` & `hardbrake-0.0.4/src/loader.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/src/manager.py` & `hardbrake-0.0.4/src/manager.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.0.3/src/utils.py` & `hardbrake-0.0.4/src/utils.py`

 * *Files identical despite different names*

