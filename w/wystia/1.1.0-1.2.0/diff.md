# Comparing `tmp/wystia-1.1.0.tar.gz` & `tmp/wystia-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wystia-1.1.0.tar", last modified: Fri Jan 28 00:35:41 2022, max compression
+gzip compressed data, was "wystia-1.2.0.tar", last modified: Fri Apr  7 21:44:52 2023, max compression
```

## Comparing `wystia-1.1.0.tar` & `wystia-1.2.0.tar`

### file list

```diff
@@ -1,78 +1,72 @@
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.218876 wystia-1.1.0/
--rw-r--r--   0 rnag     (238500323) 387158756     4131 2022-01-14 23:29:14.000000 wystia-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 rnag     (238500323) 387158756     3587 2022-01-28 00:35:05.000000 wystia-1.1.0/HISTORY.rst
--rw-r--r--   0 rnag     (238500323) 387158756     1069 2021-06-12 22:49:08.000000 wystia-1.1.0/LICENSE
--rw-r--r--   0 rnag     (238500323) 387158756      335 2021-06-16 16:51:15.000000 wystia-1.1.0/MANIFEST.in
--rw-r--r--   0 rnag     (238500323) 387158756    14464 2022-01-28 00:35:41.219053 wystia-1.1.0/PKG-INFO
--rw-r--r--   0 rnag     (238500323) 387158756     9943 2022-01-28 00:35:05.000000 wystia-1.1.0/README.rst
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.188963 wystia-1.1.0/docs/
--rw-r--r--   0 rnag     (238500323) 387158756      607 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/Makefile
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.172339 wystia-1.1.0/docs/_build/
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.172485 wystia-1.1.0/docs/_build/html/
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.191300 wystia-1.1.0/docs/_build/html/_static/
--rw-r--r--   0 rnag     (238500323) 387158756      286 2021-07-21 15:31:14.000000 wystia-1.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 rnag     (238500323) 387158756       90 2021-07-21 15:31:14.000000 wystia-1.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 rnag     (238500323) 387158756       90 2021-07-21 15:31:14.000000 wystia-1.1.0/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 rnag     (238500323) 387158756     4759 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/conf.py
--rw-r--r--   0 rnag     (238500323) 387158756       33 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/contributing.rst
--rw-r--r--   0 rnag     (238500323) 387158756       28 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/history.rst
--rw-r--r--   0 rnag     (238500323) 387158756      302 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/index.rst
--rw-r--r--   0 rnag     (238500323) 387158756     1123 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/installation.rst
--rw-r--r--   0 rnag     (238500323) 387158756      768 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/make.bat
--rw-r--r--   0 rnag     (238500323) 387158756       55 2021-07-21 18:04:54.000000 wystia-1.1.0/docs/modules.rst
--rw-r--r--   0 rnag     (238500323) 387158756      362 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/quickstart.rst
--rw-r--r--   0 rnag     (238500323) 387158756       27 2021-06-12 22:49:08.000000 wystia-1.1.0/docs/readme.rst
--rw-r--r--   0 rnag     (238500323) 387158756     4777 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/usage.rst
--rw-r--r--   0 rnag     (238500323) 387158756     1885 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/wystia.rst
--rw-r--r--   0 rnag     (238500323) 387158756      687 2021-06-17 14:50:29.000000 wystia-1.1.0/docs/wystia.utils.parse.rst
--rw-r--r--   0 rnag     (238500323) 387158756      564 2022-01-14 23:29:14.000000 wystia-1.1.0/docs/wystia.utils.rst
--rw-r--r--   0 rnag     (238500323) 387158756      423 2022-01-28 00:35:41.219842 wystia-1.1.0/setup.cfg
--rw-r--r--   0 rnag     (238500323) 387158756     1820 2022-01-28 00:35:05.000000 wystia-1.1.0/setup.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.191931 wystia-1.1.0/tests/
--rw-r--r--   0 rnag     (238500323) 387158756     2105 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/conftest.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.193659 wystia-1.1.0/tests/testdata/
--rw-r--r--   0 rnag     (238500323) 387158756       93 2021-06-16 17:29:47.000000 wystia-1.1.0/tests/testdata/sample-captions.srt
--rw-r--r--   0 rnag     (238500323) 387158756      448 2021-06-14 21:30:46.000000 wystia-1.1.0/tests/testdata/upload_response.json
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.195728 wystia-1.1.0/tests/unit/
--rw-r--r--   0 rnag     (238500323) 387158756       36 2021-06-12 22:49:08.000000 wystia-1.1.0/tests/unit/__init__.py
--rw-r--r--   0 rnag     (238500323) 387158756     1073 2022-01-14 23:29:14.000000 wystia-1.1.0/tests/unit/conftest.py
--rw-r--r--   0 rnag     (238500323) 387158756     9307 2022-01-14 23:29:14.000000 wystia-1.1.0/tests/unit/test_wystia.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.196970 wystia-1.1.0/tests/unit/utils/
--rw-r--r--   0 rnag     (238500323) 387158756        0 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.199714 wystia-1.1.0/tests/unit/utils/parse/
--rw-r--r--   0 rnag     (238500323) 387158756        0 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/parse/__init__.py
--rw-r--r--   0 rnag     (238500323) 387158756      311 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/parse/conftest.py
--rw-r--r--   0 rnag     (238500323) 387158756     1932 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/parse/test_srt.py
--rw-r--r--   0 rnag     (238500323) 387158756     2843 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/parse/test_types.py
--rw-r--r--   0 rnag     (238500323) 387158756      403 2021-07-21 18:57:35.000000 wystia-1.1.0/tests/unit/utils/test_response.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.207421 wystia-1.1.0/wystia/
--rw-r--r--   0 rnag     (238500323) 387158756      916 2022-01-28 00:35:05.000000 wystia-1.1.0/wystia/__init__.py
--rw-r--r--   0 rnag     (238500323) 387158756     8414 2022-01-28 00:35:05.000000 wystia-1.1.0/wystia/api_base.py
--rw-r--r--   0 rnag     (238500323) 387158756    26040 2022-01-28 00:35:05.000000 wystia-1.1.0/wystia/api_data.py
--rw-r--r--   0 rnag     (238500323) 387158756     2789 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/api_embed.py
--rw-r--r--   0 rnag     (238500323) 387158756     5272 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/api_helper.py
--rw-r--r--   0 rnag     (238500323) 387158756     5033 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/api_upload.py
--rw-r--r--   0 rnag     (238500323) 387158756     1161 2021-07-21 18:57:35.000000 wystia-1.1.0/wystia/config.py
--rw-r--r--   0 rnag     (238500323) 387158756      681 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/constants.py
--rw-r--r--   0 rnag     (238500323) 387158756     2063 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/errors.py
--rw-r--r--   0 rnag     (238500323) 387158756      116 2021-06-16 19:02:40.000000 wystia-1.1.0/wystia/log.py
--rw-r--r--   0 rnag     (238500323) 387158756    23219 2022-01-28 00:35:05.000000 wystia-1.1.0/wystia/models.py
--rwxr-xr-x   0 rnag     (238500323) 387158756      646 2021-04-08 19:33:37.000000 wystia-1.1.0/wystia/requests_config.py
--rw-r--r--   0 rnag     (238500323) 387158756     1985 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/requests_models.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.215498 wystia-1.1.0/wystia/utils/
--rw-r--r--   0 rnag     (238500323) 387158756        0 2021-06-14 14:07:03.000000 wystia-1.1.0/wystia/utils/__init__.py
--rw-r--r--   0 rnag     (238500323) 387158756     1048 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/utils/decorators.py
--rw-r--r--   0 rnag     (238500323) 387158756      408 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/utils/metaclasses.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.218250 wystia-1.1.0/wystia/utils/parse/
--rw-r--r--   0 rnag     (238500323) 387158756       76 2021-06-16 17:18:30.000000 wystia-1.1.0/wystia/utils/parse/__init__.py
--rw-r--r--   0 rnag     (238500323) 387158756      819 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/utils/parse/file.py
--rw-r--r--   0 rnag     (238500323) 387158756     2298 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/utils/parse/srt.py
--rw-r--r--   0 rnag     (238500323) 387158756     2936 2022-01-14 23:29:14.000000 wystia-1.1.0/wystia/utils/parse/types.py
--rw-r--r--   0 rnag     (238500323) 387158756      498 2021-06-14 14:23:58.000000 wystia-1.1.0/wystia/utils/response.py
-drwxr-xr-x   0 rnag     (238500323) 387158756        0 2022-01-28 00:35:41.211922 wystia-1.1.0/wystia.egg-info/
--rw-r--r--   0 rnag     (238500323) 387158756    14464 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/PKG-INFO
--rw-r--r--   0 rnag     (238500323) 387158756     1449 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/SOURCES.txt
--rw-r--r--   0 rnag     (238500323) 387158756        1 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/dependency_links.txt
--rw-r--r--   0 rnag     (238500323) 387158756        1 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/not-zip-safe
--rw-r--r--   0 rnag     (238500323) 387158756      116 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/requires.txt
--rw-r--r--   0 rnag     (238500323) 387158756        7 2022-01-28 00:35:40.000000 wystia-1.1.0/wystia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-07 21:44:47.000000 wystia-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-07 21:44:47.000000 wystia-1.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 21:44:47.000000 wystia-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-07 21:44:47.000000 wystia-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-07 21:44:52.429243 wystia-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-07 21:44:47.000000 wystia-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.utils.parse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 21:44:47.000000 wystia-1.2.0/docs/wystia.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 21:44:52.429243 wystia-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-07 21:44:47.000000 wystia-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/testdata/sample-captions.srt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/testdata/upload_response.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/test_wystia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/tests/unit/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/parse/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-07 21:44:47.000000 wystia-1.2.0/tests/unit/utils/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/wystia/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/api_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/requests_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/wystia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/metaclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.429243 wystia-1.2.0/wystia/utils/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/srt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/parse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 21:44:47.000000 wystia-1.2.0/wystia/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:44:52.425243 wystia-1.2.0/wystia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 21:44:52.000000 wystia-1.2.0/wystia.egg-info/top_level.txt
```

### Comparing `wystia-1.1.0/CONTRIBUTING.rst` & `wystia-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/HISTORY.rst` & `wystia-1.2.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+1.2.0 (2023-04-07)
+------------------
+
+* Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
+* Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+* Upgrade dependencies in ``requirements-dev.txt``.
+
 1.1.0 (2022-01-27)
 ------------------
 
 * Refactor any model classes that would be returned in *list* API
   calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
   simply so that ``Container`` objects will be returned by default.
```

### Comparing `wystia-1.1.0/LICENSE` & `wystia-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/PKG-INFO` & `wystia-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,403 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: wystia
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
+Description: ==========================
+        Wystia - Wistia API Helper
+        ==========================
+        
+        
+        .. image:: https://img.shields.io/pypi/v/wystia.svg
+                :target: https://pypi.org/project/wystia/
+        
+        .. image:: https://img.shields.io/pypi/l/wystia.svg
+                :target: https://pypi.org/project/wystia/
+        
+        .. image:: https://img.shields.io/pypi/pyversions/wystia.svg
+                :target: https://pypi.org/project/wystia
+        
+        .. image:: https://github.com/rnag/wystia/actions/workflows/dev.yml/badge.svg
+                :target: https://github.com/rnag/wystia/actions/workflows/dev.yml
+        
+        .. image:: https://readthedocs.org/projects/wystia/badge/?version=latest
+                :target: https://wystia.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        
+        .. image:: https://pyup.io/repos/github/rnag/wystia/shield.svg
+             :target: https://pyup.io/repos/github/rnag/wystia/
+             :alt: Updates
+        
+        
+        
+        A Python wrapper library for the Wistia API
+        
+        
+        * Free software: MIT license
+        * Documentation: https://wystia.readthedocs.io.
+        * Wistia Developer Docs: https://wistia.com/support/developers.
+        
+        Installation
+        ------------
+        
+        The Wystia library is available `on PyPI`_, and can be installed with ``pip``:
+        
+        .. code-block:: shell
+        
+            $ pip install wystia
+        
+        You'll also need to create an access token as outlined `in the docs`_.
+        
+        Usage
+        -----
+        
+        Sample usage with the `Data API <https://wistia.com/support/developers/data-api>`_:
+        
+            Note: The following example makes use of ``WistiaApi``, which is an alias to
+            the class ``WistiaDataApi``.
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaApi
+            from wystia.models import SortBy, LanguageCode, Customizations, Private
+        
+            # Setup the Wistia API token to use for requests. You can alternatively
+            # set this via the env variable 'WISTIA_API_TOKEN'.
+            WistiaApi.configure('MY-TOKEN')
+        
+            # Retrieve a list of all projects in the Wistia account,
+            # sorted A-Z and in ascending order.
+            projects = WistiaApi.list_all_projects(SortBy.NAME)
+            project_ids = [p.hashed_id for p in projects]
+            # Print the project data as a prettified JSON string
+            print(projects.prettify())
+        
+            # Retrieve a list of videos for a Wistia project.
+            # Note: If you don't require asset info (such as ADs) on each
+            #   video, I suggest calling `list_project` instead.
+            videos = WistiaApi.list_videos('project-id')
+        
+            # Retrieve info on a particular video
+            vd = WistiaApi.get_video('video-id')
+            # If the video has captions, that won't be included in the `Medias#show`
+            # response by default, so we'll need a separate API call as below.
+            # vd.process_captions(
+            #     WistiaApi.list_captions(real_video_id))
+            print(vd)
+        
+            # Update attributes on a media (video), or set a custom thumbnail on the video.
+            WistiaApi.update_video(
+                'video-id',
+                thumbnail_media_id='uploaded-thumbnail-id'
+            )
+        
+            # Get aggregated stats for a video, such as view count
+            stats = WistiaApi.get_stats_for_video('video-id')
+        
+            # Retrieve the customization data for a video
+            customizations = WistiaApi.get_customizations('video-id')
+        
+            # Update only specific customizations for a video
+            # Note the embed options are documented here:
+            #   https://wistia.com/support/developers/embed-options
+            sample_embed_options = Customizations(
+                player_color='#e7fad1',
+                # Hide comments on the media page
+                private=Private(show_comments=False)
+            )
+            WistiaApi.update_customizations('video-id', sample_embed_options)
+        
+            # Get the Spanish captions on a video
+            captions = WistiaApi.get_captions('video-id', LanguageCode.SPANISH)
+        
+            # Add (or replace) the English captions on a video
+            WistiaApi.update_captions(
+                'video-id',
+                LanguageCode.ENGLISH,
+                srt_file='path/to/file.srt'
+            )
+        
+        
+        ... or to upload media via the `Upload API <https://wistia.com/support/developers/upload-api>`_:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaUploadApi
+        
+            # Upload a file to a (default) project on Wistia
+            r = WistiaUploadApi.upload_file('path/to/my-file.mp4')
+            # Check if the video was successfully uploaded
+            # assert r.created
+            # assert r.name == 'my-file.mp4'
+        
+            # Uploads with a public link to a video, such as
+            # an S3 pre-signed url.
+            r = WistiaUploadApi.upload_link('my-s3-link',
+                                            title='My Video Name',
+                                            description='My Description')
+        
+        ... you can alternatively retrieve asset info via the public Media Embed link:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaEmbedApi
+        
+            # Get the media embed data
+            embed_data = WistiaEmbedApi.get_data('video-id')
+        
+            # Retrieve the source URL of the original media
+            source_url = WistiaEmbedApi.asset_url(media_data=embed_data)
+        
+        ... when using the *Data API*, the ``WistiaHelper`` can help to further simplify some calls:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaHelper
+        
+            # Check if the video exists in your Wistia account
+            assert WistiaHelper.video_exists('abc1234567')
+        
+            # Check if a video's name indicates the video is an archived copy of an
+            # existing video, as discussed in the below article on replacing a media:
+            #   https://wistia.com/learn/product-updates/improved-library-management-tools
+            assert WistiaHelper.is_archived_video(
+                'My Title [Archived on August 13, 2015]')
+        
+            # Update the player color on a video
+            WistiaHelper.customize_video_on_wistia('video-id', 'ffffcc')
+        
+            # Individually enable captions / AD in the player for a video
+            WistiaHelper.enable_ad('video-id')
+            WistiaHelper.enable_captions('video-id', on_by_default=False)
+        
+            # Disable captions / AD in the player for a video
+            if WistiaHelper.has_captions_enabled('video-id'):
+                print('Disabling captions and AD for the video')
+                WistiaHelper.disable_captions_and_ad('video-id')
+        
+        Getting Started
+        ---------------
+        
+        Using the methods on the API classes assume your Wistia API token
+        has previously been configured, for example via the environment. The API token will
+        then be used globally by all the API classes when making requests to the Wistia API.
+        
+        You can set the following environment variable with your API token:
+        
+        * ``WISTIA_API_TOKEN``
+        
+        Another option is to use the global ``configure`` method as shown below:
+        
+        .. code-block:: python3
+        
+            WistiaDataApi.configure('MY-API-TOKEN')
+        
+        There is additionally a `Quickstart`_ section in the docs which walks
+        through - in more detail - how to get up and running with the
+        Wystia library.
+        
+        Data API
+        --------
+        
+        The wrapper class ``WistiaDataApi`` (aliased to ``WistiaApi``) interacts
+        with the Wistia Data API (docs below):
+        
+        - https://wistia.com/support/developers/data-api
+        
+        
+        It fully implements the following sections in the API documentation:
+        
+            - Paging and Sorting Responses
+            - Projects
+            - Medias
+            - Customizations
+            - Captions
+        
+        The following sections in the API have *not* been implemented (mainly as I haven't used them before):
+        
+            - Project Sharings
+            - Account
+        
+        
+        Tips
+        ~~~~
+        
+        Containers
+        ==========
+        
+        In general, the API methods that begin with *list* - such as ``list_project`` -
+        will return a `Container`_ object, which essentially acts as a thin wrapper
+        around a collection of model classes. For all intents and purposes, this behaves
+        exactly the same as a ``list`` object.
+        
+        One of the main benefits is that it implements a ``__str__`` method, which leverages
+        the builtin ``pprint`` module in Python to pretty-print the Python object representation
+        of each model or *dataclass* instance; this will format the output more nicely, for example
+        whenever ``print(obj)`` is called on the `Container` result.
+        
+        The ``Container`` objects also implement the following convenience methods, which can
+        be used to easily display the JSON string representation of the list of dataclass instances:
+        
+            * ``to_json`` - Convert the list of instances to a JSON string.
+        
+            * ``prettify`` - Convert the list of instances to a *prettified* JSON string.
+        
+        List Medias in a Project
+        ========================
+        
+        If you need to retrieve info on videos in a project and you
+        don't need complete info such as a list of assets for the video,
+        I recommend using ``list_project`` instead of ``list_videos``. This is because
+        the `Projects#show <https://wistia.com/support/developers/data-api#projects_show>`_
+        API returns up to 500 results per request, whereas the ``Medias#list``
+        only returns the default 100 results per page.
+        
+        Assuming a project in your Wistia account has a total of about 250 media, here is the number of API
+        calls you might expect from each individual approach:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaDataApi
+        
+            videos = WistiaDataApi.list_videos('project-id')
+            assert WistiaDataApi.request_count() == 3
+        
+            # Resets request count for the next call
+            WistiaDataApi.reset_request_count()
+        
+            videos = WistiaDataApi.list_project('project-id')
+            assert WistiaDataApi.request_count() == 1
+        
+        
+        Thread Safety
+        -------------
+        
+        The Wistia API classes are completely thread safe, since ``requests.Session``
+        objects are not re-used between API calls.
+        
+        This means that if you have two (un-related) API operations to perform,
+        such as updating a video's title and adding captions on the video,
+        then you can certainly run those calls in parallel so that
+        they complete a bit faster.
+        
+        
+        Credits
+        -------
+        
+        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _on PyPI: https://pypi.org/project/wystia/
+        .. _in the docs: https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens
+        .. _Container: https://dataclass-wizard.readthedocs.io/en/latest/dataclass_wizard.html?highlight=container#dataclass_wizard.Container
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
+        
+        
+        =======
+        History
+        =======
+        
+        1.2.0 (2023-04-07)
+        ------------------
+        
+        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
+        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        * Upgrade dependencies in ``requirements-dev.txt``.
+        
+        1.1.0 (2022-01-27)
+        ------------------
+        
+        * Refactor any model classes that would be returned in *list* API
+          calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
+          simply so that ``Container`` objects will be returned by default.
+        
+        * Refactor to import ``Container`` from the ``dataclass-wizard`` library
+          instead. For backwards compatibility reasons, the ``models`` module
+          still exports the *Container* namespace.
+        
+        1.0.0 (2022-01-14)
+        ------------------
+        
+        **Breaking Changes**
+        
+        * Wystia has officially dropped support for Python versions 3.5 and 3.6.
+          The support for 3.6 needed to be dropped primarily because of the
+          ``from __future__ import annotations`` usage in the code.
+        * Refactored all API helper classes to return model class objects as a result,
+          rather than Python ``dict`` objects. In the case of any `list`- related API responses,
+          we now return a ``Container`` object so that it can be easier to print or display
+          the result for debugging purposes.
+        * All inputs to the API helper methods that previously accepted a ``dict`` object,
+          have in general been refactored to accept a model dataclass instance as an input instead.
+        * Renamed some error classes; for example, ``NoSuchMedia`` instead of ``NoSuchVideo``.
+        * Renamed some model classes; for example, ``MediaStatus`` instead of ``VideoStatus``.
+        
+        **Features and Improvements**
+        
+        * Added ``WistiaApi`` to the list of public exports, which is aliased to the
+          ``WistiaDataApi`` helper class.
+        * Added new methods to the ``WistiaDataApi`` class for more explicitly
+          interacting with *medias* instead of *videos*. For example, a ``list_medias``
+          method is added as an alternative to calling ``list_videos``.
+        * Refactored the CI process to use GitHub Workflows instead of Travis CI.
+        * Added *3.10* to the list of supported Python versions.
+        * Updated the project status from *Beta* to *Production/Stable*.
+        * Added an ``examples/`` folder in the project repo on GitHub, which
+          contains Python scripts to demonstrate sample usage.
+        * Updated docs and added a new *Quickstart* section.
+        
+        0.3.0 (2021-07-21)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add compatibility changes to extend support to Python 3.5 and 3.6
+        * WistiaHelper: Add method ``project_details`` to retrieve info on a particular Wistia project
+        * WistiaEmbedApi: Update to parse the ``.json`` response rather than the ``.jsonp`` version
+        * Makefile: Add new command ``init``, which can be used to install Dev dependencies for the project
+        
+          * Ensure the new command is compatible with Python 3.5, which has dependencies on separate
+            package versions; here we should use ``requirements-py35-dev.txt`` instead.
+        * Makefile: Update ``coverage`` command to run unit tests by default
+        
+        **Bugfixes**
+        
+        * models.VideoData: The parameter to the ``process_captions`` method is now
+          correctly type-annotated to accept a ``List`` of ``Dict``
+        
+        0.2.1 (2021-06-17)
+        ------------------
+        
+        * WistiaHelper: Add method ``enable_captions_and_ad``
+        * Remove ``.format`` usage in log statements
+        * Remove an unnecessary method ``ad_needed`` from ``VideoData``
+        * Update readme and Sphinx ``docs/``
+        
+        0.2.0 (2021-06-16)
+        ------------------
+        
+        * Fully implement all sections in the Wistia Data API
+        * Add more methods to the ``WistiaHelper`` class
+        * Request Count and API Token should now be globally shared by all API sub-classes
+        * Lot of code refactoring
+        * Exclude ``.mp4`` files from dist, to reduce total package size
+        * Add more test cases
+        * Update docs with better examples
+        
+        0.1.0 (2021-06-12)
+        ------------------
+        
+        * First release on PyPI.
+        
 Keywords: wistia,wistia api,wystia,wistia data api,wistia upload api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,391 +405,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
-License-File: LICENSE
-
-==========================
-Wystia - Wistia API Helper
-==========================
-
-
-.. image:: https://img.shields.io/pypi/v/wystia.svg
-        :target: https://pypi.org/project/wystia/
-
-.. image:: https://img.shields.io/pypi/l/wystia.svg
-        :target: https://pypi.org/project/wystia/
-
-.. image:: https://img.shields.io/pypi/pyversions/wystia.svg
-        :target: https://pypi.org/project/wystia
-
-.. image:: https://github.com/rnag/wystia/actions/workflows/dev.yml/badge.svg
-        :target: https://github.com/rnag/wystia/actions/workflows/dev.yml
-
-.. image:: https://readthedocs.org/projects/wystia/badge/?version=latest
-        :target: https://wystia.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-.. image:: https://pyup.io/repos/github/rnag/wystia/shield.svg
-     :target: https://pyup.io/repos/github/rnag/wystia/
-     :alt: Updates
-
-
-
-A Python wrapper library for the Wistia API
-
-
-* Free software: MIT license
-* Documentation: https://wystia.readthedocs.io.
-* Wistia Developer Docs: https://wistia.com/support/developers.
-
-Installation
-------------
-
-The Wystia library is available `on PyPI`_, and can be installed with ``pip``:
-
-.. code-block:: shell
-
-    $ pip install wystia
-
-You'll also need to create an access token as outlined `in the docs`_.
-
-Usage
------
-
-Sample usage with the `Data API <https://wistia.com/support/developers/data-api>`_:
-
-    Note: The following example makes use of ``WistiaApi``, which is an alias to
-    the class ``WistiaDataApi``.
-
-.. code-block:: python3
-
-    from wystia import WistiaApi
-    from wystia.models import SortBy, LanguageCode, Customizations, Private
-
-    # Setup the Wistia API token to use for requests. You can alternatively
-    # set this via the env variable 'WISTIA_API_TOKEN'.
-    WistiaApi.configure('MY-TOKEN')
-
-    # Retrieve a list of all projects in the Wistia account,
-    # sorted A-Z and in ascending order.
-    projects = WistiaApi.list_all_projects(SortBy.NAME)
-    project_ids = [p.hashed_id for p in projects]
-    # Print the project data as a prettified JSON string
-    print(projects.prettify())
-
-    # Retrieve a list of videos for a Wistia project.
-    # Note: If you don't require asset info (such as ADs) on each
-    #   video, I suggest calling `list_project` instead.
-    videos = WistiaApi.list_videos('project-id')
-
-    # Retrieve info on a particular video
-    vd = WistiaApi.get_video('video-id')
-    # If the video has captions, that won't be included in the `Medias#show`
-    # response by default, so we'll need a separate API call as below.
-    # vd.process_captions(
-    #     WistiaApi.list_captions(real_video_id))
-    print(vd)
-
-    # Update attributes on a media (video), or set a custom thumbnail on the video.
-    WistiaApi.update_video(
-        'video-id',
-        thumbnail_media_id='uploaded-thumbnail-id'
-    )
-
-    # Get aggregated stats for a video, such as view count
-    stats = WistiaApi.get_stats_for_video('video-id')
-
-    # Retrieve the customization data for a video
-    customizations = WistiaApi.get_customizations('video-id')
-
-    # Update only specific customizations for a video
-    # Note the embed options are documented here:
-    #   https://wistia.com/support/developers/embed-options
-    sample_embed_options = Customizations(
-        player_color='#e7fad1',
-        # Hide comments on the media page
-        private=Private(show_comments=False)
-    )
-    WistiaApi.update_customizations('video-id', sample_embed_options)
-
-    # Get the Spanish captions on a video
-    captions = WistiaApi.get_captions('video-id', LanguageCode.SPANISH)
-
-    # Add (or replace) the English captions on a video
-    WistiaApi.update_captions(
-        'video-id',
-        LanguageCode.ENGLISH,
-        srt_file='path/to/file.srt'
-    )
-
-
-... or to upload media via the `Upload API <https://wistia.com/support/developers/upload-api>`_:
-
-.. code-block:: python3
-
-    from wystia import WistiaUploadApi
-
-    # Upload a file to a (default) project on Wistia
-    r = WistiaUploadApi.upload_file('path/to/my-file.mp4')
-    # Check if the video was successfully uploaded
-    # assert r.created
-    # assert r.name == 'my-file.mp4'
-
-    # Uploads with a public link to a video, such as
-    # an S3 pre-signed url.
-    r = WistiaUploadApi.upload_link('my-s3-link',
-                                    title='My Video Name',
-                                    description='My Description')
-
-... you can alternatively retrieve asset info via the public Media Embed link:
-
-.. code-block:: python3
-
-    from wystia import WistiaEmbedApi
-
-    # Get the media embed data
-    embed_data = WistiaEmbedApi.get_data('video-id')
-
-    # Retrieve the source URL of the original media
-    source_url = WistiaEmbedApi.asset_url(media_data=embed_data)
-
-... when using the *Data API*, the ``WistiaHelper`` can help to further simplify some calls:
-
-.. code-block:: python3
-
-    from wystia import WistiaHelper
-
-    # Check if the video exists in your Wistia account
-    assert WistiaHelper.video_exists('abc1234567')
-
-    # Check if a video's name indicates the video is an archived copy of an
-    # existing video, as discussed in the below article on replacing a media:
-    #   https://wistia.com/learn/product-updates/improved-library-management-tools
-    assert WistiaHelper.is_archived_video(
-        'My Title [Archived on August 13, 2015]')
-
-    # Update the player color on a video
-    WistiaHelper.customize_video_on_wistia('video-id', 'ffffcc')
-
-    # Individually enable captions / AD in the player for a video
-    WistiaHelper.enable_ad('video-id')
-    WistiaHelper.enable_captions('video-id', on_by_default=False)
-
-    # Disable captions / AD in the player for a video
-    if WistiaHelper.has_captions_enabled('video-id'):
-        print('Disabling captions and AD for the video')
-        WistiaHelper.disable_captions_and_ad('video-id')
-
-Getting Started
----------------
-
-Using the methods on the API classes assume your Wistia API token
-has previously been configured, for example via the environment. The API token will
-then be used globally by all the API classes when making requests to the Wistia API.
-
-You can set the following environment variable with your API token:
-
-* ``WISTIA_API_TOKEN``
-
-Another option is to use the global ``configure`` method as shown below:
-
-.. code-block:: python3
-
-    WistiaDataApi.configure('MY-API-TOKEN')
-
-There is additionally a `Quickstart`_ section in the docs which walks
-through - in more detail - how to get up and running with the
-Wystia library.
-
-Data API
---------
-
-The wrapper class ``WistiaDataApi`` (aliased to ``WistiaApi``) interacts
-with the Wistia Data API (docs below):
-
-- https://wistia.com/support/developers/data-api
-
-
-It fully implements the following sections in the API documentation:
-
-    - Paging and Sorting Responses
-    - Projects
-    - Medias
-    - Customizations
-    - Captions
-
-The following sections in the API have *not* been implemented (mainly as I haven't used them before):
-
-    - Project Sharings
-    - Account
-
-
-Tips
-~~~~
-
-Containers
-==========
-
-In general, the API methods that begin with *list* - such as ``list_project`` -
-will return a `Container`_ object, which essentially acts as a thin wrapper
-around a collection of model classes. For all intents and purposes, this behaves
-exactly the same as a ``list`` object.
-
-One of the main benefits is that it implements a ``__str__`` method, which leverages
-the builtin ``pprint`` module in Python to pretty-print the Python object representation
-of each model or *dataclass* instance; this will format the output more nicely, for example
-whenever ``print(obj)`` is called on the `Container` result.
-
-The ``Container`` objects also implement the following convenience methods, which can
-be used to easily display the JSON string representation of the list of dataclass instances:
-
-    * ``to_json`` - Convert the list of instances to a JSON string.
-
-    * ``prettify`` - Convert the list of instances to a *prettified* JSON string.
-
-List Medias in a Project
-========================
-
-If you need to retrieve info on videos in a project and you
-don't need complete info such as a list of assets for the video,
-I recommend using ``list_project`` instead of ``list_videos``. This is because
-the `Projects#show <https://wistia.com/support/developers/data-api#projects_show>`_
-API returns up to 500 results per request, whereas the ``Medias#list``
-only returns the default 100 results per page.
-
-Assuming a project in your Wistia account has a total of about 250 media, here is the number of API
-calls you might expect from each individual approach:
-
-.. code-block:: python3
-
-    from wystia import WistiaDataApi
-
-    videos = WistiaDataApi.list_videos('project-id')
-    assert WistiaDataApi.request_count() == 3
-
-    # Resets request count for the next call
-    WistiaDataApi.reset_request_count()
-
-    videos = WistiaDataApi.list_project('project-id')
-    assert WistiaDataApi.request_count() == 1
-
-
-Thread Safety
--------------
-
-The Wistia API classes are completely thread safe, since ``requests.Session``
-objects are not re-used between API calls.
-
-This means that if you have two (un-related) API operations to perform,
-such as updating a video's title and adding captions on the video,
-then you can certainly run those calls in parallel so that
-they complete a bit faster.
-
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _on PyPI: https://pypi.org/project/wystia/
-.. _in the docs: https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens
-.. _Container: https://dataclass-wizard.readthedocs.io/en/latest/dataclass_wizard.html?highlight=container#dataclass_wizard.Container
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
-
-
-=======
-History
-=======
-
-1.1.0 (2022-01-27)
-------------------
-
-* Refactor any model classes that would be returned in *list* API
-  calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
-  simply so that ``Container`` objects will be returned by default.
-
-* Refactor to import ``Container`` from the ``dataclass-wizard`` library
-  instead. For backwards compatibility reasons, the ``models`` module
-  still exports the *Container* namespace.
-
-1.0.0 (2022-01-14)
-------------------
-
-**Breaking Changes**
-
-* Wystia has officially dropped support for Python versions 3.5 and 3.6.
-  The support for 3.6 needed to be dropped primarily because of the
-  ``from __future__ import annotations`` usage in the code.
-* Refactored all API helper classes to return model class objects as a result,
-  rather than Python ``dict`` objects. In the case of any `list`- related API responses,
-  we now return a ``Container`` object so that it can be easier to print or display
-  the result for debugging purposes.
-* All inputs to the API helper methods that previously accepted a ``dict`` object,
-  have in general been refactored to accept a model dataclass instance as an input instead.
-* Renamed some error classes; for example, ``NoSuchMedia`` instead of ``NoSuchVideo``.
-* Renamed some model classes; for example, ``MediaStatus`` instead of ``VideoStatus``.
-
-**Features and Improvements**
-
-* Added ``WistiaApi`` to the list of public exports, which is aliased to the
-  ``WistiaDataApi`` helper class.
-* Added new methods to the ``WistiaDataApi`` class for more explicitly
-  interacting with *medias* instead of *videos*. For example, a ``list_medias``
-  method is added as an alternative to calling ``list_videos``.
-* Refactored the CI process to use GitHub Workflows instead of Travis CI.
-* Added *3.10* to the list of supported Python versions.
-* Updated the project status from *Beta* to *Production/Stable*.
-* Added an ``examples/`` folder in the project repo on GitHub, which
-  contains Python scripts to demonstrate sample usage.
-* Updated docs and added a new *Quickstart* section.
-
-0.3.0 (2021-07-21)
-------------------
-
-**Features and Improvements**
-
-* Add compatibility changes to extend support to Python 3.5 and 3.6
-* WistiaHelper: Add method ``project_details`` to retrieve info on a particular Wistia project
-* WistiaEmbedApi: Update to parse the ``.json`` response rather than the ``.jsonp`` version
-* Makefile: Add new command ``init``, which can be used to install Dev dependencies for the project
-
-  * Ensure the new command is compatible with Python 3.5, which has dependencies on separate
-    package versions; here we should use ``requirements-py35-dev.txt`` instead.
-* Makefile: Update ``coverage`` command to run unit tests by default
-
-**Bugfixes**
-
-* models.VideoData: The parameter to the ``process_captions`` method is now
-  correctly type-annotated to accept a ``List`` of ``Dict``
-
-0.2.1 (2021-06-17)
-------------------
-
-* WistiaHelper: Add method ``enable_captions_and_ad``
-* Remove ``.format`` usage in log statements
-* Remove an unnecessary method ``ad_needed`` from ``VideoData``
-* Update readme and Sphinx ``docs/``
-
-0.2.0 (2021-06-16)
-------------------
-
-* Fully implement all sections in the Wistia Data API
-* Add more methods to the ``WistiaHelper`` class
-* Request Count and API Token should now be globally shared by all API sub-classes
-* Lot of code refactoring
-* Exclude ``.mp4`` files from dist, to reduce total package size
-* Add more test cases
-* Update docs with better examples
-
-0.1.0 (2021-06-12)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `wystia-1.1.0/README.rst` & `wystia-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/Makefile` & `wystia-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/conf.py` & `wystia-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/installation.rst` & `wystia-1.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/make.bat` & `wystia-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/usage.rst` & `wystia-1.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/wystia.rst` & `wystia-1.2.0/docs/wystia.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/wystia.utils.parse.rst` & `wystia-1.2.0/docs/wystia.utils.parse.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/docs/wystia.utils.rst` & `wystia-1.2.0/docs/wystia.utils.rst`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/setup.py` & `wystia-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 
 readme = (here / 'README.rst').read_text()
 history = (here / 'HISTORY.rst').read_text()
 
 setup(
     name='wystia',
-    version='1.1.0',
+    version='1.2.0',
     description='A Python wrapper library for the Wistia API',
     long_description=readme + '\n\n' + history,
     author='Ritvik Nag',
     author_email='rv.kvetch@gmail.com',
     url='https://github.com/rnag/wystia',
     packages=packages,
     include_package_data=True,
```

### Comparing `wystia-1.1.0/tests/conftest.py` & `wystia-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/tests/unit/conftest.py` & `wystia-1.2.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/tests/unit/test_wystia.py` & `wystia-1.2.0/tests/unit/test_wystia.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
     my_src_url = "https://embed-ssl.wistia.com/deliveries/abc.bin"
 
     ved = VideoEmbedData.from_dict({'type': 'Video',
                                     'hashedId': mock_video_id,
                                     'name': video_name,
                                     'createdAt': created_ts,
                                     'duration': duration,
+                                    'privacyMode': False,
+                                    'mediaId': 321,
+                                    'accountId': 123,
+                                    'analyticsHost': '',
                                     "assets": [
                                         {
                                             "type": "original",
                                             "slug": "original",
                                             "displayName": "Original file",
                                             "bitrate": 2356,
                                             "public": True,
@@ -225,14 +229,15 @@
          'id': 2208087,
          'hashed_id': mock_video_id,
          'name': video_name,
          'description': description,
          'created': created_string,
          'updated': created_string,
          'progress': '0',
+         'archived': False,
          'status': status,
          'duration': duration,
          'thumbnail':
              {
                  'url': 'http://embed.wistia.com/deliveries/abc.jpg',
                  'width': 100,
                  'height': 60
```

### Comparing `wystia-1.1.0/tests/unit/utils/parse/test_srt.py` & `wystia-1.2.0/tests/unit/utils/parse/test_srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/tests/unit/utils/parse/test_types.py` & `wystia-1.2.0/tests/unit/utils/parse/test_types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/__init__.py` & `wystia-1.2.0/wystia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 
 # A handy alias in case it comes in useful to anyone :-)
 WistiaApi = WistiaDataApi
 
 
 __author__ = 'Ritvik Nag'
 __email__ = 'rv.kvetch@gmail.com'
-__version__ = '1.1.0'
+__version__ = '1.2.0'
 
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 #   https://docs.python.org/3.8/howto/logging.html#configuring-logging-for-a-library
 logging.getLogger('wystia').addHandler(logging.NullHandler())
```

### Comparing `wystia-1.1.0/wystia/api_base.py` & `wystia-1.2.0/wystia/api_base.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/api_data.py` & `wystia-1.2.0/wystia/api_data.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/api_embed.py` & `wystia-1.2.0/wystia/api_embed.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/api_helper.py` & `wystia-1.2.0/wystia/api_helper.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/api_upload.py` & `wystia-1.2.0/wystia/api_upload.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/config.py` & `wystia-1.2.0/wystia/config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/constants.py` & `wystia-1.2.0/wystia/constants.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/errors.py` & `wystia-1.2.0/wystia/errors.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/models.py` & `wystia-1.2.0/wystia/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,15 @@
     class _(JSONWizard.Meta):
         raise_on_unknown_json_key = RAISE_ON_UNKNOWN_KEY
         skip_defaults = True
 
     # Override the type annotations as needed.
     duration: float = 0.0
     project: ProjectInfo = None
+    archived: bool | None = None
 
     # Not included in GET '/v1/medias' response, but technically
     # still part of video metadata.
     has_audio_description: bool | None = None
     captions_enabled: bool | None = None
     overlay_text: str | None = None
     caption_duration: float | None = None
@@ -405,14 +406,16 @@
 
     Ref: https://wistia.com/support/developers/embed-options
     """
     class _(JSONWizard.Meta):
         raise_on_unknown_json_key = RAISE_ON_UNKNOWN_KEY
         skip_defaults = True
 
+    vulcan: bool = True
+    anonymize_ip: bool = True
     player_color: str = ''
     still_url: str | None = None
     unaltered_still_image_asset: UnalteredStillImageAsset | None = None
     thumbnail_alt_text: str | None = None
     auto_play: bool | None = None
     silent_auto_play: bool | None = None
     end_video_behavior: str | None = None
@@ -736,14 +739,15 @@
 
     hashed_id: str
     id: int
     name: str
     type: MediaType
     description: str | None
     account_id: int
+    archived: bool
     created: datetime
     updated: datetime
     progress: float
     thumbnail: Thumbnail
     duration: float | None = None
     status: MediaStatus = MediaStatus.QUEUED
 
@@ -767,37 +771,41 @@
     created_at: datetime
     duration: float
     assets: list[EmbedAsset]
     project_id: int
     stats: EmbedStats
     distillery_url: str
     account_key: str
+    privacy_mode: bool
+    media_id: int
+    account_id: int
+    analytics_host: str
     media_key: str
     type: str
     media_type: str
     progress: float
     status: int
     branding: bool
     enable_customer_logo: bool
     seo_description: str
-    preload_preference: Any
+    preload_preference: str
     flash_player_url: str
     show_about: bool
     first_embed_for_account: bool
     first_share_for_account: bool
     keyframe_align: bool
     use_media_data_host_logic: bool
     tracking_transmit_interval: int
     # Annotating this field as a generic `dict` type for now, because
     # I've not seen this feature used before.
-    integrations: dict
+    integrations: dict[str, str]
     # integrations: Integrations
-    hls_enabled: bool
     embed_options: Customizations
     captions: list[EmbedCaption] = field(default_factory=list)
+    hls_enabled: bool = False
     transcript: Transcript | None = None
 
     # Not included in GET '/v1/medias' response, but technically
     # still part of video metadata.
     source_url: str = ''
     ad_url: str | None = None
     has_audio_description: bool = False
```

### Comparing `wystia-1.1.0/wystia/requests_config.py` & `wystia-1.2.0/wystia/requests_config.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/requests_models.py` & `wystia-1.2.0/wystia/requests_models.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/utils/decorators.py` & `wystia-1.2.0/wystia/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/utils/parse/file.py` & `wystia-1.2.0/wystia/utils/parse/file.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/utils/parse/srt.py` & `wystia-1.2.0/wystia/utils/parse/srt.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia/utils/parse/types.py` & `wystia-1.2.0/wystia/utils/parse/types.py`

 * *Files identical despite different names*

### Comparing `wystia-1.1.0/wystia.egg-info/PKG-INFO` & `wystia-1.2.0/wystia.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,403 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: wystia
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python wrapper library for the Wistia API
 Home-page: https://github.com/rnag/wystia
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
+Description: ==========================
+        Wystia - Wistia API Helper
+        ==========================
+        
+        
+        .. image:: https://img.shields.io/pypi/v/wystia.svg
+                :target: https://pypi.org/project/wystia/
+        
+        .. image:: https://img.shields.io/pypi/l/wystia.svg
+                :target: https://pypi.org/project/wystia/
+        
+        .. image:: https://img.shields.io/pypi/pyversions/wystia.svg
+                :target: https://pypi.org/project/wystia
+        
+        .. image:: https://github.com/rnag/wystia/actions/workflows/dev.yml/badge.svg
+                :target: https://github.com/rnag/wystia/actions/workflows/dev.yml
+        
+        .. image:: https://readthedocs.org/projects/wystia/badge/?version=latest
+                :target: https://wystia.readthedocs.io/en/latest/?version=latest
+                :alt: Documentation Status
+        
+        
+        .. image:: https://pyup.io/repos/github/rnag/wystia/shield.svg
+             :target: https://pyup.io/repos/github/rnag/wystia/
+             :alt: Updates
+        
+        
+        
+        A Python wrapper library for the Wistia API
+        
+        
+        * Free software: MIT license
+        * Documentation: https://wystia.readthedocs.io.
+        * Wistia Developer Docs: https://wistia.com/support/developers.
+        
+        Installation
+        ------------
+        
+        The Wystia library is available `on PyPI`_, and can be installed with ``pip``:
+        
+        .. code-block:: shell
+        
+            $ pip install wystia
+        
+        You'll also need to create an access token as outlined `in the docs`_.
+        
+        Usage
+        -----
+        
+        Sample usage with the `Data API <https://wistia.com/support/developers/data-api>`_:
+        
+            Note: The following example makes use of ``WistiaApi``, which is an alias to
+            the class ``WistiaDataApi``.
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaApi
+            from wystia.models import SortBy, LanguageCode, Customizations, Private
+        
+            # Setup the Wistia API token to use for requests. You can alternatively
+            # set this via the env variable 'WISTIA_API_TOKEN'.
+            WistiaApi.configure('MY-TOKEN')
+        
+            # Retrieve a list of all projects in the Wistia account,
+            # sorted A-Z and in ascending order.
+            projects = WistiaApi.list_all_projects(SortBy.NAME)
+            project_ids = [p.hashed_id for p in projects]
+            # Print the project data as a prettified JSON string
+            print(projects.prettify())
+        
+            # Retrieve a list of videos for a Wistia project.
+            # Note: If you don't require asset info (such as ADs) on each
+            #   video, I suggest calling `list_project` instead.
+            videos = WistiaApi.list_videos('project-id')
+        
+            # Retrieve info on a particular video
+            vd = WistiaApi.get_video('video-id')
+            # If the video has captions, that won't be included in the `Medias#show`
+            # response by default, so we'll need a separate API call as below.
+            # vd.process_captions(
+            #     WistiaApi.list_captions(real_video_id))
+            print(vd)
+        
+            # Update attributes on a media (video), or set a custom thumbnail on the video.
+            WistiaApi.update_video(
+                'video-id',
+                thumbnail_media_id='uploaded-thumbnail-id'
+            )
+        
+            # Get aggregated stats for a video, such as view count
+            stats = WistiaApi.get_stats_for_video('video-id')
+        
+            # Retrieve the customization data for a video
+            customizations = WistiaApi.get_customizations('video-id')
+        
+            # Update only specific customizations for a video
+            # Note the embed options are documented here:
+            #   https://wistia.com/support/developers/embed-options
+            sample_embed_options = Customizations(
+                player_color='#e7fad1',
+                # Hide comments on the media page
+                private=Private(show_comments=False)
+            )
+            WistiaApi.update_customizations('video-id', sample_embed_options)
+        
+            # Get the Spanish captions on a video
+            captions = WistiaApi.get_captions('video-id', LanguageCode.SPANISH)
+        
+            # Add (or replace) the English captions on a video
+            WistiaApi.update_captions(
+                'video-id',
+                LanguageCode.ENGLISH,
+                srt_file='path/to/file.srt'
+            )
+        
+        
+        ... or to upload media via the `Upload API <https://wistia.com/support/developers/upload-api>`_:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaUploadApi
+        
+            # Upload a file to a (default) project on Wistia
+            r = WistiaUploadApi.upload_file('path/to/my-file.mp4')
+            # Check if the video was successfully uploaded
+            # assert r.created
+            # assert r.name == 'my-file.mp4'
+        
+            # Uploads with a public link to a video, such as
+            # an S3 pre-signed url.
+            r = WistiaUploadApi.upload_link('my-s3-link',
+                                            title='My Video Name',
+                                            description='My Description')
+        
+        ... you can alternatively retrieve asset info via the public Media Embed link:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaEmbedApi
+        
+            # Get the media embed data
+            embed_data = WistiaEmbedApi.get_data('video-id')
+        
+            # Retrieve the source URL of the original media
+            source_url = WistiaEmbedApi.asset_url(media_data=embed_data)
+        
+        ... when using the *Data API*, the ``WistiaHelper`` can help to further simplify some calls:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaHelper
+        
+            # Check if the video exists in your Wistia account
+            assert WistiaHelper.video_exists('abc1234567')
+        
+            # Check if a video's name indicates the video is an archived copy of an
+            # existing video, as discussed in the below article on replacing a media:
+            #   https://wistia.com/learn/product-updates/improved-library-management-tools
+            assert WistiaHelper.is_archived_video(
+                'My Title [Archived on August 13, 2015]')
+        
+            # Update the player color on a video
+            WistiaHelper.customize_video_on_wistia('video-id', 'ffffcc')
+        
+            # Individually enable captions / AD in the player for a video
+            WistiaHelper.enable_ad('video-id')
+            WistiaHelper.enable_captions('video-id', on_by_default=False)
+        
+            # Disable captions / AD in the player for a video
+            if WistiaHelper.has_captions_enabled('video-id'):
+                print('Disabling captions and AD for the video')
+                WistiaHelper.disable_captions_and_ad('video-id')
+        
+        Getting Started
+        ---------------
+        
+        Using the methods on the API classes assume your Wistia API token
+        has previously been configured, for example via the environment. The API token will
+        then be used globally by all the API classes when making requests to the Wistia API.
+        
+        You can set the following environment variable with your API token:
+        
+        * ``WISTIA_API_TOKEN``
+        
+        Another option is to use the global ``configure`` method as shown below:
+        
+        .. code-block:: python3
+        
+            WistiaDataApi.configure('MY-API-TOKEN')
+        
+        There is additionally a `Quickstart`_ section in the docs which walks
+        through - in more detail - how to get up and running with the
+        Wystia library.
+        
+        Data API
+        --------
+        
+        The wrapper class ``WistiaDataApi`` (aliased to ``WistiaApi``) interacts
+        with the Wistia Data API (docs below):
+        
+        - https://wistia.com/support/developers/data-api
+        
+        
+        It fully implements the following sections in the API documentation:
+        
+            - Paging and Sorting Responses
+            - Projects
+            - Medias
+            - Customizations
+            - Captions
+        
+        The following sections in the API have *not* been implemented (mainly as I haven't used them before):
+        
+            - Project Sharings
+            - Account
+        
+        
+        Tips
+        ~~~~
+        
+        Containers
+        ==========
+        
+        In general, the API methods that begin with *list* - such as ``list_project`` -
+        will return a `Container`_ object, which essentially acts as a thin wrapper
+        around a collection of model classes. For all intents and purposes, this behaves
+        exactly the same as a ``list`` object.
+        
+        One of the main benefits is that it implements a ``__str__`` method, which leverages
+        the builtin ``pprint`` module in Python to pretty-print the Python object representation
+        of each model or *dataclass* instance; this will format the output more nicely, for example
+        whenever ``print(obj)`` is called on the `Container` result.
+        
+        The ``Container`` objects also implement the following convenience methods, which can
+        be used to easily display the JSON string representation of the list of dataclass instances:
+        
+            * ``to_json`` - Convert the list of instances to a JSON string.
+        
+            * ``prettify`` - Convert the list of instances to a *prettified* JSON string.
+        
+        List Medias in a Project
+        ========================
+        
+        If you need to retrieve info on videos in a project and you
+        don't need complete info such as a list of assets for the video,
+        I recommend using ``list_project`` instead of ``list_videos``. This is because
+        the `Projects#show <https://wistia.com/support/developers/data-api#projects_show>`_
+        API returns up to 500 results per request, whereas the ``Medias#list``
+        only returns the default 100 results per page.
+        
+        Assuming a project in your Wistia account has a total of about 250 media, here is the number of API
+        calls you might expect from each individual approach:
+        
+        .. code-block:: python3
+        
+            from wystia import WistiaDataApi
+        
+            videos = WistiaDataApi.list_videos('project-id')
+            assert WistiaDataApi.request_count() == 3
+        
+            # Resets request count for the next call
+            WistiaDataApi.reset_request_count()
+        
+            videos = WistiaDataApi.list_project('project-id')
+            assert WistiaDataApi.request_count() == 1
+        
+        
+        Thread Safety
+        -------------
+        
+        The Wistia API classes are completely thread safe, since ``requests.Session``
+        objects are not re-used between API calls.
+        
+        This means that if you have two (un-related) API operations to perform,
+        such as updating a video's title and adding captions on the video,
+        then you can certainly run those calls in parallel so that
+        they complete a bit faster.
+        
+        
+        Credits
+        -------
+        
+        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+        
+        .. _on PyPI: https://pypi.org/project/wystia/
+        .. _in the docs: https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens
+        .. _Container: https://dataclass-wizard.readthedocs.io/en/latest/dataclass_wizard.html?highlight=container#dataclass_wizard.Container
+        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
+        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+        .. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
+        
+        
+        =======
+        History
+        =======
+        
+        1.2.0 (2023-04-07)
+        ------------------
+        
+        * Update model classes to support *new* populated fields, such as ``archived`` (a ``bool`` field), as otherwise it breaks de-serialization by default.
+        * Update to replace plain ``dict`` annotation with ``dict[str, str]``, as previously it was resulting in errors when parsing the class annotations.
+        * Upgrade dependencies in ``requirements-dev.txt``.
+        
+        1.1.0 (2022-01-27)
+        ------------------
+        
+        * Refactor any model classes that would be returned in *list* API
+          calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
+          simply so that ``Container`` objects will be returned by default.
+        
+        * Refactor to import ``Container`` from the ``dataclass-wizard`` library
+          instead. For backwards compatibility reasons, the ``models`` module
+          still exports the *Container* namespace.
+        
+        1.0.0 (2022-01-14)
+        ------------------
+        
+        **Breaking Changes**
+        
+        * Wystia has officially dropped support for Python versions 3.5 and 3.6.
+          The support for 3.6 needed to be dropped primarily because of the
+          ``from __future__ import annotations`` usage in the code.
+        * Refactored all API helper classes to return model class objects as a result,
+          rather than Python ``dict`` objects. In the case of any `list`- related API responses,
+          we now return a ``Container`` object so that it can be easier to print or display
+          the result for debugging purposes.
+        * All inputs to the API helper methods that previously accepted a ``dict`` object,
+          have in general been refactored to accept a model dataclass instance as an input instead.
+        * Renamed some error classes; for example, ``NoSuchMedia`` instead of ``NoSuchVideo``.
+        * Renamed some model classes; for example, ``MediaStatus`` instead of ``VideoStatus``.
+        
+        **Features and Improvements**
+        
+        * Added ``WistiaApi`` to the list of public exports, which is aliased to the
+          ``WistiaDataApi`` helper class.
+        * Added new methods to the ``WistiaDataApi`` class for more explicitly
+          interacting with *medias* instead of *videos*. For example, a ``list_medias``
+          method is added as an alternative to calling ``list_videos``.
+        * Refactored the CI process to use GitHub Workflows instead of Travis CI.
+        * Added *3.10* to the list of supported Python versions.
+        * Updated the project status from *Beta* to *Production/Stable*.
+        * Added an ``examples/`` folder in the project repo on GitHub, which
+          contains Python scripts to demonstrate sample usage.
+        * Updated docs and added a new *Quickstart* section.
+        
+        0.3.0 (2021-07-21)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add compatibility changes to extend support to Python 3.5 and 3.6
+        * WistiaHelper: Add method ``project_details`` to retrieve info on a particular Wistia project
+        * WistiaEmbedApi: Update to parse the ``.json`` response rather than the ``.jsonp`` version
+        * Makefile: Add new command ``init``, which can be used to install Dev dependencies for the project
+        
+          * Ensure the new command is compatible with Python 3.5, which has dependencies on separate
+            package versions; here we should use ``requirements-py35-dev.txt`` instead.
+        * Makefile: Update ``coverage`` command to run unit tests by default
+        
+        **Bugfixes**
+        
+        * models.VideoData: The parameter to the ``process_captions`` method is now
+          correctly type-annotated to accept a ``List`` of ``Dict``
+        
+        0.2.1 (2021-06-17)
+        ------------------
+        
+        * WistiaHelper: Add method ``enable_captions_and_ad``
+        * Remove ``.format`` usage in log statements
+        * Remove an unnecessary method ``ad_needed`` from ``VideoData``
+        * Update readme and Sphinx ``docs/``
+        
+        0.2.0 (2021-06-16)
+        ------------------
+        
+        * Fully implement all sections in the Wistia Data API
+        * Add more methods to the ``WistiaHelper`` class
+        * Request Count and API Token should now be globally shared by all API sub-classes
+        * Lot of code refactoring
+        * Exclude ``.mp4`` files from dist, to reduce total package size
+        * Add more test cases
+        * Update docs with better examples
+        
+        0.1.0 (2021-06-12)
+        ------------------
+        
+        * First release on PyPI.
+        
 Keywords: wistia,wistia api,wystia,wistia data api,wistia upload api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,391 +405,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
-License-File: LICENSE
-
-==========================
-Wystia - Wistia API Helper
-==========================
-
-
-.. image:: https://img.shields.io/pypi/v/wystia.svg
-        :target: https://pypi.org/project/wystia/
-
-.. image:: https://img.shields.io/pypi/l/wystia.svg
-        :target: https://pypi.org/project/wystia/
-
-.. image:: https://img.shields.io/pypi/pyversions/wystia.svg
-        :target: https://pypi.org/project/wystia
-
-.. image:: https://github.com/rnag/wystia/actions/workflows/dev.yml/badge.svg
-        :target: https://github.com/rnag/wystia/actions/workflows/dev.yml
-
-.. image:: https://readthedocs.org/projects/wystia/badge/?version=latest
-        :target: https://wystia.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-.. image:: https://pyup.io/repos/github/rnag/wystia/shield.svg
-     :target: https://pyup.io/repos/github/rnag/wystia/
-     :alt: Updates
-
-
-
-A Python wrapper library for the Wistia API
-
-
-* Free software: MIT license
-* Documentation: https://wystia.readthedocs.io.
-* Wistia Developer Docs: https://wistia.com/support/developers.
-
-Installation
-------------
-
-The Wystia library is available `on PyPI`_, and can be installed with ``pip``:
-
-.. code-block:: shell
-
-    $ pip install wystia
-
-You'll also need to create an access token as outlined `in the docs`_.
-
-Usage
------
-
-Sample usage with the `Data API <https://wistia.com/support/developers/data-api>`_:
-
-    Note: The following example makes use of ``WistiaApi``, which is an alias to
-    the class ``WistiaDataApi``.
-
-.. code-block:: python3
-
-    from wystia import WistiaApi
-    from wystia.models import SortBy, LanguageCode, Customizations, Private
-
-    # Setup the Wistia API token to use for requests. You can alternatively
-    # set this via the env variable 'WISTIA_API_TOKEN'.
-    WistiaApi.configure('MY-TOKEN')
-
-    # Retrieve a list of all projects in the Wistia account,
-    # sorted A-Z and in ascending order.
-    projects = WistiaApi.list_all_projects(SortBy.NAME)
-    project_ids = [p.hashed_id for p in projects]
-    # Print the project data as a prettified JSON string
-    print(projects.prettify())
-
-    # Retrieve a list of videos for a Wistia project.
-    # Note: If you don't require asset info (such as ADs) on each
-    #   video, I suggest calling `list_project` instead.
-    videos = WistiaApi.list_videos('project-id')
-
-    # Retrieve info on a particular video
-    vd = WistiaApi.get_video('video-id')
-    # If the video has captions, that won't be included in the `Medias#show`
-    # response by default, so we'll need a separate API call as below.
-    # vd.process_captions(
-    #     WistiaApi.list_captions(real_video_id))
-    print(vd)
-
-    # Update attributes on a media (video), or set a custom thumbnail on the video.
-    WistiaApi.update_video(
-        'video-id',
-        thumbnail_media_id='uploaded-thumbnail-id'
-    )
-
-    # Get aggregated stats for a video, such as view count
-    stats = WistiaApi.get_stats_for_video('video-id')
-
-    # Retrieve the customization data for a video
-    customizations = WistiaApi.get_customizations('video-id')
-
-    # Update only specific customizations for a video
-    # Note the embed options are documented here:
-    #   https://wistia.com/support/developers/embed-options
-    sample_embed_options = Customizations(
-        player_color='#e7fad1',
-        # Hide comments on the media page
-        private=Private(show_comments=False)
-    )
-    WistiaApi.update_customizations('video-id', sample_embed_options)
-
-    # Get the Spanish captions on a video
-    captions = WistiaApi.get_captions('video-id', LanguageCode.SPANISH)
-
-    # Add (or replace) the English captions on a video
-    WistiaApi.update_captions(
-        'video-id',
-        LanguageCode.ENGLISH,
-        srt_file='path/to/file.srt'
-    )
-
-
-... or to upload media via the `Upload API <https://wistia.com/support/developers/upload-api>`_:
-
-.. code-block:: python3
-
-    from wystia import WistiaUploadApi
-
-    # Upload a file to a (default) project on Wistia
-    r = WistiaUploadApi.upload_file('path/to/my-file.mp4')
-    # Check if the video was successfully uploaded
-    # assert r.created
-    # assert r.name == 'my-file.mp4'
-
-    # Uploads with a public link to a video, such as
-    # an S3 pre-signed url.
-    r = WistiaUploadApi.upload_link('my-s3-link',
-                                    title='My Video Name',
-                                    description='My Description')
-
-... you can alternatively retrieve asset info via the public Media Embed link:
-
-.. code-block:: python3
-
-    from wystia import WistiaEmbedApi
-
-    # Get the media embed data
-    embed_data = WistiaEmbedApi.get_data('video-id')
-
-    # Retrieve the source URL of the original media
-    source_url = WistiaEmbedApi.asset_url(media_data=embed_data)
-
-... when using the *Data API*, the ``WistiaHelper`` can help to further simplify some calls:
-
-.. code-block:: python3
-
-    from wystia import WistiaHelper
-
-    # Check if the video exists in your Wistia account
-    assert WistiaHelper.video_exists('abc1234567')
-
-    # Check if a video's name indicates the video is an archived copy of an
-    # existing video, as discussed in the below article on replacing a media:
-    #   https://wistia.com/learn/product-updates/improved-library-management-tools
-    assert WistiaHelper.is_archived_video(
-        'My Title [Archived on August 13, 2015]')
-
-    # Update the player color on a video
-    WistiaHelper.customize_video_on_wistia('video-id', 'ffffcc')
-
-    # Individually enable captions / AD in the player for a video
-    WistiaHelper.enable_ad('video-id')
-    WistiaHelper.enable_captions('video-id', on_by_default=False)
-
-    # Disable captions / AD in the player for a video
-    if WistiaHelper.has_captions_enabled('video-id'):
-        print('Disabling captions and AD for the video')
-        WistiaHelper.disable_captions_and_ad('video-id')
-
-Getting Started
----------------
-
-Using the methods on the API classes assume your Wistia API token
-has previously been configured, for example via the environment. The API token will
-then be used globally by all the API classes when making requests to the Wistia API.
-
-You can set the following environment variable with your API token:
-
-* ``WISTIA_API_TOKEN``
-
-Another option is to use the global ``configure`` method as shown below:
-
-.. code-block:: python3
-
-    WistiaDataApi.configure('MY-API-TOKEN')
-
-There is additionally a `Quickstart`_ section in the docs which walks
-through - in more detail - how to get up and running with the
-Wystia library.
-
-Data API
---------
-
-The wrapper class ``WistiaDataApi`` (aliased to ``WistiaApi``) interacts
-with the Wistia Data API (docs below):
-
-- https://wistia.com/support/developers/data-api
-
-
-It fully implements the following sections in the API documentation:
-
-    - Paging and Sorting Responses
-    - Projects
-    - Medias
-    - Customizations
-    - Captions
-
-The following sections in the API have *not* been implemented (mainly as I haven't used them before):
-
-    - Project Sharings
-    - Account
-
-
-Tips
-~~~~
-
-Containers
-==========
-
-In general, the API methods that begin with *list* - such as ``list_project`` -
-will return a `Container`_ object, which essentially acts as a thin wrapper
-around a collection of model classes. For all intents and purposes, this behaves
-exactly the same as a ``list`` object.
-
-One of the main benefits is that it implements a ``__str__`` method, which leverages
-the builtin ``pprint`` module in Python to pretty-print the Python object representation
-of each model or *dataclass* instance; this will format the output more nicely, for example
-whenever ``print(obj)`` is called on the `Container` result.
-
-The ``Container`` objects also implement the following convenience methods, which can
-be used to easily display the JSON string representation of the list of dataclass instances:
-
-    * ``to_json`` - Convert the list of instances to a JSON string.
-
-    * ``prettify`` - Convert the list of instances to a *prettified* JSON string.
-
-List Medias in a Project
-========================
-
-If you need to retrieve info on videos in a project and you
-don't need complete info such as a list of assets for the video,
-I recommend using ``list_project`` instead of ``list_videos``. This is because
-the `Projects#show <https://wistia.com/support/developers/data-api#projects_show>`_
-API returns up to 500 results per request, whereas the ``Medias#list``
-only returns the default 100 results per page.
-
-Assuming a project in your Wistia account has a total of about 250 media, here is the number of API
-calls you might expect from each individual approach:
-
-.. code-block:: python3
-
-    from wystia import WistiaDataApi
-
-    videos = WistiaDataApi.list_videos('project-id')
-    assert WistiaDataApi.request_count() == 3
-
-    # Resets request count for the next call
-    WistiaDataApi.reset_request_count()
-
-    videos = WistiaDataApi.list_project('project-id')
-    assert WistiaDataApi.request_count() == 1
-
-
-Thread Safety
--------------
-
-The Wistia API classes are completely thread safe, since ``requests.Session``
-objects are not re-used between API calls.
-
-This means that if you have two (un-related) API operations to perform,
-such as updating a video's title and adding captions on the video,
-then you can certainly run those calls in parallel so that
-they complete a bit faster.
-
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _on PyPI: https://pypi.org/project/wystia/
-.. _in the docs: https://wistia.com/support/developers/data-api#creating-and-managing-access-tokens
-.. _Container: https://dataclass-wizard.readthedocs.io/en/latest/dataclass_wizard.html?highlight=container#dataclass_wizard.Container
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _Quickstart: https://wystia.readthedocs.io/en/latest/quickstart.html
-
-
-=======
-History
-=======
-
-1.1.0 (2022-01-27)
-------------------
-
-* Refactor any model classes that would be returned in *list* API
-  calls to subclass from ``JSONListWizard`` instead of ``JSONWizard``,
-  simply so that ``Container`` objects will be returned by default.
-
-* Refactor to import ``Container`` from the ``dataclass-wizard`` library
-  instead. For backwards compatibility reasons, the ``models`` module
-  still exports the *Container* namespace.
-
-1.0.0 (2022-01-14)
-------------------
-
-**Breaking Changes**
-
-* Wystia has officially dropped support for Python versions 3.5 and 3.6.
-  The support for 3.6 needed to be dropped primarily because of the
-  ``from __future__ import annotations`` usage in the code.
-* Refactored all API helper classes to return model class objects as a result,
-  rather than Python ``dict`` objects. In the case of any `list`- related API responses,
-  we now return a ``Container`` object so that it can be easier to print or display
-  the result for debugging purposes.
-* All inputs to the API helper methods that previously accepted a ``dict`` object,
-  have in general been refactored to accept a model dataclass instance as an input instead.
-* Renamed some error classes; for example, ``NoSuchMedia`` instead of ``NoSuchVideo``.
-* Renamed some model classes; for example, ``MediaStatus`` instead of ``VideoStatus``.
-
-**Features and Improvements**
-
-* Added ``WistiaApi`` to the list of public exports, which is aliased to the
-  ``WistiaDataApi`` helper class.
-* Added new methods to the ``WistiaDataApi`` class for more explicitly
-  interacting with *medias* instead of *videos*. For example, a ``list_medias``
-  method is added as an alternative to calling ``list_videos``.
-* Refactored the CI process to use GitHub Workflows instead of Travis CI.
-* Added *3.10* to the list of supported Python versions.
-* Updated the project status from *Beta* to *Production/Stable*.
-* Added an ``examples/`` folder in the project repo on GitHub, which
-  contains Python scripts to demonstrate sample usage.
-* Updated docs and added a new *Quickstart* section.
-
-0.3.0 (2021-07-21)
-------------------
-
-**Features and Improvements**
-
-* Add compatibility changes to extend support to Python 3.5 and 3.6
-* WistiaHelper: Add method ``project_details`` to retrieve info on a particular Wistia project
-* WistiaEmbedApi: Update to parse the ``.json`` response rather than the ``.jsonp`` version
-* Makefile: Add new command ``init``, which can be used to install Dev dependencies for the project
-
-  * Ensure the new command is compatible with Python 3.5, which has dependencies on separate
-    package versions; here we should use ``requirements-py35-dev.txt`` instead.
-* Makefile: Update ``coverage`` command to run unit tests by default
-
-**Bugfixes**
-
-* models.VideoData: The parameter to the ``process_captions`` method is now
-  correctly type-annotated to accept a ``List`` of ``Dict``
-
-0.2.1 (2021-06-17)
-------------------
-
-* WistiaHelper: Add method ``enable_captions_and_ad``
-* Remove ``.format`` usage in log statements
-* Remove an unnecessary method ``ad_needed`` from ``VideoData``
-* Update readme and Sphinx ``docs/``
-
-0.2.0 (2021-06-16)
-------------------
-
-* Fully implement all sections in the Wistia Data API
-* Add more methods to the ``WistiaHelper`` class
-* Request Count and API Token should now be globally shared by all API sub-classes
-* Lot of code refactoring
-* Exclude ``.mp4`` files from dist, to reduce total package size
-* Add more test cases
-* Update docs with better examples
-
-0.1.0 (2021-06-12)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `wystia-1.1.0/wystia.egg-info/SOURCES.txt` & `wystia-1.2.0/wystia.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 docs/modules.rst
 docs/quickstart.rst
 docs/readme.rst
 docs/usage.rst
 docs/wystia.rst
 docs/wystia.utils.parse.rst
 docs/wystia.utils.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
 tests/conftest.py
 tests/testdata/sample-captions.srt
 tests/testdata/upload_response.json
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_wystia.py
 tests/unit/utils/__init__.py
```

