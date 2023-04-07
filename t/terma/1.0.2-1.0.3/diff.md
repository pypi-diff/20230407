# Comparing `tmp/terma-1.0.2.tar.gz` & `tmp/terma-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terma-1.0.2.tar", last modified: Sat Apr  1 20:10:20 2023, max compression
+gzip compressed data, was "terma-1.0.3.tar", last modified: Fri Apr  7 16:51:46 2023, max compression
```

## Comparing `terma-1.0.2.tar` & `terma-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-01 20:10:20.745386 terma-1.0.2/
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     1071 2023-03-19 17:37:06.000000 terma-1.0.2/LICENSE
--rw-r--r--   0 arjunshenoy   (501) staff       (20)       73 2023-03-19 18:55:39.000000 terma-1.0.2/MANIFEST.in
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     2855 2023-04-01 20:10:20.745269 terma-1.0.2/PKG-INFO
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     2691 2023-04-01 20:10:14.000000 terma-1.0.2/README.md
--rw-r--r--   0 arjunshenoy   (501) staff       (20)       38 2023-04-01 20:10:20.745421 terma-1.0.2/setup.cfg
--rw-r--r--   0 arjunshenoy   (501) staff       (20)      478 2023-04-01 20:09:48.000000 terma-1.0.2/setup.py
-drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-01 20:10:20.744188 terma-1.0.2/terma/
--rw-r--r--   0 arjunshenoy   (501) staff       (20)        0 2023-03-19 19:05:32.000000 terma-1.0.2/terma/__init__.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     1811 2023-03-25 17:44:55.000000 terma-1.0.2/terma/app.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)      378 2023-03-18 18:14:02.000000 terma-1.0.2/terma/completer.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     1354 2023-03-25 17:49:10.000000 terma-1.0.2/terma/config.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     3125 2023-04-01 19:58:42.000000 terma-1.0.2/terma/prompt.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)      670 2023-03-18 17:40:39.000000 terma-1.0.2/terma/translator.py
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     1194 2023-03-19 19:28:49.000000 terma-1.0.2/terma/utils.py
-drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-01 20:10:20.745112 terma-1.0.2/terma.egg-info/
--rw-r--r--   0 arjunshenoy   (501) staff       (20)     2855 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/PKG-INFO
--rw-r--r--   0 arjunshenoy   (501) staff       (20)      331 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/SOURCES.txt
--rw-r--r--   0 arjunshenoy   (501) staff       (20)        1 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/dependency_links.txt
--rw-r--r--   0 arjunshenoy   (501) staff       (20)       41 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/entry_points.txt
--rw-r--r--   0 arjunshenoy   (501) staff       (20)       47 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/requires.txt
--rw-r--r--   0 arjunshenoy   (501) staff       (20)        6 2023-04-01 20:10:20.000000 terma-1.0.2/terma.egg-info/top_level.txt
+drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-07 16:51:46.018958 terma-1.0.3/
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     1071 2023-03-19 17:37:06.000000 terma-1.0.3/LICENSE
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)       73 2023-03-19 18:55:39.000000 terma-1.0.3/MANIFEST.in
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     3000 2023-04-07 16:51:46.018816 terma-1.0.3/PKG-INFO
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     2836 2023-04-07 13:53:39.000000 terma-1.0.3/README.md
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)       38 2023-04-07 16:51:46.018998 terma-1.0.3/setup.cfg
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)      478 2023-04-07 14:18:32.000000 terma-1.0.3/setup.py
+drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-07 16:51:46.017859 terma-1.0.3/terma/
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)        0 2023-03-19 19:05:32.000000 terma-1.0.3/terma/__init__.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     1811 2023-03-25 17:44:55.000000 terma-1.0.3/terma/app.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)      378 2023-03-18 18:14:02.000000 terma-1.0.3/terma/completer.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     1354 2023-03-25 17:49:10.000000 terma-1.0.3/terma/config.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     3125 2023-04-01 19:58:42.000000 terma-1.0.3/terma/prompt.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)      670 2023-03-18 17:40:39.000000 terma-1.0.3/terma/translator.py
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     2215 2023-04-07 16:43:39.000000 terma-1.0.3/terma/utils.py
+drwxr-xr-x   0 arjunshenoy   (501) staff       (20)        0 2023-04-07 16:51:46.018669 terma-1.0.3/terma.egg-info/
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)     3000 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/PKG-INFO
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)      331 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/SOURCES.txt
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)        1 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/dependency_links.txt
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)       41 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/entry_points.txt
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)       47 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/requires.txt
+-rw-r--r--   0 arjunshenoy   (501) staff       (20)        6 2023-04-07 16:51:45.000000 terma-1.0.3/terma.egg-info/top_level.txt
```

### Comparing `terma-1.0.2/LICENSE` & `terma-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `terma-1.0.2/PKG-INFO` & `terma-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terma
-Version: 1.0.2
+Version: 1.0.3
 Summary: Terminal Assistant
 Author: Arjun Shenoy A V
 Author-email: arjunshenoyav@gmail.com
 License-File: LICENSE
 
 # Terma 
 Short for Terminal Asistant, Terma is An NLP based CLI application that takes in input from the user in plain language, converts that into an appropriate bash command and finally displays this generated command along with follow up actions that the user can take. 
@@ -41,8 +41,11 @@
 
 I have a couple of ideas to improve the user experience around the application:
 
 **Output validation**: In some cases, the openAI model being used generates invalid commands based on the query inputed by the user. One approach that can be used to deal with it is to pass the output from model into another one that performs this sort of validation and ensures that the generated text is a valid os command. 
 
 **Interactive subprocess**: Would enable the users to execute commands which trigger interactive processes from with in the terma console. 
 
+**Error Explanation** : In case of errors, it would be handy to get an explanation for the errors along
+with possible actions to resolve them. 
+
 More suggestions and contributions welcome :)
```

### Comparing `terma-1.0.2/README.md` & `terma-1.0.3/terma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: terma
+Version: 1.0.3
+Summary: Terminal Assistant
+Author: Arjun Shenoy A V
+Author-email: arjunshenoyav@gmail.com
+License-File: LICENSE
+
 # Terma 
 Short for Terminal Asistant, Terma is An NLP based CLI application that takes in input from the user in plain language, converts that into an appropriate bash command and finally displays this generated command along with follow up actions that the user can take. 
 
 Inspired from the `Translate to bash` functionality in [fig.io](https://fig.io/).
 
 # Setup
 
@@ -33,8 +41,11 @@
 
 I have a couple of ideas to improve the user experience around the application:
 
 **Output validation**: In some cases, the openAI model being used generates invalid commands based on the query inputed by the user. One approach that can be used to deal with it is to pass the output from model into another one that performs this sort of validation and ensures that the generated text is a valid os command. 
 
 **Interactive subprocess**: Would enable the users to execute commands which trigger interactive processes from with in the terma console. 
 
-More suggestions and contributions welcome :) 
+**Error Explanation** : In case of errors, it would be handy to get an explanation for the errors along
+with possible actions to resolve them. 
+
+More suggestions and contributions welcome :)
```

### Comparing `terma-1.0.2/terma/app.py` & `terma-1.0.3/terma/app.py`

 * *Files identical despite different names*

### Comparing `terma-1.0.2/terma/config.py` & `terma-1.0.3/terma/config.py`

 * *Files identical despite different names*

### Comparing `terma-1.0.2/terma/prompt.py` & `terma-1.0.3/terma/prompt.py`

 * *Files identical despite different names*

### Comparing `terma-1.0.2/terma/translator.py` & `terma-1.0.3/terma/translator.py`

 * *Files identical despite different names*

### Comparing `terma-1.0.2/terma.egg-info/PKG-INFO` & `terma-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: terma
-Version: 1.0.2
-Summary: Terminal Assistant
-Author: Arjun Shenoy A V
-Author-email: arjunshenoyav@gmail.com
-License-File: LICENSE
-
 # Terma 
 Short for Terminal Asistant, Terma is An NLP based CLI application that takes in input from the user in plain language, converts that into an appropriate bash command and finally displays this generated command along with follow up actions that the user can take. 
 
 Inspired from the `Translate to bash` functionality in [fig.io](https://fig.io/).
 
 # Setup
 
@@ -41,8 +33,11 @@
 
 I have a couple of ideas to improve the user experience around the application:
 
 **Output validation**: In some cases, the openAI model being used generates invalid commands based on the query inputed by the user. One approach that can be used to deal with it is to pass the output from model into another one that performs this sort of validation and ensures that the generated text is a valid os command. 
 
 **Interactive subprocess**: Would enable the users to execute commands which trigger interactive processes from with in the terma console. 
 
-More suggestions and contributions welcome :) 
+**Error Explanation** : In case of errors, it would be handy to get an explanation for the errors along
+with possible actions to resolve them. 
+
+More suggestions and contributions welcome :)
```

