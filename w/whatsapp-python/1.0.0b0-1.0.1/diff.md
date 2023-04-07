# Comparing `tmp/whatsapp-python-1.0.0b0.tar.gz` & `tmp/whatsapp-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whatsapp-python-1.0.0b0.tar", last modified: Fri Apr  7 21:06:51 2023, max compression
+gzip compressed data, was "dist/whatsapp-python-1.0.1.tar", last modified: Fri Apr  7 21:09:55 2023, max compression
```

## Comparing `whatsapp-python-1.0.0b0.tar` & `whatsapp-python-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/
--rw-r--r--   0 filipporomani   (501) staff       (20)    18728 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/PKG-INFO
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/
--rw-r--r--   0 filipporomani   (501) staff       (20)    18728 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 filipporomani   (501) staff       (20)       40 2023-04-07 21:06:01.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/lol.py
--rw-r--r--   0 filipporomani   (501) staff       (20)      265 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)       87 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)        9 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/top_level.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)        1 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)    14594 2023-04-07 21:04:52.000000 whatsapp-python-1.0.0b0/README.md
--rw-r--r--   0 filipporomani   (501) staff       (20)     1499 2023-04-07 21:06:46.000000 whatsapp-python-1.0.0b0/setup.py
--rw-r--r--   0 filipporomani   (501) staff       (20)       38 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/setup.cfg
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:06:51.000000 whatsapp-python-1.0.0b0/whatsapp/
--rw-r--r--   0 filipporomani   (501) staff       (20)    38311 2023-04-07 21:02:51.000000 whatsapp-python-1.0.0b0/whatsapp/__init__.py
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    18726 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/PKG-INFO
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    18726 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 filipporomani   (501) staff       (20)      233 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)       78 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)        9 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/top_level.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)        1 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)    14594 2023-04-07 21:04:52.000000 whatsapp-python-1.0.1/README.md
+-rw-r--r--   0 filipporomani   (501) staff       (20)     1486 2023-04-07 21:09:48.000000 whatsapp-python-1.0.1/setup.py
+-rw-r--r--   0 filipporomani   (501) staff       (20)       38 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/setup.cfg
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    37867 2023-04-07 21:09:23.000000 whatsapp-python-1.0.1/whatsapp/__init__.py
```

### Comparing `whatsapp-python-1.0.0b0/PKG-INFO` & `whatsapp-python-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Description: # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
```

### Comparing `whatsapp-python-1.0.0b0/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-1.0.1/whatsapp_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 1.0.0b0
+Version: 1.0.1
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Description: # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
```

### Comparing `whatsapp-python-1.0.0b0/README.md` & `whatsapp-python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-python-1.0.0b0/setup.py` & `whatsapp-python-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_description = f.read()
 
 test_deps = ["python-dotenv==0.20.0", "pytest==7.1.3"]
 extras = {"test": test_deps}
 
 setup(
     name="whatsapp-python",
-    version="1.0.0b",
+    version="1.0.1",
     description="Opensource Python wrapper to WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
     packages=["whatsapp"],
-    install_requires=["requests", "requests-toolbelt", "colorama", "typing"],
+    install_requires=["requests", "requests-toolbelt", "typing"],
     tests_require=test_deps,
     extras_require=extras,
     keywords=[
         "whatsapp",
         "whatsapp-libary",
         "WhatsApp Cloud API Wrapper",
         "PyWhatsApp",
```

### Comparing `whatsapp-python-1.0.0b0/whatsapp/__init__.py` & `whatsapp-python-1.0.1/whatsapp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 Unofficial python wrapper for the WhatsApp Cloud API.
 """
 from __future__ import annotations
 import os
 import mimetypes
 import requests
 import logging
-import warnings
-from colorama import Fore, Style
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from typing import Optional, Dict, Any, List, Union, Tuple, Callable
 
 
 # Setup logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
@@ -141,19 +139,14 @@
         if r.status_code == 200:
             logging.info(f"Template sent to {recipient_id}")
             return r.json()
         logging.info(f"Template not sent to {recipient_id}")
         logging.info(f"Status code: {r.status_code}")
         logging.error(f"Response: {r.json()}")
         return r.json()
-
-    def send_templatev2(self, template, recipient_id, components, lang: str = "en_US"):
-        message = f"{Fore.RED}The 'send_templatev2' method is being deprecated and will be removed in the future. Please use the 'send_template' method instead.{Style.RESET_ALL}"
-        warnings.warn(message, DeprecationWarning)
-        return send_template(template, recipient_id, components, lang=lang)
     
     
     def send_location(self, lat, long, name, address, recipient_id):
         """
         Sends a location message to a WhatsApp user
 
         Args:
```

