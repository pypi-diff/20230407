# Comparing `tmp/razorback-0.4.3a3.tar.gz` & `tmp/razorback-0.4.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "razorback-0.4.3a3.tar", last modified: Thu Apr  6 16:16:31 2023, max compression
+gzip compressed data, was "razorback-0.4.3a4.tar", last modified: Fri Apr  7 16:15:22 2023, max compression
```

## Comparing `razorback-0.4.3a3.tar` & `razorback-0.4.3a4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.859325 razorback-0.4.3a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.847325 razorback-0.4.3a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.851325 razorback-0.4.3a3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-06 16:15:52.000000 razorback-0.4.3a3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-06 16:15:52.000000 razorback-0.4.3a3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.851325 razorback-0.4.3a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-06 16:15:52.000000 razorback-0.4.3a3/.github/workflows/continuous-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-06 16:15:52.000000 razorback-0.4.3a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-06 16:15:52.000000 razorback-0.4.3a3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 16:15:52.000000 razorback-0.4.3a3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 16:15:52.000000 razorback-0.4.3a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-06 16:16:31.859325 razorback-0.4.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-06 16:15:52.000000 razorback-0.4.3a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.851325 razorback-0.4.3a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.855325 razorback-0.4.3a3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.855325 razorback-0.4.3a3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/_static/copybutton.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.855325 razorback-0.4.3a3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/script.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.855325 razorback-0.4.3a3/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    32849 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/tutorials/handling-time-series.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   130585 2023-04-06 16:15:52.000000 razorback-0.4.3a3/docs/source/tutorials/survey-study.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-06 16:15:52.000000 razorback-0.4.3a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-06 16:15:52.000000 razorback-0.4.3a3/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 16:15:52.000000 razorback-0.4.3a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 16:16:31.859325 razorback-0.4.3a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 16:15:52.000000 razorback-0.4.3a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.847325 razorback-0.4.3a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.855325 razorback-0.4.3a3/src/razorback/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/calibrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/fourier_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.859325 razorback-0.4.3a3/src/razorback/io/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/io/ats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/io/binary_file_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/mestimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/prefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)    34897 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/signalset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-06 16:15:52.000000 razorback-0.4.3a3/src/razorback/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.859325 razorback-0.4.3a3/src/razorback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 16:16:31.000000 razorback-0.4.3a3/src/razorback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:16:31.859325 razorback-0.4.3a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-06 16:15:52.000000 razorback-0.4.3a3/tests/test_impedance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-06 16:15:52.000000 razorback-0.4.3a3/tests/test_inventory.doctest
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-06 16:15:52.000000 razorback-0.4.3a3/tests/test_merge_consecutive_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-06 16:15:52.000000 razorback-0.4.3a3/tests/test_signalset.doctest
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-06 16:15:52.000000 razorback-0.4.3a3/tests/test_tags_from_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.445056 razorback-0.4.3a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.437056 razorback-0.4.3a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-07 16:14:52.000000 razorback-0.4.3a4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-07 16:14:52.000000 razorback-0.4.3a4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-07 16:14:52.000000 razorback-0.4.3a4/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-07 16:14:52.000000 razorback-0.4.3a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-07 16:14:52.000000 razorback-0.4.3a4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 16:14:52.000000 razorback-0.4.3a4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-07 16:14:52.000000 razorback-0.4.3a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-07 16:15:22.445056 razorback-0.4.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-07 16:14:52.000000 razorback-0.4.3a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/_static/copybutton.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10544 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/script.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.441056 razorback-0.4.3a4/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    32849 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/tutorials/handling-time-series.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   130585 2023-04-07 16:14:52.000000 razorback-0.4.3a4/docs/source/tutorials/survey-study.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-07 16:14:52.000000 razorback-0.4.3a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-07 16:14:52.000000 razorback-0.4.3a4/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 16:14:52.000000 razorback-0.4.3a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:15:22.445056 razorback-0.4.3a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:14:52.000000 razorback-0.4.3a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.437056 razorback-0.4.3a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.445056 razorback-0.4.3a4/src/razorback/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/calibrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/fourier_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.445056 razorback-0.4.3a4/src/razorback/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/io/ats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/io/binary_file_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/mestimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34897 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/signalset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-07 16:14:52.000000 razorback-0.4.3a4/src/razorback/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.445056 razorback-0.4.3a4/src/razorback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 16:15:22.000000 razorback-0.4.3a4/src/razorback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:22.445056 razorback-0.4.3a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-07 16:14:52.000000 razorback-0.4.3a4/tests/test_impedance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 16:14:52.000000 razorback-0.4.3a4/tests/test_inventory.doctest
+-rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-04-07 16:14:52.000000 razorback-0.4.3a4/tests/test_merge_consecutive_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-07 16:14:52.000000 razorback-0.4.3a4/tests/test_signalset.doctest
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-07 16:14:52.000000 razorback-0.4.3a4/tests/test_tags_from_path.py
```

### Comparing `razorback-0.4.3a3/.github/ISSUE_TEMPLATE/bug_report.md` & `razorback-0.4.3a4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/.github/ISSUE_TEMPLATE/feature_request.md` & `razorback-0.4.3a4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/.github/workflows/continuous-integration.yml` & `razorback-0.4.3a4/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/LICENSE` & `razorback-0.4.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/PKG-INFO` & `razorback-0.4.3a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: razorback
-Version: 0.4.3a3
+Version: 0.4.3a4
 Summary: Robust estimation of linear response functions
 Author-email: Farid Smai <f.smai@brgm.fr>
 License: GNU GPLv3 License
 Project-URL: Homepage, https://github.com/BRGM/razorback
 Project-URL: Documentation, https://razorback.readthedocs.io
 Project-URL: Source, https://github.com/BRGM/razorback
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `razorback-0.4.3a3/README.md` & `razorback-0.4.3a4/README.md`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/Makefile` & `razorback-0.4.3a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/make.bat` & `razorback-0.4.3a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/_static/copybutton.js` & `razorback-0.4.3a4/docs/source/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/conf.py` & `razorback-0.4.3a4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/install.rst` & `razorback-0.4.3a4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/overview.rst` & `razorback-0.4.3a4/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/script.rst` & `razorback-0.4.3a4/docs/source/script.rst`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/tutorials/handling-time-series.ipynb` & `razorback-0.4.3a4/docs/source/tutorials/handling-time-series.ipynb`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/docs/source/tutorials/survey-study.ipynb` & `razorback-0.4.3a4/docs/source/tutorials/survey-study.ipynb`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/pyproject.toml` & `razorback-0.4.3a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/calibrations.py` & `razorback-0.4.3a4/src/razorback/calibrations.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/cli.py` & `razorback-0.4.3a4/src/razorback/cli.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/data.py` & `razorback-0.4.3a4/src/razorback/data.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/fourier_transform.py` & `razorback-0.4.3a4/src/razorback/fourier_transform.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/io/ats.py` & `razorback-0.4.3a4/src/razorback/io/ats.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/io/binary_file_array.py` & `razorback-0.4.3a4/src/razorback/io/binary_file_array.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/mestimator.py` & `razorback-0.4.3a4/src/razorback/mestimator.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/prefilters.py` & `razorback-0.4.3a4/src/razorback/prefilters.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         (ivid,) = np.where((cod < self._cod_min) | (cod > self._cod_max))
         return ivid
 
     def value(self, e, b):
         size = self._size
         coeff_det = self.coeff_determination
         breshape = lambda arr: arr[:len(arr)-(len(arr) % size)].reshape(
-            (divmod(len(arr), size)[0], size) + (-1,) * (arr.ndim-1)
+            (divmod(len(arr), size)[0], size) + arr.shape[1:]
         )
         cod = np.zeros(len(e))
         queue = size + (len(e) % size)
         tmp = coeff_det(breshape(e)[:-1], breshape(b)[:-1])
         breshape(cod)[:-1] = tmp[:, None]
         cod[-queue:] = coeff_det(e[None, -queue:], b[None, -queue:])
         return cod
```

### Comparing `razorback-0.4.3a3/src/razorback/signalset.py` & `razorback-0.4.3a4/src/razorback/signalset.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/utils.py` & `razorback-0.4.3a4/src/razorback/utils.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback/weights.py` & `razorback-0.4.3a4/src/razorback/weights.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/src/razorback.egg-info/PKG-INFO` & `razorback-0.4.3a4/src/razorback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: razorback
-Version: 0.4.3a3
+Version: 0.4.3a4
 Summary: Robust estimation of linear response functions
 Author-email: Farid Smai <f.smai@brgm.fr>
 License: GNU GPLv3 License
 Project-URL: Homepage, https://github.com/BRGM/razorback
 Project-URL: Documentation, https://razorback.readthedocs.io
 Project-URL: Source, https://github.com/BRGM/razorback
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `razorback-0.4.3a3/src/razorback.egg-info/SOURCES.txt` & `razorback-0.4.3a4/src/razorback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/tests/test_impedance.py` & `razorback-0.4.3a4/tests/test_impedance.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/tests/test_inventory.doctest` & `razorback-0.4.3a4/tests/test_inventory.doctest`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/tests/test_merge_consecutive_runs.py` & `razorback-0.4.3a4/tests/test_merge_consecutive_runs.py`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/tests/test_signalset.doctest` & `razorback-0.4.3a4/tests/test_signalset.doctest`

 * *Files identical despite different names*

### Comparing `razorback-0.4.3a3/tests/test_tags_from_path.py` & `razorback-0.4.3a4/tests/test_tags_from_path.py`

 * *Files identical despite different names*

