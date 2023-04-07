# Comparing `tmp/srivastav-0.0.2.tar.gz` & `tmp/srivastav-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srivastav-0.0.2.tar", last modified: Fri Apr  7 08:27:32 2023, max compression
+gzip compressed data, was "srivastav-0.0.3.tar", last modified: Fri Apr  7 18:33:44 2023, max compression
```

## Comparing `srivastav-0.0.2.tar` & `srivastav-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 08:27:32.913339 srivastav-0.0.2/
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      549 2023-04-07 08:27:32.913339 srivastav-0.0.2/PKG-INFO
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)       84 2023-04-07 05:41:40.000000 srivastav-0.0.2/pyproject.toml
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      478 2023-04-07 08:27:32.913339 srivastav-0.0.2/setup.cfg
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      604 2023-04-07 08:26:13.000000 srivastav-0.0.2/setup.py
-drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 08:27:32.909340 srivastav-0.0.2/src/
-drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 08:27:32.909340 srivastav-0.0.2/src/srivastav/
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 05:40:18.000000 srivastav-0.0.2/src/srivastav/__init__.py
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      934 2023-04-07 05:25:01.000000 srivastav-0.0.2/src/srivastav/middleware.py
-drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 08:27:32.913339 srivastav-0.0.2/src/srivastav.egg-info/
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      549 2023-04-07 08:27:32.000000 srivastav-0.0.2/src/srivastav.egg-info/PKG-INFO
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      235 2023-04-07 08:27:32.000000 srivastav-0.0.2/src/srivastav.egg-info/SOURCES.txt
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)        1 2023-04-07 08:27:32.000000 srivastav-0.0.2/src/srivastav.egg-info/dependency_links.txt
--rw-rw-r--   0 srivastav  (1000) srivastav  (1000)       10 2023-04-07 08:27:32.000000 srivastav-0.0.2/src/srivastav.egg-info/top_level.txt
+drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 18:33:44.665882 srivastav-0.0.3/
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      549 2023-04-07 18:33:44.665882 srivastav-0.0.3/PKG-INFO
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)       84 2023-04-07 05:41:40.000000 srivastav-0.0.3/pyproject.toml
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      478 2023-04-07 18:33:44.669882 srivastav-0.0.3/setup.cfg
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      644 2023-04-07 18:14:13.000000 srivastav-0.0.3/setup.py
+drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 18:33:44.661882 srivastav-0.0.3/src/
+drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 18:33:44.665882 srivastav-0.0.3/src/srivastav/
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 05:40:18.000000 srivastav-0.0.3/src/srivastav/__init__.py
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      150 2023-04-07 17:48:06.000000 srivastav-0.0.3/src/srivastav/conversion.py
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)     1115 2023-04-07 18:31:54.000000 srivastav-0.0.3/src/srivastav/middleware.py
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)     1477 2023-04-07 18:07:40.000000 srivastav-0.0.3/src/srivastav/server_info.py
+drwxrwxr-x   0 srivastav  (1000) srivastav  (1000)        0 2023-04-07 18:33:44.665882 srivastav-0.0.3/src/srivastav.egg-info/
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      549 2023-04-07 18:33:44.000000 srivastav-0.0.3/src/srivastav.egg-info/PKG-INFO
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)      328 2023-04-07 18:33:44.000000 srivastav-0.0.3/src/srivastav.egg-info/SOURCES.txt
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)        1 2023-04-07 18:33:44.000000 srivastav-0.0.3/src/srivastav.egg-info/dependency_links.txt
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)       14 2023-04-07 18:33:44.000000 srivastav-0.0.3/src/srivastav.egg-info/requires.txt
+-rw-rw-r--   0 srivastav  (1000) srivastav  (1000)       10 2023-04-07 18:33:44.000000 srivastav-0.0.3/src/srivastav.egg-info/top_level.txt
```

### Comparing `srivastav-0.0.2/PKG-INFO` & `srivastav-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srivastav
-Version: 0.0.2
+Version: 0.0.3
 Summary: Downalerts django Middleware 
 Home-page: https://github.com/downalerts/django-logger
 Author: Aman Srivastav
 Author-email: amansrivastav.bytequests@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `srivastav-0.0.2/setup.py` & `srivastav-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 
 setup(
     name='srivastav',
-    version='0.0.2',    
+    version='0.0.3',    
     description='Downalerts django Middleware ',
     url='https://github.com/downalerts/django-logger',
     author='Aman Srivastav',
     author_email='amansrivastav.bytequests@gmail.com',
     license='BSD 2-clause',
     packages=['srivastav'],
+    install_requires=['psutil>=5.9.4'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3.5',
     ],
```

### Comparing `srivastav-0.0.2/src/srivastav.egg-info/PKG-INFO` & `srivastav-0.0.3/src/srivastav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srivastav
-Version: 0.0.2
+Version: 0.0.3
 Summary: Downalerts django Middleware 
 Home-page: https://github.com/downalerts/django-logger
 Author: Aman Srivastav
 Author-email: amansrivastav.bytequests@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

