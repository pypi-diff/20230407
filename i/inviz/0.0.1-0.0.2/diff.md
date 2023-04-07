# Comparing `tmp/inviz-0.0.1.tar.gz` & `tmp/inviz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.1.tar", last modified: Thu Mar 23 21:25:06 2023, max compression
+gzip compressed data, was "inviz-0.0.2.tar", last modified: Fri Apr  7 20:22:23 2023, max compression
```

## Comparing `inviz-0.0.1.tar` & `inviz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-03-23 21:25:06.236824 inviz-0.0.1/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1071 2023-03-21 04:54:53.000000 inviz-0.0.1/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-03-21 04:54:53.000000 inviz-0.0.1/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      539 2023-03-23 21:25:06.232824 inviz-0.0.1/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1042 2023-03-21 05:19:54.000000 inviz-0.0.1/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-03-23 21:25:06.232824 inviz-0.0.1/inviz/
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-03-23 21:25:06.232824 inviz-0.0.1/inviz/inviz.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      539 2023-03-23 21:25:06.000000 inviz-0.0.1/inviz/inviz.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      212 2023-03-23 21:25:06.000000 inviz-0.0.1/inviz/inviz.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-03-23 21:25:06.000000 inviz-0.0.1/inviz/inviz.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       67 2023-03-23 21:25:06.000000 inviz-0.0.1/inviz/inviz.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-03-23 21:25:06.000000 inviz-0.0.1/inviz/inviz.egg-info/top_level.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-03-23 21:25:06.236824 inviz-0.0.1/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      945 2023-03-23 21:09:04.000000 inviz-0.0.1/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:22:23.595625 inviz-0.0.2/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-03-23 22:43:43.000000 inviz-0.0.2/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-03-23 22:43:43.000000 inviz-0.0.2/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      537 2023-04-07 20:22:23.595625 inviz-0.0.2/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2036 2023-04-07 20:17:43.000000 inviz-0.0.2/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:22:23.595625 inviz-0.0.2/inviz/
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-04-07 20:22:23.595625 inviz-0.0.2/inviz/inviz.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      537 2023-04-07 20:22:23.000000 inviz-0.0.2/inviz/inviz.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      227 2023-04-07 20:22:23.000000 inviz-0.0.2/inviz/inviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-04-07 20:22:23.000000 inviz-0.0.2/inviz/inviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       98 2023-04-07 20:22:23.000000 inviz-0.0.2/inviz/inviz.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-04-07 20:22:23.000000 inviz-0.0.2/inviz/inviz.egg-info/top_level.txt
+-rwxrwxr-x   0 maamari   (1000) maamari   (1000)     9387 2023-04-07 20:17:43.000000 inviz-0.0.2/inviz/inviz.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-04-07 20:22:23.595625 inviz-0.0.2/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1107 2023-04-07 20:20:56.000000 inviz-0.0.2/setup.py
```

### Comparing `inviz-0.0.1/LICENSE` & `inviz-0.0.2/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Karime Maamari
+Copyright (c) 2022 James Wen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `inviz-0.0.1/PKG-INFO` & `inviz-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
-Author-email: maamari@usc.edu
+Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
```

### Comparing `inviz-0.0.1/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.0.2/inviz/inviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
-Author-email: maamari@usc.edu
+Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
```

### Comparing `inviz-0.0.1/setup.py` & `inviz-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import setuptools
 
 #with open("README.md", "r") as fh:
 #    long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "James Wen",
-    author_email = "maamari@usc.edu",
+    author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
+    py_modules=["inviz"],
     package_dir={'': 'inviz'},
+#    packages=['inviz'],
+    #package_dir={'': 'inviz'},
     #long_description=long_description,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.6',              
     install_requires=["holoviews==1.15.4",
                       "spatialpandas==0.4.7",
                       "hvplot==0.8.3",
-                      "numpy==1.23.5"]                    
+                      "numpy==1.23.5",
+                      "matplotlib==3.7.1",
+                      "bokeh==3.1.0"]                    
     )
```

