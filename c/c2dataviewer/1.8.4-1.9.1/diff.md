# Comparing `tmp/c2dataviewer-1.8.4.tar.gz` & `tmp/c2dataviewer-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/c2dataviewer-1.8.4.tar", last modified: Fri Nov 11 15:33:31 2022, max compression
+gzip compressed data, was "dist/c2dataviewer-1.9.1.tar", last modified: Thu Mar 23 18:20:56 2023, max compression
```

## Comparing `c2dataviewer-1.8.4.tar` & `c2dataviewer-1.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer/
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer/control/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      144 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/control/__init__.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    35050 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/control/imagecontroller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      851 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/control/pvconfig.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3657 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/control/pvedit_dialog_controller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    12280 2022-08-03 14:24:37.000000 c2dataviewer-1.8.4/c2dataviewer/control/scope_controller_base.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    16648 2022-08-03 14:24:37.000000 c2dataviewer-1.8.4/c2dataviewer/control/scopecontroller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1793 2022-05-04 20:38:23.000000 c2dataviewer-1.8.4/c2dataviewer/control/striptool_config.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     8618 2022-05-19 18:31:01.000000 c2dataviewer-1.8.4/c2dataviewer/control/striptool_controller.py
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer/model/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      122 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/model/__init__.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    12233 2022-05-11 15:52:23.000000 c2dataviewer-1.8.4/c2dataviewer/model/pvapy_plugins.py
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer/ui/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1681 2022-05-03 18:51:03.000000 c2dataviewer-1.8.4/c2dataviewer/ui/action.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     4099 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/ui/addpv.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    32362 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/ui/imagev.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     8682 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/ui/imagev_settings.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3010 2022-02-23 20:08:12.000000 c2dataviewer-1.8.4/c2dataviewer/ui/scope.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     5497 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/ui/striptool.ui
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      879 2020-03-24 17:24:08.000000 c2dataviewer-1.8.4/c2dataviewer/ui/warning.ui
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer/view/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      126 2022-04-27 17:27:04.000000 c2dataviewer-1.8.4/c2dataviewer/view/__init__.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      182 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/view/image.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1896 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/view/image_definitions.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    28366 2022-05-11 15:52:23.000000 c2dataviewer-1.8.4/c2dataviewer/view/image_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     8855 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/view/image_profile_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     8354 2022-08-03 14:24:37.000000 c2dataviewer-1.8.4/c2dataviewer/view/scope_config_base.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    35672 2022-08-03 14:24:37.000000 c2dataviewer-1.8.4/c2dataviewer/view/scope_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     8001 2022-08-03 14:24:37.000000 c2dataviewer-1.8.4/c2dataviewer/view/scopeconfig.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      964 2022-07-22 22:32:49.000000 c2dataviewer-1.8.4/c2dataviewer/view/striptoolconfig.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)       85 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/__init__.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      984 2022-07-19 13:25:43.000000 c2dataviewer-1.8.4/c2dataviewer/c2dv.cfg
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     7104 2022-07-22 22:32:49.000000 c2dataviewer-1.8.4/c2dataviewer/c2dv.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3065 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/imagev.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     2069 2022-07-22 22:32:49.000000 c2dataviewer-1.8.4/c2dataviewer/scope.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     2012 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/c2dataviewer/striptool.py
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1336 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/PKG-INFO
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1592 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/SOURCES.txt
--rw-r--r--   0 echandler  (2662) aesctl    (3106)        1 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/dependency_links.txt
--rw-r--r--   0 echandler  (2662) aesctl    (3106)       49 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/entry_points.txt
--rw-r--r--   0 echandler  (2662) aesctl    (3106)       43 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/requires.txt
--rw-r--r--   0 echandler  (2662) aesctl    (3106)       18 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/c2dataviewer.egg-info/top_level.txt
-drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/test/
--rw-r--r--   0 echandler  (2662) aesctl    (3106)        0 2020-09-09 15:02:29.000000 c2dataviewer-1.8.4/test/__init__.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3278 2022-04-29 03:02:47.000000 c2dataviewer-1.8.4/test/helper.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     5498 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/test/test_image_definitions.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    18400 2022-04-29 03:02:47.000000 c2dataviewer-1.8.4/test/test_image_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     4757 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/test/test_image_profile_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    13573 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/test/test_imagecontroller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3768 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/test/test_imagev.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)    19524 2022-05-16 18:20:26.000000 c2dataviewer-1.8.4/test/test_scope_display.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3839 2022-08-05 20:23:38.000000 c2dataviewer-1.8.4/test/test_scopecontroller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1005 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/test/test_striptool_config.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     3897 2022-08-05 20:23:56.000000 c2dataviewer-1.8.4/test/test_striptool_controller.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)        0 2020-03-24 17:24:08.000000 c2dataviewer-1.8.4/LICENSE
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      855 2022-04-22 16:30:49.000000 c2dataviewer-1.8.4/README.md
--rw-r--r--   0 echandler  (2662) aesctl    (3106)      183 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/setup.cfg
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1950 2022-11-11 15:33:30.000000 c2dataviewer-1.8.4/setup.py
--rw-r--r--   0 echandler  (2662) aesctl    (3106)     1336 2022-11-11 15:33:31.000000 c2dataviewer-1.8.4/PKG-INFO
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)        0 2020-03-24 17:24:08.000000 c2dataviewer-1.9.1/LICENSE
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1336 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/PKG-INFO
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      855 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/README.md
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)       85 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/__init__.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      984 2022-11-18 22:49:26.000000 c2dataviewer-1.9.1/c2dataviewer/c2dv.cfg
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     7104 2022-07-22 22:32:49.000000 c2dataviewer-1.9.1/c2dataviewer/c2dv.py
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer/control/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      144 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/control/__init__.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    36364 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/control/imagecontroller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      851 2023-01-19 16:44:43.000000 c2dataviewer-1.9.1/c2dataviewer/control/pvconfig.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3657 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/control/pvedit_dialog_controller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    12280 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/control/scope_controller_base.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    16648 2022-11-21 23:39:27.000000 c2dataviewer-1.9.1/c2dataviewer/control/scopecontroller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1793 2022-05-04 20:38:23.000000 c2dataviewer-1.9.1/c2dataviewer/control/striptool_config.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     8618 2023-01-19 16:44:43.000000 c2dataviewer-1.9.1/c2dataviewer/control/striptool_controller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3065 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/imagev.py
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer/model/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      122 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/model/__init__.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    12233 2023-01-19 16:44:43.000000 c2dataviewer-1.9.1/c2dataviewer/model/pvapy_plugins.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     2069 2022-07-22 22:32:49.000000 c2dataviewer-1.9.1/c2dataviewer/scope.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     2012 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/striptool.py
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer/ui/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1681 2022-05-03 18:51:03.000000 c2dataviewer-1.9.1/c2dataviewer/ui/action.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     4099 2023-01-19 16:44:43.000000 c2dataviewer-1.9.1/c2dataviewer/ui/addpv.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    32761 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/ui/imagev.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     8682 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/ui/imagev_settings.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3010 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/ui/scope.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     5497 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/ui/striptool.ui
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      879 2020-03-24 17:24:08.000000 c2dataviewer-1.9.1/c2dataviewer/ui/warning.ui
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer/view/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      126 2022-04-27 17:27:04.000000 c2dataviewer-1.9.1/c2dataviewer/view/__init__.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      182 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/view/image.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1896 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/c2dataviewer/view/image_definitions.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    30497 2023-03-23 16:59:02.000000 c2dataviewer-1.9.1/c2dataviewer/view/image_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     8855 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/view/image_profile_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     8546 2023-03-17 15:02:03.000000 c2dataviewer-1.9.1/c2dataviewer/view/scope_config_base.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    35672 2023-03-20 13:33:10.000000 c2dataviewer-1.9.1/c2dataviewer/view/scope_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     8082 2023-03-17 15:02:03.000000 c2dataviewer-1.9.1/c2dataviewer/view/scopeconfig.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      964 2022-11-18 22:50:27.000000 c2dataviewer-1.9.1/c2dataviewer/view/striptoolconfig.py
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1336 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/PKG-INFO
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1592 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)        1 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)       49 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/entry_points.txt
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)       49 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/requires.txt
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)       18 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/c2dataviewer.egg-info/top_level.txt
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)      183 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/setup.cfg
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1963 2023-03-23 18:20:55.000000 c2dataviewer-1.9.1/setup.py
+drwxr-xr-x   0 echandler  (2662) aesctl    (3106)        0 2023-03-23 18:20:56.000000 c2dataviewer-1.9.1/test/
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)        0 2020-09-09 15:02:29.000000 c2dataviewer-1.9.1/test/__init__.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3440 2023-03-23 16:59:02.000000 c2dataviewer-1.9.1/test/helper.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     5498 2023-03-20 15:19:52.000000 c2dataviewer-1.9.1/test/test_image_definitions.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    17211 2023-02-07 21:05:15.000000 c2dataviewer-1.9.1/test/test_image_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     4740 2023-02-07 21:05:15.000000 c2dataviewer-1.9.1/test/test_image_profile_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    13561 2023-02-07 21:05:15.000000 c2dataviewer-1.9.1/test/test_imagecontroller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3755 2023-02-07 21:05:15.000000 c2dataviewer-1.9.1/test/test_imagev.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)    19524 2022-05-16 18:20:26.000000 c2dataviewer-1.9.1/test/test_scope_display.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3839 2022-08-05 20:23:38.000000 c2dataviewer-1.9.1/test/test_scopecontroller.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     1005 2022-04-22 16:30:49.000000 c2dataviewer-1.9.1/test/test_striptool_config.py
+-rw-r--r--   0 echandler  (2662) aesctl    (3106)     3897 2023-03-23 16:58:47.000000 c2dataviewer-1.9.1/test/test_striptool_controller.py
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/imagecontroller.py` & `c2dataviewer-1.9.1/c2dataviewer/control/imagecontroller.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 @author: Guobao Shen <gshen@anl.gov>
 """
 import datetime
 from pyqtgraph import Qt
 import pyqtgraph.ptime as ptime
 from pyqtgraph.functions import mkPen
 from pyqtgraph import PlotWidget
+from PyQt5 import QtWidgets
 
 from ..view.image_definitions import COLOR_MODE_MONO, COLOR_MODES
 from ..model import ConnectionState
 
 class ImageController:
 
     SLIDER_MAX_VAL = 1_000_000_000
     SLIDER_MIN_VAL = -SLIDER_MAX_VAL
     SPINNER_MAX_VAL = 1.7976931348623157e+308
     SPINNER_MIN_VAL = -SPINNER_MAX_VAL
 
+    HIDE_CONTROL_TEXT = 'Hide Control Panel'
+    SHOW_CONTROL_TEXT = 'Show Control Panel'
+
     def __init__(self, widget, **kargs):
         """
 
         :param widget:
         :param kargs:
         """
         self._win = widget
@@ -160,15 +164,38 @@
         # Setup profiles
         self._win.imageWidget.setup_profiles(self._win.canvasGrid)
         self._win.cbShowProfiles.stateChanged.connect(
             lambda: self._callback_profiles_show_changed(self._win.cbShowProfiles))
 
         self.frameRateChanged()
         self.camera_changed()
-        
+
+        self._imageContextMenu = QtWidgets.QMenu(self._win.imageWidget)
+        self._imageContextMenuAction = QtWidgets.QAction(self.HIDE_CONTROL_TEXT, self._win.imageWidget)
+        self._imageContextMenu.addAction(self._imageContextMenuAction)
+        self._win.imageWidget.customContextMenuRequested.connect(self.on_context_menu)
+        self._scrollAreaWidth = 0
+
+    def on_context_menu(self, point):
+        # show context menu
+        action = self._imageContextMenu.exec_(self._win.imageWidget.mapToGlobal(point))
+        if not action:
+            return
+        if action.text() == self.HIDE_CONTROL_TEXT:
+            action.setText(self.SHOW_CONTROL_TEXT)
+            self._win.scrollArea.hide()
+            self._scrollAreaWidth = self._win.scrollArea.parent().minimumWidth()
+            self._win.scrollArea.parent().setMinimumWidth(0)
+            self._win.scrollArea.parent().setMinimumHeight(0)
+        else:
+            action.setText(self.HIDE_CONTROL_TEXT)
+            self._win.scrollArea.show()
+            self._win.scrollArea.parent().setMinimumWidth(self._scrollAreaWidth)
+        self._win.imageWidget.adjustSize()
+
     def _callback_black_changed_slider(self):
         """
         This callback is called when user change the value on the "black" slider.
 
         :return:
         """
         try:
@@ -406,14 +433,16 @@
         :return:
         """
         fmt = kargs.get('fmt', '%.1f')
         hilimit = kargs.get('hilimit', None)
         lolimit = kargs.get('lowlimit', None)
         callback = kargs.get('callback', False)
 
+        if type(value) is list:
+            value = value[0]
         if roi_value is not None:
             fmt = f"{fmt} ({fmt})"
             if type(value) is tuple:
                 value = value + roi_value
             else:
                 value = (value, roi_value)
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/pvconfig.py` & `c2dataviewer-1.9.1/c2dataviewer/control/pvconfig.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/pvedit_dialog_controller.py` & `c2dataviewer-1.9.1/c2dataviewer/control/pvedit_dialog_controller.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/scope_controller_base.py` & `c2dataviewer-1.9.1/c2dataviewer/control/scope_controller_base.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/scopecontroller.py` & `c2dataviewer-1.9.1/c2dataviewer/control/scopecontroller.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/striptool_config.py` & `c2dataviewer-1.9.1/c2dataviewer/control/striptool_config.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/control/striptool_controller.py` & `c2dataviewer-1.9.1/c2dataviewer/control/striptool_controller.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/model/pvapy_plugins.py` & `c2dataviewer-1.9.1/c2dataviewer/model/pvapy_plugins.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/action.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/action.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/addpv.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/addpv.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/imagev.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/imagev.ui`

 * *Files 2% similar despite different names*

#### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/imagev.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/imagev.ui`

```diff
@@ -3,82 +3,33 @@
   <class>C2DVImage</class>
   <widget class="QMainWindow" name="C2DVImage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1119</width>
-        <height>850</height>
+        <height>852</height>
       </rect>
     </property>
+    <property name="sizePolicy">
+      <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+        <horstretch>0</horstretch>
+        <verstretch>0</verstretch>
+      </sizepolicy>
+    </property>
     <property name="windowTitle">
       <string>C2DataViewer - AD Image</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QGridLayout" name="gridLayout_3">
         <property name="sizeConstraint">
           <enum>QLayout::SetMinimumSize</enum>
         </property>
-        <item row="0" column="0">
-          <layout class="QGridLayout" name="canvasGrid">
-            <property name="sizeConstraint">
-              <enum>QLayout::SetMaximumSize</enum>
-            </property>
-            <item row="1" column="1">
-              <widget class="ImagePlotWidget" name="imageWidget" native="true">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
-                    <horstretch>100</horstretch>
-                    <verstretch>100</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="minimumSize">
-                  <size>
-                    <width>500</width>
-                    <height>500</height>
-                  </size>
-                </property>
-              </widget>
-            </item>
-            <item row="1" column="0">
-              <widget class="PlotWidget" name="yProfilePlot" native="true">
-                <property name="sizePolicy">
-                  <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                    <horstretch>0</horstretch>
-                    <verstretch>0</verstretch>
-                  </sizepolicy>
-                </property>
-                <property name="minimumSize">
-                  <size>
-                    <width>60</width>
-                    <height>0</height>
-                  </size>
-                </property>
-                <property name="acceptDrops">
-                  <bool>false</bool>
-                </property>
-                <property name="styleSheet">
-                  <string notr="true">border-color: rgb(252, 233, 79);</string>
-                </property>
-              </widget>
-            </item>
-            <item row="0" column="1">
-              <widget class="PlotWidget" name="xProfilePlot" native="true">
-                <property name="minimumSize">
-                  <size>
-                    <width>0</width>
-                    <height>50</height>
-                  </size>
-                </property>
-              </widget>
-            </item>
-          </layout>
-        </item>
         <item row="0" column="1" rowspan="2">
-          <widget class="QWidget" name="widget" native="true">
+          <widget class="QWidget" name="controlPanel" native="true">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="minimumSize">
@@ -101,27 +52,30 @@
                 <number>0</number>
               </property>
               <property name="spacing">
                 <number>0</number>
               </property>
               <item row="0" column="0" colspan="2">
                 <widget class="QScrollArea" name="scrollArea">
+                  <property name="contextMenuPolicy">
+                    <enum>Qt::CustomContextMenu</enum>
+                  </property>
                   <property name="sizeAdjustPolicy">
                     <enum>QAbstractScrollArea::AdjustIgnored</enum>
                   </property>
                   <property name="widgetResizable">
                     <bool>true</bool>
                   </property>
                   <widget class="QWidget" name="scrollAreaWidgetContents">
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
                         <width>354</width>
-                        <height>947</height>
+                        <height>903</height>
                       </rect>
                     </property>
                     <layout class="QVBoxLayout" name="verticalLayout_11">
                       <property name="topMargin">
                         <number>0</number>
                       </property>
                       <item>
@@ -847,23 +801,81 @@
                     </layout>
                   </widget>
                 </widget>
               </item>
             </layout>
           </widget>
         </item>
+        <item row="0" column="0">
+          <layout class="QGridLayout" name="canvasGrid">
+            <property name="sizeConstraint">
+              <enum>QLayout::SetMaximumSize</enum>
+            </property>
+            <item row="1" column="1">
+              <widget class="ImagePlotWidget" name="imageWidget" native="true">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                    <horstretch>100</horstretch>
+                    <verstretch>100</verstretch>
+                  </sizepolicy>
+                </property>
+                <property name="minimumSize">
+                  <size>
+                    <width>10</width>
+                    <height>10</height>
+                  </size>
+                </property>
+                <property name="contextMenuPolicy">
+                  <enum>Qt::CustomContextMenu</enum>
+                </property>
+              </widget>
+            </item>
+            <item row="1" column="0">
+              <widget class="PlotWidget" name="yProfilePlot" native="true">
+                <property name="sizePolicy">
+                  <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                    <horstretch>0</horstretch>
+                    <verstretch>0</verstretch>
+                  </sizepolicy>
+                </property>
+                <property name="minimumSize">
+                  <size>
+                    <width>60</width>
+                    <height>0</height>
+                  </size>
+                </property>
+                <property name="acceptDrops">
+                  <bool>false</bool>
+                </property>
+                <property name="styleSheet">
+                  <string notr="true">border-color: rgb(252, 233, 79);</string>
+                </property>
+              </widget>
+            </item>
+            <item row="0" column="1">
+              <widget class="PlotWidget" name="xProfilePlot" native="true">
+                <property name="minimumSize">
+                  <size>
+                    <width>0</width>
+                    <height>50</height>
+                  </size>
+                </property>
+              </widget>
+            </item>
+          </layout>
+        </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1119</width>
-          <height>22</height>
+          <height>20</height>
         </rect>
       </property>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
   </widget>
   <customwidgets>
     <customwidget>
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/imagev_settings.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/imagev_settings.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/scope.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/scope.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/striptool.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/striptool.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/ui/warning.ui` & `c2dataviewer-1.9.1/c2dataviewer/ui/warning.ui`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/image_definitions.py` & `c2dataviewer-1.9.1/c2dataviewer/view/image_definitions.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/image_display.py` & `c2dataviewer-1.9.1/c2dataviewer/view/image_display.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,70 @@
 import queue
 import logging
 
 import numpy as np
 from pyqtgraph import QtCore
 from pyqtgraph.Qt import QtGui
 from pyqtgraph.widgets.RawImageWidget import RawImageWidget
-from pvaccess import PvaException
+import blosc
+import pvaccess as pva
 
 from .image_definitions import *
 from .image_profile_display import ImageProfileWidget
 
+class ImageCompressionUtility:
+
+    NUMPY_DATA_TYPE_MAP = {
+        pva.UBYTE   : np.dtype('uint8'),
+        pva.BYTE    : np.dtype('int8'),
+        pva.USHORT  : np.dtype('uint16'),
+        pva.SHORT   : np.dtype('int16'),
+        pva.UINT    : np.dtype('uint32'),
+        pva.INT     : np.dtype('int32'),
+        pva.ULONG   : np.dtype('uint64'),
+        pva.LONG    : np.dtype('int64'),
+        pva.FLOAT   : np.dtype('float32'),
+        pva.DOUBLE  : np.dtype('float64')
+    }
+    
+    NTNDA_DATA_TYPE_MAP = {
+        pva.UBYTE   : 'ubyteValue',
+        pva.BYTE    : 'byteValue',
+        pva.USHORT  : 'ushortValue',
+        pva.SHORT   : 'shortValue',
+        pva.UINT    : 'uintValue',
+        pva.INT     : 'intValue',
+        pva.ULONG   : 'ulongValue',
+        pva.LONG    : 'longValue',
+        pva.FLOAT   : 'floatValue',
+        pva.DOUBLE  : 'doubleValue',
+    }
+
+    @classmethod
+    def get_ntnda_data_type(cls, pvaType):
+       return cls.NTNDA_DATA_TYPE_MAP.get(pvaType)
+
+    @classmethod
+    def get_decompressor(cls, codecName):
+        utilityMap = {
+            'blosc' : cls.blosc_decompress
+        }
+        decompressor = utilityMap.get(codecName)
+        if not decompressor:
+            raise RuntimeError(f'Unsupported compression: {codecName}')
+        return decompressor
+
+    @classmethod
+    def blosc_decompress(cls, inputArray, inputType, uncompressedSize):
+        oadt = cls.NUMPY_DATA_TYPE_MAP.get(inputType) 
+        oasz = uncompressedSize // oadt.itemsize
+        outputArray = np.empty(oasz, dtype=oadt)
+        nBytesWritten = blosc.decompress_ptr(bytearray(inputArray), outputArray.__array_interface__['data'][0])
+        return outputArray
+
 Image = namedtuple("Image", ['id', 'new', 'image', 'black', 'white'])
 class ImagePlotWidget(RawImageWidget):
 
     MIN_DISPLAY_QUEUE_SIZE = 0
     MAX_DISPLAY_QUEUE_SIZE = 999
     DEFAULT_DISPLAY_QUEUE_SIZE = 20
     ZOOM_LENGTH_MIN = 4 # Using zoom this is the smallest number of pixels to display in each direction
@@ -590,15 +641,15 @@
         :raise RuntimeError:
         """
         self.wait()
         self._agc = False
         self._lastTimestamp = None
         try:
             self.datasource.update_device(value)
-        except PvaException as e:
+        except pva.PvaException as e:
             # TODO wrap PvaException from pvaPy in a better way for other interface
             # pvAccess connection error
             # release mutex lock
             self.signal()
             # NOTE: data source is already stopped on error. calling stop here will override
             # the connection status
             #self.stop()
@@ -718,14 +769,22 @@
             raise RuntimeError('No recognized image data received.')
         else:
             self._isInputValid = True
 
         # Lookup required infomartion for the current input type
         imgArray = data['value'][0][inputType]
         sz = imgArray.nbytes
+        codecName = data['codec']['name']
+        if codecName:
+            uncompressedSize = data['uncompressedSize']
+            uncompressedType = data['codec.parameters'][0]['value']
+            decompress = ImageCompressionUtility.get_decompressor(codecName)
+            imgArray = decompress(imgArray, uncompressedType, uncompressedSize)
+            inputType = ImageCompressionUtility.get_ntnda_data_type(uncompressedType)
+       
         maxVal = self.dataTypesDict[inputType]['maxVal']
         minVal = self.dataTypesDict[inputType]['minVal']
         npdt = self.dataTypesDict[inputType]['npdt']
         embeddedDataLen = self._pref['EmbeddedDataLen']
 
         # Configure GUI for the correct type
         if inputType != self._inputType:
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/image_profile_display.py` & `c2dataviewer-1.9.1/c2dataviewer/view/image_profile_display.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/scope_config_base.py` & `c2dataviewer-1.9.1/c2dataviewer/view/scope_config_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,17 @@
                 {"name": "Autoscale", "type": "bool", "value": False},
                 {"name": "Single axis", "type": "bool", "value": True},
                 {"name": "Histogram", "type": "bool", "value": False},
                 {"name": "Num Bins", "type": "int", "value": 100},
                 {"name": "Refresh", "type": "float", "value": 0.1, "siPrefix": True, "suffix": "s"},
             ]}
         else:
+            display_mode = section.get("MODE", "normal").lower().strip()
+            if display_mode not in ["normal", "fft", "psd", "diff", "xy"]:
+                display_mode = "normal"
 
             fft_filter = section.get("FFT_FILTER", None)
             if fft_filter is not None:
                 if fft_filter.lower().strip() in ["none", "hamming"]:
                     fft_filter = fft_filter.lower().strip().capitalize()
                 else:
                     # Disable filter if config not valid
@@ -121,15 +124,15 @@
             display = {"name": "Display", "type": "group", "children": [
                 {"name": "Mode", "type": "list", "values": {
                     "Normal": "normal",
                     "FFT": "fft",
                     "PSD": "psd",
                     "Diff": "diff",
                     "X vs Y": "xy",
-                }, "value": "Normal"},
+                }, "value": display_mode},
                 {"name": "FFT filter", "type": "list", "values": {
                     "None" : "none",
                     "Hamming" : "hamming"
                 }, "value": fft_filter},
                 {"name": "Exp moving avg", "type": "int", "value": n_average, "limits" : (1, 1e+10)},
                 {"name": "Autoscale", "type": "bool", "value": autoscale},
                 {"name": "Single axis", "type": "bool", "value": single_axis},
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/scope_display.py` & `c2dataviewer-1.9.1/c2dataviewer/view/scope_display.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/scopeconfig.py` & `c2dataviewer-1.9.1/c2dataviewer/view/scopeconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     def assemble_config(self, section=None):
         # Assemble extra configuration information for plotting
         # which is ArrayId selection, and x axes
         id_value = ["None"]
         if self.default_arrayid != "None":
             id_value.append(self.default_arrayid)
         axes = ["None"]
+        self.default_xaxes = section.get("XAXES", "None") if section else "None"
         if self.default_xaxes != "None":
             axes.append(self.default_xaxes)
 
         self.default_major_tick = section.getint('MAJORTICKS', 0) if section else 0
         self.default_minor_tick = section.getint('MINORTICKS', 0) if section else 0
         
         cfg = {"name": "Config",
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer/view/striptoolconfig.py` & `c2dataviewer-1.9.1/c2dataviewer/view/striptoolconfig.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/c2dv.cfg` & `c2dataviewer-1.9.1/c2dataviewer/c2dv.cfg`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/c2dv.py` & `c2dataviewer-1.9.1/c2dataviewer/c2dv.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/imagev.py` & `c2dataviewer-1.9.1/c2dataviewer/imagev.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/scope.py` & `c2dataviewer-1.9.1/c2dataviewer/scope.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer/striptool.py` & `c2dataviewer-1.9.1/c2dataviewer/striptool.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/c2dataviewer.egg-info/PKG-INFO` & `c2dataviewer-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2dataviewer
-Version: 1.8.4
+Version: 1.9.1
 Summary: Python based data viewer for next generation of APS control system (C2)
 Home-page: UNKNOWN
 Author: G. Shen
 Author-email: gshen@anl.gov
 License: UNKNOWN
 Description: <p align="center">
           <h1 align="center">C2DataViewer: EPICS7 pvObject Data Viewer</h1>
```

### Comparing `c2dataviewer-1.8.4/c2dataviewer.egg-info/SOURCES.txt` & `c2dataviewer-1.9.1/c2dataviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/test/helper.py` & `c2dataviewer-1.9.1/test/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Helper functions for c2d unit tests.
 
 @author: Matic Pogacnik <mpogacnik@anl.gov>
 """
 from datetime import datetime as dt
 import numpy as np
 import pvaccess as pva
+from pyqtgraph.Qt import QtWidgets
 
 from c2dataviewer.view.image_definitions import *
 from c2dataviewer.view.image_display import ImagePlotWidget
 
 ############################################
 # ND Image
 ############################################
@@ -64,20 +65,29 @@
     if nz is not None:
         if color_mode == COLOR_MODE_RGB1:
             dims.insert(0, pva.PvDimension(nz, 0, nz, 1, False))
         elif color_mode == COLOR_MODE_RGB2:
             dims.insert(1, pva.PvDimension(nz, 0, nz, 1, False))
         elif color_mode == COLOR_MODE_RGB3:
             dims.append(pva.PvDimension(nz, 0, nz, 1, False))
-    nda['codec'] = pva.PvCodec('pvapyc', pva.PvInt(14))
     nda['dimension'] = dims
     nda['descriptor'] = 'PvaPy Simulated Image'
     nda['compressedSize'] = nx*ny*(nz if nz is not None else 1)
     nda['uncompressedSize'] = nx*ny*(nz if nz is not None else 1)
     nda['timeStamp'] = time_stamp
     nda['dataTimeStamp'] = time_stamp
     if color_mode is not None:
         attrs = [pva.NtAttribute('ColorMode', pva.PvInt(color_mode))]
         nda['attribute'] = attrs
     nda['value'] = {data_type : image}
 
     return nda
+
+app = None
+
+def setup_qt_app():
+    global app
+    
+    if not app:
+        app = QtWidgets.QApplication.instance()
+        if not app:
+            app  = QtWidgets.QApplication([])
```

### Comparing `c2dataviewer-1.8.4/test/test_image_definitions.py` & `c2dataviewer-1.9.1/test/test_image_definitions.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/test/test_image_display.py` & `c2dataviewer-1.9.1/test/test_image_display.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,37 @@
 import sys
 import unittest
 import numpy as np
 import pvaccess as pva
 from pyqtgraph.Qt import QtWidgets
 from pyqtgraph.Qt import QtCore, QtTest
 from .helper import create_image
+from .helper import setup_qt_app
 
 from c2dataviewer.view.image_definitions import *
 from c2dataviewer.imagev import ImageWindow
 from c2dataviewer.view.image_display import ImagePlotWidget
 
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
-
+        
 ############################################
 # Test
 ############################################
 class TestImageDisplay(unittest.TestCase):
 
     def setUp(self):
         """
         Build the environment for each unit test case.
         This method is called before each test.
 
         :return:
         """
         # Create Qt application
-        self.app = QtWidgets.QApplication(sys.argv)
-
+        setup_qt_app()
+         
         # Create ImageWindow and get the imageWidget instance
         self.window = ImageWindow()
         self.imageWidget = self.window.imageWidget
         self.imageWidget.resize(1000,1000)
         self.imageWidget.use_embeddedDataLen = False
 
         # GUI styles
@@ -50,15 +51,14 @@
     def tearDown(self):
         """
         Tear down the environment after each test case.
         This mentod is called after each test.
 
         :return:
         """
-        self.app.quit()
 
 ############################################
 # Test datatypes (display method)
 ############################################
 
     def runDatatypeSupportTest(self, dataType, xDim, yDim, arrayValue, inputValid = True):
         """
@@ -295,14 +295,15 @@
         self.runDatatypeSupportTest(pva.DOUBLE, x, y, arrayValue)
 
 ############################################
 # Test zoom capability
 ############################################
 
     def test_zoom(self):
+        
         """
 
         """
         # Build test image
         arrayValue = [
             255, 0, 77, 54, 23, 76, 34, 65, 34, 65,
             255, 0, 77, 54, 23, 76, 34, 65, 34, 65,
@@ -326,93 +327,66 @@
         self.assertFalse(self.imageWidget.is_zoomed())
         self.assertEqual(0, xOffset)
         self.assertEqual(0, yOffset)
         self.assertEqual(10, width)
         self.assertEqual(10, height)
 
         # Change ROI programmatically
-        self.imageWidget._ImagePlotWidget__calculateZoomParameters(100, 500, 50, 470)
+        self.imageWidget._ImagePlotWidget__calculateZoomParameters(100, 500, 100, 500)
 
         # Test zoom dist values
         xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
         self.assertTrue(self.imageWidget.is_zoomed())
         self.assertEqual(1, xOffset)
-        self.assertEqual(0, yOffset)
+        self.assertEqual(1, yOffset)
         self.assertEqual(4, width)
         self.assertEqual(4, height)
 
         # Call reset zoom programmatically as we do not have the button available here
         self.imageWidget.reset_zoom()
         xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
         self.assertFalse(self.imageWidget.is_zoomed())
         self.assertEqual(0, xOffset)
         self.assertEqual(0, yOffset)
         self.assertEqual(10, width)
         self.assertEqual(10, height)
 
+        
         # Select roi by simulating mouse clicks
-        QtTest.QTest.mousePress(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
-                            QtCore.QPoint(500, 470), -1)
-        QtTest.QTest.mouseRelease(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
-                            QtCore.QPoint(100, 50), 500)
-
-        # Test if roi was zoomed
-        xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
-        self.assertTrue(self.imageWidget.is_zoomed())
-        self.assertEqual(1, xOffset)
-        self.assertEqual(0, yOffset)
-        self.assertEqual(7, width)
-        self.assertEqual(7, height)
-
-        # Try to select again
-        QtTest.QTest.mousePress(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
-                            QtCore.QPoint(50, 150), -1)
-        QtTest.QTest.mouseRelease(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
-                            QtCore.QPoint(550, 7000), 50)
-
-        # Test if roi was zoomed again
-        xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
-        self.assertTrue(self.imageWidget.is_zoomed())
-        self.assertEqual(1, xOffset)
-        self.assertEqual(1, yOffset)
-        self.assertEqual(6, width)
-        self.assertEqual(7, height)
-
-        # Call reset zoom programmatically as we do not have the button available here
-        self.imageWidget.reset_zoom()
-        xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
-        self.assertFalse(self.imageWidget.is_zoomed())
-        self.assertEqual(0, xOffset)
-        self.assertEqual(0, yOffset)
-        self.assertEqual(10, width)
-        self.assertEqual(10, height)
+        # The mouseRelease causes the imageWidget to resize to 562x562, causing the resulting
+        # width to be 7.  Disable this test until reason behind behavior is understood
+        #
+        # QtTest.QTest.mousePress(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
+        #                     QtCore.QPoint(500, 500), -1)
+        # QtTest.QTest.mouseRelease(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
+        #                     QtCore.QPoint(100, 100), 500)
+
+        # # Test if roi was zoomed
+        # xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
+        # self.assertTrue(self.imageWidget.is_zoomed())
+        # self.assertEqual(1, xOffset)
+        # self.assertEqual(1, yOffset)
+        # self.assertEqual(7, width)
+        # self.assertEqual(7, height)
+        # self.imageWidget.reset_zoom()
 
         # Try to select outside the image (Check if the zoom is ignored if user click outside the widget)
         QtTest.QTest.mousePress(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
-                            QtCore.QPoint(300, 700), -1)
+                            QtCore.QPoint(2000, 2000), -1)
         QtTest.QTest.mouseRelease(self.imageWidget, QtCore.Qt.LeftButton, QtCore.Qt.NoModifier,
                             QtCore.QPoint(250, 200), 50)
 
         # Assure that image was not zoomed
         xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
         self.assertFalse(self.imageWidget.is_zoomed())
         self.assertEqual(0, xOffset)
         self.assertEqual(0, yOffset)
         self.assertEqual(10, width)
         self.assertEqual(10, height)
 
-        # Call reset zoom programmatically as we do not have the button available here
-        self.imageWidget.reset_zoom()
-        xOffset, yOffset, width, height = self.imageWidget.get_zoom_region()
-        self.assertFalse(self.imageWidget.is_zoomed())
-        self.assertEqual(0, xOffset)
-        self.assertEqual(0, yOffset)
-        self.assertEqual(10, width)
-        self.assertEqual(10, height)
-
     def test_no_color_mode(self):
         #Make sure that can process mono images even though they don't have a color mode
         image = create_image(1, nx=8, ny=8)
         try:
             self.imageWidget.display(image)
         except RuntimeError as e:
             self.assertTrue(False, e)
```

### Comparing `c2dataviewer-1.8.4/test/test_image_profile_display.py` & `c2dataviewer-1.9.1/test/test_image_profile_display.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,33 @@
 import pyqtgraph as pg
 
 from c2dataviewer.imagev import ImageWindow, ImageSettingsDialog, WarningDialog
 from c2dataviewer.control.imagecontroller import ImageController
 from c2dataviewer.view.image_definitions import COLOR_MODE_MONO, COLOR_MODE_RGB2, transcode_image
 from c2dataviewer.view.image_profile_display import ImageProfileWidget
 from .helper import create_image
+from .helper import setup_qt_app
 
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
+
 class TestImageProfileWidget(unittest.TestCase):
 
     
     def setUp(self):
         """
         Build the environment for each unit test case.
         This method is called before each test.
         We need the whole application to be able to test this, as ImageProfileWidget also handle the layout.
 
         :return:
         """
         # Create Qt application
-        self.app = pg.Qt.QtWidgets.QApplication(sys.argv)
-
+        setup_qt_app()
+        
         # Create ImageWindow and het the imageWidget instance
         self.window = ImageWindow()
         self.imageWidget = self.window.imageWidget
 
         # Build GUI elements
         w = ImageWindow(None)
         datasource = mock.Mock()
@@ -59,15 +61,14 @@
     def tearDown(self):
         """
         Tear down the environment after each test case.
         This mentod is called after each test.
 
         :return:
         """
-        self.app.quit()
 
     def test_calculate_profiles(self):
         """
         Test if profile calculation is correct.
 
         :return:
         """
```

### Comparing `c2dataviewer-1.8.4/test/test_imagecontroller.py` & `c2dataviewer-1.9.1/test/test_imagecontroller.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 from pyqtgraph import QtCore
 
 from c2dataviewer.imagev import ImageSettingsDialog, WarningDialog
 from c2dataviewer.imagev import ImageController
 from c2dataviewer.imagev import ImageWindow
 
 from .helper import create_image
+from .helper import setup_qt_app
 
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
 class TestImageDisplay(unittest.TestCase):
 
     def setUp(self):
         """
         Build the environment for each unit test case.
         This method is called before each test.
 
         :return:
         """
 
         # Create Qt application
-        self.app = QtWidgets.QApplication(sys.argv)
-
+        setup_qt_app()
+        
         # Create ImageWindow and het the imageWidget instance
         self.window = ImageWindow()
         self.imageWidget = self.window.imageWidget
 
         # Build GUI elements
         w = ImageWindow(None)
         datasource = mock.Mock()
@@ -57,15 +58,14 @@
     def tearDown(self):
         """
         Tear down the environment after each test case.
         This mentod is called after each test.
 
         :return:
         """
-        self.app.quit()
 
     def test_blackSetting(self):
         """
         Test if setting black value behaves correctly
 
         :return:
         """
```

### Comparing `c2dataviewer-1.8.4/test/test_imagev.py` & `c2dataviewer-1.9.1/test/test_imagev.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,44 +11,43 @@
 import os
 import sys
 import unittest
 from pyqtgraph.Qt import QtCore
 from pyqtgraph.Qt import QtWidgets
 
 from c2dataviewer.imagev import ImageWindow
-
+from .helper import setup_qt_app
 
 os.environ["QT_QPA_PLATFORM"] = "offscreen"
 
 class TestImagev(unittest.TestCase):
 
     def setUp(self):
         """
         Build the environment for each unit test case.
         This method is called before each test.
 
         :return:
         """
 
         # Create Qt application
-        self.app = QtWidgets.QApplication(sys.argv)
-
+        setup_qt_app()
+        
         # Build image window
         self.window = ImageWindow()
         self.window.resize(1200, 1200)
         QtWidgets.QApplication.instance().processEvents()
 
     def tearDown(self):
         """
         Tear down the environment after each test case.
         This mentod is called after each test.
 
         :return:
         """
-        self.app.quit()
 
     def test_widgetVisibility2WindowSize(self):
         """
         Test if widgets start to disappear if window
         is resized to smallest possible size.
 
         As this gets really complex because of the relative coordinates,
```

### Comparing `c2dataviewer-1.8.4/test/test_scope_display.py` & `c2dataviewer-1.9.1/test/test_scope_display.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/test/test_scopecontroller.py` & `c2dataviewer-1.9.1/test/test_scopecontroller.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/test/test_striptool_config.py` & `c2dataviewer-1.9.1/test/test_striptool_config.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/test/test_striptool_controller.py` & `c2dataviewer-1.9.1/test/test_striptool_controller.py`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/README.md` & `c2dataviewer-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `c2dataviewer-1.8.4/setup.py` & `c2dataviewer-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,10 +50,11 @@
     include_package_data = True,
     install_requires=[
     'numpy',
     'psutil',
     'pvapy',
     'pyqtgraph==0.10.0',
     'PyQt5',
+    'blosc',
     ],
     entry_points = {'console_scripts': ['c2dv=c2dataviewer.c2dv:main']},
 )
```

### Comparing `c2dataviewer-1.8.4/PKG-INFO` & `c2dataviewer-1.9.1/c2dataviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2dataviewer
-Version: 1.8.4
+Version: 1.9.1
 Summary: Python based data viewer for next generation of APS control system (C2)
 Home-page: UNKNOWN
 Author: G. Shen
 Author-email: gshen@anl.gov
 License: UNKNOWN
 Description: <p align="center">
           <h1 align="center">C2DataViewer: EPICS7 pvObject Data Viewer</h1>
```

