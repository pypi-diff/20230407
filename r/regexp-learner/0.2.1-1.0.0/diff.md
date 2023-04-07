# Comparing `tmp/regexp_learner-0.2.1.tar.gz` & `tmp/regexp_learner-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regexp_learner-0.2.1.tar", max compression
+gzip compressed data, was "regexp_learner-1.0.0.tar", max compression
```

## Comparing `regexp_learner-0.2.1.tar` & `regexp_learner-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1513 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/LICENSE
--rw-r--r--   0        0        0     2267 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/README.md
--rw-r--r--   0        0        0     1153 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      564 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/__init__.py
--rw-r--r--   0        0        0      195 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/gold/__init__.py
--rw-r--r--   0        0        0     2471 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/gold/gold.py
--rw-r--r--   0        0        0    15342 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/gold/observation_table.py
--rw-r--r--   0        0        0      252 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/lstar/__init__.py
--rw-r--r--   0        0        0     2425 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/lstar/automaton_match.py
--rw-r--r--   0        0        0     7732 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/lstar/learner.py
--rw-r--r--   0        0        0    10874 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/lstar/observation_table.py
--rw-r--r--   0        0        0     2202 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/lstar/teacher.py
--rw-r--r--   0        0        0     2197 2023-04-07 20:49:40.243477 regexp_learner-0.2.1/src/regexp_learner/strings.py
--rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 regexp_learner-0.2.1/setup.py
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 regexp_learner-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1513 2023-04-07 21:22:15.677456 regexp_learner-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2482 2023-04-07 21:22:15.677456 regexp_learner-1.0.0/README.md
+-rw-r--r--   0        0        0     1153 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      564 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/gold/__init__.py
+-rw-r--r--   0        0        0     2471 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/gold/gold.py
+-rw-r--r--   0        0        0    15342 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/gold/observation_table.py
+-rw-r--r--   0        0        0      252 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/lstar/__init__.py
+-rw-r--r--   0        0        0     2425 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/lstar/automaton_match.py
+-rw-r--r--   0        0        0     7732 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/lstar/learner.py
+-rw-r--r--   0        0        0    10874 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/lstar/observation_table.py
+-rw-r--r--   0        0        0     2202 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/lstar/teacher.py
+-rw-r--r--   0        0        0     2197 2023-04-07 21:22:15.681456 regexp_learner-1.0.0/src/regexp_learner/strings.py
+-rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 regexp_learner-1.0.0/setup.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 regexp_learner-1.0.0/PKG-INFO
```

### Comparing `regexp_learner-0.2.1/LICENSE` & `regexp_learner-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/README.md` & `regexp_learner-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Documentation](https://github.com/nokia/regexp-learner/workflows/docs/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/docs.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/regexp-learner/badge/?version=latest)](https://regexp-learner.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/nokia/regexp-learner/branch/master/graph/badge.svg?token=OZM4J0Y2VL)](https://codecov.io/gh/nokia/regexp-learner)
 
 ## Overview
 
 [regexp-learner](https://github.com/nokia/regexp-learner) is a [Python 3](http://python.org/) module providing the following algorithms:
-* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)].
+* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)], [[slides](https://github.com/nokia/regexp-learner/blob/master/Angluin.pdf)].
 * __Gold (1978):__ the Gold algorithm is presented in _Complexity of automaton identification from given data_, E. Mark Gold, 1987 [[pdf](http://sebastian.doc.gold.ac.uk/papers/Language_Learning/gold78complexity.pdf)].
 
 This module is built on top of:
 * [numpy](https://pypi.org/project/numpy/);
 * [pybgl](https://pypi.org/project/pybgl/), a lightweight graph library.
 
 A [jupyter notebook](https://pypi.org/project/jupyter/) is also provided test the algorithm. Note that the [graphviz](https://pypi.org/project/jupyter/) runnables (e.g., `dot`) is required to display the automata.
@@ -22,16 +22,17 @@
 
 * Install [Jupyter Notebook](https://pypi.org/project/jupyter/) or [Jupyter lab](https://pypi.org/project/jupyterlab/).
 * Follow [installation steps](https://github.com/nokia/regexp-learner/wiki/Installation).
 * Run `jupyter notebook` or `jupyter lab`.
 * Open the desired notebook.
 * Run the cells.
 
-
 ## Links
 
-* [Installation](https://github.com/nokia/regexp-learner/wiki/Installation)
-* [Tests](https://github.com/nokia/regexp-leader/wiki/Test)
+* [Installation](https://github.com/nokia/regexp-learner/blob/master/docs/installation.md)
+* [Documentation](https://regexp-learner.readthedocs.io/en/latest/)
+* [Coverage](https://app.codecov.io/gh/nokia/regexp-learner)
+* [Wiki](https://github.com/nokia/regexp-learner/wiki)
 
 ## License
 
 This project is licensed under the [BSD-3-Clause license](https://github.com/nokia/regexp-learner/blob/master/LICENSE).
```

### Comparing `regexp_learner-0.2.1/pyproject.toml` & `regexp_learner-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "regexp-learner"
-version = '0.2.1'
+version = '1.0.0'
 description = "Python3 module providing some algorithms to infer automata and regular expressions.\""
 authors = [
     "Marc-Olivier Buob <marc-olivier.buob@nokia-bell-labs.com>",
     "Maxime Raynal <maxime.raynal@nokia.com>",
 ]
 license = "BSD license"
 readme = "README.md"
```

### Comparing `regexp_learner-0.2.1/src/regexp_learner/__init__.py` & `regexp_learner-1.0.0/src/regexp_learner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 """Top-level package."""
 
 __author__     = "Marc-Olivier Buob, Maxime Raynal"
 __maintainer__ = "Marc-Olivier Buob, Maxime Raynal"
 __email__      = "marc-olivier.buob@nokia-bell-labs.com, maxime.raynal@nokia.com"
 __copyright__  = "Copyright (C) 2019, Nokia"
 __license__    = "BSD-3"
-__version__ = '0.2.1'  # Use single quotes for bumpversion (see setup.cfg)
+__version__ = '1.0.0'  # Use single quotes for bumpversion (see setup.cfg)
 
 from .gold import *
 from .lstar import *
 from .strings import *
```

### Comparing `regexp_learner-0.2.1/src/regexp_learner/gold/gold.py` & `regexp_learner-1.0.0/src/regexp_learner/gold/gold.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/gold/observation_table.py` & `regexp_learner-1.0.0/src/regexp_learner/gold/observation_table.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/lstar/automaton_match.py` & `regexp_learner-1.0.0/src/regexp_learner/lstar/automaton_match.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/lstar/learner.py` & `regexp_learner-1.0.0/src/regexp_learner/lstar/learner.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/lstar/observation_table.py` & `regexp_learner-1.0.0/src/regexp_learner/lstar/observation_table.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/lstar/teacher.py` & `regexp_learner-1.0.0/src/regexp_learner/lstar/teacher.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/src/regexp_learner/strings.py` & `regexp_learner-1.0.0/src/regexp_learner/strings.py`

 * *Files identical despite different names*

### Comparing `regexp_learner-0.2.1/setup.py` & `regexp_learner-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['ipython', 'numpy>=1.24.2', 'pybgl>=0.9.3']
 
 setup_kwargs = {
     'name': 'regexp-learner',
-    'version': '0.2.1',
+    'version': '1.0.0',
     'description': 'Python3 module providing some algorithms to infer automata and regular expressions."',
-    'long_description': '# regexp-learner\n\n[![PyPI](https://img.shields.io/pypi/v/regexp_learner.svg)](https://pypi.python.org/pypi/regexp_learner/)\n[![Build](https://github.com/nokia/regexp-learner/workflows/build/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/build.yml)\n[![Documentation](https://github.com/nokia/regexp-learner/workflows/docs/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/docs.yml)\n[![ReadTheDocs](https://readthedocs.org/projects/regexp-learner/badge/?version=latest)](https://regexp-learner.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/nokia/regexp-learner/branch/master/graph/badge.svg?token=OZM4J0Y2VL)](https://codecov.io/gh/nokia/regexp-learner)\n\n## Overview\n\n[regexp-learner](https://github.com/nokia/regexp-learner) is a [Python 3](http://python.org/) module providing the following algorithms:\n* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)].\n* __Gold (1978):__ the Gold algorithm is presented in _Complexity of automaton identification from given data_, E. Mark Gold, 1987 [[pdf](http://sebastian.doc.gold.ac.uk/papers/Language_Learning/gold78complexity.pdf)].\n\nThis module is built on top of:\n* [numpy](https://pypi.org/project/numpy/);\n* [pybgl](https://pypi.org/project/pybgl/), a lightweight graph library.\n\nA [jupyter notebook](https://pypi.org/project/jupyter/) is also provided test the algorithm. Note that the [graphviz](https://pypi.org/project/jupyter/) runnables (e.g., `dot`) is required to display the automata.\n\n## Usage\n\n* Install [Jupyter Notebook](https://pypi.org/project/jupyter/) or [Jupyter lab](https://pypi.org/project/jupyterlab/).\n* Follow [installation steps](https://github.com/nokia/regexp-learner/wiki/Installation).\n* Run `jupyter notebook` or `jupyter lab`.\n* Open the desired notebook.\n* Run the cells.\n\n\n## Links\n\n* [Installation](https://github.com/nokia/regexp-learner/wiki/Installation)\n* [Tests](https://github.com/nokia/regexp-leader/wiki/Test)\n\n## License\n\nThis project is licensed under the [BSD-3-Clause license](https://github.com/nokia/regexp-learner/blob/master/LICENSE).\n',
+    'long_description': '# regexp-learner\n\n[![PyPI](https://img.shields.io/pypi/v/regexp_learner.svg)](https://pypi.python.org/pypi/regexp_learner/)\n[![Build](https://github.com/nokia/regexp-learner/workflows/build/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/build.yml)\n[![Documentation](https://github.com/nokia/regexp-learner/workflows/docs/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/docs.yml)\n[![ReadTheDocs](https://readthedocs.org/projects/regexp-learner/badge/?version=latest)](https://regexp-learner.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/nokia/regexp-learner/branch/master/graph/badge.svg?token=OZM4J0Y2VL)](https://codecov.io/gh/nokia/regexp-learner)\n\n## Overview\n\n[regexp-learner](https://github.com/nokia/regexp-learner) is a [Python 3](http://python.org/) module providing the following algorithms:\n* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)], [[slides](https://github.com/nokia/regexp-learner/blob/master/Angluin.pdf)].\n* __Gold (1978):__ the Gold algorithm is presented in _Complexity of automaton identification from given data_, E. Mark Gold, 1987 [[pdf](http://sebastian.doc.gold.ac.uk/papers/Language_Learning/gold78complexity.pdf)].\n\nThis module is built on top of:\n* [numpy](https://pypi.org/project/numpy/);\n* [pybgl](https://pypi.org/project/pybgl/), a lightweight graph library.\n\nA [jupyter notebook](https://pypi.org/project/jupyter/) is also provided test the algorithm. Note that the [graphviz](https://pypi.org/project/jupyter/) runnables (e.g., `dot`) is required to display the automata.\n\n## Usage\n\n* Install [Jupyter Notebook](https://pypi.org/project/jupyter/) or [Jupyter lab](https://pypi.org/project/jupyterlab/).\n* Follow [installation steps](https://github.com/nokia/regexp-learner/wiki/Installation).\n* Run `jupyter notebook` or `jupyter lab`.\n* Open the desired notebook.\n* Run the cells.\n\n## Links\n\n* [Installation](https://github.com/nokia/regexp-learner/blob/master/docs/installation.md)\n* [Documentation](https://regexp-learner.readthedocs.io/en/latest/)\n* [Coverage](https://app.codecov.io/gh/nokia/regexp-learner)\n* [Wiki](https://github.com/nokia/regexp-learner/wiki)\n\n## License\n\nThis project is licensed under the [BSD-3-Clause license](https://github.com/nokia/regexp-learner/blob/master/LICENSE).\n',
     'author': 'Marc-Olivier Buob',
     'author_email': 'marc-olivier.buob@nokia-bell-labs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `regexp_learner-0.2.1/PKG-INFO` & `regexp_learner-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regexp-learner
-Version: 0.2.1
+Version: 1.0.0
 Summary: Python3 module providing some algorithms to infer automata and regular expressions."
 License: BSD license
 Author: Marc-Olivier Buob
 Author-email: marc-olivier.buob@nokia-bell-labs.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 [![Documentation](https://github.com/nokia/regexp-learner/workflows/docs/badge.svg)](https://github.com/nokia/regexp-learner/actions/workflows/docs.yml)
 [![ReadTheDocs](https://readthedocs.org/projects/regexp-learner/badge/?version=latest)](https://regexp-learner.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/nokia/regexp-learner/branch/master/graph/badge.svg?token=OZM4J0Y2VL)](https://codecov.io/gh/nokia/regexp-learner)
 
 ## Overview
 
 [regexp-learner](https://github.com/nokia/regexp-learner) is a [Python 3](http://python.org/) module providing the following algorithms:
-* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)].
+* __Angluin (1987):__ the L* algorithm is presented in _Learning regular sets from queries and couterexamples_, Dana Angluin, 1987 [[pdf](https://people.eecs.berkeley.edu/~dawnsong/teaching/s10/papers/angluin87.pdf)], [[slides](https://github.com/nokia/regexp-learner/blob/master/Angluin.pdf)].
 * __Gold (1978):__ the Gold algorithm is presented in _Complexity of automaton identification from given data_, E. Mark Gold, 1987 [[pdf](http://sebastian.doc.gold.ac.uk/papers/Language_Learning/gold78complexity.pdf)].
 
 This module is built on top of:
 * [numpy](https://pypi.org/project/numpy/);
 * [pybgl](https://pypi.org/project/pybgl/), a lightweight graph library.
 
 A [jupyter notebook](https://pypi.org/project/jupyter/) is also provided test the algorithm. Note that the [graphviz](https://pypi.org/project/jupyter/) runnables (e.g., `dot`) is required to display the automata.
@@ -41,17 +41,18 @@
 
 * Install [Jupyter Notebook](https://pypi.org/project/jupyter/) or [Jupyter lab](https://pypi.org/project/jupyterlab/).
 * Follow [installation steps](https://github.com/nokia/regexp-learner/wiki/Installation).
 * Run `jupyter notebook` or `jupyter lab`.
 * Open the desired notebook.
 * Run the cells.
 
-
 ## Links
 
-* [Installation](https://github.com/nokia/regexp-learner/wiki/Installation)
-* [Tests](https://github.com/nokia/regexp-leader/wiki/Test)
+* [Installation](https://github.com/nokia/regexp-learner/blob/master/docs/installation.md)
+* [Documentation](https://regexp-learner.readthedocs.io/en/latest/)
+* [Coverage](https://app.codecov.io/gh/nokia/regexp-learner)
+* [Wiki](https://github.com/nokia/regexp-learner/wiki)
 
 ## License
 
 This project is licensed under the [BSD-3-Clause license](https://github.com/nokia/regexp-learner/blob/master/LICENSE).
```

