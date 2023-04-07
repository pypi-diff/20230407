# Comparing `tmp/abraia-0.9.3.tar.gz` & `tmp/abraia-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abraia-0.9.3.tar", last modified: Sat Jan 22 18:46:10 2022, max compression
+gzip compressed data, was "abraia-0.9.4.tar", last modified: Wed Mar  2 20:04:53 2022, max compression
```

## Comparing `abraia-0.9.3.tar` & `abraia-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 18:46:10.000000 abraia-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-01-22 18:46:10.000000 abraia-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    13798 2022-01-22 18:46:10.000000 abraia-0.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia/
--rw-r--r--   0 runner    (1001) docker     (121)     7862 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/abraia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/multiple.py
--rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/deep.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    10895 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/hsi.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-01-22 18:45:20.000000 abraia-0.9.3/abraia/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11131 2022-01-22 18:45:20.000000 abraia-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 18:46:10.000000 abraia-0.9.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)       81 2022-01-22 18:45:20.000000 abraia-0.9.3/scripts/abraia.bat
--rwxr-xr-x   0 runner    (1001) docker     (121)     6905 2022-01-22 18:45:20.000000 abraia-0.9.3/scripts/abraia
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-01-22 18:45:20.000000 abraia-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13798 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-22 18:46:10.000000 abraia-0.9.3/abraia.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 20:04:53.625042 abraia-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-03-02 20:03:56.000000 abraia-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    13832 2022-03-02 20:04:53.625042 abraia-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11165 2022-03-02 20:03:56.000000 abraia-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 20:04:53.621042 abraia-0.9.4/abraia/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7862 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/abraia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5071 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/deep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10895 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/hsi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-03-02 20:03:56.000000 abraia-0.9.4/abraia/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 20:04:53.625042 abraia-0.9.4/abraia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13832 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-02 20:04:53.000000 abraia-0.9.4/abraia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 20:04:53.625042 abraia-0.9.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7032 2022-03-02 20:03:56.000000 abraia-0.9.4/scripts/abraia
+-rwxr-xr-x   0 runner    (1001) docker     (121)       81 2022-03-02 20:03:56.000000 abraia-0.9.4/scripts/abraia.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-02 20:04:53.625042 abraia-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2022-03-02 20:03:56.000000 abraia-0.9.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `abraia-0.9.3/PKG-INFO` & `abraia-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abraia
-Version: 0.9.3
+Version: 0.9.4
 Summary: Abraia Python SDK
 Home-page: https://github.com/abraia/abraia-python
 Author: Jorge Rodriguez Araujo
 Author-email: jorge@abraiasoftware.com
 License: MIT
 Description: [![Build Status](https://github.com/abraia/abraia-multiple/actions/workflows/build.yml/badge.svg)](https://github.com/abraia/abraia-multiple/actions/workflows/build.yml)
         [![Python Package](https://img.shields.io/pypi/v/abraia.svg)](https://pypi.org/project/abraia/)
@@ -116,15 +116,15 @@
         
         img = multiple.load_image('usain.jpg')
         multiple.save_image('usain.png', img)
         
         plot_image(img, 'Image')
         ```
         
-        ![plot image](https://store.abraia.me/multiple/notebooks/bolt.png)
+        ![plot image](https://github.com/abraia/abraia-multiple/raw/master/images/bolt.png)
         
         Read the image metadata and save it as a JSON file.
         
         ```python
         import json
         
         metadata = multiple.load_metadata('usain.jpg')
@@ -157,15 +157,15 @@
         folder = 'test/'
         multiple.upload_file('images/usain-bolt.jpeg', folder)
         files, folders = multiple.list_files(folder)
         
         pd.DataFrame(files)
         ```
         
-        ![files](https://store.abraia.me/multiple/notebooks/files.png)
+        ![files](https://github.com/abraia/abraia-multiple/raw/master/images/files.png)
         
         To list the root folder just omit the folder value.
         
         ### Download and remove files
         
         You can download or remove an stored file just specifying its `path`.
```

### Comparing `abraia-0.9.3/abraia/abraia.py` & `abraia-0.9.4/abraia/abraia.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/abraia/multiple.py` & `abraia-0.9.4/abraia/multiple.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/abraia/deep.py` & `abraia-0.9.4/abraia/deep.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/abraia/plot.py` & `abraia-0.9.4/abraia/plot.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/abraia/hsi.py` & `abraia-0.9.4/abraia/hsi.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/abraia/config.py` & `abraia-0.9.4/abraia/config.py`

 * *Files identical despite different names*

### Comparing `abraia-0.9.3/README.md` & `abraia-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 img = multiple.load_image('usain.jpg')
 multiple.save_image('usain.png', img)
 
 plot_image(img, 'Image')
 ```
 
-![plot image](https://store.abraia.me/multiple/notebooks/bolt.png)
+![plot image](https://github.com/abraia/abraia-multiple/raw/master/images/bolt.png)
 
 Read the image metadata and save it as a JSON file.
 
 ```python
 import json
 
 metadata = multiple.load_metadata('usain.jpg')
@@ -149,15 +149,15 @@
 folder = 'test/'
 multiple.upload_file('images/usain-bolt.jpeg', folder)
 files, folders = multiple.list_files(folder)
 
 pd.DataFrame(files)
 ```
 
-![files](https://store.abraia.me/multiple/notebooks/files.png)
+![files](https://github.com/abraia/abraia-multiple/raw/master/images/files.png)
 
 To list the root folder just omit the folder value.
 
 ### Download and remove files
 
 You can download or remove an stored file just specifying its `path`.
```

### Comparing `abraia-0.9.3/scripts/abraia` & `abraia-0.9.4/scripts/abraia`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if isinstance(src, str) and src.startswith('http'):
         return [src]
     src = os.path.join(src, '**/*') if os.path.isdir(src) else src
     return glob(src, recursive=True)
 
 
 @click.group('abraia')
-@click.version_option('0.9.3')
+@click.version_option('0.9.4')
 def cli():
     """Abraia CLI tool"""
     pass
 
 
 @cli.command()
 def configure():
@@ -60,15 +60,15 @@
     except:
         pass
 
 
 @cli.command()
 def info():
     """Show user account information"""
-    click.echo('abraia, version 0.9.3\n')
+    click.echo('abraia, version 0.9.4\n')
     try:
         user = abraia.load_user()
         output = 'Name: {}\n'.format(user.get('name'))
         output += 'Email: {}\n'.format(user.get('email'))
         output += 'Credits: {}'.format(user.get('credits'))
         click.echo(output)
     except APIError as error:
@@ -155,16 +155,15 @@
 
 
 @cli.command()
 @click.argument('path', required=False)
 def list(path):
     """List the files in abraia"""
     try:
-        path = path if path else ''
-        files, folders = abraia.list_files(path)
+        files, folders = abraia.list_files(path or '')
         output = '\n'.join(['{:>28}  {}/'.format('', click.style(f['name'], fg='blue', bold=True)) for f in folders]) + '\n'
         output += '\n'.join(['{}  {:>7}  {}'.format(f['date'], f['size'], f['name']) for f in files])
         output += '\ntotal {}'.format(len(files))
         click.echo(output)
     except APIError as error:
         echo_error(error)
 
@@ -193,19 +192,23 @@
                 click.echo(abraia.download_file(path, dest))
     except APIError as error:
         echo_error(error)
 
 
 @cli.command()
 @click.argument('path')
-@click.confirmation_option(prompt='Are you sure you want to remove the file?')
 def remove(path):
     """Remove a file from abraia"""
     try:
-        click.echo(abraia.remove_file(path))
+        files = abraia.list_files(path)[0]
+        for file in files:
+            click.echo(file['path'])
+        if files and click.confirm('Are you sure you want to remove the files?'):
+            for file in files:
+                click.echo(abraia.remove_file(file['path']))
     except APIError as error:
         echo_error(error)
 
 
 if __name__ == '__main__':
     if not abraia.userid:
         configure()
```

### Comparing `abraia-0.9.3/setup.py` & `abraia-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with pathlib.Path('requirements.txt').open() as requirements_txt:
     install_requires = [str(requirement) for requirement
         in pkg_resources.parse_requirements(requirements_txt)]
 
 setup(
     name='abraia',
-    version='0.9.3',
+    version='0.9.4',
     description='Abraia Python SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/abraia/abraia-python',
     author='Jorge Rodriguez Araujo',
     author_email='jorge@abraiasoftware.com',
     license='MIT',
```

### Comparing `abraia-0.9.3/abraia.egg-info/PKG-INFO` & `abraia-0.9.4/abraia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abraia
-Version: 0.9.3
+Version: 0.9.4
 Summary: Abraia Python SDK
 Home-page: https://github.com/abraia/abraia-python
 Author: Jorge Rodriguez Araujo
 Author-email: jorge@abraiasoftware.com
 License: MIT
 Description: [![Build Status](https://github.com/abraia/abraia-multiple/actions/workflows/build.yml/badge.svg)](https://github.com/abraia/abraia-multiple/actions/workflows/build.yml)
         [![Python Package](https://img.shields.io/pypi/v/abraia.svg)](https://pypi.org/project/abraia/)
@@ -116,15 +116,15 @@
         
         img = multiple.load_image('usain.jpg')
         multiple.save_image('usain.png', img)
         
         plot_image(img, 'Image')
         ```
         
-        ![plot image](https://store.abraia.me/multiple/notebooks/bolt.png)
+        ![plot image](https://github.com/abraia/abraia-multiple/raw/master/images/bolt.png)
         
         Read the image metadata and save it as a JSON file.
         
         ```python
         import json
         
         metadata = multiple.load_metadata('usain.jpg')
@@ -157,15 +157,15 @@
         folder = 'test/'
         multiple.upload_file('images/usain-bolt.jpeg', folder)
         files, folders = multiple.list_files(folder)
         
         pd.DataFrame(files)
         ```
         
-        ![files](https://store.abraia.me/multiple/notebooks/files.png)
+        ![files](https://github.com/abraia/abraia-multiple/raw/master/images/files.png)
         
         To list the root folder just omit the folder value.
         
         ### Download and remove files
         
         You can download or remove an stored file just specifying its `path`.
```

