# Comparing `tmp/pylettize-0.1.0.tar.gz` & `tmp/pylettize-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylettize-0.1.0.tar", max compression
+gzip compressed data, was "pylettize-0.1.1.tar", max compression
```

## Comparing `pylettize-0.1.0.tar` & `pylettize-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-27 16:03:44.975622 pylettize-0.1.0/LICENSE
--rw-r--r--   0        0        0     7727 2023-03-27 16:03:44.975622 pylettize-0.1.0/README.md
--rw-r--r--   0        0        0      110 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/__init__.py
--rw-r--r--   0        0        0     2760 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/cli.py
--rw-r--r--   0        0        0     1096 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/palettes/__init__.py
--rw-r--r--   0        0        0      167 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/palettes/gruvbox
--rw-r--r--   0        0        0       32 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/palettes/obama
--rw-r--r--   0        0        0       47 2023-03-27 16:03:44.975622 pylettize-0.1.0/pylettize/palettes/primaries
--rw-r--r--   0        0        0     2073 2023-03-27 16:03:44.985622 pylettize-0.1.0/pylettize/pylettize.py
--rw-r--r--   0        0        0      787 2023-03-28 19:06:02.632052 pylettize-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8305 1970-01-01 00:00:00.000000 pylettize-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-27 16:03:44.975622 pylettize-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7947 2023-04-07 15:24:32.581444 pylettize-0.1.1/README.md
+-rw-r--r--   0        0        0      110 2023-03-27 16:03:44.975622 pylettize-0.1.1/pylettize/__init__.py
+-rw-r--r--   0        0        0     2760 2023-04-07 12:41:48.362885 pylettize-0.1.1/pylettize/cli.py
+-rw-r--r--   0        0        0     1096 2023-04-07 15:24:27.811444 pylettize-0.1.1/pylettize/palettes/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-27 16:03:44.975622 pylettize-0.1.1/pylettize/palettes/gruvbox
+-rw-r--r--   0        0        0       32 2023-03-27 16:03:44.975622 pylettize-0.1.1/pylettize/palettes/obama
+-rw-r--r--   0        0        0       47 2023-03-27 16:03:44.975622 pylettize-0.1.1/pylettize/palettes/primaries
+-rw-r--r--   0        0        0     2073 2023-04-07 11:17:14.432984 pylettize-0.1.1/pylettize/pylettize.py
+-rw-r--r--   0        0        0      788 2023-04-07 15:27:33.161442 pylettize-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8578 1970-01-01 00:00:00.000000 pylettize-0.1.1/PKG-INFO
```

### Comparing `pylettize-0.1.0/LICENSE` & `pylettize-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylettize-0.1.0/README.md` & `pylettize-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Any image in any colormap 🎨🐍
 
-![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/frans-johansson/pylettize)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylettize)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 ![GitHub](https://img.shields.io/github/license/frans-johansson/pylettize)
 [![Coverage Status](https://coveralls.io/repos/github/frans-johansson/pylettize/badge.svg?branch=main)](https://coveralls.io/github/frans-johansson/pylettize?branch=main)
 
 Have you ever been in the middle of creating the ultimate *aesthetic* set up only to find that your favorite wallpaper does not vibe with your new color scheme? Well, fret not, `pylettize` is here for you. This is a simple piece of software allowing you to apply custom color palettes to any image you can think of. Need that classic Bliss™️ re-cast in Gruvbox colors? Look no further!
@@ -12,15 +12,17 @@
 ![The original (boring) Bliss wallpaper](doc/bliss.png)
 ![The Bliss wallpaper in the Gruvbox aesthetic](doc/bliss_gruvbox.png)
 
 
 > **Note:** This project is still in development, without a clear release date set. It is useable at the moment, but might require a bit of hacking on your end if you want it to work exactly as you want. If you want to contribute in any way shape or form, check out the contribution guidelines below!
 
 ## Installation and usage
-In its current state, the project must be installed "from source" (i.e. it is not hosted on PyPI or similar yet). Ideally the following steps would be done in a virtual environment with a minimum `pip` version of `v22.2.2`:
+The easiest way to get started is to simply install pylettize from pip by running `pip install pylettize`
+
+Alternatively, it is possible to build from source by cloning this repository. Ideally the following steps would be done in a virtual environment with a minimum `pip` version of `v22.2.2`:
 
 ```sh
 git clone https://github.com/frans-johansson/pylettize.git
 cd pylettize
 pip install -e .
 ```
 
@@ -86,22 +88,24 @@
 To round off this section, here are some planned features for the future of this little project.
 
 - Automatic palette extraction using clustering algorithms
 - 1-to-1 palette mappings using association algorithms
 - A hosted, installable package on PyPI (yes, you'll be able to `pip install` it!)
 - More default palettes!
 
+Note that there is no clear roadmap for these features, and there is no guarantee they will in fact ever be implemented (🤷)
+
 ## Contribution guidelines
 To get started, make sure you have the following requirements satisfied on your machine:
 
 - `pip v22.2.2`
-- `pipenv v2022.10.12`
-- Any `python3` version, but 3.8 is recommended
+- `poetry v.1.4.1`
+- Any `python3` version, but at least 3.8 is recommended
 
-Set up a local virtual environment by running `pipenv install --dev` in the project root directory (where the Pipfile is). You can then activate this environment by running `pipenv shell` in the same directory. To check if this step worked, try running `which python` and verify that you get a path to some sort of "virtualenv" as output.
+Set up a local virtual environment by running `poetry shell` then `poetry install` in the project root directory (where the pyproject.toml is). This should end up putting you in a brand new virtual environment associated with the project, and install all of its dependencies. To check if this step worked, try running `which python` and verify that you get a path to some sort of "virtualenv" as output.
 
 Optionally, but highly recommended to avoid headaches when submitting PRs, is to set up pre-commit hooks with `pre-commit install` in the project root (where the .pre-commit-config.yaml file is). This should ensure that your PR at least has style compliant code ✨. If you'd like to be told your code is bad before commiting, feel free to set up linting in your editor of choice. We use `flake8` with a bunch of plugins (including `mypy` and `isort`) to run the style checks, so ideally you'd want to use `flake8` locally for linting as well. In Visual Studio Code, adding the following to your settings file should suffice:
 
 ```json
 {
     "python.linting.enabled": true,
     "python.linting.flake8Enabled": true,
```

### Comparing `pylettize-0.1.0/pylettize/cli.py` & `pylettize-0.1.1/pylettize/cli.py`

 * *Files identical despite different names*

### Comparing `pylettize-0.1.0/pylettize/palettes/__init__.py` & `pylettize-0.1.1/pylettize/palettes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylettize-0.1.0/pylettize/pylettize.py` & `pylettize-0.1.1/pylettize/pylettize.py`

 * *Files identical despite different names*

### Comparing `pylettize-0.1.0/pyproject.toml` & `pylettize-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pylettize"
-version = "0.1.0"
+version = "0.1.1"
 description = "Customize the palette of any input image"
 authors = ["Frans Johansson <fransjohansson98@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8.1"
 numpy = "^1.24.2"
 scikit-image = "^0.20.0"
 docopt = "^0.6.2"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
```

### Comparing `pylettize-0.1.0/PKG-INFO` & `pylettize-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pylettize
-Version: 0.1.0
+Version: 0.1.1
 Summary: Customize the palette of any input image
 License: MIT
 Author: Frans Johansson
 Author-email: fransjohansson98@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Any image in any colormap 🎨🐍
 
-![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/frans-johansson/pylettize)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylettize)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 ![GitHub](https://img.shields.io/github/license/frans-johansson/pylettize)
 [![Coverage Status](https://coveralls.io/repos/github/frans-johansson/pylettize/badge.svg?branch=main)](https://coveralls.io/github/frans-johansson/pylettize?branch=main)
 
 Have you ever been in the middle of creating the ultimate *aesthetic* set up only to find that your favorite wallpaper does not vibe with your new color scheme? Well, fret not, `pylettize` is here for you. This is a simple piece of software allowing you to apply custom color palettes to any image you can think of. Need that classic Bliss™️ re-cast in Gruvbox colors? Look no further!
@@ -29,15 +30,17 @@
 ![The original (boring) Bliss wallpaper](doc/bliss.png)
 ![The Bliss wallpaper in the Gruvbox aesthetic](doc/bliss_gruvbox.png)
 
 
 > **Note:** This project is still in development, without a clear release date set. It is useable at the moment, but might require a bit of hacking on your end if you want it to work exactly as you want. If you want to contribute in any way shape or form, check out the contribution guidelines below!
 
 ## Installation and usage
-In its current state, the project must be installed "from source" (i.e. it is not hosted on PyPI or similar yet). Ideally the following steps would be done in a virtual environment with a minimum `pip` version of `v22.2.2`:
+The easiest way to get started is to simply install pylettize from pip by running `pip install pylettize`
+
+Alternatively, it is possible to build from source by cloning this repository. Ideally the following steps would be done in a virtual environment with a minimum `pip` version of `v22.2.2`:
 
 ```sh
 git clone https://github.com/frans-johansson/pylettize.git
 cd pylettize
 pip install -e .
 ```
 
@@ -103,22 +106,24 @@
 To round off this section, here are some planned features for the future of this little project.
 
 - Automatic palette extraction using clustering algorithms
 - 1-to-1 palette mappings using association algorithms
 - A hosted, installable package on PyPI (yes, you'll be able to `pip install` it!)
 - More default palettes!
 
+Note that there is no clear roadmap for these features, and there is no guarantee they will in fact ever be implemented (🤷)
+
 ## Contribution guidelines
 To get started, make sure you have the following requirements satisfied on your machine:
 
 - `pip v22.2.2`
-- `pipenv v2022.10.12`
-- Any `python3` version, but 3.8 is recommended
+- `poetry v.1.4.1`
+- Any `python3` version, but at least 3.8 is recommended
 
-Set up a local virtual environment by running `pipenv install --dev` in the project root directory (where the Pipfile is). You can then activate this environment by running `pipenv shell` in the same directory. To check if this step worked, try running `which python` and verify that you get a path to some sort of "virtualenv" as output.
+Set up a local virtual environment by running `poetry shell` then `poetry install` in the project root directory (where the pyproject.toml is). This should end up putting you in a brand new virtual environment associated with the project, and install all of its dependencies. To check if this step worked, try running `which python` and verify that you get a path to some sort of "virtualenv" as output.
 
 Optionally, but highly recommended to avoid headaches when submitting PRs, is to set up pre-commit hooks with `pre-commit install` in the project root (where the .pre-commit-config.yaml file is). This should ensure that your PR at least has style compliant code ✨. If you'd like to be told your code is bad before commiting, feel free to set up linting in your editor of choice. We use `flake8` with a bunch of plugins (including `mypy` and `isort`) to run the style checks, so ideally you'd want to use `flake8` locally for linting as well. In Visual Studio Code, adding the following to your settings file should suffice:
 
 ```json
 {
     "python.linting.enabled": true,
     "python.linting.flake8Enabled": true,
```

