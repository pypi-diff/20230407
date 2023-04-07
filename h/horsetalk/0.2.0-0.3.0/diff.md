# Comparing `tmp/horsetalk-0.2.0.tar.gz` & `tmp/horsetalk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horsetalk-0.2.0.tar", max compression
+gzip compressed data, was "horsetalk-0.3.0.tar", max compression
```

## Comparing `horsetalk-0.2.0.tar` & `horsetalk-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0      255 2023-04-06 23:24:42.139424 horsetalk-0.2.0/horsetalk/__init__.py
--rw-r--r--   0        0        0      312 2023-04-06 23:20:55.399111 horsetalk-0.2.0/horsetalk/breed.py
--rw-r--r--   0        0        0      353 2023-04-06 23:20:55.399111 horsetalk-0.2.0/horsetalk/case_insensitive_enum.py
--rw-r--r--   0        0        0      496 2023-04-06 23:20:55.400110 horsetalk-0.2.0/horsetalk/coat_colour.py
--rw-r--r--   0        0        0     1069 2023-04-06 23:24:42.140419 horsetalk-0.2.0/horsetalk/disaster.py
--rw-r--r--   0        0        0      408 2023-04-06 23:24:42.141418 horsetalk-0.2.0/horsetalk/gender.py
--rw-r--r--   0        0        0      707 2023-04-06 23:24:42.141418 horsetalk-0.2.0/horsetalk/obstacle.py
--rw-r--r--   0        0        0      280 2023-04-06 23:24:42.141418 horsetalk-0.2.0/horsetalk/sex.py
--rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.2.0/LICENSE
--rw-r--r--   0        0        0      645 2023-04-06 23:25:01.448965 horsetalk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.2.0/README.md
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 horsetalk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-04-07 18:00:16.675799 horsetalk-0.3.0/horsetalk/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-07 18:00:16.676802 horsetalk-0.3.0/horsetalk/aw_going_description.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.676802 horsetalk-0.3.0/horsetalk/breed.py
+-rw-r--r--   0        0        0      471 2023-04-07 18:00:16.677798 horsetalk-0.3.0/horsetalk/coat_colour.py
+-rw-r--r--   0        0        0      287 2023-04-07 18:00:16.677798 horsetalk-0.3.0/horsetalk/dirt_going_description.py
+-rw-r--r--   0        0        0      857 2023-04-07 18:00:16.677798 horsetalk-0.3.0/horsetalk/disaster.py
+-rw-r--r--   0        0        0      383 2023-04-07 18:00:16.678799 horsetalk-0.3.0/horsetalk/gender.py
+-rw-r--r--   0        0        0      477 2023-04-07 18:00:16.678799 horsetalk-0.3.0/horsetalk/obstacle.py
+-rw-r--r--   0        0        0      365 2023-04-07 18:00:16.679798 horsetalk-0.3.0/horsetalk/parsing_enum.py
+-rw-r--r--   0        0        0      296 2023-04-07 18:00:16.679798 horsetalk-0.3.0/horsetalk/racing_code.py
+-rw-r--r--   0        0        0      255 2023-04-07 18:00:16.680799 horsetalk-0.3.0/horsetalk/sex.py
+-rw-r--r--   0        0        0      285 2023-04-07 18:00:16.680799 horsetalk-0.3.0/horsetalk/surface.py
+-rw-r--r--   0        0        0      839 2023-04-07 18:00:16.680799 horsetalk-0.3.0/horsetalk/turf_going_description.py
+-rw-r--r--   0        0        0    35823 2023-04-05 21:36:38.468487 horsetalk-0.3.0/LICENSE
+-rw-r--r--   0        0        0      653 2023-04-07 18:00:16.682248 horsetalk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-04-05 21:36:38.469479 horsetalk-0.3.0/README.md
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 horsetalk-0.3.0/PKG-INFO
```

### Comparing `horsetalk-0.2.0/horsetalk/disaster.py` & `horsetalk-0.3.0/horsetalk/disaster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-from enum import Enum
-from .case_insensitive_enum import CaseInsensitiveEnumMeta
+from .parsing_enum import ParsingEnum
 
 
-class DisasterEnumMeta(CaseInsensitiveEnumMeta):
-    def __getitem__(cls, name):
-        return super().__getitem__(name.replace(" ", "_"))
-
-
-class Disaster(Enum, metaclass=DisasterEnumMeta):
+class Disaster(ParsingEnum):
     """
     An enumeration representing the reason for a horse's non-completion of a race
     """
 
     FELL = 1
     REFUSED = 2
     BROUGHT_DOWN = 3
```

### Comparing `horsetalk-0.2.0/LICENSE` & `horsetalk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `horsetalk-0.2.0/pyproject.toml` & `horsetalk-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "horsetalk"
-version = "0.2.0"
+version = "0.3.0"
 description = "A library of enums and parsers for common horseracing terminology"
 authors = ["peaky76 <robertjamespeacock@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -18,12 +18,12 @@
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
 ruff = "^0.0.261"
 
 [tool.ruff]
-ignore = ["E741"]
+ignore = ["E501", "E741"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `horsetalk-0.2.0/PKG-INFO` & `horsetalk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horsetalk
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library of enums and parsers for common horseracing terminology
 License: GPL-3.0-only
 Author: peaky76
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

