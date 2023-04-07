# Comparing `tmp/robowebserver-0.1.5.tar.gz` & `tmp/robowebserver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robowebserver-0.1.5.tar", last modified: Fri Apr  7 20:36:42 2023, max compression
+gzip compressed data, was "robowebserver-0.1.6.tar", last modified: Fri Apr  7 20:38:45 2023, max compression
```

## Comparing `robowebserver-0.1.5.tar` & `robowebserver-0.1.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.391300 robowebserver-0.1.5/
--rw-r--r--   0 hamel      (501) staff       (20)      801 2023-04-07 20:36:42.391096 robowebserver-0.1.5/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-05 04:12:07.000000 robowebserver-0.1.5/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.338836 robowebserver-0.1.5/robowebserver/
--rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-07 20:23:09.000000 robowebserver-0.1.5/robowebserver/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1030 2023-04-07 18:47:28.000000 robowebserver-0.1.5/robowebserver/ext.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.344740 robowebserver-0.1.5/robowebserver/static/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.348422 robowebserver-0.1.5/robowebserver/static/assets/
--rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-06 20:42:03.000000 robowebserver-0.1.5/robowebserver/static/assets/AssetManifest.bin
--rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-06 20:42:03.000000 robowebserver-0.1.5/robowebserver/static/assets/AssetManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-06 20:42:03.000000 robowebserver-0.1.5/robowebserver/static/assets/FontManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)  1793799 2023-04-06 20:42:03.000000 robowebserver-0.1.5/robowebserver/static/assets/NOTICES
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.353602 robowebserver-0.1.5/robowebserver/static/assets/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.354305 robowebserver-0.1.5/robowebserver/static/assets/assets/apps/
--rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-03-21 15:51:04.000000 robowebserver-0.1.5/robowebserver/static/assets/assets/apps/firebase.webp
--rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-03-21 15:51:04.000000 robowebserver-0.1.5/robowebserver/static/assets/assets/apps/gcloud.png
--rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-03-21 15:51:04.000000 robowebserver-0.1.5/robowebserver/static/assets/assets/apps/github.png
--rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-05 03:39:55.000000 robowebserver-0.1.5/robowebserver/static/assets/assets/jupyter.jpg
--rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-05 03:39:55.000000 robowebserver-0.1.5/robowebserver/static/assets/assets/oauth2redirect.html
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.354499 robowebserver-0.1.5/robowebserver/static/assets/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)     9336 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.337790 robowebserver-0.1.5/robowebserver/static/assets/packages/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.337508 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.337559 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.355076 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.355547 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.356007 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
--rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.337836 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.337883 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.356809 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.357576 robowebserver-0.1.5/robowebserver/static/assets/shaders/
--rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.381043 robowebserver-0.1.5/robowebserver/static/canvaskit/
--rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/canvaskit.wasm
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.386142 robowebserver-0.1.5/robowebserver/static/canvaskit/chromium/
--rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/chromium/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/chromium/canvaskit.wasm
--rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.wasm
--rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.worker.js
--rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-03-21 15:51:04.000000 robowebserver-0.1.5/robowebserver/static/favicon.ico
--rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-06 20:42:05.000000 robowebserver-0.1.5/robowebserver/static/flutter.js
--rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-06 20:42:05.000000 robowebserver-0.1.5/robowebserver/static/flutter_service_worker.js
--rw-r--r--   0 hamel      (501) staff       (20)     3129 2023-04-06 20:42:04.000000 robowebserver-0.1.5/robowebserver/static/index.html
--rw-r--r--   0 hamel      (501) staff       (20)  4000192 2023-04-06 20:42:05.000000 robowebserver-0.1.5/robowebserver/static/main.dart.js
--rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-06 20:42:03.000000 robowebserver-0.1.5/robowebserver/static/version.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:36:42.339886 robowebserver-0.1.5/robowebserver.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)      801 2023-04-07 20:36:41.000000 robowebserver-0.1.5/robowebserver.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2459 2023-04-07 20:36:42.000000 robowebserver-0.1.5/robowebserver.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-07 20:36:41.000000 robowebserver-0.1.5/robowebserver.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-07 18:45:10.000000 robowebserver-0.1.5/robowebserver.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-07 20:36:42.000000 robowebserver-0.1.5/robowebserver.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       14 2023-04-07 20:36:42.000000 robowebserver-0.1.5/robowebserver.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-07 20:36:42.391367 robowebserver-0.1.5/setup.cfg
--rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-07 20:34:08.000000 robowebserver-0.1.5/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.625384 robowebserver-0.1.6/
+-rw-r--r--   0 hamel      (501) staff       (20)      913 2023-04-07 20:38:45.625188 robowebserver-0.1.6/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      150 2023-04-07 20:38:34.000000 robowebserver-0.1.6/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.566685 robowebserver-0.1.6/robowebserver/
+-rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-07 20:23:09.000000 robowebserver-0.1.6/robowebserver/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1030 2023-04-07 18:47:28.000000 robowebserver-0.1.6/robowebserver/ext.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.576322 robowebserver-0.1.6/robowebserver/static/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.581503 robowebserver-0.1.6/robowebserver/static/assets/
+-rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-06 20:42:03.000000 robowebserver-0.1.6/robowebserver/static/assets/AssetManifest.bin
+-rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-06 20:42:03.000000 robowebserver-0.1.6/robowebserver/static/assets/AssetManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-06 20:42:03.000000 robowebserver-0.1.6/robowebserver/static/assets/FontManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)  1793799 2023-04-06 20:42:03.000000 robowebserver-0.1.6/robowebserver/static/assets/NOTICES
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.587401 robowebserver-0.1.6/robowebserver/static/assets/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.589709 robowebserver-0.1.6/robowebserver/static/assets/assets/apps/
+-rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-03-21 15:51:04.000000 robowebserver-0.1.6/robowebserver/static/assets/assets/apps/firebase.webp
+-rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-03-21 15:51:04.000000 robowebserver-0.1.6/robowebserver/static/assets/assets/apps/gcloud.png
+-rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-03-21 15:51:04.000000 robowebserver-0.1.6/robowebserver/static/assets/assets/apps/github.png
+-rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-05 03:39:55.000000 robowebserver-0.1.6/robowebserver/static/assets/assets/jupyter.jpg
+-rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-05 03:39:55.000000 robowebserver-0.1.6/robowebserver/static/assets/assets/oauth2redirect.html
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.590027 robowebserver-0.1.6/robowebserver/static/assets/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)     9336 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.565427 robowebserver-0.1.6/robowebserver/static/assets/packages/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.565146 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.565196 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.590790 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.591429 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.592134 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
+-rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.565475 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.565521 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.593144 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.594051 robowebserver-0.1.6/robowebserver/static/assets/shaders/
+-rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.612591 robowebserver-0.1.6/robowebserver/static/canvaskit/
+-rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-04 22:53:10.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  6756109 2023-04-04 22:53:06.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/canvaskit.wasm
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.617013 robowebserver-0.1.6/robowebserver/static/canvaskit/chromium/
+-rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-04 22:53:10.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/chromium/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  5357473 2023-04-04 22:53:04.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/chromium/canvaskit.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-04 22:54:14.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  4505819 2023-04-04 22:54:08.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-04 22:54:14.000000 robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-03-21 15:51:04.000000 robowebserver-0.1.6/robowebserver/static/favicon.ico
+-rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-06 20:42:05.000000 robowebserver-0.1.6/robowebserver/static/flutter.js
+-rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-06 20:42:05.000000 robowebserver-0.1.6/robowebserver/static/flutter_service_worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)     3129 2023-04-06 20:42:04.000000 robowebserver-0.1.6/robowebserver/static/index.html
+-rw-r--r--   0 hamel      (501) staff       (20)  4000192 2023-04-06 20:42:05.000000 robowebserver-0.1.6/robowebserver/static/main.dart.js
+-rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-06 20:42:03.000000 robowebserver-0.1.6/robowebserver/static/version.json
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-07 20:38:45.567902 robowebserver-0.1.6/robowebserver.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)      913 2023-04-07 20:38:45.000000 robowebserver-0.1.6/robowebserver.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2459 2023-04-07 20:38:45.000000 robowebserver-0.1.6/robowebserver.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-07 20:38:45.000000 robowebserver-0.1.6/robowebserver.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-07 18:45:10.000000 robowebserver-0.1.6/robowebserver.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-07 20:38:45.000000 robowebserver-0.1.6/robowebserver.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       14 2023-04-07 20:38:45.000000 robowebserver-0.1.6/robowebserver.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-07 20:38:45.625447 robowebserver-0.1.6/setup.cfg
+-rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-07 20:34:08.000000 robowebserver-0.1.6/setup.py
```

### Comparing `robowebserver-0.1.5/PKG-INFO` & `robowebserver-0.1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robowebserver
-Version: 0.1.5
+Version: 0.1.6
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Platform: UNKNOWN
@@ -18,7 +18,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A Jupyter Server Extension for ChatGPT
 
+Installation
+
+```bash
+pip instal robowebserver
+python -m jupyter serverextension enable --py robowebserver
+```
+
```

### Comparing `robowebserver-0.1.5/robowebserver/ext.py` & `robowebserver-0.1.6/robowebserver/ext.py`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/AssetManifest.bin` & `robowebserver-0.1.6/robowebserver/static/assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/AssetManifest.json` & `robowebserver-0.1.6/robowebserver/static/assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/FontManifest.json` & `robowebserver-0.1.6/robowebserver/static/assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/NOTICES` & `robowebserver-0.1.6/robowebserver/static/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/assets/apps/firebase.webp` & `robowebserver-0.1.6/robowebserver/static/assets/assets/apps/firebase.webp`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/assets/apps/gcloud.png` & `robowebserver-0.1.6/robowebserver/static/assets/assets/apps/gcloud.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/assets/apps/github.png` & `robowebserver-0.1.6/robowebserver/static/assets/assets/apps/github.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/assets/jupyter.jpg` & `robowebserver-0.1.6/robowebserver/static/assets/assets/jupyter.jpg`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/assets/oauth2redirect.html` & `robowebserver-0.1.6/robowebserver/static/assets/assets/oauth2redirect.html`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/fonts/MaterialIcons-Regular.otf` & `robowebserver-0.1.6/robowebserver/static/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_light.png` & `robowebserver-0.1.6/robowebserver/static/assets/packages/flutter_signin_button/assets/logos/google_light.png`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf` & `robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf` & `robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf` & `robowebserver-0.1.6/robowebserver/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/assets/shaders/ink_sparkle.frag` & `robowebserver-0.1.6/robowebserver/static/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/canvaskit.js` & `robowebserver-0.1.6/robowebserver/static/canvaskit/canvaskit.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/canvaskit.wasm` & `robowebserver-0.1.6/robowebserver/static/canvaskit/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/chromium/canvaskit.js` & `robowebserver-0.1.6/robowebserver/static/canvaskit/chromium/canvaskit.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/chromium/canvaskit.wasm` & `robowebserver-0.1.6/robowebserver/static/canvaskit/chromium/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.js` & `robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.wasm` & `robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.wasm`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/canvaskit/skwasm.worker.js` & `robowebserver-0.1.6/robowebserver/static/canvaskit/skwasm.worker.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/favicon.ico` & `robowebserver-0.1.6/robowebserver/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/flutter.js` & `robowebserver-0.1.6/robowebserver/static/flutter.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/flutter_service_worker.js` & `robowebserver-0.1.6/robowebserver/static/flutter_service_worker.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/index.html` & `robowebserver-0.1.6/robowebserver/static/index.html`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver/static/main.dart.js` & `robowebserver-0.1.6/robowebserver/static/main.dart.js`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/robowebserver.egg-info/PKG-INFO` & `robowebserver-0.1.6/robowebserver.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robowebserver
-Version: 0.1.5
+Version: 0.1.6
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Platform: UNKNOWN
@@ -18,7 +18,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A Jupyter Server Extension for ChatGPT
 
+Installation
+
+```bash
+pip instal robowebserver
+python -m jupyter serverextension enable --py robowebserver
+```
+
```

### Comparing `robowebserver-0.1.5/robowebserver.egg-info/SOURCES.txt` & `robowebserver-0.1.6/robowebserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robowebserver-0.1.5/setup.py` & `robowebserver-0.1.6/setup.py`

 * *Files identical despite different names*

