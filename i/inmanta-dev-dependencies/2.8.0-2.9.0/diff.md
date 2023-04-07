# Comparing `tmp/inmanta-dev-dependencies-2.8.0.tar.gz` & `tmp/inmanta-dev-dependencies-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-dev-dependencies-2.8.0.tar", max compression
+gzip compressed data, was "inmanta-dev-dependencies-2.9.0.tar", max compression
```

## Comparing `inmanta-dev-dependencies-2.8.0.tar` & `inmanta-dev-dependencies-2.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2795 2022-03-04 17:59:25.553422 inmanta-dev-dependencies-2.8.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-03-04 17:59:25.553422 inmanta-dev-dependencies-2.8.0/src/inmanta_dev_dependencies/__init__.py
--rw-r--r--   0        0        0     2191 2022-03-04 17:59:29.456716 inmanta-dev-dependencies-2.8.0/setup.py
--rw-r--r--   0        0        0     2601 2022-03-04 17:59:29.457006 inmanta-dev-dependencies-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2795 2022-03-11 17:59:21.541484 inmanta-dev-dependencies-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-03-11 17:59:21.542484 inmanta-dev-dependencies-2.9.0/src/inmanta_dev_dependencies/__init__.py
+-rw-r--r--   0        0        0     2191 2022-03-11 17:59:25.405669 inmanta-dev-dependencies-2.9.0/setup.py
+-rw-r--r--   0        0        0     2601 2022-03-11 17:59:25.405942 inmanta-dev-dependencies-2.9.0/PKG-INFO
```

### Comparing `inmanta-dev-dependencies-2.8.0/pyproject.toml` & `inmanta-dev-dependencies-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inmanta-dev-dependencies"
-version = "2.8.0"
+version = "2.9.0"
 description = "Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions."
 authors = ["Inmanta <code@inmanta.com>"]
 license = "Apache-2.0"
 packages = [
     { include = "inmanta_dev_dependencies", from = "src" },
 ]
 
@@ -35,15 +35,15 @@
 pytest-xdist = {version = "2.5.0", optional=true}
 pytest-sugar = {version = "0.9.4", optional=true}
 pytest-instafail = {version = "0.4.2", optional=true}
 inmanta-sphinx = {version = "1.5.0", optional = true}
 sphinx-argparse = {version = "0.3.1", optional = true}
 sphinx-autodoc-annotation = {version = "1.0-1", optional = true}
 sphinx-rtd-theme = {version = "1.0.0", optional = true}
-sphinx-tabs = {version = "3.2.0", optional = true}
+sphinx-tabs = {version = "3.3.0", optional = true}
 Sphinx = {version = "4.4.0", optional = true}
 sphinxcontrib-serializinghtml = {version = "1.1.5", optional = true}
 sphinxcontrib-redoc = {version = "1.6.0", optional = true}
 sphinx-click = {version = "3.1.0", optional = true}
 recommonmark = {version = "0.7.1", optional = true}
 
 # These are test and direct dependencies of certain extensions. We use carret version
```

### Comparing `inmanta-dev-dependencies-2.8.0/setup.py` & `inmanta-dev-dependencies-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,24 +44,24 @@
             'pytest-sugar==0.9.4',
             'pytest-instafail==0.4.2',
             'pytest-instafail==0.4.2'],
  'sphinx': ['inmanta-sphinx==1.5.0',
             'sphinx-argparse==0.3.1',
             'sphinx-autodoc-annotation==1.0-1',
             'sphinx-rtd-theme==1.0.0',
-            'sphinx-tabs==3.2.0',
+            'sphinx-tabs==3.3.0',
             'Sphinx==4.4.0',
             'sphinxcontrib-serializinghtml==1.1.5',
             'sphinxcontrib-redoc==1.6.0',
             'sphinx-click==3.1.0',
             'recommonmark==0.7.1']}
 
 setup_kwargs = {
     'name': 'inmanta-dev-dependencies',
-    'version': '2.8.0',
+    'version': '2.9.0',
     'description': 'Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions.',
     'long_description': None,
     'author': 'Inmanta',
     'author_email': 'code@inmanta.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `inmanta-dev-dependencies-2.8.0/PKG-INFO` & `inmanta-dev-dependencies-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-dev-dependencies
-Version: 2.8.0
+Version: 2.9.0
 Summary: Package collecting all common dev dependencies of inmanta modules and extensions to synchronize dependency versions.
 License: Apache-2.0
 Author: Inmanta
 Author-email: code@inmanta.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -42,12 +42,12 @@
 Requires-Dist: pytest-timeout (==2.1.0); extra == "async"
 Requires-Dist: pytest-xdist (==2.5.0); extra == "pytest"
 Requires-Dist: recommonmark (==0.7.1); extra == "sphinx"
 Requires-Dist: sphinx-argparse (==0.3.1); extra == "sphinx"
 Requires-Dist: sphinx-autodoc-annotation (==1.0-1); extra == "sphinx"
 Requires-Dist: sphinx-click (==3.1.0); extra == "sphinx"
 Requires-Dist: sphinx-rtd-theme (==1.0.0); extra == "sphinx"
-Requires-Dist: sphinx-tabs (==3.2.0); extra == "sphinx"
+Requires-Dist: sphinx-tabs (==3.3.0); extra == "sphinx"
 Requires-Dist: sphinxcontrib-redoc (==1.6.0); extra == "sphinx"
 Requires-Dist: sphinxcontrib-serializinghtml (==1.1.5); extra == "sphinx"
 Requires-Dist: tornado (>=6.1,<7.0); extra == "core" or extra == "extension"
 Requires-Dist: tox (==3.24.5); extra == "core" or extra == "extension"
```

