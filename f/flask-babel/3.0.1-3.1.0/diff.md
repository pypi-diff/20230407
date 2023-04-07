# Comparing `tmp/flask_babel-3.0.1.tar.gz` & `tmp/flask_babel-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_babel-3.0.1.tar", max compression
+gzip compressed data, was "flask_babel-3.1.0.tar", max compression
```

## Comparing `flask_babel-3.0.1.tar` & `flask_babel-3.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1505 2023-01-29 23:09:01.040918 flask_babel-3.0.1/CHANGELOG
--rw-r--r--   0        0        0     1457 2023-01-29 23:09:01.040918 flask_babel-3.0.1/LICENSE
--rw-r--r--   0        0        0      572 2023-01-29 23:09:01.040918 flask_babel-3.0.1/README.md
--rw-r--r--   0        0        0    27101 2023-01-29 23:09:01.040918 flask_babel-3.0.1/flask_babel/__init__.py
--rw-r--r--   0        0        0     1669 2023-01-29 23:09:01.040918 flask_babel-3.0.1/flask_babel/speaklater.py
--rw-r--r--   0        0        0     1417 2023-01-29 23:09:01.040918 flask_babel-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 flask_babel-3.0.1/setup.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 flask_babel-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1850 2023-04-07 20:25:17.028155 flask_babel-3.1.0/CHANGELOG
+-rw-r--r--   0        0        0     1457 2023-04-07 20:25:17.028155 flask_babel-3.1.0/LICENSE
+-rw-r--r--   0        0        0      572 2023-04-07 20:25:17.028155 flask_babel-3.1.0/README.md
+-rw-r--r--   0        0        0    27151 2023-04-07 20:25:17.028155 flask_babel-3.1.0/flask_babel/__init__.py
+-rw-r--r--   0        0        0     1669 2023-04-07 20:25:17.028155 flask_babel-3.1.0/flask_babel/speaklater.py
+-rw-r--r--   0        0        0     1625 2023-04-07 20:25:17.028155 flask_babel-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 flask_babel-3.1.0/PKG-INFO
```

### Comparing `flask_babel-3.0.1/CHANGELOG` & `flask_babel-3.1.0/CHANGELOG`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.1.0
+------
+
+- Documentation and packaging improvements. (#226, #223, #218, #217, #215)
+- Don't return the default locale twice (#219)
+- Fix tests breaking against babel 12.2, which changed localized times to use non-breaking-spaces. Babel 12.2 or greater
+  is now required. (#222)
+- Relax version requirements for dependencies. (#227, #225)
+
 v3.0.0
 ------
 
 Major version bump as this version removes support for Python 3.5 and 3.6, along with multiple
 major breaking changes. Hope you've been following SemVer :)
 
 - Dropped support for end-of-life Python 3.5 and 3.6, added tests for 3.10 and 3.11.
```

### Comparing `flask_babel-3.0.1/LICENSE` & `flask_babel-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_babel-3.0.1/README.md` & `flask_babel-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flask_babel-3.0.1/flask_babel/__init__.py` & `flask_babel-3.1.0/flask_babel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,16 @@
                 locale_dir = os.path.join(dirname, folder, 'LC_MESSAGES')
                 if not os.path.isdir(locale_dir):
                     continue
 
                 if any(x.endswith('.mo') for x in os.listdir(locale_dir)):
                     result.append(Locale.parse(folder))
 
-        result.append(self.default_locale)
+        if self.default_locale not in result:
+            result.append(self.default_locale)
         return result
 
     @property
     def default_locale(self) -> Locale:
         """The default locale from the configuration as an instance of a
         `babel.Locale` object.
         """
```

### Comparing `flask_babel-3.0.1/flask_babel/speaklater.py` & `flask_babel-3.1.0/flask_babel/speaklater.py`

 * *Files identical despite different names*

### Comparing `flask_babel-3.0.1/pyproject.toml` & `flask_babel-3.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "flask-babel"
-version = "3.0.1"
-description = "Adds i18n/l10n support fo Flask applications."
+version = "3.1.0"
+description = "Adds i18n/l10n support for Flask applications."
 authors = ["Armin Ronacher"]
 maintainers = ["Tyler Kennedy <tk@tkte.ch>"]
 license = "BSD-3-Clause"
 readme = "README.md"
+repository = "https://github.com/python-babel/flask-babel"
+documentation = "https://python-babel.github.io/flask-babel/"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3.7',
@@ -19,25 +21,25 @@
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: Implementation :: CPython',
     'Programming Language :: Python :: Implementation :: PyPy',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development :: Libraries :: Python Modules'
 ]
 include = [
-    "CHANGELOG",
-    "README.md",
-    "LICENSE"
+    { path = "CHANGELOG", format = "sdist" },
+    { path = "README.md", format = "sdist" },
+    { path = "LICENSE", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pytz = "^2022.7"
-Flask = "^2.0.0"
-Babel = "^2.11.0"
-Jinja2 = "^3.1.2"
+pytz = ">=2022.7"
+Flask = ">=2.0"
+Babel = ">=2.12"
+Jinja2 = ">=3.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 bumpversion = "^0.6.0"
 ghp-import = "^2.1.0"
 Sphinx = "^5.3.0"
```

### Comparing `flask_babel-3.0.1/PKG-INFO` & `flask_babel-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: flask-babel
-Version: 3.0.1
-Summary: Adds i18n/l10n support fo Flask applications.
+Version: 3.1.0
+Summary: Adds i18n/l10n support for Flask applications.
+Home-page: https://github.com/python-babel/flask-babel
 License: BSD-3-Clause
 Author: Armin Ronacher
 Maintainer: Tyler Kennedy
 Maintainer-email: tk@tkte.ch
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -23,18 +24,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Babel (>=2.11.0,<3.0.0)
-Requires-Dist: Flask (>=2.0.0,<3.0.0)
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pytz (>=2022.7,<2023.0)
+Requires-Dist: Babel (>=2.12)
+Requires-Dist: Flask (>=2.0)
+Requires-Dist: Jinja2 (>=3.1)
+Requires-Dist: pytz (>=2022.7)
+Project-URL: Documentation, https://python-babel.github.io/flask-babel/
+Project-URL: Repository, https://github.com/python-babel/flask-babel
 Description-Content-Type: text/markdown
 
 # Flask Babel
 
 ![Tests](https://github.com/python-babel/flask-babel/workflows/Tests/badge.svg?branch=master)
 [![PyPI](https://img.shields.io/pypi/v/flask-babel.svg?maxAge=2592000)](https://pypi.python.org/pypi/Flask-Babel)
```

