# Comparing `tmp/igwn-alert-overseer-0.5.2.tar.gz` & `tmp/igwn-alert-overseer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igwn-alert-overseer-0.5.2.tar", last modified: Thu Sep  1 14:00:27 2022, max compression
+gzip compressed data, was "igwn-alert-overseer-0.6.0.tar", last modified: Fri Apr  7 20:33:40 2023, max compression
```

## Comparing `igwn-alert-overseer-0.5.2.tar` & `igwn-alert-overseer-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-01 14:00:27.363101 igwn-alert-overseer-0.5.2/
--rwxr-xr-x   0 alex      (1010) admin       (80)    35149 2022-08-20 21:44:24.000000 igwn-alert-overseer-0.5.2/COPYING
--rwxr-xr-x   0 alex      (1010) admin       (80)       16 2022-08-20 21:44:24.000000 igwn-alert-overseer-0.5.2/MANIFEST.in
--rw-r--r--   0 alex      (1010) admin       (80)      427 2022-09-01 14:00:27.363151 igwn-alert-overseer-0.5.2/PKG-INFO
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-01 14:00:27.362117 igwn-alert-overseer-0.5.2/bin/
--rwxr-xr-x   0 alex      (1010) admin       (80)    13301 2022-09-01 13:42:52.000000 igwn-alert-overseer-0.5.2/bin/igwn_alert_overseer
--rwxr-xr-x   0 alex      (1010) admin       (80)     1483 2022-08-20 21:44:24.000000 igwn-alert-overseer-0.5.2/bin/overseer_test_client
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-01 14:00:27.362231 igwn-alert-overseer-0.5.2/igwn_alert_overseer/
--rw-r--r--   0 alex      (1010) admin       (80)      797 2022-08-22 02:20:09.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer/__init__.py
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-01 14:00:27.363016 igwn-alert-overseer-0.5.2/igwn_alert_overseer/overseer/
--rwxr-xr-x   0 alex      (1010) admin       (80)      798 2022-08-22 02:20:09.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer/overseer/__init__.py
--rwxr-xr-x   0 alex      (1010) admin       (80)     3481 2022-08-22 02:20:09.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer/overseer/overseer_client.py
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-01 14:00:27.362804 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/
--rw-r--r--   0 alex      (1010) admin       (80)      427 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1010) admin       (80)      474 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1010) admin       (80)        1 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1010) admin       (80)       20 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/namespace_packages.txt
--rw-r--r--   0 alex      (1010) admin       (80)       26 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/requires.txt
--rw-r--r--   0 alex      (1010) admin       (80)       20 2022-09-01 14:00:27.000000 igwn-alert-overseer-0.5.2/igwn_alert_overseer.egg-info/top_level.txt
--rwxr-xr-x   0 alex      (1010) admin       (80)       73 2022-09-01 14:00:27.363343 igwn-alert-overseer-0.5.2/setup.cfg
--rwxr-xr-x   0 alex      (1010) admin       (80)     1657 2022-09-01 13:42:52.000000 igwn-alert-overseer-0.5.2/setup.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 20:33:40.335861 igwn-alert-overseer-0.6.0/
+-rwxr-xr-x   0 alex      (1010) admin       (80)    35149 2022-08-20 21:44:24.000000 igwn-alert-overseer-0.6.0/COPYING
+-rwxr-xr-x   0 alex      (1010) admin       (80)       16 2022-08-20 21:44:24.000000 igwn-alert-overseer-0.6.0/MANIFEST.in
+-rw-r--r--   0 alex      (1010) admin       (80)      389 2023-04-07 20:33:40.335912 igwn-alert-overseer-0.6.0/PKG-INFO
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 20:33:40.334898 igwn-alert-overseer-0.6.0/bin/
+-rwxr-xr-x   0 alex      (1010) admin       (80)    13345 2023-04-07 19:41:17.000000 igwn-alert-overseer-0.6.0/bin/igwn_alert_overseer
+-rwxr-xr-x   0 alex      (1010) admin       (80)     1929 2023-04-07 19:41:17.000000 igwn-alert-overseer-0.6.0/bin/overseer_test_client
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 20:33:40.335007 igwn-alert-overseer-0.6.0/igwn_alert_overseer/
+-rw-r--r--   0 alex      (1010) admin       (80)      757 2023-04-07 19:41:17.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer/__init__.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 20:33:40.335771 igwn-alert-overseer-0.6.0/igwn_alert_overseer/overseer/
+-rwxr-xr-x   0 alex      (1010) admin       (80)      741 2023-04-07 19:41:17.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer/overseer/__init__.py
+-rwxr-xr-x   0 alex      (1010) admin       (80)     1661 2023-04-07 19:41:17.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer/overseer/overseer_client.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 20:33:40.335536 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/
+-rw-r--r--   0 alex      (1010) admin       (80)      389 2023-04-07 20:33:40.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1010) admin       (80)      422 2023-04-07 20:33:40.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1010) admin       (80)        1 2023-04-07 20:33:40.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       39 2023-04-07 20:33:40.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/requires.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       20 2023-04-07 20:33:40.000000 igwn-alert-overseer-0.6.0/igwn_alert_overseer.egg-info/top_level.txt
+-rwxr-xr-x   0 alex      (1010) admin       (80)       73 2023-04-07 20:33:40.336112 igwn-alert-overseer-0.6.0/setup.cfg
+-rwxr-xr-x   0 alex      (1010) admin       (80)     1647 2023-04-07 20:33:06.000000 igwn-alert-overseer-0.6.0/setup.py
```

### Comparing `igwn-alert-overseer-0.5.2/COPYING` & `igwn-alert-overseer-0.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `igwn-alert-overseer-0.5.2/bin/igwn_alert_overseer` & `igwn-alert-overseer-0.6.0/bin/igwn_alert_overseer`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,15 @@
                     ovrseer_logger.info("sending %s to topic %s" % (message_id, topic))
                     self.factory.client.publish_to_topic(topic, message)
                     ovrseer_logger.info("sent %s to topic %s" % (message_id, topic))
                 except Exception as e:
                     ovrseer_logger.error("SEND FAILED: %s" % str(e))
     
             self.transport.write(str.encode(json.dumps({'success': True})))
+            self.transport.loseConnection()
 
 
 class IGWNAOverseerFactory(ServerFactory):
 
     protocol = IGWNAOverseerProtocol
 
     def __init__(self, client = None, thread = None):
```

### Comparing `igwn-alert-overseer-0.5.2/igwn_alert_overseer/__init__.py` & `igwn-alert-overseer-0.6.0/igwn_alert_overseer/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) Branson Stephens (2022)
+# Copyright (C) Branson Stephens, Alexander Pace (2022)
 #
 # This file is part of lvalert-overseer
 #
 # lvalert-overseer is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,8 +12,7 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with lvalert-overseer.  If not, see <http://www.gnu.org/licenses/>.
 
-__import__('pkg_resources').declare_namespace(__name__)
```

### Comparing `igwn-alert-overseer-0.5.2/setup.py` & `igwn-alert-overseer-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with lvalert-overseer.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 from setuptools import setup, find_packages
 
-version = "0.5.2"
+version = "0.6.0"
 AUTHOR = 'Alexander Pace'
 AUTHOR_EMAIL = 'alexander.pace@ligo.org'
 LICENSE = 'GPLv3'
 
 description = "igwn-alert Overseer Server and Client Tools"
 long_description = """The igwn-alert overseer provides a way to maintain an open
 connection to igwn-alert for sending message, and to log the outgoing and
@@ -35,13 +35,13 @@
     version=version,
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     description=description,
     long_description=long_description,
     url=None,
     license=LICENSE,
-    namespace_packages=['igwn_alert_overseer'],
     packages=find_packages(),
     scripts=['bin/igwn_alert_overseer', 'bin/overseer_test_client'],
     install_requires=['twisted',
-                      'igwn-alert>=0.2.2'],
+                      'tornado>=6.2',
+                      'igwn-alert>=0.3.1'],
 )
```

