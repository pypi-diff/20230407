# Comparing `tmp/swsh-0.1.6.tar.gz` & `tmp/swsh-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swsh-0.1.6.tar", last modified: Thu Apr  6 19:06:30 2023, max compression
+gzip compressed data, was "swsh-0.1.7.tar", last modified: Fri Apr  7 19:54:49 2023, max compression
```

## Comparing `swsh-0.1.6.tar` & `swsh-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-06 19:06:30.654281 swsh-0.1.6/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-06 19:06:30.653984 swsh-0.1.6/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.6/README.md
--rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-06 19:06:30.654375 swsh-0.1.6/setup.cfg
--rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-06 19:04:00.000000 swsh-0.1.6/setup.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-06 19:06:30.652162 swsh-0.1.6/swsh/
--rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-05 20:48:52.000000 swsh-0.1.6/swsh/buy_a_phone_number.py
--rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.6/swsh/functions.py
--rwxr-xr-x   0 shane      (501) staff       (20)   136124 2023-04-05 20:48:43.000000 swsh-0.1.6/swsh/swsh.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-06 19:06:30.653771 swsh-0.1.6/swsh.egg-info/
--rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/SOURCES.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/dependency_links.txt
--rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/entry_points.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/not-zip-safe
--rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/requires.txt
--rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-06 19:06:30.000000 swsh-0.1.6/swsh.egg-info/top_level.txt
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.078259 swsh-0.1.7/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 19:54:49.078111 swsh-0.1.7/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)     1241 2023-04-05 15:05:42.000000 swsh-0.1.7/README.md
+-rw-r--r--   0 shane      (501) staff       (20)       38 2023-04-07 19:54:49.078302 swsh-0.1.7/setup.cfg
+-rw-r--r--   0 shane      (501) staff       (20)     1024 2023-04-07 19:51:07.000000 swsh-0.1.7/setup.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.076246 swsh-0.1.7/swsh/
+-rwxr-xr-x   0 shane      (501) staff       (20)     3254 2023-04-05 20:48:52.000000 swsh-0.1.7/swsh/buy_a_phone_number.py
+-rwxr-xr-x   0 shane      (501) staff       (20)    13786 2023-03-29 20:31:13.000000 swsh-0.1.7/swsh/functions.py
+-rwxr-xr-x   0 shane      (501) staff       (20)   136490 2023-04-07 19:46:25.000000 swsh-0.1.7/swsh/swsh.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-07 19:54:49.077933 swsh-0.1.7/swsh.egg-info/
+-rw-r--r--   0 shane      (501) staff       (20)      660 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)      273 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/SOURCES.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/dependency_links.txt
+-rw-r--r--   0 shane      (501) staff       (20)       40 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/entry_points.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-06 19:06:30.000000 swsh-0.1.7/swsh.egg-info/not-zip-safe
+-rw-r--r--   0 shane      (501) staff       (20)       83 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/requires.txt
+-rw-r--r--   0 shane      (501) staff       (20)        5 2023-04-07 19:54:49.000000 swsh-0.1.7/swsh.egg-info/top_level.txt
```

### Comparing `swsh-0.1.6/PKG-INFO` & `swsh-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.6
+Version: 0.1.7
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `swsh-0.1.6/README.md` & `swsh-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `swsh-0.1.6/setup.py` & `swsh-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Natural Language :: English',
   'Topic :: Communications',
   'Topic :: Software Development'
 ]
 
 setup(
   name='swsh',
-  version='0.1.6',
+  version='0.1.7',
   description='SignalWire interactive SHell',
   entry_points={
     'console_scripts': ['swsh=swsh.swsh:main']
   },
   #long_description=read('README.md'),
   long_description_content_type="text/markdown",
   classifiers=CLASSIFIERS,
```

### Comparing `swsh-0.1.6/swsh/buy_a_phone_number.py` & `swsh-0.1.7/swsh/buy_a_phone_number.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.6/swsh/functions.py` & `swsh-0.1.7/swsh/functions.py`

 * *Files identical despite different names*

### Comparing `swsh-0.1.6/swsh/swsh.py` & `swsh-0.1.7/swsh/swsh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 import cmd2
 import os
 import argparse
-from swsh.functions import *
-from swsh.buy_a_phone_number import *
+from functions import *
+#from swsh.buy_a_phone_number import *
 import json
 import time
 import re
 import urllib.parse
 from signalwire.rest import Client as signalwire_client
 
 
@@ -183,14 +183,15 @@
     base_sip_endpoint_parser = cmd2.Cmd2ArgumentParser()
     base_sip_endpoint_subparsers = base_sip_endpoint_parser.add_subparsers(title='SIP ENDPOINT',help='sip_endpoint help')
 
     # create the sip_endpoint list subcommand
     sip_endpoint_parser_list = base_sip_endpoint_subparsers.add_parser('list', help='List SIP Endpoints')
     sip_endpoint_parser_list.add_argument('-i', '--id', help='List SIP Endpoint by unique SignalWire ID')
     sip_endpoint_parser_list.add_argument('-j', '--json', action='store_true', help='Output SIP Endpoint(s) in JSON format')
+    sip_endpoint_parser_list.add_argument('-n', '--name', type=str, nargs='+', help='Search for SIP Endpoint by username')
 
     # create the sip_endpoint update subcommand
     sip_endpoint_parser_update = base_sip_endpoint_subparsers.add_parser('update', help='Update a SIP Endpoint')
     sip_endpoint_parser_update.add_argument('-u', '--username', help='update username of the sip endpoint')
     sip_endpoint_parser_update.add_argument('-p', '--password', help='update password of the sip endpoint')
     sip_endpoint_parser_update.add_argument('-s', '--send-as',  help='default caller id for sip endpoint (Must belong to the Project!)')
     sip_endpoint_parser_update.add_argument('-c', '--caller-id', nargs='+', help='Friendly Caller ID Name (SIP to SIP only)' )
@@ -227,14 +228,20 @@
                 new_arg=get_shell_env(var)
                 setattr(args, arg, new_arg)
                 
         query_params = ""
         if args.id:
             sid = args.id
             query_params="/" + sid
+        elif args.name:
+            query_params = "?"
+            if args.name:
+                name = ' '.join(args.name)
+                name = urllib.parse.quote(name)
+                query_params = query_params + "filter_username=%s&" % name
 
         output, status_code =  sip_endpoint_func(query_params)
         valid = validate_http(status_code)
         if valid:
             # Format the output depending on user args
             output = json.loads(output)
             if args.id and args.json:
```

### Comparing `swsh-0.1.6/swsh.egg-info/PKG-INFO` & `swsh-0.1.7/swsh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swsh
-Version: 0.1.6
+Version: 0.1.7
 Summary: SignalWire interactive SHell
 Home-page: https://github.com/signalwire/swish
 Author: Shane Harrell
 Author-email: shane.harrell@signalwire.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

