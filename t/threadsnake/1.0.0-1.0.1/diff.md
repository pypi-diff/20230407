# Comparing `tmp/threadsnake-1.0.0.tar.gz` & `tmp/threadsnake-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsnake-1.0.0.tar", last modified: Wed Nov  9 02:14:00 2022, max compression
+gzip compressed data, was "threadsnake-1.0.1.tar", last modified: Fri Apr  7 21:09:28 2023, max compression
```

## Comparing `threadsnake-1.0.0.tar` & `threadsnake-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,54 @@
-drwxrwxrwx   0        0        0        0 2022-11-09 02:14:00.263393 threadsnake-1.0.0/
--rw-rw-rw-   0        0        0    35821 2022-11-05 13:40:41.000000 threadsnake-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      882 2022-11-09 02:14:00.262392 threadsnake-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       83 2022-11-05 15:15:09.000000 threadsnake-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2022-11-05 15:10:20.000000 threadsnake-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-09 02:14:00.264400 threadsnake-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1196 2022-11-06 12:33:10.000000 threadsnake-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.535641 threadsnake-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.608749 threadsnake-1.0.0/src/threadsnake/
--rw-rw-rw-   0        0        0        0 2022-10-30 16:43:38.000000 threadsnake-1.0.0/src/threadsnake/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.634322 threadsnake-1.0.0/src/threadsnake/html/
--rw-rw-rw-   0        0        0        0 2022-11-06 14:45:26.000000 threadsnake-1.0.0/src/threadsnake/html/__init__.py
--rw-rw-rw-   0        0        0      557 2022-11-06 14:52:50.000000 threadsnake-1.0.0/src/threadsnake/html/tools.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.728762 threadsnake-1.0.0/src/threadsnake/http/
--rw-rw-rw-   0        0        0        0 2022-10-30 16:44:32.000000 threadsnake-1.0.0/src/threadsnake/http/__init__.py
--rw-rw-rw-   0        0        0     2469 2022-11-06 14:36:21.000000 threadsnake-1.0.0/src/threadsnake/http/application.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.921717 threadsnake-1.0.0/src/threadsnake/http/core/
--rw-rw-rw-   0        0        0        0 2022-11-02 22:49:53.000000 threadsnake-1.0.0/src/threadsnake/http/core/__init__.py
--rw-rw-rw-   0        0        0     2922 2022-11-05 23:05:02.000000 threadsnake-1.0.0/src/threadsnake/http/core/common.py
--rw-rw-rw-   0        0        0     1082 2022-11-05 13:36:57.000000 threadsnake-1.0.0/src/threadsnake/http/core/constants.py
--rw-rw-rw-   0        0        0     4173 2022-11-05 13:43:14.000000 threadsnake-1.0.0/src/threadsnake/http/core/httprequest.py
--rw-rw-rw-   0        0        0     6051 2022-11-05 22:57:29.000000 threadsnake-1.0.0/src/threadsnake/http/core/httpresponse.py
--rw-rw-rw-   0        0        0     2237 2022-11-05 13:37:46.000000 threadsnake-1.0.0/src/threadsnake/http/core/httpserver.py
--rw-rw-rw-   0        0        0     2624 2022-11-05 13:37:59.000000 threadsnake-1.0.0/src/threadsnake/http/core/server.py
--rw-rw-rw-   0        0        0     1305 2022-11-05 13:38:04.000000 threadsnake-1.0.0/src/threadsnake/http/core/session.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.964717 threadsnake-1.0.0/src/threadsnake/http/core/values/
--rw-rw-rw-   0        0        0       80 2022-11-05 22:54:44.000000 threadsnake-1.0.0/src/threadsnake/http/core/values/__init__.py
--rw-rw-rw-   0        0        0      418 2022-11-06 11:15:02.000000 threadsnake-1.0.0/src/threadsnake/http/core/values/contenttypes.py
--rw-rw-rw-   0        0        0     2276 2022-11-05 22:52:38.000000 threadsnake-1.0.0/src/threadsnake/http/core/values/responsecodes.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:14:00.183560 threadsnake-1.0.0/src/threadsnake/http/middlewares/
--rw-rw-rw-   0        0        0        0 2022-11-04 04:42:21.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/__init__.py
--rw-rw-rw-   0        0        0      378 2022-11-05 15:20:30.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/app.py
--rw-rw-rw-   0        0        0     1661 2022-11-05 13:38:15.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/authorization.py
--rw-rw-rw-   0        0        0     1407 2022-11-05 13:38:34.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/bodyparser.py
--rw-rw-rw-   0        0        0      342 2022-11-05 13:47:33.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/cors.py
--rw-rw-rw-   0        0        0     1370 2022-11-05 15:19:19.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/defaultheaders.py
--rw-rw-rw-   0        0        0      695 2022-11-05 13:46:11.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/jsonbodyparser.py
--rw-rw-rw-   0        0        0     4135 2022-11-05 15:10:20.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/multipartformdataparser.py
--rw-rw-rw-   0        0        0     2008 2022-11-05 14:45:23.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/requests.py
--rw-rw-rw-   0        0        0     2242 2022-11-05 13:39:33.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/session.py
--rw-rw-rw-   0        0        0     1483 2022-11-06 14:37:23.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/static.py
--rw-rw-rw-   0        0        0      481 2022-11-05 14:09:58.000000 threadsnake-1.0.0/src/threadsnake/http/middlewares/timemeassure.py
--rw-rw-rw-   0        0        0     5039 2022-11-05 14:30:47.000000 threadsnake-1.0.0/src/threadsnake/http/router.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:14:00.247537 threadsnake-1.0.0/src/threadsnake/http/tools/
--rw-rw-rw-   0        0        0        0 2022-11-05 15:44:25.000000 threadsnake-1.0.0/src/threadsnake/http/tools/__init__.py
--rw-rw-rw-   0        0        0     1232 2022-11-05 13:39:56.000000 threadsnake-1.0.0/src/threadsnake/http/tools/common.py
--rw-rw-rw-   0        0        0     4357 2022-11-06 14:22:48.000000 threadsnake-1.0.0/src/threadsnake/http/tools/routing.py
--rw-rw-rw-   0        0        0     1371 2022-11-05 14:21:48.000000 threadsnake-1.0.0/src/threadsnake/http/types.py
-drwxrwxrwx   0        0        0        0 2022-11-09 02:14:00.260379 threadsnake-1.0.0/src/threadsnake/turbo/
--rw-rw-rw-   0        0        0      202 2022-11-05 15:43:46.000000 threadsnake-1.0.0/src/threadsnake/turbo/__init__.py
--rw-rw-rw-   0        0        0        8 2022-11-09 02:13:43.000000 threadsnake-1.0.0/src/threadsnake/version.txt
-drwxrwxrwx   0        0        0        0 2022-11-09 02:13:59.630502 threadsnake-1.0.0/src/threadsnake.egg-info/
--rw-rw-rw-   0        0        0      882 2022-11-09 02:13:59.000000 threadsnake-1.0.0/src/threadsnake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1613 2022-11-09 02:13:59.000000 threadsnake-1.0.0/src/threadsnake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-09 02:13:59.000000 threadsnake-1.0.0/src/threadsnake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-11-09 02:13:59.000000 threadsnake-1.0.0/src/threadsnake.egg-info/top_level.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.931063 threadsnake-1.0.1/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.1/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-04-07 21:09:28.927063 threadsnake-1.0.1/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.1/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-07 21:09:28.931063 threadsnake-1.0.1/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1420 2023-04-07 21:09:21.000000 threadsnake-1.0.1/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.903063 threadsnake-1.0.1/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.911063 threadsnake-1.0.1/src/threadsnake/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.915063 threadsnake-1.0.1/src/threadsnake/html/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/html/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      577 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/html/tools.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.919063 threadsnake-1.0.1/src/threadsnake/http/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/application.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/constants.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httprequest.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httpresponse.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/httpserver.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2559 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/server.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/session.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/core/values/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/contenttypes.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/core/values/responsecodes.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/middlewares/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/app.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/authorization.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/bodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/cors.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1332 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/defaultheaders.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/jsonbodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/multipartformdataparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/requests.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/session.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/static.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      467 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/middlewares/timemeassure.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/router.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/http/tools/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4248 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/tools/routing.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/http/types.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.927063 threadsnake-1.0.1/src/threadsnake/turbo/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.1/src/threadsnake/turbo/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 21:09:28.915063 threadsnake-1.0.1/src/threadsnake.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      775 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1575 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-07 21:09:28.000000 threadsnake-1.0.1/src/threadsnake.egg-info/top_level.txt
```

### Comparing `threadsnake-1.0.0/LICENSE` & `threadsnake-1.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `threadsnake-1.0.0/src/threadsnake/html/tools.py` & `threadsnake-1.0.1/src/threadsnake/html/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Dict
-
-def tag(name:str, content:str = None, attributes:Dict[str, str] = None, cls=None) -> str:
-    result = f'<{name}'
-    attributes = attributes or {}
-    if cls is not None: attributes['class'] = cls
-    attrib:str = ' '.join([f'{i}="{attributes[i]}"' for i in attributes])
-    result += attrib
-    if content is not None:
-        result += '/>'
-    else:
-        result += '>' + content + f'</{name}>'
-
-def link(location:str, text:str, cls:str = None):
-    return tag('a', text, {
-        "href": location
-    }, cls)
+from typing import Dict
+
+def tag(name:str, content:str = None, cls=None, *children, **attributes) -> str:
+    result = f'<{name}'
+    attributes = attributes or {}
+    if cls is not None: attributes['class'] = cls
+    attrib:str = ' '.join([f'{i}="{attributes[i]}"' for i in attributes])
+    result += attrib
+    if len(children) == 0:
+        result += '/>'
+    else:
+        result += '>'
+        for child in children:
+            result += child
+        result += f'</{name}>'
+
+def link(location:str, text:str, cls:str = None):
+    return tag('a', text, cls, href=location)
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/application.py` & `threadsnake-1.0.1/src/threadsnake/http/application.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from typing import Dict, List
-
-from .core.httprequest import retrieve_query_pass
-from .core.httpserver import HttpServer, HttpServerMessage
-from .router import Router
-from .types import Callback, Middleware
-import __main__
-import os
-
-class Application(HttpServer, Router):
-    def __init__(self, port: int, hostName: str = 'localhost', backlog: int = 8, chunkSize: int = 1024):
-        HttpServer.__init__(self, port, hostName, backlog, chunkSize)
-        Router.__init__(self)
-        self.stack:List[Middleware] = []
-        self.folder:str = os.path.dirname(__main__.__file__)
-    
-    def configure(self, middleware:Middleware):
-        self.stack.append(middleware)
-        return self
-
-    def on_handle(self, message: HttpServerMessage) -> bytes:
-        if len(message.data) == 0:
-            return
-        
-        stack:List[Middleware] = self.stack.copy()
-        
-        def next():
-            if len(stack) > 0 and not message.res.ended:
-                stack.pop()(self, message.req, message.res, next)
-
-        message.req = retrieve_query_pass(message.req)
-        callback:Callback = None
-        params:Dict[str, str]
-        callback, params = self.test_path(message.req.method, message.req.path)
-        if callback:
-            message.req.params.update(params)
-            stack.append(self.create_middleware(callback))
-
-        stack.reverse()
-        try:    
-            next()
-        except Exception as e:
-            message.res.end(str(e)).status(500, 'Internal Server Error')
-
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from typing import Dict, List
+
+from .core.httprequest import retrieve_query_pass
+from .core.httpserver import HttpServer, HttpServerMessage
+from .router import Router
+from .types import Callback, Middleware
+import __main__
+import os
+
+class Application(HttpServer, Router):
+    def __init__(self, port: int, hostName: str = 'localhost', backlog: int = 8, chunkSize: int = 1024):
+        HttpServer.__init__(self, port, hostName, backlog, chunkSize)
+        Router.__init__(self)
+        self.stack:List[Middleware] = []
+        self.folder:str = os.path.dirname(__main__.__file__)
+    
+    def configure(self, middleware:Middleware):
+        self.stack.append(middleware)
+        return self
+
+    def on_handle(self, message: HttpServerMessage) -> bytes:
+        if len(message.data) == 0:
+            return
+        
+        stack:List[Middleware] = self.stack.copy()
+        
+        def next():
+            if len(stack) > 0 and not message.res.ended:
+                stack.pop()(self, message.req, message.res, next)
+
+        message.req = retrieve_query_pass(message.req)
+        callback:Callback = None
+        params:Dict[str, str]
+        callback, params = self.test_path(message.req.method, message.req.path)
+        if callback:
+            message.req.params.update(params)
+            stack.append(self.create_middleware(callback))
+
+        stack.reverse()
+        try:    
+            next()
+        except Exception as e:
+            message.res.end(str(e)).status(500, 'Internal Server Error')
+
         return message.res.to_bytes()
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/common.py` & `threadsnake-1.0.1/src/threadsnake/http/core/common.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import re
-import socket
-import time
-from typing import Any, Callable, Dict, List, Tuple
-
-from .values.contenttypes import contentTypes
-from .values.responsecodes import responseCodes
-
-ClientAddress = Tuple[str, int]
-OnReceiveCallback = Callable[[Any, socket.socket, ClientAddress], bytes]
-
-
-def get_content_type(path:str):
-    contentType = 'text/plain'
-    if '.' in path:
-        extension:str = path.split(".")[-1:][0]
-        for i in contentTypes:
-            if extension in contentTypes[i]:
-                contentType = i
-                if contentType.endswith("/"):
-                    contentType += extension
-                break
-    return contentType
-
-def map_dictionary(data:str, rowSeparator:str, keySeparator:str) -> Dict[str, str]:
-    table:List[List[str]] = [
-        [j.strip() for j in i.split(keySeparator, 1)]
-        for i in data.split(rowSeparator) 
-        if len(i.split(keySeparator)) == 2
-    ]
-    return {row[0]:row[1] for row in table}
-
-def decode_querystring(data:str) -> Dict[str, str]:
-    data = data.replace('+', ' ').replace('%20', ' ')#space
-    data = data.replace('%2B', '+')#space
-    data = data.replace('%7E', '~')#space
-    references = [(i, chr(int(re.findall(r'[\d]+', i)[0]))) for i in re.findall(r'&#[\d]+;', data)]
-    for ref in references:
-        data = data.replace(ref[0], ref[1])
-    return data
-
-def get_cookie_expiration_UTC(durationSec:float) -> str:
-    return time.strftime("%a, %d %b %Y %H:%M:%S GMT", time.gmtime(time.time() + durationSec))
-
-def get_port(port:int, max_port=65535) -> int:
-        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        while port <= max_port:
-            try:
-                sock.bind(('', port))
-                sock.close()
-                return port
-            except OSError:
-                port += 1
-        else:
-            raise IOError('no free ports')
-
-def get_status_text_from_status_code(statusCode:int) -> str:
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import re
+import socket
+import time
+from typing import Any, Callable, Dict, List, Tuple
+
+from .values.contenttypes import contentTypes
+from .values.responsecodes import responseCodes
+
+ClientAddress = Tuple[str, int]
+OnReceiveCallback = Callable[[Any, socket.socket, ClientAddress], bytes]
+
+
+def get_content_type(path:str):
+    contentType = 'text/plain'
+    if '.' in path:
+        extension:str = path.split(".")[-1:][0]
+        for i in contentTypes:
+            if extension in contentTypes[i]:
+                contentType = i
+                if contentType.endswith("/"):
+                    contentType += extension
+                break
+    return contentType
+
+def map_dictionary(data:str, rowSeparator:str, keySeparator:str) -> Dict[str, str]:
+    table:List[List[str]] = [
+        [j.strip() for j in i.split(keySeparator, 1)]
+        for i in data.split(rowSeparator) 
+        if len(i.split(keySeparator)) == 2
+    ]
+    return {row[0]:row[1] for row in table}
+
+def decode_querystring(data:str) -> Dict[str, str]:
+    data = data.replace('+', ' ').replace('%20', ' ')#space
+    data = data.replace('%2B', '+')#space
+    data = data.replace('%7E', '~')#space
+    references = [(i, chr(int(re.findall(r'[\d]+', i)[0]))) for i in re.findall(r'&#[\d]+;', data)]
+    for ref in references:
+        data = data.replace(ref[0], ref[1])
+    return data
+
+def get_cookie_expiration_UTC(durationSec:float) -> str:
+    return time.strftime("%a, %d %b %Y %H:%M:%S GMT", time.gmtime(time.time() + durationSec))
+
+def get_port(port:int, max_port=65535) -> int:
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        while port <= max_port:
+            try:
+                sock.bind(('', port))
+                sock.close()
+                return port
+            except OSError:
+                port += 1
+        else:
+            raise IOError('no free ports')
+
+def get_status_text_from_status_code(statusCode:int) -> str:
     return responseCodes.get(statusCode, 'Unknown')
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/constants.py` & `threadsnake-1.0.1/src/threadsnake/http/core/constants.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-HEADER_CONTENT_TYPE = 'Content-Type'
-HEADER_CONTENT_LENGTH = 'Content-Length'
-HEADER_CONTENT_DISPOSITION = 'Content-Disposition'
-HEADER_COOKIES = 'Cookie'
-HEADER_LOCATION = 'Location'
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+HEADER_CONTENT_TYPE = 'Content-Type'
+HEADER_CONTENT_LENGTH = 'Content-Length'
+HEADER_CONTENT_DISPOSITION = 'Content-Disposition'
+HEADER_COOKIES = 'Cookie'
+HEADER_LOCATION = 'Location'
 LINESEP = '\r\n'
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/httprequest.py` & `threadsnake-1.0.1/src/threadsnake/http/core/httprequest.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import json
-from socket import socket
-from typing import Any, Dict, List
-
-from .session import Session
-
-from .common import decode_querystring, map_dictionary
-from .constants import HEADER_CONTENT_TYPE, HEADER_COOKIES
-from .server import ClientAddress
-
-class HttpQuery:
-    def __init__(self) -> None:
-        self.url = ''
-        self.querystring = ''
-        self.path = ''
-    
-    def load_query(self, url:str) -> Dict[str, str]:
-        self.url = url
-        self.path = url
-        if '?' in url:
-            self.path, url = url.split('?', 1)
-            self.querystring = decode_querystring(url)
-            return map_dictionary(self.querystring, '&', '=')
-        return dict()
-
-class Cookies:
-    def __init__(self, values:Dict[str, str] = None) -> None:
-        self.values = values or dict()
-
-    def load_cookies(self, raw:str):
-        self.values = map_dictionary(raw, ';', '=')
-        return self
-
-class HttpRequest(HttpQuery):
-    def __init__(self, raw:str, client:socket, clientAddress:ClientAddress) -> None:
-        HttpQuery.__init__(self)
-        self.client = client
-        self.clientAddress = clientAddress
-        self.headers:Dict[str, str] = {}
-        self.params:Dict[str, str] = {}
-        self.cookies:Cookies = Cookies()
-        self.contentType:str = ''
-        self.files:Dict[str, str] = {}
-        self.authorization = {}
-        self.session:Session = None
-        self.data:Any = None
-        self.raw = ''
-        self.body:str = ''
-        self.method:str = ''
-        self.httpVersion:str = ''
-        self.load(raw)
-
-    def load(self, raw:str):
-        self.raw = raw
-        requestParts:List[str] = raw.split('\r\n\r\n', maxsplit=1)
-        statusAndHeaders:List[str] = requestParts[0].split('\r\n')
-        self.load_status(statusAndHeaders[0])
-        self.load_headers(statusAndHeaders[1:])
-        if len(requestParts) > 1:
-            self.load_body(requestParts[1])
-
-    def load_status(self, statusLine:str):
-        status:List[str] = statusLine.split(' ')
-        self.method = status[0]
-        self.httpVersion = status[2] if len(status) > 2 else 'HTTP/1.1'
-        if len(status) > 1:
-            self.params = self.load_query(status[1])
-
-
-    def load_headers(self, headers:List[str]):
-        headerPairs:List[List[str]] = [
-            [j.strip() for j in i.split(':', 1)] 
-            for i in headers
-            if len(i.split(':')) == 2
-        ]
-        self.headers = {header[0]:header[1] for header in headerPairs}
-        if HEADER_COOKIES in self.headers:
-            self.cookies = Cookies().load_cookies(self.headers[HEADER_COOKIES])
-        if HEADER_CONTENT_TYPE in self.headers:
-            self.contentType = self.headers[HEADER_CONTENT_TYPE]
-
-    def load_body(self, body:str):
-        self.body = body
-
-    def json(self):
-        try:
-            return json.loads(self.body)
-        except:
-            return None
-
-def retrieve_query_pass(req:HttpRequest) -> HttpRequest:
-    if ':' in req.path:
-        path:List[str] = req.path.split('/')
-        req.path = '/'.join([i for i in path if len(i.split(':', 1)) != 2])
-        req.params.update({i[0]:i[1] for i in path if len(i.split(':', 1)) == 2})
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import json
+from socket import socket
+from typing import Any, Dict, List
+
+from .session import Session
+
+from .common import decode_querystring, map_dictionary
+from .constants import HEADER_CONTENT_TYPE, HEADER_COOKIES
+from .server import ClientAddress
+
+class HttpQuery:
+    def __init__(self) -> None:
+        self.url = ''
+        self.querystring = ''
+        self.path = ''
+    
+    def load_query(self, url:str) -> Dict[str, str]:
+        self.url = url
+        self.path = url
+        if '?' in url:
+            self.path, url = url.split('?', 1)
+            self.querystring = decode_querystring(url)
+            return map_dictionary(self.querystring, '&', '=')
+        return dict()
+
+class Cookies:
+    def __init__(self, values:Dict[str, str] = None) -> None:
+        self.values = values or dict()
+
+    def load_cookies(self, raw:str):
+        self.values = map_dictionary(raw, ';', '=')
+        return self
+
+class HttpRequest(HttpQuery):
+    def __init__(self, raw:str, client:socket, clientAddress:ClientAddress) -> None:
+        HttpQuery.__init__(self)
+        self.client = client
+        self.clientAddress = clientAddress
+        self.headers:Dict[str, str] = {}
+        self.params:Dict[str, str] = {}
+        self.cookies:Cookies = Cookies()
+        self.contentType:str = ''
+        self.files:Dict[str, str] = {}
+        self.authorization = {}
+        self.session:Session = None
+        self.data:Any = None
+        self.raw = ''
+        self.body:str = ''
+        self.method:str = ''
+        self.httpVersion:str = ''
+        self.load(raw)
+
+    def load(self, raw:str):
+        self.raw = raw
+        requestParts:List[str] = raw.split('\r\n\r\n', maxsplit=1)
+        statusAndHeaders:List[str] = requestParts[0].split('\r\n')
+        self.load_status(statusAndHeaders[0])
+        self.load_headers(statusAndHeaders[1:])
+        if len(requestParts) > 1:
+            self.load_body(requestParts[1])
+
+    def load_status(self, statusLine:str):
+        status:List[str] = statusLine.split(' ')
+        self.method = status[0]
+        self.httpVersion = status[2] if len(status) > 2 else 'HTTP/1.1'
+        if len(status) > 1:
+            self.params = self.load_query(status[1])
+
+
+    def load_headers(self, headers:List[str]):
+        headerPairs:List[List[str]] = [
+            [j.strip() for j in i.split(':', 1)] 
+            for i in headers
+            if len(i.split(':')) == 2
+        ]
+        self.headers = {header[0]:header[1] for header in headerPairs}
+        if HEADER_COOKIES in self.headers:
+            self.cookies = Cookies().load_cookies(self.headers[HEADER_COOKIES])
+        if HEADER_CONTENT_TYPE in self.headers:
+            self.contentType = self.headers[HEADER_CONTENT_TYPE]
+
+    def load_body(self, body:str):
+        self.body = body
+
+    def json(self):
+        try:
+            return json.loads(self.body)
+        except:
+            return None
+
+def retrieve_query_pass(req:HttpRequest) -> HttpRequest:
+    if ':' in req.path:
+        path:List[str] = req.path.split('/')
+        req.path = '/'.join([i for i in path if len(i.split(':', 1)) != 2])
+        req.params.update({i[0]:i[1] for i in path if len(i.split(':', 1)) == 2})
     return req
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/httpresponse.py` & `threadsnake-1.0.1/src/threadsnake/http/core/httpresponse.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import json
-from typing import Any, Dict, List
-from .common import get_content_type, get_cookie_expiration_UTC, get_status_text_from_status_code
-from .constants import HEADER_CONTENT_DISPOSITION, HEADER_CONTENT_LENGTH, HEADER_CONTENT_TYPE, HEADER_LOCATION, LINESEP
-
-class ResponseHead:
-    def __init__(self) -> None:
-        self.httpVersion:str = 'HTTP/1.1'
-        self.responseStatus:int = 404
-        self.responseStatusText:str = 'NotFound'
-        self.headers:Dict[str, List[str]] = dict()
-    
-    def append_header(self, name:str, value:str):
-        if name not in self.headers:
-            self.headers[name] = []
-        self.headers[name].append(value)
-    
-    def set_header(self, name:str, value:str):
-        self.headers[name] = [value]
-
-    def get_header(self, name:str) -> str:
-        if name in self.headers:
-            return self.headers[name][0]
-        return None
- 
-    def get_headers(self, name:str) -> List[str]:
-        if name in self.headers:
-            return self.headers[name]
-        return None
-
-    def remove_header(self, name:str) -> str:
-        if name in self.headers:
-            del self.headers[name]
-
-    def set_cookie(self, name:str, value:str, durationSec:float = None, domain:str = None, path:str = None):
-        cookieString = [value]
-        if durationSec != None: cookieString.append(f'Expires={get_cookie_expiration_UTC(durationSec)}')
-        if domain is not None: cookieString.append(f'Domain={domain}')
-        if path is not None: cookieString.append(f'Path={path}')
-        cookieHeader = f'{name}=' + '; '.join(cookieString)
-        self.append_header('Set-Cookie', cookieHeader)
-
-    def to_string(self) -> str:
-        result:str = f'{self.httpVersion} {self.responseStatus} {self.responseStatusText} {LINESEP}'
-        for header in self.headers:
-            for headerValue in self.headers[header]:
-                result += f'{header}: {headerValue}{LINESEP}'
-        return result
-
-class HttpResponse(ResponseHead):
-    def __init__(self) -> None:
-        ResponseHead.__init__(self)
-        self.body:str = ''
-        self.encoding:str = 'latin-1'
-        self.ended:bool = False
-    
-    def end(self, data:str = None, status:int = None):
-        self.ended = True
-        return self.status(status).write(data)
-
-    def status(self, responseCode:int = None, responseText:str = None):
-        self.responseStatus = responseCode or self.responseStatus
-        responseText = responseText or get_status_text_from_status_code(self.responseStatus)
-        self.responseStatusText = responseText
-        return self
-
-    def append_header(self, name: str, value: str):
-        ResponseHead.append_header(self, name, value)
-        return self
-
-    def set_header(self, name: str, value: str):
-        ResponseHead.set_header(self, name, value)
-        return self
-
-    def set_cookie(self, name: str, value: str, durationSec: float = None, domain: str = None, path: str = None):
-        ResponseHead.set_cookie(self, name, value, durationSec, domain, path)
-        return self
-
-    def content_disposition(self, value:str, fileName:str = None):
-        if fileName is not None:
-            value += f'; filename="{fileName}"'
-        return self.set_header(HEADER_CONTENT_DISPOSITION, value)
-
-    def content_type(self, value:str):
-        return self.set_header(HEADER_CONTENT_TYPE, value)
-
-    def redirect(self, value:str):
-        return self.set_header(HEADER_LOCATION, value)
-
-    def set_encoding(self, value:str):
-        self.encoding = value
-        return self
-
-    def write(self, data:str):
-        self.body += data
-        return self
-
-    def json(self, data:Any):
-        return self\
-        .write(json.dumps(data))\
-        .content_type('application/json')\
-        .status(200, 'OK')
-
-    def html(self, data:str):
-        return self\
-        .write(data)\
-        .content_type('text/html')\
-        .status(200, 'OK')
-
-    def read_file(self, fileName:str, encoding:str = None):
-        self.set_encoding(encoding or self.encoding)
-        with open(fileName, 'r', encoding=self.encoding) as f:
-            self.write(f.read())
-        return self.status(200, 'OK').content_type(get_content_type(fileName))
-
-    def file(self, fileName:str, data:str, contentType:str = None, encoding:str = None):
-        self.content_disposition('attachment', fileName)
-        self.set_encoding(encoding or self.encoding)
-        self.status(200, 'OK')
-        if contentType is not None:
-            self.content_type(contentType)
-        self.body = data
-
-    def download(self, path:str, fileName:str, contentType:str = None, encoding:str = None):
-        self.fileName('attachment', fileName)
-        self.body = ""
-        return self.read_file(path, encoding)
-
-    def to_bytes(self)->bytes:
-        return str(self).encode(self.encoding)
-
-    def __str__(self) -> str:
-        if HEADER_LOCATION not in self.headers:
-            self.set_header(HEADER_CONTENT_LENGTH, len(self.body))
-        return ResponseHead.to_string(self) + LINESEP + self.body
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import json
+from typing import Any, Dict, List
+from .common import get_content_type, get_cookie_expiration_UTC, get_status_text_from_status_code
+from .constants import HEADER_CONTENT_DISPOSITION, HEADER_CONTENT_LENGTH, HEADER_CONTENT_TYPE, HEADER_LOCATION, LINESEP
+
+class ResponseHead:
+    def __init__(self) -> None:
+        self.httpVersion:str = 'HTTP/1.1'
+        self.responseStatus:int = 404
+        self.responseStatusText:str = 'NotFound'
+        self.headers:Dict[str, List[str]] = dict()
+    
+    def append_header(self, name:str, value:str):
+        if name not in self.headers:
+            self.headers[name] = []
+        self.headers[name].append(value)
+    
+    def set_header(self, name:str, value:str):
+        self.headers[name] = [value]
+
+    def get_header(self, name:str) -> str:
+        if name in self.headers:
+            return self.headers[name][0]
+        return None
+ 
+    def get_headers(self, name:str) -> List[str]:
+        if name in self.headers:
+            return self.headers[name]
+        return None
+
+    def remove_header(self, name:str) -> str:
+        if name in self.headers:
+            del self.headers[name]
+
+    def set_cookie(self, name:str, value:str, durationSec:float = None, domain:str = None, path:str = None):
+        cookieString = [value]
+        if durationSec != None: cookieString.append(f'Expires={get_cookie_expiration_UTC(durationSec)}')
+        if domain is not None: cookieString.append(f'Domain={domain}')
+        if path is not None: cookieString.append(f'Path={path}')
+        cookieHeader = f'{name}=' + '; '.join(cookieString)
+        self.append_header('Set-Cookie', cookieHeader)
+
+    def to_string(self) -> str:
+        result:str = f'{self.httpVersion} {self.responseStatus} {self.responseStatusText} {LINESEP}'
+        for header in self.headers:
+            for headerValue in self.headers[header]:
+                result += f'{header}: {headerValue}{LINESEP}'
+        return result
+
+class HttpResponse(ResponseHead):
+    def __init__(self) -> None:
+        ResponseHead.__init__(self)
+        self.body:str = ''
+        self.encoding:str = 'latin-1'
+        self.ended:bool = False
+    
+    def end(self, data:str = None, status:int = None):
+        self.ended = True
+        return self.status(status).write(data)
+
+    def status(self, responseCode:int = None, responseText:str = None):
+        self.responseStatus = responseCode or self.responseStatus
+        responseText = responseText or get_status_text_from_status_code(self.responseStatus)
+        self.responseStatusText = responseText
+        return self
+
+    def append_header(self, name: str, value: str):
+        ResponseHead.append_header(self, name, value)
+        return self
+
+    def set_header(self, name: str, value: str):
+        ResponseHead.set_header(self, name, value)
+        return self
+
+    def set_cookie(self, name: str, value: str, durationSec: float = None, domain: str = None, path: str = None):
+        ResponseHead.set_cookie(self, name, value, durationSec, domain, path)
+        return self
+
+    def content_disposition(self, value:str, fileName:str = None):
+        if fileName is not None:
+            value += f'; filename="{fileName}"'
+        return self.set_header(HEADER_CONTENT_DISPOSITION, value)
+
+    def content_type(self, value:str):
+        return self.set_header(HEADER_CONTENT_TYPE, value)
+
+    def redirect(self, value:str):
+        return self.set_header(HEADER_LOCATION, value)
+
+    def set_encoding(self, value:str):
+        self.encoding = value
+        return self
+
+    def write(self, data:str):
+        self.body += data
+        return self
+
+    def json(self, data:Any):
+        return self\
+        .write(json.dumps(data))\
+        .content_type('application/json')\
+        .status(200, 'OK')
+
+    def html(self, data:str):
+        return self\
+        .write(data)\
+        .content_type('text/html')\
+        .status(200, 'OK')
+
+    def read_file(self, fileName:str, encoding:str = None):
+        self.set_encoding(encoding or self.encoding)
+        with open(fileName, 'r', encoding=self.encoding) as f:
+            self.write(f.read())
+        return self.status(200, 'OK').content_type(get_content_type(fileName))
+
+    def file(self, fileName:str, data:str, contentType:str = None, encoding:str = None):
+        self.content_disposition('attachment', fileName)
+        self.set_encoding(encoding or self.encoding)
+        self.status(200, 'OK')
+        if contentType is not None:
+            self.content_type(contentType)
+        self.body = data
+
+    def download(self, path:str, fileName:str, contentType:str = None, encoding:str = None):
+        self.fileName('attachment', fileName)
+        self.body = ""
+        return self.read_file(path, encoding)
+
+    def to_bytes(self)->bytes:
+        return str(self).encode(self.encoding)
+
+    def __str__(self) -> str:
+        if HEADER_LOCATION not in self.headers:
+            self.set_header(HEADER_CONTENT_LENGTH, len(self.body))
+        return ResponseHead.to_string(self) + LINESEP + self.body
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/httpserver.py` & `threadsnake-1.0.1/src/threadsnake/http/core/httpserver.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import socket
-from .httprequest import HttpRequest
-from .httpresponse import HttpResponse
-from .server import ClientAddress, Server
-
-class HttpServerMessage:
-    def __init__(self, client:socket.socket, address:ClientAddress, data:bytearray) -> None:
-        self.client:socket.socket = client
-        self.address:ClientAddress = address
-        self.data:bytearray = None
-        self.req:HttpRequest = None
-        self.res:HttpResponse = HttpResponse()
-        self.load_request(data)
-
-    def load_request(self, data:bytearray):
-        self.data = data
-        try:
-            self.req = HttpRequest(data.decode('latin-1'), self.client, self.address)
-        except:
-            self.res.status(403, 'Bad Request')
-        return self
-
-class HttpServer(Server):
-    def __init__(self, port: int, hostName: str = 'localhost', backlog: int = 8, chunkSize: int = 1024) -> None:
-        super().__init__(port, self.on_receive, hostName, backlog, chunkSize)
-
-    def on_handle(self, message:HttpServerMessage) -> bytes:
-        return b'HTTP/1.1 200 OK\n\n'
-
-    def on_receive(self, client:socket.socket, address:ClientAddress, data:bytearray) -> bytes:
-        if len(data) != 0:
-            message = HttpServerMessage(client, address, data)
-            return self.on_handle(message)
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import socket
+from .httprequest import HttpRequest
+from .httpresponse import HttpResponse
+from .server import ClientAddress, Server
+
+class HttpServerMessage:
+    def __init__(self, client:socket.socket, address:ClientAddress, data:bytearray) -> None:
+        self.client:socket.socket = client
+        self.address:ClientAddress = address
+        self.data:bytearray = None
+        self.req:HttpRequest = None
+        self.res:HttpResponse = HttpResponse()
+        self.load_request(data)
+
+    def load_request(self, data:bytearray):
+        self.data = data
+        try:
+            self.req = HttpRequest(data.decode('latin-1'), self.client, self.address)
+        except:
+            self.res.status(403, 'Bad Request')
+        return self
+
+class HttpServer(Server):
+    def __init__(self, port: int, hostName: str = 'localhost', backlog: int = 8, chunkSize: int = 1024) -> None:
+        super().__init__(port, self.on_receive, hostName, backlog, chunkSize)
+
+    def on_handle(self, message:HttpServerMessage) -> bytes:
+        return b'HTTP/1.1 200 OK\n\n'
+
+    def on_receive(self, client:socket.socket, address:ClientAddress, data:bytearray) -> bytes:
+        if len(data) != 0:
+            message = HttpServerMessage(client, address, data)
+            return self.on_handle(message)
         return b'HTTP/1.1 200 OK\n\n'
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/server.py` & `threadsnake-1.0.1/src/threadsnake/http/core/server.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import asyncio
-import socket
-from .common import ClientAddress, OnReceiveCallback
-
-class Server:
-    def __init__(self, port:int, onReceive:OnReceiveCallback, hostName:str = 'localhost', backlog:int = 8, chunkSize:int = 1024) -> None:
-        self.port = port
-        self.hostname = hostName
-        self.backlog = backlog
-        self.chunkSize = chunkSize
-        self.onReceive = onReceive
-
-    def loop(self):
-        return asyncio.get_event_loop()
-
-    async def read(self, client:socket.socket, size:int) -> bytes:
-        try:
-            return await asyncio.wait_for(self.loop().sock_recv(client, size), 0.1)
-        except Exception as e:
-            return b''
-
-    async def on_accept(self, client:socket.socket, address:ClientAddress):
-        data:bytearray = bytearray()
-        while True:
-            chunk:bytes = await self.read(client, self.chunkSize)
-            if len(chunk) == 0:
-                break
-            data.extend(chunk)
-        response:bytes = self.onReceive(client, address, data)
-        await self.loop().sock_sendall(client, response)
-        client.close()
-
-    async def run(self):
-        serverSocket:socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        serverSocket.bind((self.hostname, self.port))
-        serverSocket.listen(self.backlog)
-        serverSocket.setblocking(False)
-        
-        loop:asyncio.AbstractEventLoop = self.loop()
-
-        while True:
-            client:socket.socket = None
-            address:ClientAddress = ('', 0)
-            client, address = await loop.sock_accept(serverSocket)
-            loop.create_task(self.on_accept(client, address))
-
-    def start(self):
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import asyncio
+import socket
+from .common import ClientAddress, OnReceiveCallback
+
+class Server:
+    def __init__(self, port:int, onReceive:OnReceiveCallback, hostName:str = 'localhost', backlog:int = 8, chunkSize:int = 1024) -> None:
+        self.port = port
+        self.hostname = hostName
+        self.backlog = backlog
+        self.chunkSize = chunkSize
+        self.onReceive = onReceive
+
+    def loop(self):
+        return asyncio.get_event_loop()
+
+    async def read(self, client:socket.socket, size:int) -> bytes:
+        try:
+            return await asyncio.wait_for(self.loop().sock_recv(client, size), 0.1)
+        except Exception as e:
+            return b''
+
+    async def on_accept(self, client:socket.socket, address:ClientAddress):
+        data:bytearray = bytearray()
+        while True:
+            chunk:bytes = await self.read(client, self.chunkSize)
+            if len(chunk) == 0:
+                break
+            data.extend(chunk)
+        response:bytes = self.onReceive(client, address, data)
+        await self.loop().sock_sendall(client, response)
+        client.close()
+
+    async def run(self):
+        serverSocket:socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        serverSocket.bind((self.hostname, self.port))
+        serverSocket.listen(self.backlog)
+        serverSocket.setblocking(False)
+        
+        loop:asyncio.AbstractEventLoop = self.loop()
+
+        while True:
+            client:socket.socket = None
+            address:ClientAddress = ('', 0)
+            client, address = await loop.sock_accept(serverSocket)
+            loop.create_task(self.on_accept(client, address))
+
+    def start(self):
         asyncio.run(self.run())
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/core/session.py` & `threadsnake-1.0.1/src/threadsnake/http/core/session.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from typing import Any, Dict
-
-class Session:
-    def __init__(self) -> None:
-        self.values:Dict[str,Any] = dict()
-    
-    def set(self, key:str, value:Any):
-        self.values[key] = value
-
-    def has(self, key:str) -> bool:
-        return key in self.values
-
-    def get(self, key:str, default:Any) -> Any:
-        if not self.has(key):
-            self.set(key, default)
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from typing import Any, Dict
+
+class Session:
+    def __init__(self) -> None:
+        self.values:Dict[str,Any] = dict()
+    
+    def set(self, key:str, value:Any):
+        self.values[key] = value
+
+    def has(self, key:str) -> bool:
+        return key in self.values
+
+    def get(self, key:str, default:Any) -> Any:
+        if not self.has(key):
+            self.set(key, default)
         return self.values[key]
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/authorization.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/authorization.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from base64 import b64decode
-from ...http.types import Next
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-
-def authorization(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
-    authKey:str = 'Authorization'
-    if authKey in req.headers:
-        authType, authValue = req.headers[authKey].split(' ', 1)
-        req.authorization[authType] = ''
-        if authType == 'Bearer':
-            req.authorization[authType] = authValue 
-        elif authType == 'Basic':
-            user, password = b64decode(authValue.encode()).decode().split(':')
-            req.authorization[authType] = {'user':user, 'password':password}
-        del req.headers[authKey]
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from base64 import b64decode
+from ...http.types import Next
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+
+def authorization(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
+    authKey:str = 'Authorization'
+    if authKey in req.headers:
+        authType, authValue = req.headers[authKey].split(' ', 1)
+        req.authorization[authType] = ''
+        if authType == 'Bearer':
+            req.authorization[authType] = authValue 
+        elif authType == 'Basic':
+            user, password = b64decode(authValue.encode()).decode().split(':')
+            req.authorization[authType] = {'user':user, 'password':password}
+        del req.headers[authKey]
     next()
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/bodyparser.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/static.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from ...http.types import Next
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-from ..core.common import decode_querystring, map_dictionary
-
-def body_parser(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
-    if req.contentType != None and 'x-www-form-urlencoded' in req.contentType:
-        rawParams:str = decode_querystring(req.body.strip())
-        req.params.update(map_dictionary(rawParams, '&', '='))
-    next()
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import os
+from ...http.types import Middleware, Next
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+
+def static(rootFolder:str = 'static') -> Middleware:
+    def middleware(app:Application, req:HttpRequest, res:HttpResponse, next:Next):
+        normalizedUrl = req.path.replace('\\', os.sep).replace('..', '')
+        filename:str = os.sep.join([app.folder, rootFolder, normalizedUrl])
+        if os.path.isfile(filename):
+            res.read_file(filename)
+        else:
+            next()
+    return middleware
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/jsonbodyparser.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/jsonbodyparser.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import json
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-from ...http.types import Next
-
-def json_body_parser(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
-    '''
-    Configures "json" request type. If identifies a valid json in the request body, it sets
-    the dict property of the current HttpRequest instance with the json content.
-    '''
-    if req.contentType in ['application/json', 'text/json']:
-        try:
-            req.data = json.loads(req.body.strip())
-        except:
-            res.status(400, 'Bad Request').write("Can't decode json body")
+import json
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+from ...http.types import Next
+
+def json_body_parser(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
+    '''
+    Configures "json" request type. If identifies a valid json in the request body, it sets
+    the dict property of the current HttpRequest instance with the json content.
+    '''
+    if req.contentType in ['application/json', 'text/json']:
+        try:
+            req.data = json.loads(req.body.strip())
+        except:
+            res.status(400, 'Bad Request').write("Can't decode json body")
     next()
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/multipartformdataparser.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/multipartformdataparser.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import os
-from time import time
-from typing import Callable, Dict, List
-from uuid import uuid4
-
-from ...http.core.common import map_dictionary
-from ...http.types import Middleware, Next
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-
-
-def save_as_binary(tempFolder:str, data:str):
-    tempFileName:str = os.sep.join([tempFolder, str(uuid4()).replace('-', '')+'.tmp'])
-    if not os.path.isdir(tempFolder):
-        os.mkdir(tempFolder)
-    with open(tempFileName,'wb') as f:
-        f.write(data.encode('latin-1'))
-    return tempFileName
-
-def get_chunked(req:HttpRequest) -> str:
-    body:str = req.body
-    if 'chunked' in req.headers.get('Transfer-Encoding', '') and '\r\n' in body:
-        res = ''
-        chunk_i = 1
-        while chunk_i > 0:
-            split = body.split('\r\n', maxsplit=1)
-            chunk, body = split if len(split) == 2 else [split[0], '']
-            chunk_i = int(chunk, 16)
-            res += body[:chunk_i]
-            body = body[chunk_i+2:]
-        body = res
-    return body
-
-def build_file_decoder(files:Dict[str, float], folder:str, duration:int):
-    def decode_body_parameter(parameter:str, req:HttpRequest):
-        header, value = parameter.split('\r\n\r\n', maxsplit=1)
-        header = header.replace('\r\n', '; ').replace(': ', '=').replace('"', '')
-        headerDict = map_dictionary(header, ';', '=')
-        if 'filename' in headerDict:
-            filename:str = headerDict['filename']
-            tempFileLocation:str = save_as_binary(folder, value)
-            req.files[filename] = tempFileLocation
-            files[tempFileLocation] = time() + duration
-        elif 'name' in headerDict:
-            req.params[headerDict['name']] = value
-    return decode_body_parameter
-
-def remove_old_files(files:Dict[str, float]) -> None:
-    removedFiles:List[str] = []
-    for file in files:
-        if files[file] < time():
-            try:
-                os.remove(file)
-                removedFiles.append(file)
-            except:
-                print(f'error removing file: {file}')
-    for file in removedFiles:
-        del files[file]
-
-def multipart_form_data_parser(tempFolder:str = None, filesDurationSec:int = 30) -> Middleware:
-    files:Dict[str, float] = {}
-    tempFolder = tempFolder or os.sep.join(['.', 'temp'])
-    decoder:Callable[[str, HttpRequest], None] = None
-    decoder = build_file_decoder(files, tempFolder, filesDurationSec)
-    def middleware(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
-        if 'multipart/form-data' in req.contentType:
-            boundary:str = ''
-            req.contentType, boundary = [i.strip() for i in req.contentType.split(';', 1)]
-            boundary = boundary.strip().replace('boundary=', '--').replace('"', '')
-            body:str = get_chunked(req)
-            bodyParameters:List[str] = [i.strip() for i in body.split(boundary)]
-            for param in bodyParameters:
-                if param == '--' or len(param) == 0:
-                    continue
-                decoder(param, req)
-        remove_old_files(files)
-        next()
-    return middleware
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import os
+from time import time
+from typing import Callable, Dict, List
+from uuid import uuid4
+
+from ...http.core.common import map_dictionary
+from ...http.types import Middleware, Next
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+
+
+def save_as_binary(tempFolder:str, data:str):
+    tempFileName:str = os.sep.join([tempFolder, str(uuid4()).replace('-', '')+'.tmp'])
+    if not os.path.isdir(tempFolder):
+        os.mkdir(tempFolder)
+    with open(tempFileName,'wb') as f:
+        f.write(data.encode('latin-1'))
+    return tempFileName
+
+def get_chunked(req:HttpRequest) -> str:
+    body:str = req.body
+    if 'chunked' in req.headers.get('Transfer-Encoding', '') and '\r\n' in body:
+        res = ''
+        chunk_i = 1
+        while chunk_i > 0:
+            split = body.split('\r\n', maxsplit=1)
+            chunk, body = split if len(split) == 2 else [split[0], '']
+            chunk_i = int(chunk, 16)
+            res += body[:chunk_i]
+            body = body[chunk_i+2:]
+        body = res
+    return body
+
+def build_file_decoder(files:Dict[str, float], folder:str, duration:int):
+    def decode_body_parameter(parameter:str, req:HttpRequest):
+        header, value = parameter.split('\r\n\r\n', maxsplit=1)
+        header = header.replace('\r\n', '; ').replace(': ', '=').replace('"', '')
+        headerDict = map_dictionary(header, ';', '=')
+        if 'filename' in headerDict:
+            filename:str = headerDict['filename']
+            tempFileLocation:str = save_as_binary(folder, value)
+            req.files[filename] = tempFileLocation
+            files[tempFileLocation] = time() + duration
+        elif 'name' in headerDict:
+            req.params[headerDict['name']] = value
+    return decode_body_parameter
+
+def remove_old_files(files:Dict[str, float]) -> None:
+    removedFiles:List[str] = []
+    for file in files:
+        if files[file] < time():
+            try:
+                os.remove(file)
+                removedFiles.append(file)
+            except:
+                print(f'error removing file: {file}')
+    for file in removedFiles:
+        del files[file]
+
+def multipart_form_data_parser(tempFolder:str = None, filesDurationSec:int = 30) -> Middleware:
+    files:Dict[str, float] = {}
+    tempFolder = tempFolder or os.sep.join(['.', 'temp'])
+    decoder:Callable[[str, HttpRequest], None] = None
+    decoder = build_file_decoder(files, tempFolder, filesDurationSec)
+    def middleware(app:Application, req:HttpRequest, res:HttpResponse, next:Next) -> None:
+        if 'multipart/form-data' in req.contentType:
+            boundary:str = ''
+            req.contentType, boundary = [i.strip() for i in req.contentType.split(';', 1)]
+            boundary = boundary.strip().replace('boundary=', '--').replace('"', '')
+            body:str = get_chunked(req)
+            bodyParameters:List[str] = [i.strip() for i in body.split(boundary)]
+            for param in bodyParameters:
+                if param == '--' or len(param) == 0:
+                    continue
+                decoder(param, req)
+        remove_old_files(files)
+        next()
+    return middleware
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/requests.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/requests.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import List
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-from ...http.types import CallbackMutator, Callback, RequestPredicate
-
-def validates_request(predicate:RequestPredicate, onFailMessage:str = None, onFailStatus:int = 400) -> CallbackMutator:
-    '''
-    Generalizes request validation using a "predicate" function wich receives the current HttpRequestInstance
-    and returns a boolean. If the result is false, the client receives an "onFailStatus" status code and an
-    "onFailMessage" message. Otherwise the pipeline executes normally.
-    '''
-    def mutator(middleware:Callback) -> Callback:
-        def callback(app:Application, req:HttpRequest, res: HttpResponse) -> None:
-            if predicate(req):
-                middleware(app, req, res)
-            else:
-                res.end(onFailMessage or "Bad Request", onFailStatus)
-        return callback
-    return mutator
-
-def accepts(contentTypes:List[str]) -> CallbackMutator:
-    '''
-    Validates the HttpRequest content-type against the list of "contentTypes", with are the allowed ones. 
-    Returns an UnsuportedMediaType status code if the content-type is not in the list. Otherwise the 
-    pipeline executes normally. Delegates to "validates_request".
-    '''
-    return validates_request(lambda r: r.contentType in contentTypes, onFailStatus=415)
-
-def accepts_json(callback:Callback) -> Callback:
-    '''Especialization of accepts wich just allows json requests.'''
-    return accepts(['application/json', 'text/json'])(callback)
-
-def requires_parameters(parameters:List[str]) -> CallbackMutator:
-    def predicate(req:HttpRequest) -> bool:
-        receivedParameters:List[str] = [i for i in req.params]
-        return len([i for i in parameters if i not in receivedParameters]) == 0
-    message:str = 'Required parameters: ' + ', '.join(parameters)
+from typing import List
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+from ...http.types import CallbackMutator, Callback, RequestPredicate
+
+def validates_request(predicate:RequestPredicate, onFailMessage:str = None, onFailStatus:int = 400) -> CallbackMutator:
+    '''
+    Generalizes request validation using a "predicate" function wich receives the current HttpRequestInstance
+    and returns a boolean. If the result is false, the client receives an "onFailStatus" status code and an
+    "onFailMessage" message. Otherwise the pipeline executes normally.
+    '''
+    def mutator(middleware:Callback) -> Callback:
+        def callback(app:Application, req:HttpRequest, res: HttpResponse) -> None:
+            if predicate(req):
+                middleware(app, req, res)
+            else:
+                res.end(onFailMessage or "Bad Request", onFailStatus)
+        return callback
+    return mutator
+
+def accepts(contentTypes:List[str]) -> CallbackMutator:
+    '''
+    Validates the HttpRequest content-type against the list of "contentTypes", with are the allowed ones. 
+    Returns an UnsuportedMediaType status code if the content-type is not in the list. Otherwise the 
+    pipeline executes normally. Delegates to "validates_request".
+    '''
+    return validates_request(lambda r: r.contentType in contentTypes, onFailStatus=415)
+
+def accepts_json(callback:Callback) -> Callback:
+    '''Especialization of accepts wich just allows json requests.'''
+    return accepts(['application/json', 'text/json'])(callback)
+
+def requires_parameters(parameters:List[str]) -> CallbackMutator:
+    def predicate(req:HttpRequest) -> bool:
+        receivedParameters:List[str] = [i for i in req.params]
+        return len([i for i in parameters if i not in receivedParameters]) == 0
+    message:str = 'Required parameters: ' + ', '.join(parameters)
     return validates_request(predicate, message)
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/middlewares/session.py` & `threadsnake-1.0.1/src/threadsnake/http/middlewares/session.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from time import time
-from typing import Dict, Tuple
-import uuid
-
-from ...http.types import Middleware, Next
-from ..core.session import Session
-from ..core.httprequest import HttpRequest
-from ..core.httpresponse import HttpResponse
-from ..application import Application
-
-def session(cookieName:str, durationSec:float = 300) -> Middleware:
-    sessions:Dict[str, Tuple[Session, float]] = dict()
-    lastCheck:float = time()
-
-    def removeExpired():
-        nonlocal lastCheck
-        if time() - lastCheck > durationSec / 10:
-            lastCheck = time()
-            expiredSessions = [i for i in sessions if sessions[i][1] < time()]
-            for e in expiredSessions:
-                del sessions[e]
-
-    def middleware(app:Application, req:HttpRequest, res:HttpResponse, next:Next):
-        removeExpired()
-        sessionId:str = None
-        if cookieName not in req.cookies.values:
-            sessionId = str(uuid.uuid4())
-            res.set_cookie(cookieName, sessionId, durationSec)
-        else:
-            sessionId = req.cookies.values[cookieName]
-
-        if sessionId not in sessions:
-            sessions[sessionId] = [Session(), durationSec + time()]
-        else:
-            sessions[sessionId][1] = durationSec + time()
-
-        req.session = sessions[sessionId][0]
-        next()
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from time import time
+from typing import Dict, Tuple
+import uuid
+
+from ...http.types import Middleware, Next
+from ..core.session import Session
+from ..core.httprequest import HttpRequest
+from ..core.httpresponse import HttpResponse
+from ..application import Application
+
+def session(cookieName:str, durationSec:float = 300) -> Middleware:
+    sessions:Dict[str, Tuple[Session, float]] = dict()
+    lastCheck:float = time()
+
+    def removeExpired():
+        nonlocal lastCheck
+        if time() - lastCheck > durationSec / 10:
+            lastCheck = time()
+            expiredSessions = [i for i in sessions if sessions[i][1] < time()]
+            for e in expiredSessions:
+                del sessions[e]
+
+    def middleware(app:Application, req:HttpRequest, res:HttpResponse, next:Next):
+        removeExpired()
+        sessionId:str = None
+        if cookieName not in req.cookies.values:
+            sessionId = str(uuid.uuid4())
+            res.set_cookie(cookieName, sessionId, durationSec)
+        else:
+            sessionId = req.cookies.values[cookieName]
+
+        if sessionId not in sessions:
+            sessions[sessionId] = [Session(), durationSec + time()]
+        else:
+            sessions[sessionId][1] = durationSec + time()
+
+        req.session = sessions[sessionId][0]
+        next()
     return middleware
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/router.py` & `threadsnake-1.0.1/src/threadsnake/http/router.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import re
-from typing import Any, Callable, Dict, List, Tuple
-
-from .core.httprequest import HttpRequest
-from .core.httpresponse import HttpResponse
-from .types import Callback, CallbackMutator, Middleware, Next
-
-class Router:
-
-    patterns:List[Tuple[str, str]] = [
-        (r"{([\w]+)\:int}", r"(?P<\1>[-]?[\\d]+)"), #Int pattern
-        (r"{([\w]+)\:float}", r"(?P<\1>[-]?[\\d]+[\\.]?[\\d]?)"), #Float pattern
-        (r"{([\w]+)\:re\(([\w\W]+?)\)}", r"(?P<\1>\2)"), #Regex pattern
-        (r"{([\w]+)}", r"(?P<\1>[\\w]+)"), #General pattern
-    ]
-
-    def __init__(self) -> None:
-        self.routes:Dict[str, Dict[str, Callback]] = dict()
-        self.calbackMutator:CallbackMutator = lambda a: a
-
-    def normalize_route(self, route:str) -> str:
-        if not route.endswith('/'):
-            route += '/'
-        if not route.startswith('/'):
-            route = '/' + route
-        while '//' in route:
-            route = route.replace('//', '/')  
-        while route.endswith('/') and len(route) > 1:
-            route = route[:-1]  
-        return route
-    
-    def register_callback(self, httpMethod:str, route:str) -> CallbackMutator:
-        ref:Router = self
-        route = self.normalize_route(route)
-        httpMethod = httpMethod.upper()
-        def decorator(callback:Callback) -> Callback:
-            callback = self.calbackMutator(callback)
-            if httpMethod not in ref.routes:
-                ref.routes[httpMethod] = {route:callback}
-            else:
-                ref.routes[httpMethod][route] = callback
-            return callback
-        return decorator
-
-    def use_globally(self, mutator:CallbackMutator):
-        currentMutator:CallbackMutator = self.calbackMutator
-        newMutator:CallbackMutator = lambda c: mutator(currentMutator(c))
-        self.calbackMutator = newMutator
-        return self
-
-    def get(self, route) -> CallbackMutator:
-        return self.register_callback('GET', route)
-
-    def post(self, route) -> CallbackMutator:
-        return self.register_callback('POST', route)
-
-    def put(self, route) -> CallbackMutator:
-        return self.register_callback('PUT', route)
-
-    def delete(self, route) -> CallbackMutator:
-        return self.register_callback('DELETE', route)
-
-    def use_router(self, router, root):
-        for method in router.routes:
-            for action in router.routes[method]:
-                self.register_callback(method,f'{root}{action}')(router.routes[method][action])
-        return self
-
-    def serve(self, route:str, content:str, encoding:str):
-        fileName:str = sub(sub(route, '/'), '\\')
-        inner_callback:Callback = lambda app, req, res : res.file(fileName, content, encoding=encoding)
-        self.get(route)(inner_callback)
-        return self
-
-    def __getattr__(self, method) -> Callable[[str],CallbackMutator]:
-        def inner(route) -> CallbackMutator:
-            return self.register_callback(method.upper(), route)
-        return inner
-
-    def test_path(self, method:str, path:str) -> Tuple[Callback, Dict[str,str]]:
-        callback:Callback = None
-        queryParams:Dict[str, str] = dict()
-        if method.upper() in self.routes:
-            paths:List[str] = self.routes[method.upper()].copy()
-            for route in paths:
-                pattern:str = route
-                for regex in Router.patterns:
-                    pattern = re.sub(regex[0], regex[1], pattern)
-                match = re.match(f'^{pattern}$', path)
-                if match:
-                    callback = self.routes[method.upper()][route]
-                    queryParams = match.groupdict()
-                    break
-        return callback, queryParams
-
-    def create_middleware(self, callback:Callback) -> Middleware:
-        def inner_callback(app:Any, req:HttpRequest, res:HttpResponse, next:Next):
-            res.status(200, 'OK')
-            callback(app, req, res)
-            next()
-        return inner_callback
-
-def sub(data:str, token:str) -> str:
-    return data if token not in data else data[data.index(token)+1:]
-
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import re
+from typing import Any, Callable, Dict, List, Tuple
+
+from .core.httprequest import HttpRequest
+from .core.httpresponse import HttpResponse
+from .types import Callback, CallbackMutator, Middleware, Next
+
+class Router:
+
+    patterns:List[Tuple[str, str]] = [
+        (r"{([\w]+)\:int}", r"(?P<\1>[-]?[\\d]+)"), #Int pattern
+        (r"{([\w]+)\:float}", r"(?P<\1>[-]?[\\d]+[\\.]?[\\d]?)"), #Float pattern
+        (r"{([\w]+)\:re\(([\w\W]+?)\)}", r"(?P<\1>\2)"), #Regex pattern
+        (r"{([\w]+)}", r"(?P<\1>[\\w]+)"), #General pattern
+    ]
+
+    def __init__(self) -> None:
+        self.routes:Dict[str, Dict[str, Callback]] = dict()
+        self.calbackMutator:CallbackMutator = lambda a: a
+
+    def normalize_route(self, route:str) -> str:
+        if not route.endswith('/'):
+            route += '/'
+        if not route.startswith('/'):
+            route = '/' + route
+        while '//' in route:
+            route = route.replace('//', '/')  
+        while route.endswith('/') and len(route) > 1:
+            route = route[:-1]  
+        return route
+    
+    def register_callback(self, httpMethod:str, route:str) -> CallbackMutator:
+        ref:Router = self
+        route = self.normalize_route(route)
+        httpMethod = httpMethod.upper()
+        def decorator(callback:Callback) -> Callback:
+            callback = self.calbackMutator(callback)
+            if httpMethod not in ref.routes:
+                ref.routes[httpMethod] = {route:callback}
+            else:
+                ref.routes[httpMethod][route] = callback
+            return callback
+        return decorator
+
+    def use_globally(self, mutator:CallbackMutator):
+        currentMutator:CallbackMutator = self.calbackMutator
+        newMutator:CallbackMutator = lambda c: mutator(currentMutator(c))
+        self.calbackMutator = newMutator
+        return self
+
+    def get(self, route) -> CallbackMutator:
+        return self.register_callback('GET', route)
+
+    def post(self, route) -> CallbackMutator:
+        return self.register_callback('POST', route)
+
+    def put(self, route) -> CallbackMutator:
+        return self.register_callback('PUT', route)
+
+    def delete(self, route) -> CallbackMutator:
+        return self.register_callback('DELETE', route)
+
+    def use_router(self, router, root):
+        for method in router.routes:
+            for action in router.routes[method]:
+                self.register_callback(method,f'{root}{action}')(router.routes[method][action])
+        return self
+
+    def serve(self, route:str, content:str, encoding:str):
+        fileName:str = sub(sub(route, '/'), '\\')
+        inner_callback:Callback = lambda app, req, res : res.file(fileName, content, encoding=encoding)
+        self.get(route)(inner_callback)
+        return self
+
+    def __getattr__(self, method) -> Callable[[str],CallbackMutator]:
+        def inner(route) -> CallbackMutator:
+            return self.register_callback(method.upper(), route)
+        return inner
+
+    def test_path(self, method:str, path:str) -> Tuple[Callback, Dict[str,str]]:
+        callback:Callback = None
+        queryParams:Dict[str, str] = dict()
+        if method.upper() in self.routes:
+            paths:List[str] = self.routes[method.upper()].copy()
+            for route in paths:
+                pattern:str = route
+                for regex in Router.patterns:
+                    pattern = re.sub(regex[0], regex[1], pattern)
+                match = re.match(f'^{pattern}$', path)
+                if match:
+                    callback = self.routes[method.upper()][route]
+                    queryParams = match.groupdict()
+                    break
+        return callback, queryParams
+
+    def create_middleware(self, callback:Callback) -> Middleware:
+        def inner_callback(app:Any, req:HttpRequest, res:HttpResponse, next:Next):
+            res.status(200, 'OK')
+            callback(app, req, res)
+            next()
+        return inner_callback
+
+def sub(data:str, token:str) -> str:
+    return data if token not in data else data[data.index(token)+1:]
+
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/tools/common.py` & `threadsnake-1.0.1/src/threadsnake/http/tools/common.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from ..core.httpresponse import HttpResponse
-
-def status(res:HttpResponse, responseCode:int) -> None:
-    res.status(responseCode)
-
-def not_found(res:HttpResponse) -> None:
-    res.status(404, "NotFound")
-
-def bad_request(res:HttpResponse) -> None:
-    res.status(400, "BadRequest")
-
-def ok(res:HttpResponse) -> None:
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from ..core.httpresponse import HttpResponse
+
+def status(res:HttpResponse, responseCode:int) -> None:
+    res.status(responseCode)
+
+def not_found(res:HttpResponse) -> None:
+    res.status(404, "NotFound")
+
+def bad_request(res:HttpResponse) -> None:
+    res.status(400, "BadRequest")
+
+def ok(res:HttpResponse) -> None:
     res.status(200, "Ok")
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/tools/routing.py` & `threadsnake-1.0.1/src/threadsnake/http/tools/routing.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-import importlib
-import importlib.util
-import os
-import sys
-from types import ModuleType
-from typing import List, Tuple
-from uuid import uuid4
-import __main__
-
-from ..application import Application
-from ..router import Router
-
-ConfiguredRoute = Tuple[str, List[Router]]
-
-def import_module(path:str) -> ModuleType:
-    if not path.endswith('.py'):
-        path += '.py'    
-    moduleName:str = os.path.basename(path) + str(uuid4()).replace('-', '')
-    spec = importlib.util.spec_from_file_location(moduleName, path)
-    module:ModuleType = importlib.util.module_from_spec(spec)
-    sys.modules[moduleName] = module
-    spec.loader.exec_module(module)
-    return module
-
-def routes_to(app:Application, path:str, root:str):
-    baseFolder:str = os.path.dirname(__main__.__file__)
-    fullSearchPath = os.sep.join([baseFolder, path.replace('/', os.sep)])
-    module:ModuleType = import_module(fullSearchPath)
-    for property in dir(module):
-        router = getattr(module, property)
-        if isinstance(router, Router):
-            app.use_router(router, root)
-
-def routes_to_folder(app:Application, path:str):
-    location:str = os.path.dirname(os.path.abspath(__main__.__file__))
-    fullSearchPath = os.sep.join([location, path])
-    fullSearchPath = fullSearchPath.replace('/', os.sep).replace('\\', os.sep)
-    files = [
-        [path, result[0][len(fullSearchPath)+1:].replace('\\', '/'), file[:-3]] 
-        for result in os.walk(fullSearchPath) for file in result[2]
-        if file.endswith('.py')
-    ]
-    routes = [
-        [
-            '/'.join([j for j in i if len(j) > 0]),
-            '/'.join([j for j in i[1:] if len(j) > 0])
-        ]
-        for i in files
-    ]
-    for route in routes:
-        path, root = route
-        routes_to(app, path, root)
-
-##def get_routers(moduleName:str) -> List[Router]:
-##    routers:List[Router] = []
-##    module:ModuleType = importlib.import_module(moduleName)
-##    for property in dir(module):
-##        if isinstance(getattr(module, property), Router):
-##            routers.append(getattr(module, property))
-##    return routers
-##
-##def load_router(path:str) -> ConfiguredRoute:
-##    if not path.endswith('.py'):
-##        return
-##    path = path[:-3]
-##    pathParts:List[str] = [i for i in path.replace(os.sep, '.').split('.') if len(i) > 0]
-##    module:str = '.'.join(pathParts)
-##    path:str = '/'.join(pathParts[1:])
-##    return path, get_routers(module)
-##
-##def get_files(folder:str) -> List[str]:
-##    filo = [os.sep.join([j[0], i]) for j in os.walk(folder) for i in j[2]]
-##    print(folder, filo)
-##    input('')
-##
-##def load_routes(path:str) -> List[ConfiguredRoute]:
-##    baseFolder:str = os.path.dirname(__main__.__file__)
-##    fullSearchPath = os.sep.join([baseFolder, path])
-##    get_files(fullSearchPath)
-##    base:str = os.path.abspath(os.curdir)
-##    print(f"{baseFolder} on {base}")
-##    configuredRoutes: List[ConfiguredRoute] = []
-##    modules:List[str] = [i for i in os.listdir(fullSearchPath) if i.endswith('.py')]
-##    input(modules)
-##    for module in modules:
-##        configuredRoutes.append(load_router(os.sep.join([path, module])))
-##    return configuredRoutes
-##        
-##def configure_routes(app:Application, path:str) -> None:
-##    for configuredRoute in load_routes(path):
-##        for router in configuredRoute[1]:
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+import importlib
+import importlib.util
+import os
+import sys
+from types import ModuleType
+from typing import List, Tuple
+from uuid import uuid4
+import __main__
+
+from ..application import Application
+from ..router import Router
+
+ConfiguredRoute = Tuple[str, List[Router]]
+
+def import_module(path:str) -> ModuleType:
+    if not path.endswith('.py'):
+        path += '.py'    
+    moduleName:str = os.path.basename(path) + str(uuid4()).replace('-', '')
+    spec = importlib.util.spec_from_file_location(moduleName, path)
+    module:ModuleType = importlib.util.module_from_spec(spec)
+    sys.modules[moduleName] = module
+    spec.loader.exec_module(module)
+    return module
+
+def routes_to(app:Application, path:str, root:str):
+    baseFolder:str = os.path.dirname(__main__.__file__)
+    fullSearchPath = os.sep.join([baseFolder, path.replace('/', os.sep)])
+    module:ModuleType = import_module(fullSearchPath)
+    for property in dir(module):
+        router = getattr(module, property)
+        if isinstance(router, Router):
+            app.use_router(router, root)
+
+def routes_to_folder(app:Application, path:str):
+    location:str = os.path.dirname(os.path.abspath(__main__.__file__))
+    fullSearchPath = os.sep.join([location, path])
+    fullSearchPath = fullSearchPath.replace('/', os.sep).replace('\\', os.sep)
+    files = [
+        [path, result[0][len(fullSearchPath)+1:].replace('\\', '/'), file[:-3]] 
+        for result in os.walk(fullSearchPath) for file in result[2]
+        if file.endswith('.py')
+    ]
+    routes = [
+        [
+            '/'.join([j for j in i if len(j) > 0]),
+            '/'.join([j for j in i[1:] if len(j) > 0])
+        ]
+        for i in files
+    ]
+    for route in routes:
+        path, root = route
+        routes_to(app, path, root)
+
+##def get_routers(moduleName:str) -> List[Router]:
+##    routers:List[Router] = []
+##    module:ModuleType = importlib.import_module(moduleName)
+##    for property in dir(module):
+##        if isinstance(getattr(module, property), Router):
+##            routers.append(getattr(module, property))
+##    return routers
+##
+##def load_router(path:str) -> ConfiguredRoute:
+##    if not path.endswith('.py'):
+##        return
+##    path = path[:-3]
+##    pathParts:List[str] = [i for i in path.replace(os.sep, '.').split('.') if len(i) > 0]
+##    module:str = '.'.join(pathParts)
+##    path:str = '/'.join(pathParts[1:])
+##    return path, get_routers(module)
+##
+##def get_files(folder:str) -> List[str]:
+##    filo = [os.sep.join([j[0], i]) for j in os.walk(folder) for i in j[2]]
+##    print(folder, filo)
+##    input('')
+##
+##def load_routes(path:str) -> List[ConfiguredRoute]:
+##    baseFolder:str = os.path.dirname(__main__.__file__)
+##    fullSearchPath = os.sep.join([baseFolder, path])
+##    get_files(fullSearchPath)
+##    base:str = os.path.abspath(os.curdir)
+##    print(f"{baseFolder} on {base}")
+##    configuredRoutes: List[ConfiguredRoute] = []
+##    modules:List[str] = [i for i in os.listdir(fullSearchPath) if i.endswith('.py')]
+##    input(modules)
+##    for module in modules:
+##        configuredRoutes.append(load_router(os.sep.join([path, module])))
+##    return configuredRoutes
+##        
+##def configure_routes(app:Application, path:str) -> None:
+##    for configuredRoute in load_routes(path):
+##        for router in configuredRoute[1]:
 ##            app.use_router(router, configuredRoute[0])
```

### Comparing `threadsnake-1.0.0/src/threadsnake/http/types.py` & `threadsnake-1.0.1/src/threadsnake/http/types.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-##    Threadsnake. A tiny experimental server-side express-like library.
-##    Copyright (C) 2022  Erick Fernando Mora Ramirez
-##
-##    This program is free software: you can redistribute it and/or modify
-##    it under the terms of the GNU General Public License as published by
-##    the Free Software Foundation, either version 3 of the License, or
-##    (at your option) any later version.
-##
-##    This program is distributed in the hope that it will be useful,
-##    but WITHOUT ANY WARRANTY; without even the implied warranty of
-##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-##    GNU General Public License for more details.
-##
-##    You should have received a copy of the GNU General Public License
-##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-##
-##    mailto:erickfernandomoraramirez@gmail.com
-
-from .core.httprequest import HttpRequest
-from .core.httpresponse import HttpResponse
-from typing import Any, Callable, Dict
-
-Next = Callable[[], None]
-Middleware = Callable[[Any, HttpRequest, HttpResponse, Next], None]
-Callback = Callable[[Any, HttpRequest, HttpResponse], None]
-ServerCallback = Callable[[HttpRequest, HttpResponse], None]
-CallbackMutator = Callable[[Callback], Callback]
-DictProvider = Callable[[], Dict[str, str]]
-RequestPredicate = Callable[[HttpRequest], bool]
+##    Threadsnake. A tiny experimental server-side express-like library.
+##    Copyright (C) 2022  Erick Fernando Mora Ramirez
+##
+##    This program is free software: you can redistribute it and/or modify
+##    it under the terms of the GNU General Public License as published by
+##    the Free Software Foundation, either version 3 of the License, or
+##    (at your option) any later version.
+##
+##    This program is distributed in the hope that it will be useful,
+##    but WITHOUT ANY WARRANTY; without even the implied warranty of
+##    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+##    GNU General Public License for more details.
+##
+##    You should have received a copy of the GNU General Public License
+##    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+##
+##    mailto:erickfernandomoraramirez@gmail.com
+
+from .core.httprequest import HttpRequest
+from .core.httpresponse import HttpResponse
+from typing import Any, Callable, Dict
+
+Next = Callable[[], None]
+Middleware = Callable[[Any, HttpRequest, HttpResponse, Next], None]
+Callback = Callable[[Any, HttpRequest, HttpResponse], None]
+ServerCallback = Callable[[HttpRequest, HttpResponse], None]
+CallbackMutator = Callable[[Callback], Callback]
+DictProvider = Callable[[], Dict[str, str]]
+RequestPredicate = Callable[[HttpRequest], bool]
```

### Comparing `threadsnake-1.0.0/src/threadsnake.egg-info/SOURCES.txt` & `threadsnake-1.0.1/src/threadsnake.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
-README.md
 pyproject.toml
 setup.py
 src/threadsnake/__init__.py
-src/threadsnake/version.txt
 src/threadsnake.egg-info/PKG-INFO
 src/threadsnake.egg-info/SOURCES.txt
 src/threadsnake.egg-info/dependency_links.txt
 src/threadsnake.egg-info/top_level.txt
 src/threadsnake/html/__init__.py
 src/threadsnake/html/tools.py
 src/threadsnake/http/__init__.py
```

