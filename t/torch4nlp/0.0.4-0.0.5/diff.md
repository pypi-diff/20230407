# Comparing `tmp/torch4nlp-0.0.4.tar.gz` & `tmp/torch4nlp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4nlp-0.0.4.tar", last modified: Fri Apr  7 16:13:21 2023, max compression
+gzip compressed data, was "torch4nlp-0.0.5.tar", last modified: Fri Apr  7 17:15:30 2023, max compression
```

## Comparing `torch4nlp-0.0.4.tar` & `torch4nlp-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.575973 torch4nlp-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-07 14:29:28.000000 torch4nlp-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      229 2023-04-07 16:13:21.574975 torch4nlp-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-04-05 15:24:25.000000 torch4nlp-0.0.4/README.md
--rw-rw-rw-   0        0        0      235 2023-04-07 16:13:00.000000 torch4nlp-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 16:13:21.575973 torch4nlp-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      416 2023-04-07 16:01:21.000000 torch4nlp-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.551040 torch4nlp-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.558021 torch4nlp-0.0.4/src/torch4nlp/
--rw-rw-rw-   0        0        0       46 2023-04-07 15:33:44.000000 torch4nlp-0.0.4/src/torch4nlp/__init__.py
--rw-rw-rw-   0        0        0      286 2023-04-05 10:30:16.000000 torch4nlp-0.0.4/src/torch4nlp/client.py
--rw-rw-rw-   0        0        0       45 2023-04-07 15:51:06.000000 torch4nlp-0.0.4/src/torch4nlp/test.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.570986 torch4nlp-0.0.4/src/torch4nlp/text_classification/
--rw-rw-rw-   0        0        0        0 2023-04-07 14:31:31.000000 torch4nlp-0.0.4/src/torch4nlp/text_classification/__init__.py
--rw-rw-rw-   0        0        0      786 2023-04-05 15:21:29.000000 torch4nlp-0.0.4/src/torch4nlp/text_classification/data_utils.py
--rw-rw-rw-   0        0        0       18 2023-04-07 14:00:30.000000 torch4nlp-0.0.4/src/torch4nlp/text_classification/file_utils.py
--rw-rw-rw-   0        0        0      374 2023-04-05 15:21:19.000000 torch4nlp-0.0.4/src/torch4nlp/text_classification/models.py
--rw-rw-rw-   0        0        0      136 2023-04-05 15:21:38.000000 torch4nlp-0.0.4/src/torch4nlp/text_classification/train.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.572981 torch4nlp-0.0.4/src/torch4nlp/text_similarity/
--rw-rw-rw-   0        0        0        0 2023-04-07 14:31:38.000000 torch4nlp-0.0.4/src/torch4nlp/text_similarity/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 15:20:46.000000 torch4nlp-0.0.4/src/torch4nlp/text_similarity/data_utils.py
--rw-rw-rw-   0        0        0        0 2023-04-05 15:20:53.000000 torch4nlp-0.0.4/src/torch4nlp/text_similarity/models.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.573984 torch4nlp-0.0.4/src/torch4nlp/utils/
--rw-rw-rw-   0        0        0        0 2023-04-07 14:31:44.000000 torch4nlp-0.0.4/src/torch4nlp/utils/__init__.py
--rw-rw-rw-   0        0        0     1811 2023-04-05 15:19:15.000000 torch4nlp-0.0.4/src/torch4nlp/utils/file_util.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:13:21.566998 torch4nlp-0.0.4/src/torch4nlp.egg-info/
--rw-rw-rw-   0        0        0      229 2023-04-07 16:13:21.000000 torch4nlp-0.0.4/src/torch4nlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-04-07 16:13:21.000000 torch4nlp-0.0.4/src/torch4nlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 16:13:21.000000 torch4nlp-0.0.4/src/torch4nlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 16:13:21.000000 torch4nlp-0.0.4/src/torch4nlp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-07 16:13:21.000000 torch4nlp-0.0.4/src/torch4nlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.297820 torch4nlp-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-07 14:29:28.000000 torch4nlp-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      153 2023-04-07 17:15:30.296822 torch4nlp-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-04-05 15:24:25.000000 torch4nlp-0.0.5/README.md
+-rw-rw-rw-   0        0        0      235 2023-04-07 17:15:20.000000 torch4nlp-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 17:15:30.297820 torch4nlp-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.272889 torch4nlp-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.280867 torch4nlp-0.0.5/src/torch4nlp/
+-rw-rw-rw-   0        0        0       41 2023-04-07 17:02:57.000000 torch4nlp-0.0.5/src/torch4nlp/__init__.py
+-rw-rw-rw-   0        0        0      286 2023-04-05 10:30:16.000000 torch4nlp-0.0.5/src/torch4nlp/client.py
+-rw-rw-rw-   0        0        0      416 2023-04-07 16:01:21.000000 torch4nlp-0.0.5/src/torch4nlp/setup.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 16:24:45.000000 torch4nlp-0.0.5/src/torch4nlp/test.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.292834 torch4nlp-0.0.5/src/torch4nlp/text_classification/
+-rw-rw-rw-   0        0        0        0 2023-04-07 14:31:31.000000 torch4nlp-0.0.5/src/torch4nlp/text_classification/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-04-05 15:21:29.000000 torch4nlp-0.0.5/src/torch4nlp/text_classification/data_utils.py
+-rw-rw-rw-   0        0        0       18 2023-04-07 14:00:30.000000 torch4nlp-0.0.5/src/torch4nlp/text_classification/file_utils.py
+-rw-rw-rw-   0        0        0      374 2023-04-05 15:21:19.000000 torch4nlp-0.0.5/src/torch4nlp/text_classification/models.py
+-rw-rw-rw-   0        0        0      136 2023-04-05 15:21:38.000000 torch4nlp-0.0.5/src/torch4nlp/text_classification/train.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.294828 torch4nlp-0.0.5/src/torch4nlp/text_similarity/
+-rw-rw-rw-   0        0        0        0 2023-04-07 14:31:38.000000 torch4nlp-0.0.5/src/torch4nlp/text_similarity/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:20:46.000000 torch4nlp-0.0.5/src/torch4nlp/text_similarity/data_utils.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 15:20:53.000000 torch4nlp-0.0.5/src/torch4nlp/text_similarity/models.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.295826 torch4nlp-0.0.5/src/torch4nlp/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-07 14:31:44.000000 torch4nlp-0.0.5/src/torch4nlp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-04-05 15:19:15.000000 torch4nlp-0.0.5/src/torch4nlp/utils/file_util.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:15:30.288846 torch4nlp-0.0.5/src/torch4nlp.egg-info/
+-rw-rw-rw-   0        0        0      153 2023-04-07 17:15:30.000000 torch4nlp-0.0.5/src/torch4nlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-04-07 17:15:30.000000 torch4nlp-0.0.5/src/torch4nlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 17:15:30.000000 torch4nlp-0.0.5/src/torch4nlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-07 17:15:30.000000 torch4nlp-0.0.5/src/torch4nlp.egg-info/top_level.txt
```

### Comparing `torch4nlp-0.0.4/LICENSE` & `torch4nlp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4nlp-0.0.4/README.md` & `torch4nlp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `torch4nlp-0.0.4/src/torch4nlp/text_classification/data_utils.py` & `torch4nlp-0.0.5/src/torch4nlp/text_classification/data_utils.py`

 * *Files identical despite different names*

### Comparing `torch4nlp-0.0.4/src/torch4nlp/utils/file_util.py` & `torch4nlp-0.0.5/src/torch4nlp/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `torch4nlp-0.0.4/src/torch4nlp.egg-info/SOURCES.txt` & `torch4nlp-0.0.5/src/torch4nlp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 src/torch4nlp/__init__.py
 src/torch4nlp/client.py
+src/torch4nlp/setup.py
 src/torch4nlp/test.py
 src/torch4nlp.egg-info/PKG-INFO
 src/torch4nlp.egg-info/SOURCES.txt
 src/torch4nlp.egg-info/dependency_links.txt
-src/torch4nlp.egg-info/not-zip-safe
 src/torch4nlp.egg-info/top_level.txt
 src/torch4nlp/text_classification/__init__.py
 src/torch4nlp/text_classification/data_utils.py
 src/torch4nlp/text_classification/file_utils.py
 src/torch4nlp/text_classification/models.py
 src/torch4nlp/text_classification/train.py
 src/torch4nlp/text_similarity/__init__.py
```

