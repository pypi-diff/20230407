# Comparing `tmp/whatsapp-python-1.0.1.tar.gz` & `tmp/whatsapp-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whatsapp-python-1.0.1.tar", last modified: Fri Apr  7 21:09:55 2023, max compression
+gzip compressed data, was "dist/whatsapp-python-1.0.2.tar", last modified: Fri Apr  7 21:14:15 2023, max compression
```

## Comparing `whatsapp-python-1.0.1.tar` & `whatsapp-python-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/
--rw-r--r--   0 filipporomani   (501) staff       (20)    18726 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/PKG-INFO
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/
--rw-r--r--   0 filipporomani   (501) staff       (20)    18726 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 filipporomani   (501) staff       (20)      233 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)       78 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)        9 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/top_level.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)        1 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 filipporomani   (501) staff       (20)    14594 2023-04-07 21:04:52.000000 whatsapp-python-1.0.1/README.md
--rw-r--r--   0 filipporomani   (501) staff       (20)     1486 2023-04-07 21:09:48.000000 whatsapp-python-1.0.1/setup.py
--rw-r--r--   0 filipporomani   (501) staff       (20)       38 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/setup.cfg
-drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:09:55.000000 whatsapp-python-1.0.1/whatsapp/
--rw-r--r--   0 filipporomani   (501) staff       (20)    37867 2023-04-07 21:09:23.000000 whatsapp-python-1.0.1/whatsapp/__init__.py
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    18467 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/PKG-INFO
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    18467 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 filipporomani   (501) staff       (20)      233 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)       78 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)        9 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/top_level.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)        1 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 filipporomani   (501) staff       (20)    14391 2023-04-07 21:13:52.000000 whatsapp-python-1.0.2/README.md
+-rw-r--r--   0 filipporomani   (501) staff       (20)     1486 2023-04-07 21:14:11.000000 whatsapp-python-1.0.2/setup.py
+-rw-r--r--   0 filipporomani   (501) staff       (20)       38 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/setup.cfg
+drwxr-xr-x   0 filipporomani   (501) staff       (20)        0 2023-04-07 21:14:15.000000 whatsapp-python-1.0.2/whatsapp/
+-rw-r--r--   0 filipporomani   (501) staff       (20)    37867 2023-04-07 21:09:23.000000 whatsapp-python-1.0.2/whatsapp/__init__.py
```

### Comparing `whatsapp-python-1.0.1/PKG-INFO` & `whatsapp-python-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Description: # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
         
-        [![Made in Tanzania](https://img.shields.io/badge/made%20in-tanzania-008751.svg?style=flat-square)](https://github.com/Tanzania-Developers-Community/made-in-tanzania)
+        ![Made in Tanzania](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
         [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
         [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
         [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
         
         Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
         Forked from [Neurotech-HQ/whatsapp](https://github.com/Neurotech-HQ/heyoo)
         
@@ -42,28 +42,21 @@
         ```
         
         ### Installing via pip
         
         ```bash
         # For Windows 
         
-        pip install  --upgrade whatsapp-python
+        pip install --upgrade whatsapp-python
         
         #For Linux | MAC 
         
         pip3 install --upgrade whatsapp-python
         ```
         
-        ### Running on Docker
-        To run an instance in docker run the commands below
-        ```bash
-        $ docker compose build
-        $ docker compose up
-        ```
-        
         ## Setting up
         
         To get started using this package, you will need **TOKEN** and **TEST WHATSAPP NUMBER** (the library works either with a production phone number, if you have one) which you can get from the [Facebook Developer Portal](https://developers.facebook.com/)
         
         Here are steps to follow for you to get started:
         
         1. [Go to your apps](https://developers.facebook.com/apps)
```

### Comparing `whatsapp-python-1.0.1/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-1.0.2/whatsapp_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Description: # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
         
-        [![Made in Tanzania](https://img.shields.io/badge/made%20in-tanzania-008751.svg?style=flat-square)](https://github.com/Tanzania-Developers-Community/made-in-tanzania)
+        ![Made in Tanzania](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
         [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
         [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
         [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
         
         Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
         Forked from [Neurotech-HQ/whatsapp](https://github.com/Neurotech-HQ/heyoo)
         
@@ -42,28 +42,21 @@
         ```
         
         ### Installing via pip
         
         ```bash
         # For Windows 
         
-        pip install  --upgrade whatsapp-python
+        pip install --upgrade whatsapp-python
         
         #For Linux | MAC 
         
         pip3 install --upgrade whatsapp-python
         ```
         
-        ### Running on Docker
-        To run an instance in docker run the commands below
-        ```bash
-        $ docker compose build
-        $ docker compose up
-        ```
-        
         ## Setting up
         
         To get started using this package, you will need **TOKEN** and **TEST WHATSAPP NUMBER** (the library works either with a production phone number, if you have one) which you can get from the [Facebook Developer Portal](https://developers.facebook.com/)
         
         Here are steps to follow for you to get started:
         
         1. [Go to your apps](https://developers.facebook.com/apps)
```

### Comparing `whatsapp-python-1.0.1/README.md` & `whatsapp-python-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
-[![Made in Tanzania](https://img.shields.io/badge/made%20in-tanzania-008751.svg?style=flat-square)](https://github.com/Tanzania-Developers-Community/made-in-tanzania)
+![Made in Tanzania](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
 Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
 Forked from [Neurotech-HQ/whatsapp](https://github.com/Neurotech-HQ/heyoo)
 
@@ -34,28 +34,21 @@
 ```
 
 ### Installing via pip
 
 ```bash
 # For Windows 
 
-pip install  --upgrade whatsapp-python
+pip install --upgrade whatsapp-python
 
 #For Linux | MAC 
 
 pip3 install --upgrade whatsapp-python
 ```
 
-### Running on Docker
-To run an instance in docker run the commands below
-```bash
-$ docker compose build
-$ docker compose up
-```
-
 ## Setting up
 
 To get started using this package, you will need **TOKEN** and **TEST WHATSAPP NUMBER** (the library works either with a production phone number, if you have one) which you can get from the [Facebook Developer Portal](https://developers.facebook.com/)
 
 Here are steps to follow for you to get started:
 
 1. [Go to your apps](https://developers.facebook.com/apps)
```

### Comparing `whatsapp-python-1.0.1/setup.py` & `whatsapp-python-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = f.read()
 
 test_deps = ["python-dotenv==0.20.0", "pytest==7.1.3"]
 extras = {"test": test_deps}
 
 setup(
     name="whatsapp-python",
-    version="1.0.1",
+    version="1.0.2",
     description="Opensource Python wrapper to WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
```

### Comparing `whatsapp-python-1.0.1/whatsapp/__init__.py` & `whatsapp-python-1.0.2/whatsapp/__init__.py`

 * *Files identical despite different names*

