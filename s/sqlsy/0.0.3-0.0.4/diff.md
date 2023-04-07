# Comparing `tmp/sqlsy-0.0.3.tar.gz` & `tmp/sqlsy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsy-0.0.3.tar", last modified: Thu Apr  6 02:03:59 2023, max compression
+gzip compressed data, was "sqlsy-0.0.4.tar", last modified: Fri Apr  7 17:09:31 2023, max compression
```

## Comparing `sqlsy-0.0.3.tar` & `sqlsy-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-06 02:03:59.819790 sqlsy-0.0.3/
--rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-06 02:03:59.819790 sqlsy-0.0.3/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)     2549 2023-04-06 01:38:15.000000 sqlsy-0.0.3/README.md
--rw-r--r--   0 logic     (1000) logic     (1000)      729 2023-04-06 02:02:03.000000 sqlsy-0.0.3/pyproject.toml
--rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-06 02:03:59.819790 sqlsy-0.0.3/setup.cfg
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-06 02:03:59.815790 sqlsy-0.0.3/src/
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-06 02:03:59.819790 sqlsy-0.0.3/src/sqlsy/
--rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-05 00:55:42.000000 sqlsy-0.0.3/src/sqlsy/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)       98 2023-04-05 00:56:42.000000 sqlsy-0.0.3/src/sqlsy/__main__.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     5272 2023-04-06 01:27:32.000000 sqlsy-0.0.3/src/sqlsy/engine.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-06 02:03:59.819790 sqlsy-0.0.3/src/sqlsy/utils/
--rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-03 17:18:12.000000 sqlsy-0.0.3/src/sqlsy/utils/__init__.py
--rw-r--r--   0 logic     (1000) logic     (1000)      724 2023-04-06 02:01:51.000000 sqlsy-0.0.3/src/sqlsy/utils/custom_callbacks.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     1212 2023-04-06 01:32:47.000000 sqlsy-0.0.3/src/sqlsy/utils/mapping.py
--rwxrwxr--   0 logic     (1000) logic     (1000)     1798 2023-04-05 14:42:37.000000 sqlsy-0.0.3/src/sqlsy/utils/schema.py
-drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-06 02:03:59.819790 sqlsy-0.0.3/src/sqlsy.egg-info/
--rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/PKG-INFO
--rw-r--r--   0 logic     (1000) logic     (1000)      405 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/SOURCES.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/dependency_links.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       46 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/entry_points.txt
--rw-r--r--   0 logic     (1000) logic     (1000)       44 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/requires.txt
--rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-06 02:03:59.000000 sqlsy-0.0.3/src/sqlsy.egg-info/top_level.txt
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-07 17:09:31.160633 sqlsy-0.0.4/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)     2549 2023-04-06 01:38:15.000000 sqlsy-0.0.4/README.md
+-rw-r--r--   0 logic     (1000) logic     (1000)      739 2023-04-07 17:09:25.000000 sqlsy-0.0.4/pyproject.toml
+-rw-r--r--   0 logic     (1000) logic     (1000)       38 2023-04-07 17:09:31.160633 sqlsy-0.0.4/setup.cfg
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.156633 sqlsy-0.0.4/src/
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy/
+-rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-05 00:55:42.000000 sqlsy-0.0.4/src/sqlsy/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)       98 2023-04-05 00:56:42.000000 sqlsy-0.0.4/src/sqlsy/__main__.py
+-rwxrwxr--   0 logic     (1000) logic     (1000)     5338 2023-04-07 16:59:04.000000 sqlsy-0.0.4/src/sqlsy/engine.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy/utils/
+-rw-r--r--   0 logic     (1000) logic     (1000)        0 2023-04-03 17:18:12.000000 sqlsy-0.0.4/src/sqlsy/utils/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)      846 2023-04-07 17:07:57.000000 sqlsy-0.0.4/src/sqlsy/utils/custom_callbacks.py
+-rwxrwxr--   0 logic     (1000) logic     (1000)     1257 2023-04-07 17:08:20.000000 sqlsy-0.0.4/src/sqlsy/utils/mapping.py
+-rwxrwxr--   0 logic     (1000) logic     (1000)     1948 2023-04-07 16:47:15.000000 sqlsy-0.0.4/src/sqlsy/utils/schema.py
+drwxr-xr-x   0 logic     (1000) logic     (1000)        0 2023-04-07 17:09:31.160633 sqlsy-0.0.4/src/sqlsy.egg-info/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3040 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)      405 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/SOURCES.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        1 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/dependency_links.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       46 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/entry_points.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)       50 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/requires.txt
+-rw-r--r--   0 logic     (1000) logic     (1000)        6 2023-04-07 17:09:31.000000 sqlsy-0.0.4/src/sqlsy.egg-info/top_level.txt
```

### Comparing `sqlsy-0.0.3/PKG-INFO` & `sqlsy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fill your database Quickly with dummy data
 Author-email: shoaib wani <shoaibwani010@gmail.com>
 Project-URL: Homepage, https://github.com/pyloris/sqlsy
 Keywords: sql,sql dummy data,fake data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `sqlsy-0.0.3/README.md` & `sqlsy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlsy-0.0.3/pyproject.toml` & `sqlsy-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlsy"
-version = "0.0.3"
+version = "0.0.4"
 description = "Fill your database Quickly with dummy data"
 readme = "README.md"
 authors = [{ name="shoaib wani", email="shoaibwani010@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["sql", "sql dummy data", "fake data"]
 requires-python = ">=3.9"
 classifiers = [
@@ -17,15 +17,16 @@
 	"Programming Language :: Python :: 3.11",
 	"Topic :: Database"
 ]
 dependencies = [
 	"mysql-connector-python",
 	"faker",
 	"rich",
-	"termcolor"
+	"termcolor",
+	"numpy"
 ]
 
 [project.urls]
 Homepage = "https://github.com/pyloris/sqlsy"
 
 [project.scripts]
 sqlsy = "sqlsy.__main__:main"
```

### Comparing `sqlsy-0.0.3/src/sqlsy/engine.py` & `sqlsy-0.0.4/src/sqlsy/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
 		# store for printing the table
 		self.cols = schema.keys()
 
 		for data in schema.values():
 
 			if data['type'] == 'int':
 				query_holders.append("%d")
+			elif data['type'] == 'float':
+				query_holders.append("%f")
 			else:
 				query_holders.append('"%s"')
 
 		# build the query
 		vals += "("+",".join(query_holders)+");"
 
 		# final query
```

### Comparing `sqlsy-0.0.3/src/sqlsy/utils/custom_callbacks.py` & `sqlsy-0.0.4/src/sqlsy/utils/custom_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import random
 from sqlsy.engine import Engine
-
+import numpy as np
 
 random.seed()
 
-
 # choose from sequence at random
 def random_choice(sequence: list):
 	return random.choice(sequence)
 
 
+# generate random floats
+def random_float(n1:int, n2:int):
+	return random.choice(np.arange(n1, n2, 0.1))
+
 # make multiple calls independent
 def sequential_choice():
 	state ={}
 	def internal(sequence:list):
 		nonlocal state
 		col = Engine.get_col()
 		state.setdefault(col, 0)
@@ -27,11 +30,10 @@
 def sequence():
 	state = {}
 	# generate sequence of numbers
 	def internal(n1:int, n2:int):
 		nonlocal state
 		col = Engine.get_col()   # get current column being filled
 		state.setdefault(col, n1)
-
 		state[col] += 1
 		return state[col]-1
 	return internal
```

### Comparing `sqlsy-0.0.3/src/sqlsy/utils/mapping.py` & `sqlsy-0.0.4/src/sqlsy/utils/mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #### 
 # This file contains all the mappings provided
 # mappings map the user provided strings (pre-defined)
 # to specific faker module functions.
 #####
 
-from .custom_callbacks import random_choice, sequential_choice, sequence
+from .custom_callbacks import random_choice, sequential_choice, sequence, random_float
 from faker import Faker
 
 
 fake = Faker()
 
 
 varchar = {
@@ -38,14 +38,15 @@
 }
 
 
 # generate pure random numbers for entropy
 numbers = {
 	'random_int':fake.random_int,
 	'random_digit':fake.random_int,
+	'random_float':random_float,
 	'sequence':sequence()
 }
 
 
 custom = {
 	'random_choice':random_choice,
 	'sequential_choice':sequential_choice()
```

### Comparing `sqlsy-0.0.3/src/sqlsy/utils/schema.py` & `sqlsy-0.0.4/src/sqlsy/utils/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,21 @@
 def Int(*, hook=None, custom_func=None, args:list=None, this=None):
 	# used in dynamic query building
 	this['type'] = 'int'
 	return this
 
 
 @datatype
+def Float(*, hook=None, custom_func=None, args:list=None, this=None):
+	# store the float type
+	this['type'] = 'float'
+	return this
+
+
+@datatype
 def Char(*, hook=None, custom_func=None, args:list=None, this=None):
 	this['type'] = 'char(255)'
 	return this
 
 
 @datatype
 def VarChar(*, hook=None, custom_func=None, args:list = None, this=None):
```

### Comparing `sqlsy-0.0.3/src/sqlsy.egg-info/PKG-INFO` & `sqlsy-0.0.4/src/sqlsy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fill your database Quickly with dummy data
 Author-email: shoaib wani <shoaibwani010@gmail.com>
 Project-URL: Homepage, https://github.com/pyloris/sqlsy
 Keywords: sql,sql dummy data,fake data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

