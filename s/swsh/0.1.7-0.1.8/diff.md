# Comparing `tmp/swsh-0.1.7.tar.gz` & `tmp/swsh-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swsh-0.1.7.tar", last modified: Fri Apr  7 19:54:49 2023, max compression
+gzip compressed data, was "swsh-0.1.8.tar", last modified: Fri Apr  7 20:00:03 2023, max compression
```

## Comparing `swsh-0.1.7.tar` & `swsh-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.078259 swsh-0.1.7/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 19:54:49.078111 swsh-0.1.7/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.7/README.md
--rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-07 19:54:49.078302 swsh-0.1.7/setup.cfg
--rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-07 19:51:07.000000 swsh-0.1.7/setup.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.076246 swsh-0.1.7/swsh/
--rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-05 20:48:52.000000 swsh-0.1.7/swsh/buy_a_phone_number.py
--rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.7/swsh/functions.py
--rwxr-xr-x   0 shane      (501) staff       (20)   136490 2023-04-07 19:46:25.000000 swsh-0.1.7/swsh/swsh.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.077933 swsh-0.1.7/swsh.egg-info/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/SOURCES.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/dependency_links.txt
--rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/entry_points.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.7/swsh.egg-info/not-zip-safe
--rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/requires.txt
--rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/top_level.txt
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.003085 swsh-0.1.8/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 20:00:03.002282 swsh-0.1.8/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.8/README.md
+-rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-07 20:00:03.003138 swsh-0.1.8/setup.cfg
+-rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-07 19:59:40.000000 swsh-0.1.8/setup.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.000056 swsh-0.1.8/swsh/
+-rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-05 20:48:52.000000 swsh-0.1.8/swsh/buy_a_phone_number.py
+-rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.8/swsh/functions.py
+-rwxr-xr-x   0 shane      (501) staff       (20)   136494 2023-04-07 19:57:21.000000 swsh-0.1.8/swsh/swsh.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 20:00:03.002069 swsh-0.1.8/swsh.egg-info/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/SOURCES.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/dependency_links.txt
+-rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/entry_points.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.8/swsh.egg-info/not-zip-safe
+-rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/requires.txt
+-rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-07 20:00:02.000000 swsh-0.1.8/swsh.egg-info/top_level.txt
```

### Comparing `swsh-0.1.7/PKG-INFO` & `swsh-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.7
+Version: 0.1.8
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `swsh-0.1.7/README.md` & `swsh-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `swsh-0.1.7/setup.py` & `swsh-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Natural Language :: English',
   'Topic :: Communications',
   'Topic :: Software Development'
 ]
 
 setup(
   name='swsh',
-  version='0.1.7',
+  version='0.1.8',
   description='SignalWire interactive SHell',
   entry_points={
     'console_scripts': ['swsh=swsh.swsh:main']
   },
   #long_description=read('README.md'),
   long_description_content_type="text/markdown",
   classifiers=CLASSIFIERS,
```

### Comparing `swsh-0.1.7/swsh/buy_a_phone_number.py` & `swsh-0.1.8/swsh/buy_a_phone_number.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.7/swsh/functions.py` & `swsh-0.1.8/swsh/functions.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.7/swsh/swsh.py` & `swsh-0.1.8/swsh/swsh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 import cmd2
 import os
 import argparse
-from functions import *
-#from swsh.buy_a_phone_number import *
+from swsh.functions import *
+from swsh.buy_a_phone_number import *
 import json
 import time
 import re
 import urllib.parse
 from signalwire.rest import Client as signalwire_client
```

### Comparing `swsh-0.1.7/swsh.egg-info/PKG-INFO` & `swsh-0.1.8/swsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.7
+Version: 0.1.8
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

