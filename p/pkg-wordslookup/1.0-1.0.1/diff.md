# Comparing `tmp/pkg_wordslookup-1.0.tar.gz` & `tmp/pkg_wordslookup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_wordslookup-1.0.tar", max compression
+gzip compressed data, was "pkg_wordslookup-1.0.1.tar", max compression
```

## Comparing `pkg_wordslookup-1.0.tar` & `pkg_wordslookup-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-04-07 10:28:35.111575 pkg_wordslookup-1.0/LICENSE
--rw-r--r--   0        0        0      720 2023-04-07 15:51:12.289630 pkg_wordslookup-1.0/pyproject.toml
--rw-r--r--   0        0        0      897 2023-04-07 10:28:35.127378 pkg_wordslookup-1.0/README.md
--rw-r--r--   0        0        0      119 2023-04-07 10:28:35.221396 pkg_wordslookup-1.0/src/pkg_wordslookup/__init__.py
--rw-r--r--   0        0        0      793 2023-04-07 15:46:07.114461 pkg_wordslookup-1.0/src/pkg_wordslookup/pkg_wordslookup.py
--rw-r--r--   0        0        0      876 2023-02-05 13:56:22.154220 pkg_wordslookup-1.0/src/pkg_wordslookup/zen.txt
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 pkg_wordslookup-1.0/setup.py
--rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 pkg_wordslookup-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-07 10:28:35.111575 pkg_wordslookup-1.0.1/LICENSE
+-rw-r--r--   0        0        0      722 2023-04-07 16:43:18.218485 pkg_wordslookup-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-04-07 10:28:35.127378 pkg_wordslookup-1.0.1/README.md
+-rw-r--r--   0        0        0      119 2023-04-07 10:28:35.221396 pkg_wordslookup-1.0.1/src/pkg_wordslookup/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-07 16:36:12.691696 pkg_wordslookup-1.0.1/src/pkg_wordslookup/pkg_wordslookup.py
+-rw-r--r--   0        0        0      876 2023-02-05 13:56:22.154220 pkg_wordslookup-1.0.1/src/pkg_wordslookup/zen.txt
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 pkg_wordslookup-1.0.1/setup.py
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 pkg_wordslookup-1.0.1/PKG-INFO
```

### Comparing `pkg_wordslookup-1.0/LICENSE` & `pkg_wordslookup-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pkg_wordslookup-1.0/pyproject.toml` & `pkg_wordslookup-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pkg_wordslookup"
-version = "1.0"
+version = "1.0.1"
 description = "This package will look the instances of a specific word provided as an input inside a file also provided as an input. The package will give the amount of times the word is in the file and it will print the line in which the word is placed"
 authors = ["Gabriel Coronel"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pkg_wordslookup-1.0/README.md` & `pkg_wordslookup-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pkg_wordslookup-1.0/src/pkg_wordslookup/pkg_wordslookup.py` & `pkg_wordslookup-1.0.1/src/pkg_wordslookup/pkg_wordslookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     for line in text:
         line = clean_text(line)
         if input_word in line:
             result = result + line
             n+=1
     summary = "\nThe word \"{}\" appeared {} times".format(input_word, n)
     result = result + summary
-    print(result)
+    print(summary)
     return result
```

### Comparing `pkg_wordslookup-1.0/src/pkg_wordslookup/zen.txt` & `pkg_wordslookup-1.0.1/src/pkg_wordslookup/zen.txt`

 * *Files identical despite different names*

### Comparing `pkg_wordslookup-1.0/setup.py` & `pkg_wordslookup-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['pkg_wordslookup']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pkg-wordslookup',
-    'version': '1.0',
+    'version': '1.0.1',
     'description': 'This package will look the instances of a specific word provided as an input inside a file also provided as an input. The package will give the amount of times the word is in the file and it will print the line in which the word is placed',
     'long_description': '# pkg_wordslookup\n\nThis package will look the instances of a specific word provided as an input inside a file also provided as an input. The package will give the amount of times the word is in the file and it will print the line in which the word is placed\n\n## Installation\n\n```bash\n$ pip install pkg_wordslookup\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`pkg_wordslookup` was created by Gabriel Coronel. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`pkg_wordslookup` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Gabriel Coronel',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pkg_wordslookup-1.0/PKG-INFO` & `pkg_wordslookup-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-wordslookup
-Version: 1.0
+Version: 1.0.1
 Summary: This package will look the instances of a specific word provided as an input inside a file also provided as an input. The package will give the amount of times the word is in the file and it will print the line in which the word is placed
 License: MIT
 Author: Gabriel Coronel
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

