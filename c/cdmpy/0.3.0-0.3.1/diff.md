# Comparing `tmp/cdmpy-0.3.0.tar.gz` & `tmp/cdmpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmpy-0.3.0.tar", last modified: Fri Apr  7 19:08:18 2023, max compression
+gzip compressed data, was "cdmpy-0.3.1.tar", last modified: Fri Apr  7 19:33:11 2023, max compression
```

## Comparing `cdmpy-0.3.0.tar` & `cdmpy-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.089051 cdmpy-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:17.983037 cdmpy-0.3.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.017038 cdmpy-0.3.0/.github/workflows/
--rw-rw-rw-   0        0        0     1651 2023-04-07 18:46:29.000000 cdmpy-0.3.0/.github/workflows/main.yml
--rw-rw-rw-   0        0        0      144 2023-04-07 17:34:54.000000 cdmpy-0.3.0/.gitignore
--rw-rw-rw-   0        0        0      234 2023-04-07 14:34:19.000000 cdmpy-0.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      944 2023-04-07 17:34:54.000000 cdmpy-0.3.0/CHANGELOG
--rw-rw-rw-   0        0        0     1061 2023-04-07 18:43:32.000000 cdmpy-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     3466 2023-04-07 19:08:18.086052 cdmpy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3012 2023-04-07 19:06:56.000000 cdmpy-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.029043 cdmpy-0.3.0/cdm/
--rw-rw-rw-   0        0        0      282 2023-04-07 19:06:42.000000 cdmpy-0.3.0/cdm/__init__.py
--rw-rw-rw-   0        0        0     2880 2023-04-07 19:06:39.000000 cdmpy-0.3.0/cdm/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.033042 cdmpy-0.3.0/cdm/bin/
--rwxrwxrwx   0        0        0  6431119 2023-04-07 17:34:54.000000 cdmpy-0.3.0/cdm/bin/fio.exe
--rw-rw-rw-   0        0        0     9141 2023-04-07 18:46:58.000000 cdmpy-0.3.0/cdm/cdm.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.071040 cdmpy-0.3.0/cdmpy.egg-info/
--rw-rw-rw-   0        0        0     3466 2023-04-07 19:08:17.000000 cdmpy-0.3.0/cdmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-07 19:08:17.000000 cdmpy-0.3.0/cdmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:08:17.000000 cdmpy-0.3.0/cdmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-07 19:08:17.000000 cdmpy-0.3.0/cdmpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-07 19:08:17.000000 cdmpy-0.3.0/cdmpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      590 2023-04-07 19:07:01.000000 cdmpy-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 19:08:18.089051 cdmpy-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 19:08:18.081042 cdmpy-0.3.0/tests/
--rw-rw-rw-   0        0        0       61 2023-04-07 18:47:59.000000 cdmpy-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0      455 2023-04-07 18:48:08.000000 cdmpy-0.3.0/tests/test_cdm.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.569326 cdmpy-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.503022 cdmpy-0.3.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.540315 cdmpy-0.3.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1651 2023-04-07 19:32:20.000000 cdmpy-0.3.1/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      144 2023-04-07 17:34:54.000000 cdmpy-0.3.1/.gitignore
+-rw-rw-rw-   0        0        0      234 2023-04-07 14:34:19.000000 cdmpy-0.3.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      944 2023-04-07 17:34:54.000000 cdmpy-0.3.1/CHANGELOG
+-rw-rw-rw-   0        0        0     1061 2023-04-07 18:43:32.000000 cdmpy-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3586 2023-04-07 19:33:11.568328 cdmpy-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3012 2023-04-07 19:06:56.000000 cdmpy-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.548307 cdmpy-0.3.1/cdm/
+-rw-rw-rw-   0        0        0      263 2023-04-07 19:28:42.000000 cdmpy-0.3.1/cdm/__init__.py
+-rw-rw-rw-   0        0        0     2888 2023-04-07 19:30:48.000000 cdmpy-0.3.1/cdm/__main__.py
+-rw-rw-rw-   0        0        0     8855 2023-04-07 19:29:17.000000 cdmpy-0.3.1/cdm/fio_cdm.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.560309 cdmpy-0.3.1/cdmpy.egg-info/
+-rw-rw-rw-   0        0        0     3586 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-07 19:33:11.000000 cdmpy-0.3.1/cdmpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      683 2023-04-07 19:31:32.000000 cdmpy-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 19:33:11.570324 cdmpy-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-07 19:33:11.566307 cdmpy-0.3.1/tests/
+-rw-rw-rw-   0        0        0       61 2023-04-07 18:47:59.000000 cdmpy-0.3.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-04-07 19:24:37.000000 cdmpy-0.3.1/tests/test_cdm.py
```

### Comparing `cdmpy-0.3.0/.github/workflows/main.yml` & `cdmpy-0.3.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.0/CHANGELOG` & `cdmpy-0.3.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.0/LICENSE` & `cdmpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.0/PKG-INFO` & `cdmpy-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cdmpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
-Author-email: Lu Xu <oliver_lew@outlook.com>
+Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
 License: MIT
+Project-URL: repository, https://github.com/Pythoniasm/cdmpy
 Keywords: CrystalDiskMark,disk utilities,hdd,ssd
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cdmpy
```

### Comparing `cdmpy-0.3.0/README.md` & `cdmpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cdmpy-0.3.0/cdm/__main__.py` & `cdmpy-0.3.1/cdm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # License: MIT
 # Original Repo: https://github.com/OliverLew/fio-cdm
 # Packaging: https://github.com/Pythoniasm/cdmpy
 
 import argparse
 import logging
 
-from cdm import Job
+from cdm.fio_cdm import Job
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
         description="A python script to show disk test results with fio"
     )
     parser.add_argument(
```

### Comparing `cdmpy-0.3.0/cdm/cdm.py` & `cdmpy-0.3.1/cdm/fio_cdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # Author: Lu Xu <oliver_lew@outlook.com">
 # License: MIT
 # Original Repo: https://github.com/OliverLew/fio-cdm
-# Packaging: https://github.com/Pythoniasm/pycdm
+# Packaging: https://github.com/Pythoniasm/cdmpy
 
-import platform
 import configparser
 import json
 import logging
 import os
 import shutil
 import sys
 import tempfile
 
 from subprocess import Popen, PIPE
-from pathlib import Path
-
-
-FIO_BINARY_WINDOWS_PATH = Path(__file__).parent.joinpath("bin/fio.exe").resolve()
 
 
 class Job:
     def __init__(
         self,
         target,
         size,
@@ -165,21 +160,15 @@
         if self.mix:
             print(
                 "Mixed rw: read {:2.0f}%, write {:2.0f}%".format(
                     self.mix, 100 - self.mix
                 )
             )
 
-        system = platform.system()
-        if system == "Windows":
-            fio_path = FIO_BINARY_WINDOWS_PATH
-        else:
-            fio_path = "fio"
-
-        FIO_COMMAND = [fio_path, "--output-format", "json", self._jobfile_name]
+        FIO_COMMAND = ["fio", "--output-format", "json", self._jobfile_name]
         try:
             res = Popen(FIO_COMMAND, stdout=PIPE)
             output, _ = res.communicate()
         except KeyboardInterrupt:
             logging.info("interrupted, cleaning up before exit...")
             exit()
         except FileNotFoundError:
```

### Comparing `cdmpy-0.3.0/cdmpy.egg-info/PKG-INFO` & `cdmpy-0.3.1/cdmpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cdmpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms.
-Author-email: Lu Xu <oliver_lew@outlook.com>
+Author-email: Lu Xu <oliver_lew@outlook.com>, Pyhoniasm <26092465+Pythoniasm@users.noreply.github.com>
 License: MIT
+Project-URL: repository, https://github.com/Pythoniasm/cdmpy
 Keywords: CrystalDiskMark,disk utilities,hdd,ssd
 Requires-Python: >=3.9.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cdmpy
```

### Comparing `cdmpy-0.3.0/pyproject.toml` & `cdmpy-0.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cdmpy"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
-    {name = "Lu Xu", email = "oliver_lew@outlook.com"}
+    {name = "Lu Xu", email = "oliver_lew@outlook.com"},
+    {name = "Pyhoniasm", email = "26092465+Pythoniasm@users.noreply.github.com"}
 ]
 description = "A python script to generate CrystalDiskMark-style test result with fio. Should work across multi platforms."
-readme = "README.md"
-requires-python = ">=3.9.13"
 keywords = ["CrystalDiskMark", "disk utilities", "hdd", "ssd"]
 license = {text = "MIT"}
+readme = "README.md"
+requires-python = ">=3.9.13"
 dependencies = []
 
-[tool.setuptools.package-data]
-"cdm" = ["bin/fio.exe"]
+[project.urls]
+repository = 'https://github.com/Pythoniasm/cdmpy'
 
 [project.scripts]
 cdm = "cdm:entrypoint"
```

