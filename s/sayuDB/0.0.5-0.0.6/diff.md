# Comparing `tmp/sayuDB-0.0.5.tar.gz` & `tmp/sayuDB-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-0.0.5.tar", last modified: Sun Apr  2 10:39:04 2023, max compression
+gzip compressed data, was "sayuDB-0.0.6.tar", last modified: Fri Apr  7 20:05:47 2023, max compression
```

## Comparing `sayuDB-0.0.5.tar` & `sayuDB-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 10:39:04.832862 sayuDB-0.0.5/
--rw-rw-rw-   0        0        0     1064 2023-04-02 10:29:14.000000 sayuDB-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     6072 2023-04-02 10:39:04.832862 sayuDB-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5767 2023-04-02 10:29:14.000000 sayuDB-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 10:39:04.821687 sayuDB-0.0.5/sayuDB/
--rw-rw-rw-   0        0        0      635 2023-04-02 10:29:14.000000 sayuDB-0.0.5/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     3905 2023-04-02 10:38:05.000000 sayuDB-0.0.5/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    14085 2023-04-02 10:29:14.000000 sayuDB-0.0.5/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2084 2023-04-02 10:29:14.000000 sayuDB-0.0.5/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3150 2023-04-02 10:29:14.000000 sayuDB-0.0.5/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-04-02 10:39:04.831848 sayuDB-0.0.5/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     6072 2023-04-02 10:39:04.000000 sayuDB-0.0.5/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-02 10:39:04.000000 sayuDB-0.0.5/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 10:39:04.000000 sayuDB-0.0.5/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-02 10:39:04.000000 sayuDB-0.0.5/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-02 10:39:04.000000 sayuDB-0.0.5/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 10:39:04.832862 sayuDB-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     6275 2023-04-02 10:37:40.000000 sayuDB-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.797187 sayuDB-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-07 17:42:40.000000 sayuDB-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-04-07 20:05:47.793187 sayuDB-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5967 2023-04-07 17:42:40.000000 sayuDB-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.793187 sayuDB-0.0.6/sayuDB/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-07 17:42:40.000000 sayuDB-0.0.6/sayuDB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-04-07 20:04:03.000000 sayuDB-0.0.6/sayuDB/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    14085 2023-04-07 19:03:04.000000 sayuDB-0.0.6/sayuDB/processor.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-04-07 19:28:19.000000 sayuDB-0.0.6/sayuDB/remote.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-04-07 20:02:49.000000 sayuDB-0.0.6/sayuDB/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 20:05:47.793187 sayuDB-0.0.6/sayuDB.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-07 20:05:47.000000 sayuDB-0.0.6/sayuDB.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 20:05:47.797187 sayuDB-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-04-07 20:04:44.000000 sayuDB-0.0.6/setup.py
```

### Comparing `sayuDB-0.0.5/LICENSE` & `sayuDB-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Arsybai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Arsybai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sayuDB-0.0.5/PKG-INFO` & `sayuDB-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,8 @@
-Metadata-Version: 2.1
-Name: sayuDB
-Version: 0.0.5
-Summary: Database management system based on python and JSON.
-Home-page: https://github.com/Arsybai/sayuDB
-Author: Arsybai
-Author-email: me@arsybai.com
-License: MIT
-Keywords: database
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
 
 # Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
@@ -38,36 +28,44 @@
 Before you can use sayuDB you need to install it, of course.
 Just clone this repository and place it to your project folder.
 ```shell
 > pip3 install sayuDB
 ```
 for help menu:
 ```shell
-> python3 sayuDB --h
+> python3 -m sayuDB --h
 ```
 
 #### 1.2 Creating database
 The first test to see whether you can access the database server is to try to create a database.
 
 To create a new database, in this example named `myDB`, you use the following funtion:
 ```python
 import sayuDB
 
 # Creating database
 sayuDB.create_database('myDB')
 ```
+
+```shell
+> python3 -m sayuDB create database <database_name>
+```
 You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
 
 If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
 ```python
 import sayuDB
 
 sayuDB.drop_database('myDB')
 ```
 
+```shell
+> python3 -m sayuDB drop database <database_name>
+```
+
 You can import export using:
 ```python
 # Exporting database (must use file name)
 sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
 # Importing database
 sayuDB.import_database(path_='/<path>/filename.ezdb')
 ```
```

### Comparing `sayuDB-0.0.5/README.md` & `sayuDB-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-![banner](https://images.arsybai.app/images/pOMsOCbxLR.png)
+Metadata-Version: 2.1
+Name: sayuDB
+Version: 0.0.6
+Summary: Database management system based on python and JSON.
+Home-page: https://github.com/Arsybai/sayuDB
+Author: Arsybai
+Author-email: me@arsybai.com
+License: MIT
+Keywords: database
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
@@ -28,44 +39,36 @@
 Before you can use sayuDB you need to install it, of course.
 Just clone this repository and place it to your project folder.
 ```shell
 > pip3 install sayuDB
 ```
 for help menu:
 ```shell
-> python3 -m sayuDB --h
+> python3 sayuDB --h
 ```
 
 #### 1.2 Creating database
 The first test to see whether you can access the database server is to try to create a database.
 
 To create a new database, in this example named `myDB`, you use the following funtion:
 ```python
 import sayuDB
 
 # Creating database
 sayuDB.create_database('myDB')
 ```
-
-```shell
-> python3 -m sayuDB create database <database_name>
-```
 You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
 
 If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
 ```python
 import sayuDB
 
 sayuDB.drop_database('myDB')
 ```
 
-```shell
-> python3 -m sayuDB drop database <database_name>
-```
-
 You can import export using:
 ```python
 # Exporting database (must use file name)
 sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
 # Importing database
 sayuDB.import_database(path_='/<path>/filename.ezdb')
 ```
@@ -194,7 +197,9 @@
 Look at the new state of the data:
 ```shell
 name       age  city
 -------  -----  ------------------
 Arsybai     23  Solo, Indonesia
 Moepoi      21  Jakarta, Indonesia
 ```
+
+
```

### Comparing `sayuDB-0.0.5/sayuDB/__init__.py` & `sayuDB-0.0.6/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-0.0.5/sayuDB/processor.py` & `sayuDB-0.0.6/sayuDB/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                 datas_ = sorted(datas_, key=itemgetter(key_))
             elif sort_ == 'desc':
                 datas_ = sorted(datas_, key=itemgetter(key_), reverse=True)
                     
         #the anu anu
         if as_json:
             try:
-                return json.dumps(datas_)
+                return json.loads(datas_)
             except:
                 return datas_
         headeer_ = []
         rows_ = []
         try:
             if datas_ != []:
                 for i in datas_[0]:
```

### Comparing `sayuDB-0.0.5/sayuDB/remote.py` & `sayuDB-0.0.6/sayuDB/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,10 +47,8 @@
         response = sendRequest(self.host+'/commit', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database, 'content':str(encode_base64(content))}, 'POST')
         if response != 'ok':
             exit(response)
         return True
     
     def pull_database(self, database:str):
         response = sendRequest(self.host+'/pull', {'username':encode_base64(self.username), 'password':encode_base64(self.password), 'database':database})
-        if response != 'ok':
-            exit(response)
-        return True
+        return json.loads(response)
```

### Comparing `sayuDB-0.0.5/sayuDB/server.py` & `sayuDB-0.0.6/sayuDB/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,66 +15,70 @@
     return encoded_string
 
 def decode_base64(encoded_string):
     decoded_bytes = base64.b64decode(encoded_string.encode('utf-8'))
     decoded_string = decoded_bytes.decode('utf-8')
     return decoded_string
 
-with open(f'{os.path.dirname(__file__)}/users.json', 'r') as user:
-    user = json.load(user)
-with open(f'{os.path.dirname(__file__)}/config.json', 'r') as config:
-    config = json.load(config)
+def user():
+    with open(f'{os.path.dirname(__file__)}/users.json', 'r') as user:
+        user = json.load(user)
+    return user
+def config():
+    with open(f'{os.path.dirname(__file__)}/config.json', 'r') as config:
+        config = json.load(config)
+    return config
 
 def save_conf():
     with open('users.json', 'w')as wconf:
-        json.dump(user, wconf, indent=4)
+        json.dump(user(), wconf, indent=4)
     with open('config.json', 'w')as wconf:
-        json.dump(config, wconf, indent=4)
+        json.dump(config(), wconf, indent=4)
     return
 
 def checkAuth():
     username = decode_base64(request.form['username'])
     password = decode_base64(request.form['password'])
     if username not in user:
         return "User not found"
-    if password != user[username]['password']:
+    if password != user()[username]['password']:
         return "Invalid credentials"
     if username == 'root':
         return "Action rejected"
     return True
 
 def hasAccess(username, database):
-    if database in user[username]['access']:
+    if database in user()[username]['access']:
         return True
     return
 
 @app.route('/')
 def ping():
     return 'ok'
 
 @app.route('/oauth')
 def oauth():
     username = decode_base64(request.form['username'])
     password = decode_base64(request.form['password'])
-    if username not in user:
+    if username not in user():
         return "User not found"
-    if password != user[username]['password']:
+    if password != user()[username]['password']:
         return "Invalid credentials"
     return 'ok'
 
 @app.route('/existence')
 def database_existence():
     username = decode_base64(request.form['username'])
     database = request.form['database']
     db = sayuDB.show_databases()
     if database not in db:
         return "Database not found in server"
     if not checkAuth():
         return "Authorization rejected"
-    if username not in user or database not in user[username]['access']:
+    if username not in user() or database not in user()[username]['access']:
         return "Database not found in server"
     return 'ok'
     
 @app.route('/commit', methods=['POST'])
 def commit():
     username = decode_base64(request.form['username'])
     database = request.form['database']
```

### Comparing `sayuDB-0.0.5/sayuDB.egg-info/PKG-INFO` & `sayuDB-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-Metadata-Version: 2.1
-Name: sayuDB
-Version: 0.0.5
-Summary: Database management system based on python and JSON.
-Home-page: https://github.com/Arsybai/sayuDB
-Author: Arsybai
-Author-email: me@arsybai.com
-License: MIT
-Keywords: database
-Description-Content-Type: text/markdown
-License-File: LICENSE
+import setuptools
 
-# Documentation
+setuptools.setup(
+    name="sayuDB",
+    version="0.0.6",
+    author="Arsybai",
+    description="Database management system based on python and JSON.",
+    packages=["sayuDB"],
+    license="MIT",
+    author_email="me@arsybai.com",
+    url="https://github.com/Arsybai/sayuDB",
+    keywords=[
+        'database',
+    ],
+    install_requires=[
+    'requests',
+    'tabulate',
+    'flask'
+    ],
+    long_description_content_type="text/markdown",
+    long_description="""# Documentation
 
 ##### Table of content
 ###### Preface
 1. [What is sayuDB](#1_What_is_sayuDB_18)
 
 ###### Tutorial
 1. [Getting Started](#1-getting-started)
@@ -196,7 +204,9 @@
 Look at the new state of the data:
 ```shell
 name       age  city
 -------  -----  ------------------
 Arsybai     23  Solo, Indonesia
 Moepoi      21  Jakarta, Indonesia
 ```
+"""
+)
```

### Comparing `sayuDB-0.0.5/setup.py` & `sayuDB-0.0.6/sayuDB.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,212 +1,205 @@
-import setuptools
-
-setuptools.setup(
-    name="sayuDB",
-    version="0.0.5",
-    author="Arsybai",
-    description="Database management system based on python and JSON.",
-    packages=["sayuDB"],
-    license="MIT",
-    author_email="me@arsybai.com",
-    url="https://github.com/Arsybai/sayuDB",
-    keywords=[
-        'database',
-    ],
-    install_requires=[
-    'requests',
-    'tabulate',
-    'flask'
-    ],
-    long_description_content_type="text/markdown",
-    long_description="""# Documentation
-
-##### Table of content
-###### Preface
-1. [What is sayuDB](#1_What_is_sayuDB_18)
-
-###### Tutorial
-1. [Getting Started](#1-getting-started)
-- 1.1 [Installation](#11-installation)
-- 1.2 [Creating database](#12-creating-database)
-- 1.3 [Creating a New Table](#13-creating-a-new-table)
-- 1.4 [Populating a table with rows](#14-pupulating-a-table-with-rows)
-- 1.5 [Querying a Table](#15-querying-a-table)
-- 1.6 [Updates](#updates)
-- 1.7 [Deletion](#17-deletion)
-
----
-# Preface
-### 1. What is sayuDB
-sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
-It supports a large part of the SQL standard feature
-
-# Tutorial
-### 1. Getting Started
-#### 1.1 Installation
-Before you can use sayuDB you need to install it, of course.
-Just clone this repository and place it to your project folder.
-```shell
-> pip3 install sayuDB
-```
-for help menu:
-```shell
-> python3 sayuDB --h
-```
-
-#### 1.2 Creating database
-The first test to see whether you can access the database server is to try to create a database.
-
-To create a new database, in this example named `myDB`, you use the following funtion:
-```python
-import sayuDB
-
-# Creating database
-sayuDB.create_database('myDB')
-```
-You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
-
-If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
-```python
-import sayuDB
-
-sayuDB.drop_database('myDB')
-```
-
-You can import export using:
-```python
-# Exporting database (must use file name)
-sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
-# Importing database
-sayuDB.import_database(path_='/<path>/filename.ezdb')
-```
-
-#### 1.3 Creating a New Table
-You can create a new table by specifying the table name, along with all column names and their types:
-
-you must define the database first with:
-```python
-import sayuDB
-
-db = sayuDB.sayuDB(database='myDB')
-```
-
-then
-```python
-db.create_table('people', [
-    ['name','str'],
-    ['age','int'],
-    ['city','str']
-])
-```
-sayuDB currenly support data types `str`,`int`,`float`,`dict`
-
-If you want to show the table, using this following function:
-```python
-db.show_table(name='people')
-```
-it will returned as printed table:
-```shell
-name    column    datas
-------  --------  -------
-```
-
-Finally, it should be mentioned that if you don't need a table any longer or want to recreate it differently you can remove it using the following function:
-```python
-db.drop_table(name='people')
-```
-
-#### 1.4 Populating a Table With Rows
-The `insert_row` function is used to populate a table with rows:
-```python
-db.insert_row(table='people', col='name,age,city', contents=['Arsybai', 23, 'Solo, Indonesia'])
-```
-_You can also use col as list. EX `['name','age','city']`_
-
-### 1.5 Querying a Table
-To retrieve data from a table, the table is queried. An `select_row` funtion is used to do this. The funtion is divided into a select list (the part that lists the columns to be returned), a table list (the part that lists the tables from which to retrieve the data), and an optional qualification (the part that specifies any restrictions). For example, to retrieve all the rows of table `people`, type:
-```python
-data = db.select_row(table='people', col='*')
-print(data)
-```
-Here `*` is a shorthand for “all columns”. So the same result would be had with:
-```python
-db.select_row(table='people', col='name,age,city')
-```
-The output should be:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Ataro       25  Bekasi, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-
-If you want the output is json, use `as_json=True`:
-```python
-data = db.select_row(table='people', col='*', as_json=True)
-print(data)
-```
-
-A query can be “qualified” by adding a `where` clause that specifies which rows are wanted:
-```python
-data = db.select_row(table='people', col='*', where='age=23')
-print(data)
-```
-you can also use ` contain ` for specific column that contain some value:
-```python
-data = db.select_row(table='people', col='*', where='age contain 23')
-print(data)
-```
-Result:
-```shell
-name       age  city
--------  -----  ---------------
-Arsybai     23  Solo, Indonesia
-```
-
-You can request that the results of a query be returned in sorted order:
-```python
-data = db.select_row(table='people', col='*', order_by='age|asc')
-print(data)
-```
-_The order should be `asc` or `desc`_
-
-Result:
-```shell
-name       age  city
--------  -----  ------------------
-Moepoi      21  Jakarta, Indonesia
-Arsybai     23  Solo, Indonesia
-Ataro       25  Bekasi, Indonesia
-```
-
-#### Updates
-You can update existing rows using the `update_row`.
-as example I want to set `Ataro` age to `26`:
-```python
-db.update_row(table='people', set_='age=26', where='name=Ataro')
-```
-Look at the new state of the data:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Ataro       26  Bekasi, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-
-#### Deletion
-Rows can be removed from a table using the `delete_row`:
-```python
-db.delete_row(table='people', where='name=Ataro')
-```
-
-Look at the new state of the data:
-```shell
-name       age  city
--------  -----  ------------------
-Arsybai     23  Solo, Indonesia
-Moepoi      21  Jakarta, Indonesia
-```
-"""
-)
+Metadata-Version: 2.1
+Name: sayuDB
+Version: 0.0.6
+Summary: Database management system based on python and JSON.
+Home-page: https://github.com/Arsybai/sayuDB
+Author: Arsybai
+Author-email: me@arsybai.com
+License: MIT
+Keywords: database
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Documentation
+
+##### Table of content
+###### Preface
+1. [What is sayuDB](#1_What_is_sayuDB_18)
+
+###### Tutorial
+1. [Getting Started](#1-getting-started)
+- 1.1 [Installation](#11-installation)
+- 1.2 [Creating database](#12-creating-database)
+- 1.3 [Creating a New Table](#13-creating-a-new-table)
+- 1.4 [Populating a table with rows](#14-pupulating-a-table-with-rows)
+- 1.5 [Querying a Table](#15-querying-a-table)
+- 1.6 [Updates](#updates)
+- 1.7 [Deletion](#17-deletion)
+
+---
+# Preface
+### 1. What is sayuDB
+sayuDB is an database management system based on python and JSON. Developed at Clee Ltd. This project actually for personal purpose only but for some reason I publish it.
+It supports a large part of the SQL standard feature
+
+# Tutorial
+### 1. Getting Started
+#### 1.1 Installation
+Before you can use sayuDB you need to install it, of course.
+Just clone this repository and place it to your project folder.
+```shell
+> pip3 install sayuDB
+```
+for help menu:
+```shell
+> python3 sayuDB --h
+```
+
+#### 1.2 Creating database
+The first test to see whether you can access the database server is to try to create a database.
+
+To create a new database, in this example named `myDB`, you use the following funtion:
+```python
+import sayuDB
+
+# Creating database
+sayuDB.create_database('myDB')
+```
+You can also create databases with other names. sayuDB allows you to create any number of databases at a given site. Database names must have an alphabetic first character, can not contain space and are limited to 63 bytes in length.
+
+If you do not want to use your database anymore you can remove it. For example, you can destroy it using the following function:
+```python
+import sayuDB
+
+sayuDB.drop_database('myDB')
+```
+
+You can import export using:
+```python
+# Exporting database (must use file name)
+sayuDB.export_database('<name_of_database>', path_='<path>/filename.ezdb')
+# Importing database
+sayuDB.import_database(path_='/<path>/filename.ezdb')
+```
+
+#### 1.3 Creating a New Table
+You can create a new table by specifying the table name, along with all column names and their types:
+
+you must define the database first with:
+```python
+import sayuDB
+
+db = sayuDB.sayuDB(database='myDB')
+```
+
+then
+```python
+db.create_table('people', [
+    ['name','str'],
+    ['age','int'],
+    ['city','str']
+])
+```
+sayuDB currenly support data types `str`,`int`,`float`,`dict`
+
+If you want to show the table, using this following function:
+```python
+db.show_table(name='people')
+```
+it will returned as printed table:
+```shell
+name    column    datas
+------  --------  -------
+```
+
+Finally, it should be mentioned that if you don't need a table any longer or want to recreate it differently you can remove it using the following function:
+```python
+db.drop_table(name='people')
+```
+
+#### 1.4 Populating a Table With Rows
+The `insert_row` function is used to populate a table with rows:
+```python
+db.insert_row(table='people', col='name,age,city', contents=['Arsybai', 23, 'Solo, Indonesia'])
+```
+_You can also use col as list. EX `['name','age','city']`_
+
+### 1.5 Querying a Table
+To retrieve data from a table, the table is queried. An `select_row` funtion is used to do this. The funtion is divided into a select list (the part that lists the columns to be returned), a table list (the part that lists the tables from which to retrieve the data), and an optional qualification (the part that specifies any restrictions). For example, to retrieve all the rows of table `people`, type:
+```python
+data = db.select_row(table='people', col='*')
+print(data)
+```
+Here `*` is a shorthand for “all columns”. So the same result would be had with:
+```python
+db.select_row(table='people', col='name,age,city')
+```
+The output should be:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Ataro       25  Bekasi, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+
+If you want the output is json, use `as_json=True`:
+```python
+data = db.select_row(table='people', col='*', as_json=True)
+print(data)
+```
+
+A query can be “qualified” by adding a `where` clause that specifies which rows are wanted:
+```python
+data = db.select_row(table='people', col='*', where='age=23')
+print(data)
+```
+you can also use ` contain ` for specific column that contain some value:
+```python
+data = db.select_row(table='people', col='*', where='age contain 23')
+print(data)
+```
+Result:
+```shell
+name       age  city
+-------  -----  ---------------
+Arsybai     23  Solo, Indonesia
+```
+
+You can request that the results of a query be returned in sorted order:
+```python
+data = db.select_row(table='people', col='*', order_by='age|asc')
+print(data)
+```
+_The order should be `asc` or `desc`_
+
+Result:
+```shell
+name       age  city
+-------  -----  ------------------
+Moepoi      21  Jakarta, Indonesia
+Arsybai     23  Solo, Indonesia
+Ataro       25  Bekasi, Indonesia
+```
+
+#### Updates
+You can update existing rows using the `update_row`.
+as example I want to set `Ataro` age to `26`:
+```python
+db.update_row(table='people', set_='age=26', where='name=Ataro')
+```
+Look at the new state of the data:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Ataro       26  Bekasi, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+
+#### Deletion
+Rows can be removed from a table using the `delete_row`:
+```python
+db.delete_row(table='people', where='name=Ataro')
+```
+
+Look at the new state of the data:
+```shell
+name       age  city
+-------  -----  ------------------
+Arsybai     23  Solo, Indonesia
+Moepoi      21  Jakarta, Indonesia
+```
+
+
```

