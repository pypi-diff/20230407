# Comparing `tmp/poetry_dotenv-0.3.0.tar.gz` & `tmp/poetry_dotenv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_dotenv-0.3.0.tar", max compression
+gzip compressed data, was "poetry_dotenv-0.4.0.tar", max compression
```

## Comparing `poetry_dotenv-0.3.0.tar` & `poetry_dotenv-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1077 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/LICENSE
--rw-r--r--   0        0        0     7871 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/README.md
--rw-r--r--   0        0        0     6153 2023-01-29 19:23:20.101057 poetry_dotenv-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      657 2023-01-29 19:23:19.997056 poetry_dotenv-0.3.0/src/poetry_dotenv/__init__.py
--rw-r--r--   0        0        0      314 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5396 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6010 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1445 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3402 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2023-01-29 19:21:45.860258 poetry_dotenv-0.3.0/src/poetry_dotenv/py.typed
--rw-r--r--   0        0        0     9203 1970-01-01 00:00:00.000000 poetry_dotenv-0.3.0/setup.py
--rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 poetry_dotenv-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-07 11:55:02.709681 poetry_dotenv-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8841 2023-04-07 17:04:27.407659 poetry_dotenv-0.4.0/README.md
+-rw-r--r--   0        0        0     6154 2023-04-07 11:54:29.826053 poetry_dotenv-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-04-07 17:06:22.084517 poetry_dotenv-0.4.0/src/poetry_dotenv/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-07 17:05:35.519510 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0      556 2023-04-07 17:08:29.001157 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8429 2023-04-07 17:08:29.004080 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/__pycache__/core.cpython-311.pyc
+-rw-r--r--   0        0        0    11292 2023-04-07 17:08:29.007303 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0        0        0     3068 2023-04-07 17:08:29.011699 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/__pycache__/variables.cpython-311.pyc
+-rw-r--r--   0        0        0     5409 2023-04-07 17:05:35.560855 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6010 2023-04-07 11:53:27.509693 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1445 2023-04-07 11:53:27.510745 poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     3674 2023-04-07 17:11:56.284645 poetry_dotenv-0.4.0/src/poetry_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-07 11:53:27.512773 poetry_dotenv-0.4.0/src/poetry_dotenv/py.typed
+-rw-r--r--   0        0        0    10878 1970-01-01 00:00:00.000000 poetry_dotenv-0.4.0/PKG-INFO
```

### Comparing `poetry_dotenv-0.3.0/LICENSE` & `poetry_dotenv-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_dotenv-0.3.0/README.md` & `poetry_dotenv-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+> ⚠️ __Warning__
+>
+> This package has been deprecated and is no longer maintained, `poetry-dotenv` has moved to [`poetry-plugin-dotenv`](https://pypi.org/project/poetry-plugin-dotenv)
+
+
 <div align="center">
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="logo" src="https://github.com/volopivoshenko/poetry-dotenv/blob/main/docs/static/assets/logo.svg?raw=True" height=200>
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="logo" src="https://github.com/volopivoshenko/poetry-plugin-dotenv/blob/main/docs/static/assets/logo.svg?raw=True" height=200>
     </a>
 </div>
 
 <p align="center">
     <a href="https://opensource.org/licenses/MIT">
-        <img alt="license" src="https://img.shields.io/pypi/l/poetry-dotenv?logo=opensourceinitiative">
+        <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-dotenv?logo=python">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-plugin-dotenv?logo=python">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="pypi" src="https://img.shields.io/pypi/v/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="pypi" src="https://img.shields.io/pypi/v/poetry-plugin-dotenv?logo=pypi">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/releases">
-        <img alt="release" src="https://img.shields.io/github/v/release/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/releases">
+        <img alt="release" src="https://img.shields.io/github/v/release/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
     <a href="https://numpydoc.readthedocs.io/en/latest/format.html">
         <img alt="numpydoc" src="https://img.shields.io/badge/docstrings-numpy-1f425f.svg?logo=numpy">
     </a>
 </p>
 
 <p align="center">
@@ -40,97 +45,107 @@
     </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/dependabot">
         <img alt="dependabot" src="https://img.shields.io/badge/dependabot-enable-success?logo=Dependabot">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/ci.yaml">
-        <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/ci.yaml?label=CI&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/ci.yaml">
+        <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/ci.yaml?label=CI&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/cd.yaml">
-        <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/cd.yaml?label=CD&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/cd.yaml">
+        <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/cd.yaml?label=CD&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/codeql.yaml">
-        <img alt="CodeQL" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/codeql.yaml?label=CodeQL&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/codeql.yaml">
+        <img alt="CodeQL" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/codeql.yaml?label=CodeQL&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/dependency-review.yaml">
-        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/dependency-review.yaml">
+        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-plugin-dotenv?logo=pypi">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://codecov.io/gh/volopivoshenko/poetry-dotenv">
-        <img alt="coverage" src="https://img.shields.io/codecov/c/gh/volopivoshenko/poetry-dotenv?logo=codecov&token=yyck08xfTN"/>
+    <a href="https://codecov.io/gh/volopivoshenko/poetry-plugin-dotenv">
+        <img alt="coverage" src="https://img.shields.io/codecov/c/gh/volopivoshenko/poetry-plugin-dotenv?logo=codecov&token=yyck08xfTN"/>
     </a>
-    <a href="https://codeclimate.com/github/volopivoshenko/poetry-dotenv/maintainability">
-        <img alt="codeclimate" src="https://img.shields.io/codeclimate/maintainability/volopivoshenko/poetry-dotenv?logo=codeclimate">
+    <a href="https://codeclimate.com/github/volopivoshenko/poetry-plugin-dotenv/maintainability">
+        <img alt="codeclimate" src="https://img.shields.io/codeclimate/maintainability/volopivoshenko/poetry-plugin-dotenv?logo=codeclimate">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-plugin-dotenv?logo=pypi">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/">
-        <img alt="stars" src="https://img.shields.io/github/stars/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/">
+        <img alt="stars" src="https://img.shields.io/github/stars/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/issues">
+        <img alt="issues" src="https://img.shields.io/github/issues/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues-closed/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/issues">
+        <img alt="issues" src="https://img.shields.io/github/issues-closed/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/pulls">
+        <img alt="pr" src="https://img.shields.io/github/issues-pr/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/pulls">
+        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/graphs/contributors">
-        <img alt="contributors" src="https://img.shields.io/github/contributors/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/graphs/contributors">
+        <img alt="contributors" src="https://img.shields.io/github/contributors/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/commits/main">
-        <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/commits/main">
+        <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
+    <!-- <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
+    </a> -->
+    <a href="https://stand-with-ukraine.pp.ua/">
+        <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
+    </a>
+    <a href="https://stand-with-ukraine.pp.ua">
+        <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
 
+
+
 - [🔮 Overview](#-overview)
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
-`poetry-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
+`poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
 **This plugin doesn't have any dependencies, but therefore it also supports features that `python-dotenv` supports (e.g. templates, interpolating variables using `POSIX` variable expansions etc).**
 
 # ⚙️ Installation
 
 ```bash
-poetry self add poetry-dotenv
+poetry self add poetry-plugin-dotenv
 ```
 
 # 👩🏻‍💻 Usage
 
 By default, plugin will load the `.env` file from the current working directory or "higher directories".
 
 To prevent ``poetry`` from loading the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment variable.
 
 If your dotenv file is located in a different path or has a different name you may set the ``POETRY_DOTENV_LOCATION`` environment variable.
 
+<img alt="logo" src="https://github.com/volopivoshenko/poetry-plugin-dotenv/blob/main/docs/static/assets/demo.gif?raw=True">
+
 ```dotenv
 # .env
 DB__HOST=localhost
 DB__DBNAME=prod
 DB__USER=admin
 DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
+> â ï¸ __Warning__ > > This package has been deprecated and is no longer
+maintained, `poetry-dotenv` has moved to [`poetry-plugin-dotenv`](https://
+pypi.org/project/poetry-plugin-dotenv)
                                     [logo]
                 [license] [python] [pypi] [release] [numpydoc]
               [black] [isort] [wemake] [mypy] [semantic_release]
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
                  [coverage] [codeclimate] [downloads] [stars]
               [issues] [issues] [pr] [pr] [contributors] [commit]
-                                [buymeacoffee]
+                     [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
-[ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-dotenv` - is the
-plugin that automatically loads environment variables from a dotenv file into
-the environment before `poetry` commands are run. **This plugin doesn't have
-any dependencies, but therefore it also supports features that `python-dotenv`
-supports (e.g. templates, interpolating variables using `POSIX` variable
-expansions etc).** # âï¸ Installation ```bash poetry self add poetry-dotenv
-``` # ð©ð»âð» Usage By default, plugin will load the `.env` file from
-the current working directory or "higher directories". To prevent ``poetry``
-from loading the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment
-variable. If your dotenv file is located in a different path or has a different
-name you may set the ``POETRY_DOTENV_LOCATION`` environment variable. ```dotenv
-# .env DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
+[ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
+the plugin that automatically loads environment variables from a dotenv file
+into the environment before `poetry` commands are run. **This plugin doesn't
+have any dependencies, but therefore it also supports features that `python-
+dotenv` supports (e.g. templates, interpolating variables using `POSIX`
+variable expansions etc).** # âï¸ Installation ```bash poetry self add
+poetry-plugin-dotenv ``` # ð©ð»âð» Usage By default, plugin will load
+the `.env` file from the current working directory or "higher directories". To
+prevent ``poetry`` from loading the dotenv file, set the
+``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
+located in a different path or has a different name you may set the
+``POETRY_DOTENV_LOCATION`` environment variable. [logo] ```dotenv # .env
+DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ``` ```dotenv # .env.dev DB__HOST=localhost DB__DBNAME=dev DB__USER=root
 DB__PASSWORD=root DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@$
 {DB__HOST}/${DB__DBNAME} ``` ```python # main.py import os if __name__ ==
 "__main__": try: print(f"Host: {os.environ['DB__HOST']!r}") print(f"Name:
 {os.environ['DB__DBNAME']!r}") print(f"Username: {os.environ['DB__USER']!r}")
 print(f"Password: {os.environ['DB__PASSWORD']!r}") print(f"Engine: {os.environ
```

### Comparing `poetry_dotenv-0.3.0/pyproject.toml` & `poetry_dotenv-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-dotenv"
-version = "0.3.0"
+version = "0.4.0"
 description = "poetry-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
     "python",
     "pypi",
@@ -44,50 +44,50 @@
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/volopivoshenko/poetry-dotenv/issues"
 "Releases" = "https://github.com/volopivoshenko/poetry-dotenv/releases"
 "Say Thanks!" = "https://www.buymeacoffee.com/volopivoshenko"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-poetry = "^1.3.2"
+python = ">=3.8.1,<4.0"
+poetry = "^1.4.2"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.0.1"
-poethepoet = "^0.18.1"
-ipython = "^8.9.0"
-ipdb = "^0.13.11"
-nitpick = "^0.32.0"
+pre-commit = "^3.2.1"
+poethepoet = "^0.19.0"
+ipython = "^8.11.0"
+ipdb = "^0.13.13"
+nitpick = "^0.33.1"
 
 [tool.poetry.group.formatters.dependencies]
 isort = "^5.12.0"
-black = "^22.12.0"
+black = "^23.3.0"
 pyupgrade = "^3.3.1"
 yesqa = "^1.4.0"
 
 [tool.poetry.group.linters.dependencies]
-mypy = "^0.991"
+mypy = "^1.1.1"
 wemake-python-styleguide = "^0.17.0"
 pyproject-flake8 = "^3.9.2"
-flake8-pytest-style = "^1.6.0"
+flake8-pytest-style = "^1.7.2"
 deptry = "^0.8.0"
-codespell = "^2.2.2"
+codespell = "^2.2.4"
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.2.1"
-xdoctest = "^1.1.0"
+pytest = "^7.2.2"
+xdoctest = "^1.1.1"
 pytest-lazy-fixture = "^0.6.3"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 pytest-sugar = "^0.9.6"
-coverage = { version = "^7.1.0", extras = ["toml"] }
-sh = "^1.14.3"
+coverage = { version = "^7.2.2", extras = ["toml"] }
+sh = "^2.0.3"
 
 [tool.poetry.group.ci.dependencies]
-python-semantic-release = "^7.33.0"
+python-semantic-release = "^7.33.2"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-dotenv = "poetry_dotenv.plugin:DotenvPlugin"
 
 [tool.semantic_release]
 branch = "main"
 changelog_file = "CHANGELOG.md"
@@ -141,31 +141,24 @@
 # S101 - asserts are necessary for the tests
 # WPS118 - long names for the tests contain description of the tests
 # WPS226 - overuse of the literals is a common thing in the tests
 # WPS342 - raw strings are necessary for the parsers' tests
 # WPS430 - nested functions are necessary for the parameterized pytest fixtures
 # WPS204, WPS440 - overuse of the expression is a common thing in the tests
 # WPS442 - pytest fixtures don't violate "variables from outer scopes"
-extend-ignore = [
-    "NIP",
-    "D202",
-    "DAR",
-    "WPS305",
-    "WPS306",
-    "WPS472",
-]
+extend-ignore = ["NIP", "D202", "DAR", "WPS305", "WPS306", "WPS472"]
 # NIP - no need to use nitpick plugin
 # D202 - code is hard to read without a blank line after a docstring
 # DAR - there is no sense to put all sections in docstring
 # WPS305 - f-strings are more readable than .format()
 # WPS306 - no need to inherit from object
 # WPS472 - unpacking for the single variable is more readable than indexing
 
 [tool.codespell]
-skip = "tests,.git,.mypy_cache,.pytest_cache,.idea,.vscode"
+skip = "tests,pyproject.toml,poetry.lock,.git,.mypy_cache,.pytest_cache,.idea,.vscode"
 
 [tool.deptry]
 ignore_transitive = ["cleo", "poetry_dotenv"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["src", "tests"]
```

### Comparing `poetry_dotenv-0.3.0/src/poetry_dotenv/__init__.py` & `poetry_dotenv-0.4.0/src/poetry_dotenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-dotenv"
 __summary__ = "poetry-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
-__uri__ = "https://github.com/volopivoshenko/poetry-dotenv"
+__uri__ = "https://github.com/volopivoshenko/poetry-plugin-dotenv"
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/core.py` & `poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
                     yield mapping.key, mapping.value  # type: ignore
 
     def set_as_environment_variables(self) -> bool:
         """Load current dotenv as a system environment variable."""
 
         if self.dict():
             for key, value in self.dict().items():
-
                 if key in os.environ and not self.override:
                     continue
 
                 if value:
                     os.environ[key] = value
 
             return True
@@ -95,15 +94,15 @@
     values: typing.Iterable[tuple[str, str]],
     override: bool,
 ) -> typing.OrderedDict[str, str]:
     """Resolve dotenv variables."""
 
     new_values: typing.OrderedDict[str, str] = OrderedDict()
 
-    for (name, value) in values:
+    for name, value in values:
         if value is None:
             result = None  # pragma: nocover
 
         else:
             atoms = variables.parse(value)
             env: typing.OrderedDict[str, str] = OrderedDict()
 
@@ -113,15 +112,15 @@
 
             else:
                 env.update(new_values)
                 env.update(os.environ)
 
             result = "".join(atom.resolve(env) for atom in atoms)
 
-        new_values[name] = result
+        new_values[name] = result  # type: ignore
 
     return new_values
 
 
 def walk_to_root(path: str) -> typing.Iterator[str]:
     """Yield directories starting from the given directory up to the root."""
```

### Comparing `poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/parsers.py` & `poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_dotenv-0.3.0/src/poetry_dotenv/dotenv/variables.py` & `poetry_dotenv-0.4.0/src/poetry_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_dotenv-0.3.0/src/poetry_dotenv/plugin.py` & `poetry_dotenv-0.4.0/src/poetry_dotenv/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Module that contains the core functionality of the plugin."""
 
+from __future__ import annotations
+
 import os
 import enum
 
 from cleo.events.console_command_event import ConsoleCommandEvent
 from cleo.events.console_events import COMMAND
 from poetry.console.application import Application
 from poetry.console.commands.env_command import EnvCommand
@@ -11,18 +13,18 @@
 
 from poetry_dotenv import dotenv
 
 
 class Verbosity(enum.Enum):  # pragma: no cover
     """Levels of verbosity."""
 
-    info: str = "<info>{0!s}</info>"
-    debug: str = "<debug>{0!s}</debug>"
-    warning: str = "<warning>{0!s}</warning>"
-    error: str = "<error>{0!s}</error>"
+    info = "<info>{0!s}</info>"
+    debug = "<debug>{0!s}</debug>"
+    warning = "<warning>{0!s}</warning>"
+    error = "<error>{0!s}</error>"
 
 
 class Logger:  # pragma: no cover
     """Logger of the ``poetry`` events.
 
     Because this logger is used for the plugin that are running before the main command,
     all the messages will be logged only in the debug mode.
@@ -72,24 +74,24 @@
     If your dotenv file is located in a different path or has a different name you may set
     the ``POETRY_DOTENV_LOCATION`` environment variable.
     """
 
     def activate(self, application: Application) -> None:  # pragma: no cover
         """Activate the plugin."""
 
-        application.event_dispatcher.add_listener(
-            event_name=COMMAND,
-            listener=self.load,
-        )
+        application.event_dispatcher.add_listener(COMMAND, listener=self.load)  # type: ignore
 
     def load(self, event: ConsoleCommandEvent, *args, **kwargs) -> None:
         """Load a dotenv file."""
 
         logger = Logger(event)
 
+        deprecation_msg = """This package has been deprecated and is no longer maintained, `poetry-dotenv` has moved to `poetry-plugin-dotenv` (https://pypi.org/project/poetry-plugin-dotenv)"""  # noqa: E501
+        event.io.write_line(Verbosity.warning.value.format(deprecation_msg))
+
         dont_load_dotenv = os.getenv("POETRY_DONT_LOAD_DOTENV")
         dotenv_location = os.getenv("POETRY_DOTENV_LOCATION")
         is_env_command = isinstance(event.command, EnvCommand)
 
         if is_env_command and dont_load_dotenv:
             logger.warning("Not loading environment variables.")
```

### Comparing `poetry_dotenv-0.3.0/PKG-INFO` & `poetry_dotenv-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 Metadata-Version: 2.1
 Name: poetry-dotenv
-Version: 0.3.0
+Version: 0.4.0
 Summary: poetry-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/volopivoshenko/poetry-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
 Maintainer-email: volodymyr.pivoshenko@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: poetry (>=1.3.2,<2.0.0)
+Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Project-URL: Documentation, https://github.com/volopivoshenko/poetry-dotenv
 Project-URL: Issues, https://github.com/volopivoshenko/poetry-dotenv/issues
 Project-URL: Repository, https://github.com/volopivoshenko/poetry-dotenv
 Project-URL: Releases, https://github.com/volopivoshenko/poetry-dotenv/releases
 Project-URL: Say Thanks!, https://www.buymeacoffee.com/volopivoshenko
 Description-Content-Type: text/markdown
 
+> ⚠️ __Warning__
+>
+> This package has been deprecated and is no longer maintained, `poetry-dotenv` has moved to [`poetry-plugin-dotenv`](https://pypi.org/project/poetry-plugin-dotenv)
+
+
 <div align="center">
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="logo" src="https://github.com/volopivoshenko/poetry-dotenv/blob/main/docs/static/assets/logo.svg?raw=True" height=200>
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="logo" src="https://github.com/volopivoshenko/poetry-plugin-dotenv/blob/main/docs/static/assets/logo.svg?raw=True" height=200>
     </a>
 </div>
 
 <p align="center">
     <a href="https://opensource.org/licenses/MIT">
-        <img alt="license" src="https://img.shields.io/pypi/l/poetry-dotenv?logo=opensourceinitiative">
+        <img alt="license" src="https://img.shields.io/pypi/l/poetry-plugin-dotenv?logo=opensourceinitiative">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-dotenv?logo=python">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="python" src="https://img.shields.io/pypi/pyversions/poetry-plugin-dotenv?logo=python">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="pypi" src="https://img.shields.io/pypi/v/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="pypi" src="https://img.shields.io/pypi/v/poetry-plugin-dotenv?logo=pypi">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/releases">
-        <img alt="release" src="https://img.shields.io/github/v/release/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/releases">
+        <img alt="release" src="https://img.shields.io/github/v/release/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
     <a href="https://numpydoc.readthedocs.io/en/latest/format.html">
         <img alt="numpydoc" src="https://img.shields.io/badge/docstrings-numpy-1f425f.svg?logo=numpy">
     </a>
 </p>
 
 <p align="center">
@@ -81,97 +85,107 @@
     </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/dependabot">
         <img alt="dependabot" src="https://img.shields.io/badge/dependabot-enable-success?logo=Dependabot">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/ci.yaml">
-        <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/ci.yaml?label=CI&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/ci.yaml">
+        <img alt="CI" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/ci.yaml?label=CI&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/cd.yaml">
-        <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/cd.yaml?label=CD&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/cd.yaml">
+        <img alt="CD" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/cd.yaml?label=CD&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/codeql.yaml">
-        <img alt="CodeQL" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/codeql.yaml?label=CodeQL&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/codeql.yaml">
+        <img alt="CodeQL" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/codeql.yaml?label=CodeQL&logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/actions/workflows/dependency-review.yaml">
-        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/actions/workflows/dependency-review.yaml">
+        <img alt="Dependency Review" src="https://img.shields.io/github/actions/workflow/status/volopivoshenko/poetry-plugin-dotenv/dependency-review.yaml?label=Dependency%20Review&logo=github">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="wheel" src="https://img.shields.io/pypi/wheel/poetry-plugin-dotenv?logo=pypi">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://codecov.io/gh/volopivoshenko/poetry-dotenv">
-        <img alt="coverage" src="https://img.shields.io/codecov/c/gh/volopivoshenko/poetry-dotenv?logo=codecov&token=yyck08xfTN"/>
+    <a href="https://codecov.io/gh/volopivoshenko/poetry-plugin-dotenv">
+        <img alt="coverage" src="https://img.shields.io/codecov/c/gh/volopivoshenko/poetry-plugin-dotenv?logo=codecov&token=yyck08xfTN"/>
     </a>
-    <a href="https://codeclimate.com/github/volopivoshenko/poetry-dotenv/maintainability">
-        <img alt="codeclimate" src="https://img.shields.io/codeclimate/maintainability/volopivoshenko/poetry-dotenv?logo=codeclimate">
+    <a href="https://codeclimate.com/github/volopivoshenko/poetry-plugin-dotenv/maintainability">
+        <img alt="codeclimate" src="https://img.shields.io/codeclimate/maintainability/volopivoshenko/poetry-plugin-dotenv?logo=codeclimate">
     </a>
-    <a href="https://pypi.org/project/poetry-dotenv">
-        <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-dotenv?logo=pypi">
+    <a href="https://pypi.org/project/poetry-plugin-dotenv">
+        <img alt="downloads" src="https://img.shields.io/pypi/dm/poetry-plugin-dotenv?logo=pypi">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/">
-        <img alt="stars" src="https://img.shields.io/github/stars/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/">
+        <img alt="stars" src="https://img.shields.io/github/stars/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/issues">
+        <img alt="issues" src="https://img.shields.io/github/issues/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/issues">
-        <img alt="issues" src="https://img.shields.io/github/issues-closed/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/issues">
+        <img alt="issues" src="https://img.shields.io/github/issues-closed/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/pulls">
+        <img alt="pr" src="https://img.shields.io/github/issues-pr/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/pulls">
-        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/pulls">
+        <img alt="pr" src="https://img.shields.io/github/issues-pr-closed/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/graphs/contributors">
-        <img alt="contributors" src="https://img.shields.io/github/contributors/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/graphs/contributors">
+        <img alt="contributors" src="https://img.shields.io/github/contributors/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
-    <a href="https://github.com/volopivoshenko/poetry-dotenv/commits/main">
-        <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-dotenv?logo=github">
+    <a href="https://github.com/volopivoshenko/poetry-plugin-dotenv/commits/main">
+        <img alt="commit" src="https://img.shields.io/github/last-commit/volopivoshenko/poetry-plugin-dotenv?logo=github">
     </a>
 </p>
 
 <p align="center">
-    <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
+    <!-- <a href="https://www.buymeacoffee.com/volopivoshenko" target="_blank">
         <img alt="buymeacoffee" src="https://img.shields.io/badge/buy_me_-a_coffee-ff6964?logo=buymeacoffee">
+    </a> -->
+    <a href="https://stand-with-ukraine.pp.ua/">
+        <img alt="standwithukraine" src="https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB">
+    </a>
+    <a href="https://stand-with-ukraine.pp.ua">
+        <img alt="standwithukraine" src="https://img.shields.io/badge/made_in-Ukraine-ffd700.svg?labelColor=0057b7">
     </a>
 </p>
 
+
+
 - [🔮 Overview](#-overview)
 - [⚙️ Installation](#️-installation)
 - [👩🏻‍💻 Usage](#-usage)
 
 # 🔮 Overview
 
-`poetry-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
+`poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
 **This plugin doesn't have any dependencies, but therefore it also supports features that `python-dotenv` supports (e.g. templates, interpolating variables using `POSIX` variable expansions etc).**
 
 # ⚙️ Installation
 
 ```bash
-poetry self add poetry-dotenv
+poetry self add poetry-plugin-dotenv
 ```
 
 # 👩🏻‍💻 Usage
 
 By default, plugin will load the `.env` file from the current working directory or "higher directories".
 
 To prevent ``poetry`` from loading the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment variable.
 
 If your dotenv file is located in a different path or has a different name you may set the ``POETRY_DOTENV_LOCATION`` environment variable.
 
+<img alt="logo" src="https://github.com/volopivoshenko/poetry-plugin-dotenv/blob/main/docs/static/assets/demo.gif?raw=True">
+
 ```dotenv
 # .env
 DB__HOST=localhost
 DB__DBNAME=prod
 DB__USER=admin
 DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
```

#### html2text {}

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 2.1 Name: poetry-dotenv Version: 0.3.0 Summary: poetry-dotenv
+Metadata-Version: 2.1 Name: poetry-dotenv Version: 0.4.0 Summary: poetry-dotenv
 - is the plugin that automatically loads environment variables from a dotenv
 file into the environment before poetry commands are run. Home-page: https://
 github.com/volopivoshenko/poetry-dotenv License: MIT Keywords:
 python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,cross-platform,hacktoberfest Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko
-Maintainer-email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8,<4.0
+Maintainer-email: volodymyr.pivoshenko@gmail.com Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Other Environment Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Scientific/Engineering Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist: poetry
-(>=1.3.2,<2.0.0) Project-URL: Documentation, https://github.com/volopivoshenko/
-poetry-dotenv Project-URL: Issues, https://github.com/volopivoshenko/poetry-
-dotenv/issues Project-URL: Repository, https://github.com/volopivoshenko/
-poetry-dotenv Project-URL: Releases, https://github.com/volopivoshenko/poetry-
-dotenv/releases Project-URL: Say Thanks!, https://www.buymeacoffee.com/
-volopivoshenko Description-Content-Type: text/markdown
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: poetry (>=1.4.2,<2.0.0) Project-URL: Documentation, https://
+github.com/volopivoshenko/poetry-dotenv Project-URL: Issues, https://
+github.com/volopivoshenko/poetry-dotenv/issues Project-URL: Repository, https:/
+/github.com/volopivoshenko/poetry-dotenv Project-URL: Releases, https://
+github.com/volopivoshenko/poetry-dotenv/releases Project-URL: Say Thanks!,
+https://www.buymeacoffee.com/volopivoshenko Description-Content-Type: text/
+markdown > â ï¸ __Warning__ > > This package has been deprecated and is no
+longer maintained, `poetry-dotenv` has moved to [`poetry-plugin-dotenv`](https:
+//pypi.org/project/poetry-plugin-dotenv)
                                     [logo]
                 [license] [python] [pypi] [release] [numpydoc]
               [black] [isort] [wemake] [mypy] [semantic_release]
           [dependabot] [CI] [CD] [CodeQL] [Dependency_Review] [wheel]
                  [coverage] [codeclimate] [downloads] [stars]
               [issues] [issues] [pr] [pr] [contributors] [commit]
-                                [buymeacoffee]
+                     [standwithukraine] [standwithukraine]
 - [ð® Overview](#-overview) - [âï¸ Installation](#ï¸-installation) -
-[ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-dotenv` - is the
-plugin that automatically loads environment variables from a dotenv file into
-the environment before `poetry` commands are run. **This plugin doesn't have
-any dependencies, but therefore it also supports features that `python-dotenv`
-supports (e.g. templates, interpolating variables using `POSIX` variable
-expansions etc).** # âï¸ Installation ```bash poetry self add poetry-dotenv
-``` # ð©ð»âð» Usage By default, plugin will load the `.env` file from
-the current working directory or "higher directories". To prevent ``poetry``
-from loading the dotenv file, set the ``POETRY_DONT_LOAD_DOTENV`` environment
-variable. If your dotenv file is located in a different path or has a different
-name you may set the ``POETRY_DOTENV_LOCATION`` environment variable. ```dotenv
-# .env DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
+[ð©ð»âð» Usage](#-usage) # ð® Overview `poetry-plugin-dotenv` - is
+the plugin that automatically loads environment variables from a dotenv file
+into the environment before `poetry` commands are run. **This plugin doesn't
+have any dependencies, but therefore it also supports features that `python-
+dotenv` supports (e.g. templates, interpolating variables using `POSIX`
+variable expansions etc).** # âï¸ Installation ```bash poetry self add
+poetry-plugin-dotenv ``` # ð©ð»âð» Usage By default, plugin will load
+the `.env` file from the current working directory or "higher directories". To
+prevent ``poetry`` from loading the dotenv file, set the
+``POETRY_DONT_LOAD_DOTENV`` environment variable. If your dotenv file is
+located in a different path or has a different name you may set the
+``POETRY_DOTENV_LOCATION`` environment variable. [logo] ```dotenv # .env
+DB__HOST=localhost DB__DBNAME=prod DB__USER=admin DB__PASSWORD=admin
 DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@${DB__HOST}/${DB__DBNAME}
 ``` ```dotenv # .env.dev DB__HOST=localhost DB__DBNAME=dev DB__USER=root
 DB__PASSWORD=root DB__ENGINE=postgresql://${DB__USER}:${DB__PASSWORD}@$
 {DB__HOST}/${DB__DBNAME} ``` ```python # main.py import os if __name__ ==
 "__main__": try: print(f"Host: {os.environ['DB__HOST']!r}") print(f"Name:
 {os.environ['DB__DBNAME']!r}") print(f"Username: {os.environ['DB__USER']!r}")
 print(f"Password: {os.environ['DB__PASSWORD']!r}") print(f"Engine: {os.environ
```

