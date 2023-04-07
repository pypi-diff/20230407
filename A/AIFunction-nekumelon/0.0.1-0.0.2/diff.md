# Comparing `tmp/AIFunction-nekumelon-0.0.1.tar.gz` & `tmp/AIFunction-nekumelon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFunction-nekumelon-0.0.1.tar", last modified: Fri Apr  7 19:28:45 2023, max compression
+gzip compressed data, was "AIFunction-nekumelon-0.0.2.tar", last modified: Fri Apr  7 19:40:23 2023, max compression
```

## Comparing `AIFunction-nekumelon-0.0.1.tar` & `AIFunction-nekumelon-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.794241 AIFunction-nekumelon-0.0.1/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1057 2023-04-07 19:24:18.000000 AIFunction-nekumelon-0.0.1/LICENSE
--rw-r--r--   0 nekumelon   (501) staff       (20)     1085 2023-04-07 19:28:45.793200 AIFunction-nekumelon-0.0.1/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      639 2023-04-07 19:21:07.000000 AIFunction-nekumelon-0.0.1/README.md
--rw-r--r--   0 nekumelon   (501) staff       (20)      439 2023-04-07 19:27:51.000000 AIFunction-nekumelon-0.0.1/pyproject.toml
--rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-07 19:28:45.794478 AIFunction-nekumelon-0.0.1/setup.cfg
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.785170 AIFunction-nekumelon-0.0.1/src/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.790570 AIFunction-nekumelon-0.0.1/src/AIFunction_nekumelon.egg-info/
--rw-r--r--   0 nekumelon   (501) staff       (20)     1085 2023-04-07 19:28:45.000000 AIFunction-nekumelon-0.0.1/src/AIFunction_nekumelon.egg-info/PKG-INFO
--rw-r--r--   0 nekumelon   (501) staff       (20)      285 2023-04-07 19:28:45.000000 AIFunction-nekumelon-0.0.1/src/AIFunction_nekumelon.egg-info/SOURCES.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-07 19:28:45.000000 AIFunction-nekumelon-0.0.1/src/AIFunction_nekumelon.egg-info/dependency_links.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)       22 2023-04-07 19:28:45.000000 AIFunction-nekumelon-0.0.1/src/AIFunction_nekumelon.egg-info/top_level.txt
--rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:23:33.000000 AIFunction-nekumelon-0.0.1/src/__init__.py
--rw-r--r--   0 nekumelon   (501) staff       (20)     2556 2023-04-07 19:20:00.000000 AIFunction-nekumelon-0.0.1/src/main.py
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.780157 AIFunction-nekumelon-0.0.1/src/modules/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.780326 AIFunction-nekumelon-0.0.1/src/modules/web/
-drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:28:45.791413 AIFunction-nekumelon-0.0.1/src/modules/web/OpenAI/
--rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-nekumelon-0.0.1/src/modules/web/OpenAI/OpenAI.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.796413 AIFunction-nekumelon-0.0.2/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      423 2023-04-07 19:40:23.795845 AIFunction-nekumelon-0.0.2/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      439 2023-04-07 19:40:05.000000 AIFunction-nekumelon-0.0.2/pyproject.toml
+-rw-r--r--   0 nekumelon   (501) staff       (20)       38 2023-04-07 19:40:23.796553 AIFunction-nekumelon-0.0.2/setup.cfg
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.785652 AIFunction-nekumelon-0.0.2/src/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.792585 AIFunction-nekumelon-0.0.2/src/AIFunction_nekumelon.egg-info/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      423 2023-04-07 19:40:23.000000 AIFunction-nekumelon-0.0.2/src/AIFunction_nekumelon.egg-info/PKG-INFO
+-rw-r--r--   0 nekumelon   (501) staff       (20)      267 2023-04-07 19:40:23.000000 AIFunction-nekumelon-0.0.2/src/AIFunction_nekumelon.egg-info/SOURCES.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        1 2023-04-07 19:40:23.000000 AIFunction-nekumelon-0.0.2/src/AIFunction_nekumelon.egg-info/dependency_links.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)       22 2023-04-07 19:40:23.000000 AIFunction-nekumelon-0.0.2/src/AIFunction_nekumelon.egg-info/top_level.txt
+-rw-r--r--   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:23:33.000000 AIFunction-nekumelon-0.0.2/src/__init__.py
+-rw-r--r--   0 nekumelon   (501) staff       (20)     2556 2023-04-07 19:20:00.000000 AIFunction-nekumelon-0.0.2/src/main.py
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.784254 AIFunction-nekumelon-0.0.2/src/modules/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.784435 AIFunction-nekumelon-0.0.2/src/modules/web/
+drwxr-xr-x   0 nekumelon   (501) staff       (20)        0 2023-04-07 19:40:23.793370 AIFunction-nekumelon-0.0.2/src/modules/web/OpenAI/
+-rw-r--r--   0 nekumelon   (501) staff       (20)      297 2023-04-07 19:11:52.000000 AIFunction-nekumelon-0.0.2/src/modules/web/OpenAI/OpenAI.py
```

### Comparing `AIFunction-nekumelon-0.0.1/src/main.py` & `AIFunction-nekumelon-0.0.2/src/main.py`

 * *Files identical despite different names*

