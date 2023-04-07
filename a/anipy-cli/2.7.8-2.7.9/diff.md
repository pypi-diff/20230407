# Comparing `tmp/anipy_cli-2.7.8.tar.gz` & `tmp/anipy_cli-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-2.7.8.tar", last modified: Tue Feb 21 16:09:43 2023, max compression
+gzip compressed data, was "anipy_cli-2.7.9.tar", last modified: Thu Mar  2 20:43:57 2023, max compression
```

## Comparing `anipy_cli-2.7.8.tar` & `anipy_cli-2.7.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.449827 anipy_cli-2.7.8/anipy_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/arg_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/anipy_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/anipy_cli/cli/clis/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/base_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/binge_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/default_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/history_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/mal_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/clis/seasonal_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/anipy_cli/cli/menus/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/menus/base_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/menus/mal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/menus/seasonal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/mal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/anipy_cli/player/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/anipy_cli/player/players/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/mpv.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/mpv_contrl.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/syncplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/player/players/vlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/run_anipy_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/seasonal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/url_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/anipy_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 16:09:43.449827 anipy_cli-2.7.8/anipy_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-21 16:09:43.000000 anipy_cli-2.7.8/anipy_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 16:09:43.453827 anipy_cli-2.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-21 16:09:18.000000 anipy_cli-2.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/arg_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/base_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/binge_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/default_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/history_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/mal_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/clis/seasonal_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli/cli/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/base_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/mal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/menus/seasonal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/mal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/anipy_cli/player/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/anipy_cli/player/players/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/mpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/mpv_contrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/syncplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/player/players/vlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/run_anipy_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/seasonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/url_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/anipy_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:43:57.842925 anipy_cli-2.7.9/anipy_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 20:43:57.000000 anipy_cli-2.7.9/anipy_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:43:57.846925 anipy_cli-2.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-02 20:43:41.000000 anipy_cli-2.7.9/setup.py
```

### Comparing `anipy_cli-2.7.8/LICENSE` & `anipy_cli-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/PKG-INFO` & `anipy_cli-2.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy_cli
-Version: 2.7.8
+Version: 2.7.9
 Summary: Little tool in python to watch anime from the terminal (the better way to watch anime)
 Home-page: https://github.com/sdaqo/anipy-cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 License: GPL-3.0
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anipy_cli Version: 2.7.8 Summary: Little tool in
+Metadata-Version: 2.1 Name: anipy_cli Version: 2.7.9 Summary: Little tool in
 python to watch anime from the terminal (the better way to watch anime) Home-
 page: https://github.com/sdaqo/anipy-cli Author: sdaqo Author-email:
 sdaqo.dev@protonmail.com License: GPL-3.0 Requires-Python: >3.9 Description-
 Content-Type: text/markdown License-File: LICENSE ![waving](https://capsule-
 render.vercel.app/api?type=waving&height=200&text=sdaqo/anipy-
 cli&fontAlign=60&fontAlignY=40&color=021224&fontColor=b0b8b2&animation=fadeIn)
 https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-
```

### Comparing `anipy_cli-2.7.8/README.md` & `anipy_cli-2.7.9/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/__init__.py` & `anipy_cli-2.7.9/anipy_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/arg_parser.py` & `anipy_cli-2.7.9/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/base_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/binge_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/default_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/download_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/history_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/history_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/mal_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/clis/seasonal_cli.py` & `anipy_cli-2.7.9/anipy_cli/cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/menus/base_menu.py` & `anipy_cli-2.7.9/anipy_cli/cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/menus/mal_menu.py` & `anipy_cli-2.7.9/anipy_cli/cli/menus/mal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/menus/menu.py` & `anipy_cli-2.7.9/anipy_cli/cli/menus/menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/menus/seasonal_menu.py` & `anipy_cli-2.7.9/anipy_cli/cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/cli/util.py` & `anipy_cli-2.7.9/anipy_cli/cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/colors.py` & `anipy_cli-2.7.9/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/config.py` & `anipy_cli-2.7.9/anipy_cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,17 @@
 
     def _create_config(self):
         try:
             self._get_config_path().mkdir(exist_ok=True, parents=True)
             config_options = {}
             # generate config based on attrs and default values of config class
             for attribute, value in Config.__dict__.items():
+                if attribute.startswith("_"):
+                    continue
+
                 if isinstance(value, property):
                     val = self.__getattribute__(attribute)
                     config_options[attribute] = (
                         str(val) if isinstance(val, Path) else val
                     )
             self._config_file.touch()
             with open(self._config_file, "w") as file:
```

### Comparing `anipy_cli-2.7.8/anipy_cli/download.py` & `anipy_cli-2.7.9/anipy_cli/download.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/history.py` & `anipy_cli-2.7.9/anipy_cli/history.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/mal.py` & `anipy_cli-2.7.9/anipy_cli/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/misc.py` & `anipy_cli-2.7.9/anipy_cli/misc.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/player.py` & `anipy_cli-2.7.9/anipy_cli/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/players/base.py` & `anipy_cli-2.7.9/anipy_cli/player/players/base.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/players/mpv.py` & `anipy_cli-2.7.9/anipy_cli/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/players/mpv_contrl.py` & `anipy_cli-2.7.9/anipy_cli/player/players/mpv_contrl.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/players/syncplay.py` & `anipy_cli-2.7.9/anipy_cli/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/player/players/vlc.py` & `anipy_cli-2.7.9/anipy_cli/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/query.py` & `anipy_cli-2.7.9/anipy_cli/query.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/seasonal.py` & `anipy_cli-2.7.9/anipy_cli/seasonal.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli/url_handler.py` & `anipy_cli-2.7.9/anipy_cli/url_handler.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/anipy_cli.egg-info/PKG-INFO` & `anipy_cli-2.7.9/anipy_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 2.7.8
+Version: 2.7.9
 Summary: Little tool in python to watch anime from the terminal (the better way to watch anime)
 Home-page: https://github.com/sdaqo/anipy-cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 License: GPL-3.0
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 2.7.8 Summary: Little tool in
+Metadata-Version: 2.1 Name: anipy-cli Version: 2.7.9 Summary: Little tool in
 python to watch anime from the terminal (the better way to watch anime) Home-
 page: https://github.com/sdaqo/anipy-cli Author: sdaqo Author-email:
 sdaqo.dev@protonmail.com License: GPL-3.0 Requires-Python: >3.9 Description-
 Content-Type: text/markdown License-File: LICENSE ![waving](https://capsule-
 render.vercel.app/api?type=waving&height=200&text=sdaqo/anipy-
 cli&fontAlign=60&fontAlignY=40&color=021224&fontColor=b0b8b2&animation=fadeIn)
 https://user-images.githubusercontent.com/63876564/162056019-ed0e7a60-78f6-
```

### Comparing `anipy_cli-2.7.8/anipy_cli.egg-info/SOURCES.txt` & `anipy_cli-2.7.9/anipy_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anipy_cli-2.7.8/setup.py` & `anipy_cli-2.7.9/setup.py`

 * *Files identical despite different names*

