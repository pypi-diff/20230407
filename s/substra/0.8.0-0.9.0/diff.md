# Comparing `tmp/substra-0.8.0.tar.gz` & `tmp/substra-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/substra-0.8.0.tar", last modified: Thu Dec  3 18:34:33 2020, max compression
+gzip compressed data, was "/home/runner/work/substra/substra/dist/tmp8easl10b/substra-0.9.0.tar", last modified: Wed Apr 21 08:22:15 2021, max compression
```

## Comparing `substra-0.8.0.tar` & `substra-0.9.0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-12-03 18:33:33.000000 substra-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    10746 2020-12-03 18:34:33.000000 substra-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8972 2020-12-03 18:33:33.000000 substra-0.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-12-03 18:34:33.000000 substra-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1994 2020-12-03 18:33:33.000000 substra-0.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/
--rw-rw-r--   0 travis    (2000) travis    (2000)      763 2020-12-03 18:33:33.000000 substra-0.8.0/substra/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2020-12-03 18:33:33.000000 substra-0.8.0/substra/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-12-03 18:33:33.000000 substra-0.8.0/substra/cli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37535 2020-12-03 18:33:33.000000 substra-0.8.0/substra/cli/interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19313 2020-12-03 18:33:33.000000 substra-0.8.0/substra/cli/printers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-12-03 18:33:33.000000 substra-0.8.0/substra/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      797 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      921 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/assets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/sdk/backends/
--rw-rw-r--   0 travis    (2000) travis    (2000)      846 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      972 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/sdk/backends/local/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39944 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/backend.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/sdk/backends/local/compute/
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/compute/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2665 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/compute/spawner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17026 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/compute/worker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5678 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/dal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/local/db.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra/sdk/backends/remote/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/remote/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9193 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/remote/backend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8656 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/backends/remote/rest_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28795 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7311 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/compute_plan.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4085 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1384 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/hasher.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9123 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12597 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5613 2020-12-03 18:33:33.000000 substra-0.8.0/substra/sdk/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10746 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1594 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-12-03 18:34:33.000000 substra-0.8.0/substra.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-12-03 18:33:33.000000 substra-0.8.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11194 2020-12-03 18:33:33.000000 substra-0.8.0/tests/datastore.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-03 18:34:33.000000 substra-0.8.0/tests/sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3220 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4823 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_add.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      933 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_cancel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3601 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2196 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_describe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2482 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_download.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1475 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_get.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2265 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_leaderboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1927 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_rest_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1300 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/test_update.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2020-12-03 18:33:33.000000 substra-0.8.0/tests/sdk/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14511 2020-12-03 18:33:33.000000 substra-0.8.0/tests/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1934 2020-12-03 18:33:33.000000 substra-0.8.0/tests/test_printers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2020-12-03 18:33:33.000000 substra-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10761 2021-04-21 08:22:07.000000 substra-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-04-21 08:22:07.000000 substra-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12638 2021-04-21 08:22:15.000000 substra-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10840 2021-04-21 08:22:07.000000 substra-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-04-21 08:22:15.000000 substra-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2021-04-21 08:22:07.000000 substra-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2021-04-21 08:22:07.000000 substra-0.9.0/substra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2021-04-21 08:22:07.000000 substra-0.9.0/substra/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-04-21 08:22:07.000000 substra-0.9.0/substra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39201 2021-04-21 08:22:07.000000 substra-0.9.0/substra/cli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19583 2021-04-21 08:22:07.000000 substra-0.9.0/substra/cli/printers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-04-21 08:22:07.000000 substra-0.9.0/substra/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/sdk/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/sdk/backends/local/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40255 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/sdk/backends/local/compute/
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/compute/spawner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17371 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/compute/worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6681 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/dal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/local/db.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra/sdk/backends/remote/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9676 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/remote/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8732 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/backends/remote/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32191 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7311 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/compute_plan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4289 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3848 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9170 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12643 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5613 2021-04-21 08:22:07.000000 substra-0.9.0/substra/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12638 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-04-21 08:22:15.000000 substra-0.9.0/substra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-04-21 08:22:07.000000 substra-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11737 2021-04-21 08:22:07.000000 substra-0.9.0/tests/datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-21 08:22:15.000000 substra-0.9.0/tests/sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3453 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16687 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/data_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3601 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3215 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-04-21 08:22:07.000000 substra-0.9.0/tests/sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15526 2021-04-21 08:22:07.000000 substra-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2021-04-21 08:22:07.000000 substra-0.9.0/tests/test_printers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2963 2021-04-21 08:22:07.000000 substra-0.9.0/tests/test_utils.py
```

### Comparing `substra-0.8.0/PKG-INFO` & `substra-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: substra
-Version: 0.8.0
+Version: 0.9.0
 Summary: Substra CLI for interacting with substra-backend
 Home-page: https://github.com/SubstraFoundation/substra
 Author: Owkin
 Author-email: fldev@owkin.com
 License: Apache 2.0
-Description: # ![Substra](./substra-logo.svg)
+Description: <h1><img src="substra-logo.svg" alt="substra" width="200"/></h1>
         
         CLI and SDK for interacting with Substra platform.
         
         [Documentation website](https://doc.substra.ai/)
         
         ## Table of contents
         
@@ -105,17 +105,20 @@
         | substra  | substra-chaincode  | substra-backend  | substra-tests  | hlf-k8s  | substra-frontend  | substra-tools |
         |---|---|---|---|---|---| --- |
         | [`0.4.0-alpha.3`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.3) | [`0.0.8-alpha.6`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.6) | [`0.0.12-alpha.13`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.13) | [`0.2.0-alpha.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.1) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.4.0-alpha.4`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.4) | [`0.0.8-alpha.9`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.9) | [`0.0.12-alpha.20`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.20) | [`0.2.0-alpha.2`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.2) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.4.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12) | [`0.2.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0) | [`0.0.11`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.5.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.5.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.14`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.14) | [`0.3.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.3.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
         | [`0.6.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.6.0) | [`0.0.10`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.10) | [`0.0.19`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.19) | [`0.4.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.4.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.17`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.17) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
-        | [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://hub.helm.sh/charts/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-        | [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://hub.helm.sh/charts/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.1.1`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.1.1) | [`0.1.5`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.5) <br>[`helm chart 1.6.0`](https://hub.helm.sh/charts/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.15`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.15) <br>[`helm chart 5.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/5.0.1) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        | [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+        | [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://artifacthub.io/packages/helm/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.0) | [`0.1.6`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.6) <br>[`helm chart 1.6.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 5.1.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/5.1.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.2`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.2) | [`0.1.9`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.9) <br>[`helm chart 1.9.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.9.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 6.2.2`](https://artifacthub.io/packages/helm/substra/hlf-k8s/6.2.2) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+         [`0.9.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.9.0) | [`0.3.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.3.0) | [`0.1.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.12) <br>[`helm chart 2.0.3`](https://artifacthub.io/packages/helm/substra/substra-backend/2.0.3) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.1) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 7.0.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/7.0.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        
         
         **Adding entries to the compatibility table**
         
         - Please ensure that all the tests from [`substra-tests`](https://github.com/SubstraFoundation/substra-tests/) pass
         
         ```sh
         $ cd substra-tests
```

### Comparing `substra-0.8.0/README.md` & `substra-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ![Substra](./substra-logo.svg)
+<h1><img src="substra-logo.svg" alt="substra" width="200"/></h1>
 
 CLI and SDK for interacting with Substra platform.
 
 [Documentation website](https://doc.substra.ai/)
 
 ## Table of contents
 
@@ -97,17 +97,20 @@
 | substra  | substra-chaincode  | substra-backend  | substra-tests  | hlf-k8s  | substra-frontend  | substra-tools |
 |---|---|---|---|---|---| --- |
 | [`0.4.0-alpha.3`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.3) | [`0.0.8-alpha.6`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.6) | [`0.0.12-alpha.13`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.13) | [`0.2.0-alpha.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.1) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
 | [`0.4.0-alpha.4`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.4) | [`0.0.8-alpha.9`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.9) | [`0.0.12-alpha.20`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.20) | [`0.2.0-alpha.2`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.2) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
 | [`0.4.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12) | [`0.2.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0) | [`0.0.11`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
 | [`0.5.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.5.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.14`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.14) | [`0.3.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.3.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
 | [`0.6.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.6.0) | [`0.0.10`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.10) | [`0.0.19`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.19) | [`0.4.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.4.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.17`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.17) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
-| [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://hub.helm.sh/charts/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-| [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://hub.helm.sh/charts/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-| [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.1.1`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.1.1) | [`0.1.5`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.5) <br>[`helm chart 1.6.0`](https://hub.helm.sh/charts/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.15`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.15) <br>[`helm chart 5.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/5.0.1) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+| [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+| [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://artifacthub.io/packages/helm/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+| [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.0) | [`0.1.6`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.6) <br>[`helm chart 1.6.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 5.1.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/5.1.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+| [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.2`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.2) | [`0.1.9`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.9) <br>[`helm chart 1.9.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.9.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 6.2.2`](https://artifacthub.io/packages/helm/substra/hlf-k8s/6.2.2) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+ [`0.9.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.9.0) | [`0.3.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.3.0) | [`0.1.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.12) <br>[`helm chart 2.0.3`](https://artifacthub.io/packages/helm/substra/substra-backend/2.0.3) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.1) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 7.0.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/7.0.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+
 
 **Adding entries to the compatibility table**
 
 - Please ensure that all the tests from [`substra-tests`](https://github.com/SubstraFoundation/substra-tests/) pass
 
 ```sh
 $ cd substra-tests
```

### Comparing `substra-0.8.0/setup.py` & `substra-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/__init__.py` & `substra-0.9.0/substra/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/__version__.py` & `substra-0.9.0/substra/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
```

### Comparing `substra-0.8.0/substra/cli/__init__.py` & `substra-0.9.0/substra/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/cli/interface.py` & `substra-0.9.0/substra/cli/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1012,39 +1012,87 @@
     # method must exist in sdk
     method = getattr(client, f'describe_{asset_name.lower()}')
     description = method(asset_key)
     renderer = consolemd.Renderer()
     renderer.render(description)
 
 
+@cli.group()
+@click.pass_context
+def node(ctx):
+    """Display node description."""
+
+
+@node.command('info')
+@click_global_conf_with_output_format
+@click.pass_context
+@error_printer
+def node_info(ctx):
+    """Display node info."""
+    client = get_client(ctx.obj)
+    res = client.node_info()
+    printer = printers.NodeInfoPrinter()
+    printer.print(res)
+
+
 @cli.command()
 @click.argument('asset-name', type=click.Choice([
     assets.ALGO,
     assets.COMPOSITE_ALGO,
     assets.AGGREGATE_ALGO,
     assets.DATASET,
     assets.OBJECTIVE,
+    assets.MODEL
 ]))
 @click.argument('key')
 @click.option('--folder', type=click.Path(), help='destination folder',
               default='.')
+@click.option('--from-traintuple', 'model_src',
+              help=(
+                  '(model download only) if this option is set, '
+                  'the KEY argument refers to a traintuple key'
+              ),
+              flag_value='model_from_traintuple')
+@click.option('--from-aggregatetuple', 'model_src',
+              help=(
+                  '(model download only) if this option is set, '
+                  'the KEY argument refers to an aggregatetuple key'
+              ),
+              flag_value='model_from_aggregatetuple')
+@click.option('--from-composite-head', 'model_src',
+              help=(
+                  '(model download only) if this option is set, '
+                  'the KEY argument refers to a composite traintuple key'
+              ),
+              flag_value='head_model_from_composite_traintuple')
+@click.option('--from-composite-trunk', 'model_src',
+              help=(
+                  '(model download only) if this option is set, '
+                  'the KEY argument refers to a composite traintuple key'
+              ),
+              flag_value='trunk_model_from_composite_traintuple')
 @click_global_conf
 @click.pass_context
 @error_printer
-def download(ctx, asset_name, key, folder):
+def download(ctx, asset_name, key, folder, model_src):
     """Download asset implementation.
 
     \b
     - algo: the algo and its dependencies
     - dataset: the opener script
     - objective: the metrics and its dependencies
+    - model: the output model
     """
     client = get_client(ctx.obj)
-    # method must exist in sdk
-    method = getattr(client, f'download_{asset_name.lower()}')
+
+    if asset_name == assets.MODEL:
+        method = getattr(client, f'download_{model_src}' if model_src else 'download_model')
+    else:
+        method = getattr(client, f'download_{asset_name.lower()}')
+
     res = method(key, folder)
     display(res)
 
 
 @cli.command()
 @click.argument('objective_key')
 @click_option_expand
```

### Comparing `substra-0.8.0/substra/cli/printers.py` & `substra-0.9.0/substra/cli/printers.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,25 @@
         Field('Metadata', 'metadata'),
         PermissionField('Permissions', 'permissions'),
     )
 
     download_message = 'Download this algorithm\'s code:'
 
 
+class NodeInfoPrinter(BasePrinter):
+    single_fields = (
+        Field('HOST', 'host'),
+        Field('CHANNEL', 'channel'),
+        MappingField('CONFIG', 'config'),
+    )
+
+    def print(self, data):
+        self.print_details(data, self.single_fields, expand=True)
+
+
 class ComputePlanPrinter(AssetPrinter):
     asset_name = 'compute_plan'
 
     list_fields = (
         CountField('Traintuples count', 'traintuple_keys'),
         CountField('Composite traintuples count', 'composite_traintuple_keys'),
         CountField('Aggregatetuples count', 'aggregatetuple_keys'),
```

### Comparing `substra-0.8.0/substra/config.py` & `substra-0.9.0/substra/config.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/__init__.py` & `substra-0.9.0/substra/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/assets.py` & `substra-0.9.0/substra/sdk/assets.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/backends/__init__.py` & `substra-0.9.0/substra/sdk/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/backends/base.py` & `substra-0.9.0/substra/sdk/backends/base.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/backends/local/backend.py` & `substra-0.9.0/substra/sdk/backends/local/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-from pathlib import Path
 import shutil
 import typing
 import warnings
 from distutils import util
 
 import substra
 from substra.sdk import schemas, models, exceptions, fs, graph, compute_plan as compute_plan_module
@@ -29,15 +28,15 @@
 _MAX_LEN_VALUE_METADATA = 100
 DEBUG_OWNER = "debug_owner"
 
 
 class Local(base.BaseBackend):
     def __init__(self, backend, *args, **kwargs):
         self._support_chainkeys = bool(util.strtobool(os.getenv("CHAINKEYS_ENABLED", 'False')))
-        self._chainkey_dir = Path(os.getenv("CHAINKEYS_DIR", Path.home() / ".substra_chainkeys"))
+        self._chainkey_dir = compute.LOCAL_DIR / "chainkeys"
         if self._support_chainkeys:
             print(f"Chainkeys support is on, the directory is {self._chainkey_dir}")
         # create a store to abstract the db
         self._db = dal.DataAccess(backend)
         self._worker = compute.Worker(
             self._db,
             support_chainkeys=self._support_chainkeys,
@@ -945,24 +944,34 @@
             for field in url_field_path.split("."):
                 file_path = getattr(file_path, field, None)
             # Copy the file to the destination folder
             shutil.copyfile(file_path, destination)
         else:
             self._db.remote_download(asset_type, url_field_path, key, destination)
 
+    def download_model(self, key, destination_file):
+        if self._db.is_local(key):
+            asset = self._db.get(type_=schemas.Type.Model, key=key)
+            shutil.copyfile(asset.storage_address, destination_file)
+        else:
+            self._db.remote_download_model(key, destination_file)
+
     def describe(self, asset_type, key):
         if self._db.is_local(key):
             asset = self._db.get(type_=asset_type, key=key)
             if not hasattr(asset, "description") or not asset.description:
                 raise ValueError("This element does not have a description.")
             with open(asset.description.storage_address, "r", encoding="utf-8") as f:
                 return f.read()
         else:
             return self._db.get_remote_description(asset_type, key)
 
+    def node_info(self):
+        return {"type": "local backend"}
+
     def leaderboard(self, objective_key, sort='desc'):
         objective = self._db.get(schemas.Type.Objective, objective_key)
         testtuples = self._db.list(schemas.Type.Testtuple, filters=None)
         certified_testtuples = [
             self.__format_for_leaderboard(t)
             for t in testtuples
             if t.objective.key == objective_key and t.certified
```

### Comparing `substra-0.8.0/substra/sdk/backends/local/compute/spawner.py` & `substra-0.9.0/substra/sdk/backends/local/compute/spawner.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,21 @@
         self._docker = docker.from_env()
         self._user = os.getuid()
 
     def spawn(self, name, archive_path, command, volumes=None, envs=None):
         """Spawn a docker container (blocking)."""
         with tempfile.TemporaryDirectory() as tmpdir:
             _uncompress(archive_path, tmpdir)
-            self._docker.images.build(path=tmpdir, tag=name, rm=True)
+            try:
+                self._docker.images.build(path=tmpdir, tag=name, rm=True)
+            except docker.errors.BuildError as exc:
+                for line in exc.build_log:
+                    if 'stream' in line:
+                        print(line['stream'].strip())
+                raise
 
         container = self._docker.containers.run(
             name,
             command=command,
             volumes=volumes or {},
             environment=envs,
             remove=False,
```

### Comparing `substra-0.8.0/substra/sdk/backends/local/compute/worker.py` & `substra-0.9.0/substra/sdk/backends/local/compute/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 import shutil
 import uuid
 
 from substra.sdk import schemas, fs, models
 from substra.sdk.backends.local import dal
 from substra.sdk.backends.local.compute import spawner
 
+LOCAL_DIR = pathlib.Path.cwd() / "local-worker"
+
 _CONTAINER_MODEL_PATH = "/sandbox/model"
 
 _VOLUME_INPUT_DATASAMPLES = {"bind": "/sandbox/data", "mode": "ro"}
 _VOLUME_MODELS_RO = {"bind": _CONTAINER_MODEL_PATH, "mode": "ro"}
 _VOLUME_MODELS_RW = {"bind": _CONTAINER_MODEL_PATH, "mode": "rw"}
 _VOLUME_OPENER = {"bind": "/sandbox/opener/__init__.py", "mode": "ro"}
 _VOLUME_OUTPUT_PRED = {"bind": "/sandbox/pred", "mode": "rw"}
 _VOLUME_LOCAL = {"bind": "/sandbox/local", "mode": "rw"}
-_VOLUME_LOCAL_READ_ONLY = {"bind": "/sandbox/local", "mode": "ro"}
 _VOLUME_CHAINKEYS = {"bind": "/sandbox/chainkeys", "mode": "rw"}
 
 _VOLUME_INPUT_MODELS_RO = {"bind": "/sandbox/input_models", "mode": "ro"}
 _VOLUME_OUTPUT_MODELS_RW = {"bind": "/sandbox/output_models", "mode": "rw"}
 
 
 def _mkdir(path, delete_if_exists=False):
@@ -51,15 +52,15 @@
     return pathlib.Path(os.path.join(volume, model_key).replace(volume, container_volume["bind"]))
 
 
 class Worker:
     """ML Worker."""
 
     def __init__(self, db: dal.DataAccess, support_chainkeys: bool, chainkey_dir=None):
-        self._wdir = os.path.join(os.getcwd(), "local-worker")
+        self._wdir = LOCAL_DIR
         self._db = db
         self._spawner = spawner.get()
         self._support_chainkeys = support_chainkeys
         self._chainkey_dir = chainkey_dir
 
     def _get_owner(self, tuple_):
         if isinstance(tuple_, models.Aggregatetuple):
@@ -101,15 +102,16 @@
         return data_volume
 
     def _save_output_model(self, tuple_, model_name, models_volume) -> models.OutModel:
         tmp_path = os.path.join(models_volume, model_name)
         model_dir = _mkdir(os.path.join(self._wdir, "models", tuple_.key))
         model_path = os.path.join(model_dir, model_name)
         shutil.copy(tmp_path, model_path)
-        return models.OutModel(key=str(uuid.uuid4()), checksum=fs.hash_file(model_path),
+        return models.OutModel(key=self._db.get_local_key(str(uuid.uuid4())),
+                               checksum=fs.hash_file(model_path),
                                storage_address=model_path)
 
     def _get_command_models_composite(self, is_train, tuple_, models_volume, container_volume):
         command = ""
         model_head_key = None
         model_trunk_key = None
         if not is_train:
@@ -197,17 +199,18 @@
                 volumes[dataset.opener.storage_address] = _VOLUME_OPENER
                 if self._db.is_local(tuple_.dataset.key):
                     data_volume = self._get_data_volume(tuple_dir, tuple_)
                     volumes[data_volume] = _VOLUME_INPUT_DATASAMPLES
 
             if tuple_.compute_plan_key:
                 #  Shared compute plan volume
+                owner = self._get_owner(tuple_)
                 local_volume = _mkdir(
                     os.path.join(
-                        self._wdir, "compute_plans", "local", tuple_.compute_plan_key
+                        self._wdir, "compute_plans", owner, tuple_.compute_plan_key
                     )
                 )
                 volumes[local_volume] = _VOLUME_LOCAL
                 if self._support_chainkeys:
                     chainkey_volume = self._get_chainkey_volume(tuple_)
                     if chainkey_volume is not None:
                         volumes[chainkey_volume] = _VOLUME_CHAINKEYS
@@ -312,17 +315,18 @@
 
             # If use fake data, no data volume
             if self._db.is_local(dataset.key):
                 data_volume = self._get_data_volume(tuple_dir, tuple_)
                 volumes[data_volume] = _VOLUME_INPUT_DATASAMPLES
 
             if tuple_.compute_plan_key:
+                owner = self._get_owner(tuple_)
                 local_volume = _mkdir(
                     os.path.join(
-                        self._wdir, "compute_plans", "local", tuple_.compute_plan_key
+                        self._wdir, "compute_plans", owner, tuple_.compute_plan_key
                     )
                 )
                 volumes[local_volume] = _VOLUME_LOCAL
                 if self._support_chainkeys:
                     chainkey_volume = self._get_chainkey_volume(tuple_)
                     volumes[chainkey_volume] = _VOLUME_CHAINKEYS
 
@@ -376,16 +380,21 @@
             # Calculate the metrics
             volumes = {
                 predictions_volume: _VOLUME_OUTPUT_PRED,
                 dataset.opener.storage_address: _VOLUME_OPENER,
             }
 
             if self._db.is_local(dataset.key):
+                data_sample_paths = self._get_data_sample_paths_arg(
+                    _VOLUME_INPUT_DATASAMPLES['bind'],
+                    tuple_.dataset
+                )
                 volumes[data_volume] = _VOLUME_INPUT_DATASAMPLES
                 command = "--fake-data-mode DISABLED"
+                command += f" --data-sample-paths {data_sample_paths}"
             else:
                 command = "--fake-data-mode FAKE_Y"
                 command += f" --n-fake-samples {len(tuple_.dataset.data_sample_keys)}"
 
             container_name = 'metrics_run_local'
             logs_predict = self._spawner.spawn(
                 container_name,
```

### Comparing `substra-0.8.0/substra/sdk/backends/local/dal.py` & `substra-0.9.0/substra/sdk/backends/local/dal.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 
     def add(self, asset):
         return self._db.add(asset)
 
     def remote_download(self, asset_type, url_field_path, key, destination):
         self._remote.download(asset_type, url_field_path, key, destination)
 
+    def remote_download_model(self, key, destination_file):
+        self._remote.download_model(key, destination_file)
+
     def get_remote_description(self, asset_type, key):
         return self._remote.describe(asset_type, key)
 
     def get_with_files(self, type_: schemas.Type, key: str):
         """Get the asset with files on the local disk for execution.
         This does not load the description as it is not required for execution.
         """
@@ -112,15 +115,18 @@
 
             attr = getattr(asset, field_name)
             attr.storage_address = asset_path
             return asset
 
     def get(self, type_, key: str, log: bool = True):
         if self.is_local(key):
-            return self._db.get(type_, key, log)
+            if type_ == schemas.Type.Model:
+                return self._get_local_model(key)
+            else:
+                return self._db.get(type_, key, log)
         elif self._remote:
             return self._remote.get(type_, key)
         else:
             # TODO: better error that says do not have a remote ?
             raise exceptions.NotFound(f"Wrong pk {key}", 404)
 
     def list(self, type_, filters):
@@ -169,7 +175,25 @@
                 f"Could not copy {file_path}",
                 400
             )
         return tmp_file
 
     def update(self, asset):
         return self._db.update(asset)
+
+    def _get_local_model(self, key):
+
+        for t in self.list(schemas.Type.Traintuple, filters=None):
+            if t.out_model and t.out_model.key == key:
+                return t.out_model
+
+        for t in self.list(schemas.Type.CompositeTraintuple, filters=None):
+            if t.out_head_model.out_model and t.out_head_model.out_model.key == key:
+                return t.out_head_model.out_model
+            if t.out_trunk_model.out_model and t.out_trunk_model.out_model.key == key:
+                return t.out_trunk_model.out_model
+
+        for t in self.list(schemas.Type.Aggregatetuple, filters=None):
+            if t.out_model and t.out_model.key == key:
+                return t.out_model
+
+        raise exceptions.NotFound(f"Wrong pk {key}", 404)
```

### Comparing `substra-0.8.0/substra/sdk/backends/local/db.py` & `substra-0.9.0/substra/sdk/backends/local/db.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/backends/remote/backend.py` & `substra-0.9.0/substra/sdk/backends/remote/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -231,20 +231,32 @@
         chunk_size = 1024
         with open(destination, 'wb') as f:
             for chunk in response.iter_content(chunk_size):
                 f.write(chunk)
 
         return destination
 
+    def download_model(self, key, destination_file):
+        response = self._client.get_data(f'{self._client.base_url}/model/{key}/file/', stream=True)
+        chunk_size = 1024
+        with open(destination_file, 'wb') as f:
+            for chunk in response.iter_content(chunk_size):
+                f.write(chunk)
+        return destination_file
+
     def describe(self, asset_type, key):
         data = self.get(asset_type, key)
         url = data.description.storage_address
         r = self._client.get_data(url)
         return r.text
 
+    def node_info(self):
+        response = self._client.get_data(f'{self._client.base_url}/info/')
+        return response.json()
+
     def leaderboard(self, objective_key, sort='desc'):
         return self._client.request(
             'get',
             schemas.Type.Objective.to_server(),
             f'{objective_key}/leaderboard',
             params={'sort': sort},
         )
```

### Comparing `substra-0.8.0/substra/sdk/backends/remote/rest_client.py` & `substra-0.9.0/substra/sdk/backends/remote/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Client():
     """REST Client to communicate with Substra server."""
 
+    @property
+    def base_url(self) -> str:
+        return self._base_url
+
     def __init__(self, url, insecure, token):
         self._default_kwargs = {
             'verify': not insecure,
         }
         self._headers = {
             'Authorization': f"Token {token}",
             'Accept': 'application/json;version=0.0',
@@ -130,29 +134,29 @@
             if e.response.status_code in [502, 503, 504]:
                 raise exceptions.GatewayUnavailable.from_request_exception(e)
 
             raise exceptions.HTTPError.from_request_exception(e)
 
         return r
 
+    @utils.retry_on_exception(exceptions=(exceptions.GatewayUnavailable))
     def _request(self, request_name, url, **request_kwargs):
         """Wrapper to __request to emit a log for each HTTP request."""
         ts = time.time()
         error = None
         try:
             return self.__request(request_name, url, **request_kwargs)
         except Exception as e:
             error = e.__class__.__name__
             raise
         finally:
             te = time.time()
             elaps = (te - ts) * 1000
             logger.debug(f'{request_name} {url}: done in {elaps:.2f}ms error={error}')
 
-    @utils.retry_on_exception(exceptions=(exceptions.GatewayUnavailable))
     def request(self, request_name, asset_name, path=None, json_response=True,
                 **request_kwargs):
         """Base request."""
 
         path = path or ''
         url = f"{self._base_url}/{asset_name}/{path}"
         if not url.endswith("/"):
```

### Comparing `substra-0.8.0/substra/sdk/client.py` & `substra-0.9.0/substra/sdk/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -626,15 +626,15 @@
             batch_size (int, optional): If 'auto_batching' is True, change `batch_size`
                 to define the number of tuples uploaded in each batch (default 20).
 
         Returns:
             models.ComputePlan: updated compute plan, as described in the
             [models.ComputePlan](sdk_models.md#ComputePlan) model
         """
-        spec = schemas.UpdateComputePlanSpec(**data)
+        spec = self._get_spec(schemas.UpdateComputePlanSpec, data)
         spec_options = {
             "auto_batching": auto_batching,
             "batch_size": batch_size,
         }
         return self._backend.update_compute_plan(
             key,
             spec,
@@ -718,14 +718,88 @@
             schemas.Type.Objective,
             'metrics.storage_address',
             key,
             os.path.join(destination_folder, 'metrics.py'),
         )
 
     @logit
+    def download_model(self, key: str, folder) -> None:
+        """Download model to destination file.
+
+        This model was saved using the 'save_model' function of the algorithm.
+        To load and use the model, please refer to the 'load_model' and 'predict' functions of the
+        algorithm.
+        """
+        self._backend.download_model(key, os.path.join(folder, f'model_{key}'))
+
+    @logit
+    def download_model_from_traintuple(self, tuple_key: str, folder) -> None:
+        """Download traintuple model to destination file.
+
+        This model was saved using the 'save_model' function of the algorithm.
+        To load and use the model, please refer to the 'load_model' and 'predict' functions of the
+        algorithm.
+        """
+        self._download_model_from_tuple(schemas.Type.Traintuple, tuple_key, folder)
+
+    @logit
+    def download_model_from_aggregatetuple(self, tuple_key: str, folder) -> None:
+        """Download aggregatetuple model to destination file.
+
+        This model was saved using the 'save_model' function of the algorithm.
+        To load and use the model, please refer to the 'load_model' and 'predict' functions of the
+        algorithm.
+        """
+        self._download_model_from_tuple(schemas.Type.Aggregatetuple, tuple_key, folder)
+
+    @logit
+    def download_head_model_from_composite_traintuple(self, tuple_key: str, folder) -> None:
+        """Download composite traintuple head model to destination file.
+
+        This model was saved using the 'save_model' function of the algorithm.
+        To load and use the model, please refer to the 'load_model' and 'predict' functions of the
+        algorithm.
+        """
+        self._download_model_from_tuple(schemas.Type.CompositeTraintuple, tuple_key, folder, "head")
+
+    @logit
+    def download_trunk_model_from_composite_traintuple(self, tuple_key: str, folder) -> None:
+        """Download composite traintuple trunk model to destination file.
+
+        This model was saved using the 'save_model' function of the algorithm.
+        To load and use the model, please refer to the 'load_model' and 'predict' functions of the
+        algorithm.
+        """
+        self._download_model_from_tuple(schemas.Type.CompositeTraintuple, tuple_key, folder,
+                                        "trunk")
+
+    def _download_model_from_tuple(self, tuple_type, tuple_key, folder, head_trunk=None) -> None:
+        """Download model to a destination file."""
+        tuple = self._backend.get(tuple_type, tuple_key)
+
+        if tuple_type == schemas.Type.CompositeTraintuple:
+            if head_trunk == "head":
+                model = tuple.out_head_model.out_model
+            elif head_trunk == "trunk":
+                model = tuple.out_trunk_model.out_model
+            else:
+                raise exceptions.InvalidRequest(
+                    'head_trunk parameter must have value "head" or "trunk"'
+                )
+        else:
+            model = tuple.out_model
+
+        if not model:
+            desc = f'{head_trunk} ' if head_trunk else ""
+            msg = f'{tuple_type} {tuple_key}, status "{tuple.status}" has no {desc}out-model'
+            raise exceptions.NotFound(msg, 404)
+
+        self.download_model(model.key, folder)
+
+    @logit
     def describe_algo(self, key: str) -> str:
         """Get algo description."""
         return self._backend.describe(schemas.Type.Algo, key)
 
     @logit
     def describe_aggregate_algo(self, key: str) -> str:
         """Get aggregate algo description."""
@@ -743,14 +817,19 @@
 
     @logit
     def describe_objective(self, key: str) -> str:
         """Get objective description."""
         return self._backend.describe(schemas.Type.Objective, key)
 
     @logit
+    def node_info(self) -> str:
+        """Get node information."""
+        return self._backend.node_info()
+
+    @logit
     def leaderboard(self, objective_key: str, sort: str = 'desc') -> str:
         """Get objective leaderboard"""
         return self._backend.leaderboard(objective_key, sort='desc')
 
     @logit
     def cancel_compute_plan(self, key: str) -> models.ComputePlan:
         """Cancel execution of compute plan, the returned object is described
```

### Comparing `substra-0.8.0/substra/sdk/compute_plan.py` & `substra-0.9.0/substra/sdk/compute_plan.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/config.py` & `substra-0.9.0/substra/sdk/config.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/exceptions.py` & `substra-0.9.0/substra/sdk/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 class RequestException(SDKException):
     def __init__(self, msg, status_code):
         self.msg = msg
         self.status_code = status_code
         super().__init__(msg)
 
     @classmethod
-    def from_request_exception(cls, request_exception, msg=None):
-        if msg is None:
-            msg = str(request_exception)
-        else:
+    def from_request_exception(cls, request_exception):
+        msg = None
+        try:
+            msg = request_exception.response.json()['message']
             msg = f"{request_exception}: {msg}"
+        except Exception:
+            msg = str(request_exception)
 
         try:
             status_code = request_exception.response.status_code
         except AttributeError:
             status_code = None
 
         return cls(msg, status_code)
@@ -69,15 +71,20 @@
 
     @classmethod
     def from_request_exception(cls, request_exception):
         try:
             error = request_exception.response.json()
         except ValueError:
             error = request_exception.response
-        msg = error.get("message", str(error))
+
+        get_method = getattr(error, "get", None)
+        if callable(get_method):
+            msg = get_method("message", str(error))
+        else:
+            msg = str(error)
 
         try:
             status_code = request_exception.response.status_code
         except AttributeError:
             status_code = None
 
         return cls(msg, status_code, error)
```

### Comparing `substra-0.8.0/substra/sdk/fs.py` & `substra-0.9.0/substra/sdk/fs.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/graph.py` & `substra-0.9.0/substra/sdk/graph.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra/sdk/models.py` & `substra-0.9.0/substra/sdk/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,16 @@
 class OutModel(schemas._PydanticConfig):
     """Out model of a traintuple, aggregate tuple or out trunk
     model of a composite traintuple"""
     key: str
     checksum: str
     storage_address: UriPath
 
+    type_: ClassVar[str] = schemas.Type.Model
+
 
 class _TraintupleAlgo(schemas._PydanticConfig):
     """Algo associated to a traintuple"""
     key: str
     checksum: str
     storage_address: UriPath
     name: str
```

### Comparing `substra-0.8.0/substra/sdk/schemas.py` & `substra-0.9.0/substra/sdk/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
     ) -> "TraintupleSpec":
         return TraintupleSpec(
             algo_key=spec.algo_key,
             data_manager_key=spec.data_manager_key,
             train_data_sample_keys=spec.train_data_sample_keys,
             in_models_keys=[
                 id_to_key[parent_id] for parent_id in spec.in_models_ids
-            ],
+            ] if spec.in_models_ids is not None else list(),
             tag=spec.tag,
             compute_plan_key=compute_plan_key,
             rank=rank,
             metadata=spec.metadata
         )
```

### Comparing `substra-0.8.0/substra/sdk/utils.py` & `substra-0.9.0/substra/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/substra.egg-info/PKG-INFO` & `substra-0.9.0/substra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: substra
-Version: 0.8.0
+Version: 0.9.0
 Summary: Substra CLI for interacting with substra-backend
 Home-page: https://github.com/SubstraFoundation/substra
 Author: Owkin
 Author-email: fldev@owkin.com
 License: Apache 2.0
-Description: # ![Substra](./substra-logo.svg)
+Description: <h1><img src="substra-logo.svg" alt="substra" width="200"/></h1>
         
         CLI and SDK for interacting with Substra platform.
         
         [Documentation website](https://doc.substra.ai/)
         
         ## Table of contents
         
@@ -105,17 +105,20 @@
         | substra  | substra-chaincode  | substra-backend  | substra-tests  | hlf-k8s  | substra-frontend  | substra-tools |
         |---|---|---|---|---|---| --- |
         | [`0.4.0-alpha.3`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.3) | [`0.0.8-alpha.6`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.6) | [`0.0.12-alpha.13`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.13) | [`0.2.0-alpha.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.1) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.4.0-alpha.4`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0-alpha.4) | [`0.0.8-alpha.9`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8-alpha.9) | [`0.0.12-alpha.20`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12-alpha.20) | [`0.2.0-alpha.2`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0-alpha.2) | [`0.0.11-alpha.1`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11-alpha.1) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.4.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.4.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.12) | [`0.2.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.2.0) | [`0.0.11`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.11) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | |
         | [`0.5.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.5.0) | [`0.0.8`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.8) | [`0.0.14`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.14) | [`0.3.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.3.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.16`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.16) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
         | [`0.6.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.6.0) | [`0.0.10`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.10) | [`0.0.19`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.0.19) | [`0.4.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.4.0) | [`0.0.12`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.12) | [`0.0.17`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.17) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.5.0) |
-        | [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://hub.helm.sh/charts/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-        | [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://hub.helm.sh/charts/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
-        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.1.1`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.1.1) | [`0.1.5`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.5) <br>[`helm chart 1.6.0`](https://hub.helm.sh/charts/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.15`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.15) <br>[`helm chart 5.0.1`](https://hub.helm.sh/charts/substra/hlf-k8s/5.0.1) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://hub.helm.sh/charts/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        | [`0.7.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.0) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.2`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.2) <br>[`helm chart 1.4.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.4.0) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+        | [`0.7.1`](https://github.com/SubstraFoundation/substra/releases/tag/0.7.1) | [`0.0.11`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.0.11) | [`0.1.3`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.3) <br>[`helm chart 1.5.1`](https://artifacthub.io/packages/helm/substra/substra-backend/1.5.1) | [`0.5.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.5.0) | [`0.0.13`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.13) <br>[`helm chart 3.0.1`](https://artifacthub.io/packages/helm/substra/hlf-k8s/3.0.1) | [`0.0.19`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.19) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.6.1) |
+        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.0) | [`0.1.6`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.6) <br>[`helm chart 1.6.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.6.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 5.1.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/5.1.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        | [`0.8.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.8.0) | [`0.2.2`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.2.2) | [`0.1.9`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.9) <br>[`helm chart 1.9.0`](https://artifacthub.io/packages/helm/substra/substra-backend/1.9.0) | [`0.6.0`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.0) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 6.2.2`](https://artifacthub.io/packages/helm/substra/hlf-k8s/6.2.2) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+         [`0.9.0`](https://github.com/SubstraFoundation/substra/releases/tag/0.9.0) | [`0.3.0`](https://github.com/SubstraFoundation/substra-chaincode/releases/tag/0.3.0) | [`0.1.12`](https://github.com/SubstraFoundation/substra-backend/releases/tag/0.1.12) <br>[`helm chart 2.0.3`](https://artifacthub.io/packages/helm/substra/substra-backend/2.0.3) | [`0.6.1`](https://github.com/SubstraFoundation/substra-tests/releases/tag/0.6.1) | [`0.0.16`](https://github.com/SubstraFoundation/hlf-k8s/releases/tag/0.0.16) <br>[`helm chart 7.0.0`](https://artifacthub.io/packages/helm/substra/hlf-k8s/7.0.0) | [`0.0.20`](https://github.com/SubstraFoundation/substra-frontend/releases/tag/0.0.20) <br>[`helm chart 1.0.0-alpha.2`](https://artifacthub.io/packages/helm/substra/substra-frontend/1.0.0-alpha.2) | [`0.7.0`](https://github.com/SubstraFoundation/substra-tools/releases/tag/0.7.0) |
+        
         
         **Adding entries to the compatibility table**
         
         - Please ensure that all the tests from [`substra-tests`](https://github.com/SubstraFoundation/substra-tests/) pass
         
         ```sh
         $ cd substra-tests
```

### Comparing `substra-0.8.0/substra.egg-info/SOURCES.txt` & `substra-0.9.0/substra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 substra/__init__.py
 substra/__version__.py
 substra/config.py
@@ -42,14 +43,15 @@
 tests/__init__.py
 tests/datastore.py
 tests/test_cli.py
 tests/test_printers.py
 tests/test_utils.py
 tests/sdk/__init__.py
 tests/sdk/conftest.py
+tests/sdk/data_factory.py
 tests/sdk/test_add.py
 tests/sdk/test_cancel.py
 tests/sdk/test_config.py
 tests/sdk/test_debug.py
 tests/sdk/test_describe.py
 tests/sdk/test_download.py
 tests/sdk/test_get.py
```

### Comparing `substra-0.8.0/tests/__init__.py` & `substra-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/datastore.py` & `substra-0.9.0/tests/datastore.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,15 +158,19 @@
             "03a1f878-768e-a862-4942-d46a3b438c37"
         ],
         "opener_checksum": "8dd01465003a9b1e01c99c904d86aa518b3a5dd9dc8d40fe7d075c726ac073ca",
     },
     "compute_plan_key": "",
     "in_models": None,
     "log": "[00-01-0032-d415995]",
-    "out_model": None,
+    "out_model": {
+        "key": "11a1f878-768e-a862-4942-d46a3b438c37",
+        "checksum": "8dd01465003a9b1e01c99c904d86aa518b3a5dd9dc8d40fe7d075c726ac073ca",
+        "storage_address": ""
+    },
     "permissions": {
         "process": {
             "public": False,
             "authorized_ids": []
         }
     },
     "rank": 0,
@@ -185,15 +189,19 @@
         "checksum": "0acc5180e09b6a6ac250f4f3c172e2893f617aa1c22ef1f379019d20fe44142f",
         "storage_address": ""
     },
     "creator": "e75db4df2532dc1313ebb5c2462f1eb813b94c3e67de29f6e4b2272ae60385f5",
     "compute_plan_key": "",
     "in_models": [],
     "log": "[00-01-0032-d415995]",
-    "out_model": None,
+    "out_model": {
+        "key": "11a1f878-768e-a862-4942-d46a3b438c37",
+        "checksum": "8dd01465003a9b1e01c99c904d86aa518b3a5dd9dc8d40fe7d075c726ac073ca",
+        "storage_address": ""
+    },
     "permissions": {
         "process": {
             "public": False,
             "authorized_ids": []
         }
     },
     "rank": 0,
@@ -360,7 +368,13 @@
         "62378ca1b5c84e73a3d588adab7e20b2":
         "1197bbfc-4a18-9ea0-37a6-835895a81bb8",
     },
     "metadata": {
         "foo": "bar"
     }
 }
+
+MODEL = {
+    "key": "8a90514f-88c7-0002-608a-9868681dd158",
+    "checksum": "8a90514f88c70002608a9868681dd1589ea598e78d00a8cd7783c3ea0f9ceb09",
+    "storage_address": "/some/path/model",
+}
```

### Comparing `substra-0.8.0/tests/sdk/__init__.py` & `substra-0.9.0/tests/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/conftest.py` & `substra-0.9.0/tests/sdk/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 
 import substra
+from . import data_factory
 
 
 def pytest_configure(config):
     config.addinivalue_line(
         "markers", "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     )
 
@@ -109,7 +110,17 @@
         paths.append(str(data_sample_dir_path))
 
     return {
         "paths": paths,
         "data_manager_keys": ["42"],
         "test_only": False,
     }
+
+
+@pytest.fixture(scope="session")
+def asset_factory():
+    return data_factory.AssetsFactory("test_debug")
+
+
+@pytest.fixture()
+def data_sample(asset_factory):
+    return asset_factory.create_data_sample()
```

### Comparing `substra-0.8.0/tests/sdk/test_add.py` & `substra-0.9.0/tests/sdk/test_add.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_cancel.py` & `substra-0.9.0/tests/sdk/test_cancel.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_config.py` & `substra-0.9.0/tests/sdk/test_config.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_describe.py` & `substra-0.9.0/tests/sdk/test_describe.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_download.py` & `substra-0.9.0/tests/sdk/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,70 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import os
-
 import substra
+from substra.sdk import models, schemas
 
 from .. import datastore
-from .utils import mock_requests_responses, mock_requests, mock_response
+from .utils import mock_requests
 
 
-@pytest.mark.parametrize(
-    'asset_name, filename', [
-        ('dataset', 'opener.py'),
-        ('algo', 'algo.tar.gz'),
-        ('aggregate_algo', 'aggregate_algo.tar.gz'),
-        ('composite_algo', 'composite_algo.tar.gz'),
-        ('objective', 'metrics.py')
-    ]
-)
-def test_download_asset(asset_name, filename, tmp_path, client, mocker):
+@pytest.mark.parametrize('asset_name', [
+    'objective',
+    'dataset',
+    'algo',
+    'aggregate_algo',
+    'composite_algo',
+    'testtuple',
+    'traintuple',
+    'aggregatetuple',
+    'composite_traintuple',
+    'compute_plan',
+])
+def test_get_asset(asset_name, client, mocker):
     item = getattr(datastore, asset_name.upper())
-    responses = [
-        mock_response(item),  # metadata
-        mock_response('foo'),  # data
-    ]
-    m = mock_requests_responses(mocker, 'get', responses)
-
-    method = getattr(client, f'download_{asset_name}')
-    method("foo", tmp_path)
-
-    temp_file = str(tmp_path) + '/' + filename
-    assert os.path.exists(temp_file)
-    m.assert_called()
-
+    method = getattr(client, f'get_{asset_name}')
 
-@pytest.mark.parametrize(
-    'asset_name', ['dataset', 'algo', 'aggregate_algo', 'composite_algo', 'objective']
-)
-def test_download_asset_not_found(asset_name, tmp_path, client, mocker):
-    m = mock_requests(mocker, "get", status=404)
+    m = mock_requests(mocker, "get", response=item)
 
-    with pytest.raises(substra.sdk.exceptions.NotFound):
-        method = getattr(client, f'download_{asset_name}')
-        method('foo', tmp_path)
+    response = method("magic-key")
 
-    assert m.call_count == 1
+    assert response == models.SCHEMA_TO_MODEL[schemas.Type(asset_name)](**item)
+    m.assert_called()
 
 
-@pytest.mark.parametrize(
-    'asset_name', ['dataset', 'algo', 'aggregate_algo', 'composite_algo', 'objective']
-)
-def test_download_content_not_found(asset_name, tmp_path, client, mocker):
-    item = getattr(datastore, asset_name.upper())
-    responses = [
-        mock_response(item),  # metadata
-        mock_response('foo', status=404),  # description
-    ]
-    m = mock_requests_responses(mocker, 'get', responses)
-
-    method = getattr(client, f'download_{asset_name}')
+def test_get_asset_not_found(client, mocker):
+    mock_requests(mocker, "get", status=404)
 
     with pytest.raises(substra.sdk.exceptions.NotFound):
-        method("key", tmp_path)
-
-    assert m.call_count == 2
+        client.get_dataset("magic-key")
```

### Comparing `substra-0.8.0/tests/sdk/test_get.py` & `substra-0.9.0/tests/sdk/test_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,44 +8,47 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-import substra
 from substra.sdk import models, schemas
 
 from .. import datastore
 from .utils import mock_requests
 
 
-@pytest.mark.parametrize('asset_name', [
-    'objective',
-    'dataset',
-    'algo',
-    'aggregate_algo',
-    'composite_algo',
-    'testtuple',
-    'traintuple',
-    'aggregatetuple',
-    'composite_traintuple',
-    'compute_plan',
-])
-def test_get_asset(asset_name, client, mocker):
-    item = getattr(datastore, asset_name.upper())
-    method = getattr(client, f'get_{asset_name}')
+def test_update_dataset(client, mocker):
+    m = mock_requests(mocker, "post", response={"key": "dataset_key"})
 
-    m = mock_requests(mocker, "get", response=item)
+    response = client.link_dataset_with_objective(
+        'a key',
+        'an another key',
+    )
 
-    response = method("magic-key")
-
-    assert response == models.SCHEMA_TO_MODEL[schemas.Type(asset_name)](**item)
+    assert response == "dataset_key"
     m.assert_called()
 
 
-def test_get_asset_not_found(client, mocker):
-    mock_requests(mocker, "get", status=404)
+def test_update_compute_plan(client, mocker):
+    item = datastore.COMPUTE_PLAN
+    m = mock_requests(mocker, "post", response=item)
+    m_get = mock_requests(mocker, "get", response=datastore.COMPUTE_PLAN)
+
+    response = client.update_compute_plan('foo', {})
+
+    assert response == models.ComputePlan(**item)
+    m.assert_called
+    m_get.assert_called
+
+
+def test_update_compute_plan_with_schema(client, mocker):
+    item = datastore.COMPUTE_PLAN
+    m = mock_requests(mocker, "post", response=item)
+    m_get = mock_requests(mocker, "get", response=datastore.COMPUTE_PLAN)
+
+    response = client.update_compute_plan('foo', schemas.UpdateComputePlanSpec())
 
-    with pytest.raises(substra.sdk.exceptions.NotFound):
-        client.get_dataset("magic-key")
+    assert response == models.ComputePlan(**item)
+    m.assert_called
+    m_get.assert_called
```

### Comparing `substra-0.8.0/tests/sdk/test_graph.py` & `substra-0.9.0/tests/sdk/test_graph.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_leaderboard.py` & `substra-0.9.0/tests/sdk/test_leaderboard.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_list.py` & `substra-0.9.0/tests/sdk/test_list.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/test_rest_client.py` & `substra-0.9.0/tests/sdk/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/sdk/utils.py` & `substra-0.9.0/tests/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/test_cli.py` & `substra-0.9.0/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -318,14 +318,48 @@
 
 def test_command_download(workdir, mocker):
     m = mock_client_call(mocker, 'download_objective')
     client_execute(workdir, ['download', 'objective', 'fakekey'])
     m.assert_called()
 
 
+def test_command_download_model(workdir, mocker):
+    m = mock_client_call(mocker, 'download_model')
+    client_execute(workdir, ['download', 'model', 'fakekey'])
+    m.assert_called()
+
+    m = mock_client_call(mocker, 'download_model_from_traintuple')
+    client_execute(
+        workdir,
+        ['download', 'model', '--from-traintuple', 'fakekey']
+    )
+    m.assert_called()
+
+    m = mock_client_call(mocker, 'download_model_from_aggregatetuple')
+    client_execute(
+        workdir,
+        ['download', 'model', '--from-aggregatetuple', 'fakekey']
+    )
+    m.assert_called()
+
+    m = mock_client_call(mocker, 'download_head_model_from_composite_traintuple')
+    client_execute(
+        workdir,
+        ['download', 'model', '--from-composite-head', 'fakekey']
+    )
+    m.assert_called()
+
+    m = mock_client_call(mocker, 'download_trunk_model_from_composite_traintuple')
+    client_execute(
+        workdir,
+        ['download', 'model', '--from-composite-trunk', 'fakekey']
+    )
+    m.assert_called()
+
+
 def test_command_cancel_compute_plan(workdir, mocker):
     m = mock_client_call(
         mocker,
         'cancel_compute_plan',
         models.ComputePlan(**datastore.COMPUTE_PLAN)
     )
     client_execute(workdir, ['cancel', 'compute_plan', 'fakekey'])
```

### Comparing `substra-0.8.0/tests/test_printers.py` & `substra-0.9.0/tests/test_printers.py`

 * *Files identical despite different names*

### Comparing `substra-0.8.0/tests/test_utils.py` & `substra-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

