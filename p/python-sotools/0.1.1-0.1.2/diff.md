# Comparing `tmp/python-sotools-0.1.1.tar.gz` & `tmp/python-sotools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sotools-0.1.1.tar", last modified: Mon Mar  6 17:32:18 2023, max compression
+gzip compressed data, was "python-sotools-0.1.2.tar", last modified: Fri Apr  7 21:23:00 2023, max compression
```

## Comparing `python-sotools-0.1.1.tar` & `python-sotools-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.353277 python-sotools-0.1.1/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       51 2022-02-24 21:18:50.000000 python-sotools-0.1.1/.coveragerc
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.343277 python-sotools-0.1.1/.github/
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.346610 python-sotools-0.1.1/.github/workflows/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      623 2022-02-24 21:25:31.000000 python-sotools-0.1.1/.github/workflows/coverage.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      603 2022-02-24 21:28:59.000000 python-sotools-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      647 2022-02-24 22:27:09.000000 python-sotools-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       77 2023-03-06 17:24:24.000000 python-sotools-0.1.1/.gitignore
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      657 2023-03-06 16:46:09.000000 python-sotools-0.1.1/HISTORY
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-03-06 17:32:18.353277 python-sotools-0.1.1/PKG-INFO
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1548 2023-03-06 16:40:47.000000 python-sotools-0.1.1/README.md
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      926 2023-03-06 17:06:41.000000 python-sotools-0.1.1/pyproject.toml
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.349944 python-sotools-0.1.1/python_sotools.egg-info/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/PKG-INFO
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1051 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/SOURCES.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        1 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/dependency_links.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       91 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/entry_points.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       11 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/requires.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        8 2023-03-06 17:32:18.000000 python-sotools-0.1.1/python_sotools.egg-info/top_level.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       33 2022-02-24 21:17:21.000000 python-sotools-0.1.1/requirements.txt
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       38 2023-03-06 17:32:18.353277 python-sotools-0.1.1/setup.cfg
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.349944 python-sotools-0.1.1/sotools/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2286 2023-03-06 16:46:09.000000 python-sotools-0.1.1/sotools/__init__.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.349944 python-sotools-0.1.1/sotools/dl_cache/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     6434 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2338 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/dl_cache.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.349944 python-sotools-0.1.1/sotools/dl_cache/extensions/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1003 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/extensions/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      718 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/extensions/generator.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1922 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/extensions/hwcaps.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3466 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/flags.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3376 2022-06-02 20:48:51.000000 python-sotools-0.1.1/sotools/dl_cache/structure.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      455 2023-03-06 16:40:47.000000 python-sotools-0.1.1/sotools/ldd.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11541 2023-03-06 16:54:57.000000 python-sotools-0.1.1/sotools/libraryset.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3506 2023-03-06 16:46:09.000000 python-sotools-0.1.1/sotools/linker.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.353277 python-sotools-0.1.1/sotools/scripts/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 16:40:47.000000 python-sotools-0.1.1/sotools/scripts/__init__.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1664 2023-03-06 16:40:47.000000 python-sotools-0.1.1/sotools/scripts/ldconfig.py
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1194 2023-03-06 16:40:47.000000 python-sotools-0.1.1/sotools/scripts/ldd.py
--rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1074 2023-03-06 16:40:47.000000 python-sotools-0.1.1/sotools/scripts/sowhich.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      124 2022-01-31 23:30:48.000000 python-sotools-0.1.1/sotools/util.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      160 2023-03-06 17:32:18.000000 python-sotools-0.1.1/sotools/version.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.353277 python-sotools-0.1.1/tests/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        0 2022-05-25 21:08:28.000000 python-sotools-0.1.1/tests/__init__.py
-drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 17:32:18.353277 python-sotools-0.1.1/tests/assets/
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11236 2022-03-08 17:17:01.000000 python-sotools-0.1.1/tests/assets/embedded.so.cache
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    16847 2022-03-08 17:17:01.000000 python-sotools-0.1.1/tests/assets/modern.so.cache
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    66251 2022-06-02 20:48:51.000000 python-sotools-0.1.1/tests/assets/with_hwcaps.so.cache
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    10256 2022-06-02 20:48:51.000000 python-sotools-0.1.1/tests/test_dl_cache.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1018 2022-03-08 21:55:56.000000 python-sotools-0.1.1/tests/test_libraries.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     4389 2022-03-08 21:22:29.000000 python-sotools-0.1.1/tests/test_libraries_set.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1062 2022-06-02 20:48:51.000000 python-sotools-0.1.1/tests/test_tools.py
--rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      512 2023-03-06 16:46:08.000000 python-sotools-0.1.1/tox.ini
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.840027 python-sotools-0.1.2/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       51 2022-02-24 21:18:50.000000 python-sotools-0.1.2/.coveragerc
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.826693 python-sotools-0.1.2/.github/
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.830027 python-sotools-0.1.2/.github/workflows/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      623 2022-02-24 21:25:31.000000 python-sotools-0.1.2/.github/workflows/coverage.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      603 2022-02-24 21:28:59.000000 python-sotools-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      647 2022-02-24 22:27:09.000000 python-sotools-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       77 2023-03-06 17:24:24.000000 python-sotools-0.1.2/.gitignore
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      788 2023-04-07 21:20:55.000000 python-sotools-0.1.2/HISTORY
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-07 21:23:00.840027 python-sotools-0.1.2/PKG-INFO
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1548 2023-03-06 16:40:47.000000 python-sotools-0.1.2/README.md
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      926 2023-03-06 17:06:41.000000 python-sotools-0.1.2/pyproject.toml
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/python_sotools.egg-info/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2058 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/PKG-INFO
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1188 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/SOURCES.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        1 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/dependency_links.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       91 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/entry_points.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       11 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/requires.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        8 2023-04-07 21:23:00.000000 python-sotools-0.1.2/python_sotools.egg-info/top_level.txt
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       38 2023-04-07 21:23:00.840027 python-sotools-0.1.2/setup.cfg
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/sotools/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2286 2023-03-06 16:46:09.000000 python-sotools-0.1.2/sotools/__init__.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.833360 python-sotools-0.1.2/sotools/dl_cache/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     6434 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     2338 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/dl_cache.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/sotools/dl_cache/extensions/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1003 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      718 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/generator.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1922 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/extensions/hwcaps.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3466 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/flags.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3376 2022-06-02 20:48:51.000000 python-sotools-0.1.2/sotools/dl_cache/structure.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      455 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/ldd.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11541 2023-03-06 16:54:57.000000 python-sotools-0.1.2/sotools/libraryset.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     3870 2023-04-07 20:58:44.000000 python-sotools-0.1.2/sotools/linker.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/sotools/scripts/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)        0 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/__init__.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1664 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/ldconfig.py
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1194 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/ldd.py
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)     1074 2023-03-06 16:40:47.000000 python-sotools-0.1.2/sotools/scripts/sowhich.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      124 2022-01-31 23:30:48.000000 python-sotools-0.1.2/sotools/util.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      160 2023-04-07 21:23:00.000000 python-sotools-0.1.2/sotools/version.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/tests/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       68 2023-04-07 20:45:59.000000 python-sotools-0.1.2/tests/__init__.py
+drwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)        0 2023-04-07 21:23:00.836694 python-sotools-0.1.2/tests/assets/
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    11236 2022-03-08 17:17:01.000000 python-sotools-0.1.2/tests/assets/embedded.so.cache
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0
+-rwxr-xr-x   0 jskutnik  (1000) jskutnik  (1000)    14736 2023-04-07 20:12:33.000000 python-sotools-0.1.2/tests/assets/libmakebelieve.so.0.0.1
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)       36 2023-04-07 20:12:32.000000 python-sotools-0.1.2/tests/assets/make-believe.c
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    16847 2022-03-08 17:17:01.000000 python-sotools-0.1.2/tests/assets/modern.so.cache
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    66251 2022-06-02 20:48:51.000000 python-sotools-0.1.2/tests/assets/with_hwcaps.so.cache
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)    10077 2023-04-07 19:26:28.000000 python-sotools-0.1.2/tests/test_dl_cache.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1018 2022-03-08 21:55:56.000000 python-sotools-0.1.2/tests/test_libraries.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     4389 2022-03-08 21:22:29.000000 python-sotools-0.1.2/tests/test_libraries_set.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1749 2023-04-07 21:15:26.000000 python-sotools-0.1.2/tests/test_linker.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)     1062 2022-06-02 20:48:51.000000 python-sotools-0.1.2/tests/test_tools.py
+-rw-r--r--   0 jskutnik  (1000) jskutnik  (1000)      497 2023-04-07 19:13:50.000000 python-sotools-0.1.2/tox.ini
```

### Comparing `python-sotools-0.1.1/.github/workflows/coverage.yml` & `python-sotools-0.1.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/.github/workflows/lint.yml` & `python-sotools-0.1.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/.github/workflows/test.yml` & `python-sotools-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/PKG-INFO` & `python-sotools-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sotools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of dynamic linking tools
 Author-email: Jean-Baptiste Skutnik <jb.skutnik@gmail.com>
 License: BSD-3-Clause
 Keywords: elf,linking,linux,libraries,system
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `python-sotools-0.1.1/README.md` & `python-sotools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/pyproject.toml` & `python-sotools-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/python_sotools.egg-info/PKG-INFO` & `python-sotools-0.1.2/python_sotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sotools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of dynamic linking tools
 Author-email: Jean-Baptiste Skutnik <jb.skutnik@gmail.com>
 License: BSD-3-Clause
 Keywords: elf,linking,linux,libraries,system
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `python-sotools-0.1.1/python_sotools.egg-info/SOURCES.txt` & `python-sotools-0.1.2/python_sotools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .coveragerc
 .gitignore
 HISTORY
 README.md
 pyproject.toml
-requirements.txt
 tox.ini
 .github/workflows/coverage.yml
 .github/workflows/lint.yml
 .github/workflows/test.yml
 python_sotools.egg-info/PKG-INFO
 python_sotools.egg-info/SOURCES.txt
 python_sotools.egg-info/dependency_links.txt
@@ -31,11 +30,16 @@
 sotools/scripts/ldconfig.py
 sotools/scripts/ldd.py
 sotools/scripts/sowhich.py
 tests/__init__.py
 tests/test_dl_cache.py
 tests/test_libraries.py
 tests/test_libraries_set.py
+tests/test_linker.py
 tests/test_tools.py
 tests/assets/embedded.so.cache
+tests/assets/libmakebelieve.so.0
+tests/assets/libmakebelieve.so.0.0
+tests/assets/libmakebelieve.so.0.0.1
+tests/assets/make-believe.c
 tests/assets/modern.so.cache
 tests/assets/with_hwcaps.so.cache
```

### Comparing `python-sotools-0.1.1/sotools/__init__.py` & `python-sotools-0.1.2/sotools/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/__init__.py` & `python-sotools-0.1.2/sotools/dl_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/dl_cache.py` & `python-sotools-0.1.2/sotools/dl_cache/dl_cache.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/extensions/__init__.py` & `python-sotools-0.1.2/sotools/dl_cache/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/extensions/generator.py` & `python-sotools-0.1.2/sotools/dl_cache/extensions/generator.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/extensions/hwcaps.py` & `python-sotools-0.1.2/sotools/dl_cache/extensions/hwcaps.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/flags.py` & `python-sotools-0.1.2/sotools/dl_cache/flags.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/dl_cache/structure.py` & `python-sotools-0.1.2/sotools/dl_cache/structure.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/libraryset.py` & `python-sotools-0.1.2/sotools/libraryset.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/linker.py` & `python-sotools-0.1.2/sotools/linker.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,55 +32,71 @@
         None,
         os.environ.get('LD_LIBRARY_PATH', "").split(':'),
     )
 
     return (ld_library_path, DEFAULT_PATHS)
 
 
-def resolve(soname: str,
-            rpath: Optional[List[str]] = None,
-            runpath: Optional[List[str]] = None,
-            arch_flags: Optional[Flags] = None) -> Optional[str]:
+def _valid(path: Path) -> bool:
+    """Check a path is an existing directory"""
+    return path.is_dir()
+
+
+def _search_paths(
+    soname: str,
+    paths: List[Path],
+    reason: str = "",
+) -> Optional[Path]:
+    """
+    Search a list of paths for a given soname and return the first match
+
+    soname:     The library name to search
+    paths:      The list of paths to look into
+    reason:     To mimic LD_DEBUG, optional reason of the search
+    """
+    if paths:
+        path_list_str = os.pathsep.join(map(lambda x: x.as_posix(), paths))
+        logging.debug(f"search path={path_list_str}\t\t({reason or ''})")
+
+    for dir_ in filter(_valid, paths):
+        potential_lib = Path(dir_, soname)
+        logging.debug(f"trying file={potential_lib.as_posix()}")
+        if potential_lib.exists():
+            return potential_lib
+
+    return None
+
+
+def resolve(
+    soname: str,
+    rpath: Optional[List[str]] = None,
+    runpath: Optional[List[str]] = None,
+    arch_flags: Optional[Flags] = None,
+    absolute: bool = False,
+) -> Optional[Path]:
     """
     Get a path towards a library from a given soname.
     Implements system rules and takes the environment into account
 
     soname:     'key' to lookup for a library
     rpath:      rpath to use for this lookup
     runpath:    runpath to use for this lookup
     arch_flags: flags to look for; useful for 32bit libraries on 64bit systems
                 See sotools.dl_cache.flags.Flags for info
+    absolute:   output an absolute path to the final object if a link is found
 
     The method will return a resolved path for the given soname or None if
     no matching entry could be found.
     """
 
-    found = Path()
+    found = None
 
     def _found() -> bool:
         """Check if a returned path corresponds to the soname"""
-        return found != Path()
-
-    def _valid(path: Path) -> bool:
-        """Check a path is an existing directory"""
-        return path.is_dir()
-
-    def _search_paths(soname: str, paths: List[Path], reason: str) -> Path:
-        """Search a list of paths and return the first match"""
-        if paths:
-            path_list_str = os.pathsep.join(map(lambda x: x.as_posix(), paths))
-            logging.debug(f"search path={path_list_str}\t\t({reason or ''})")
-
-        for dir_ in filter(_valid, paths):
-            potential_lib = Path(dir_, soname)
-            logging.debug(f"trying file={potential_lib.as_posix()}")
-            if potential_lib.exists():
-                return potential_lib
-
-        return Path()
+        return found not in {None, Path()}
 
     rpath = list(map(Path, list(rpath or [])))
     runpath = list(map(Path, list(runpath or [])))
     cache_entries = cache_libraries(arch_flags=arch_flags)
     system_path = map(Path, _linker_path()[1])
 
     env_path, system_path = _linker_path()
@@ -111,10 +127,13 @@
     # Finally, search the hardcoded system paths
     for tuple_ in default_paths:
         if not _found():
             found = _search_paths(soname, *tuple_)
 
     if _found():
         logging.debug(f"found matching library={found}")
-        return found.resolve()
+        if absolute:
+            found = found.resolve()
+            logging.debug(f"-> link to library={found}")
+        return found
 
     return None
```

### Comparing `python-sotools-0.1.1/sotools/scripts/ldconfig.py` & `python-sotools-0.1.2/sotools/scripts/ldconfig.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/scripts/ldd.py` & `python-sotools-0.1.2/sotools/scripts/ldd.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/sotools/scripts/sowhich.py` & `python-sotools-0.1.2/sotools/scripts/sowhich.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/assets/embedded.so.cache` & `python-sotools-0.1.2/tests/assets/embedded.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/assets/modern.so.cache` & `python-sotools-0.1.2/tests/assets/modern.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/assets/with_hwcaps.so.cache` & `python-sotools-0.1.2/tests/assets/with_hwcaps.so.cache`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/test_dl_cache.py` & `python-sotools-0.1.2/tests/test_dl_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 import unittest
 from pathlib import Path
-from sotools.dl_cache.structure import (BinaryStruct,
-                                        deserialize_null_terminated_string)
-from sotools.dl_cache.extensions import (CacheExtension, CacheExtensionSection,
-                                         CacheExtensionTag,
-                                         cache_extension_sections)
-from sotools.dl_cache.dl_cache import (_cache_type, _CacheType, _CacheHeader,
-                                       _CacheHeaderNew, _CacheHeaderOld,
-                                       _FileEntryNew, _FileEntryOld)
-from sotools.dl_cache.extensions.hwcaps import (dl_cache_hwcap_extension,
-                                                HWCAPSection)
+from sotools.dl_cache.structure import (
+    BinaryStruct,
+    deserialize_null_terminated_string,
+)
+from sotools.dl_cache.extensions import (
+    CacheExtension,
+    CacheExtensionSection,
+    CacheExtensionTag,
+    cache_extension_sections,
+)
+from sotools.dl_cache.dl_cache import (
+    _CacheHeader,
+    _CacheHeaderNew,
+    _CacheHeaderOld,
+    _CacheType,
+    _FileEntryNew,
+    _FileEntryOld,
+    _cache_type,
+)
+from sotools.dl_cache.extensions.hwcaps import (
+    HWCAPSection,
+    dl_cache_hwcap_extension,
+)
 from sotools.dl_cache.flags import Flags
-from sotools.dl_cache import (cache_libraries, _cache_libraries, get_generator,
-                              search_cache, _parse_cache, DynamicLinkerCache)
+from sotools.dl_cache import (
+    DynamicLinkerCache,
+    _cache_libraries,
+    _parse_cache,
+    cache_libraries,
+    get_generator,
+    search_cache,
+)
 
 EMBEDDED_CACHE = f'{Path(__file__).parent}/assets/embedded.so.cache'
 MODERN_CACHE = f'{Path(__file__).parent}/assets/modern.so.cache'
 HWCAPS_CACHE = f'{Path(__file__).parent}/assets/with_hwcaps.so.cache'
 
 
 class DLCacheTest(unittest.TestCase):
```

### Comparing `python-sotools-0.1.1/tests/test_libraries.py` & `python-sotools-0.1.2/tests/test_libraries.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/test_libraries_set.py` & `python-sotools-0.1.2/tests/test_libraries_set.py`

 * *Files identical despite different names*

### Comparing `python-sotools-0.1.1/tests/test_tools.py` & `python-sotools-0.1.2/tests/test_tools.py`

 * *Files identical despite different names*

