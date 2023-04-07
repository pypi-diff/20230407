# Comparing `tmp/chacha20poly1305_reuseable-0.2.1.tar.gz` & `tmp/chacha20poly1305_reuseable-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chacha20poly1305_reuseable-0.2.1.tar", max compression
+gzip compressed data, was "chacha20poly1305_reuseable-0.2.2.tar", max compression
```

## Comparing `chacha20poly1305_reuseable-0.2.1.tar` & `chacha20poly1305_reuseable-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12880 2023-04-07 20:06:31.982048 chacha20poly1305_reuseable-0.2.1/LICENSE
--rw-r--r--   0        0        0     4027 2023-04-07 20:06:31.982048 chacha20poly1305_reuseable-0.2.1/README.md
--rw-r--r--   0        0        0      905 2023-04-07 20:06:31.982048 chacha20poly1305_reuseable-0.2.1/build_ext.py
--rw-r--r--   0        0        0     2131 2023-04-07 20:06:32.778068 chacha20poly1305_reuseable-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1772 2023-04-07 20:06:31.982048 chacha20poly1305_reuseable-0.2.1/src/chacha20poly1305_reuseable/__init__.pxd
--rw-r--r--   0        0        0     8865 2023-04-07 20:06:32.746067 chacha20poly1305_reuseable-0.2.1/src/chacha20poly1305_reuseable/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 20:06:31.982048 chacha20poly1305_reuseable-0.2.1/src/chacha20poly1305_reuseable/py.typed
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.1/setup.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    12880 2023-04-07 21:10:09.433538 chacha20poly1305_reuseable-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4027 2023-04-07 21:10:09.433538 chacha20poly1305_reuseable-0.2.2/README.md
+-rw-r--r--   0        0        0      905 2023-04-07 21:10:09.433538 chacha20poly1305_reuseable-0.2.2/build_ext.py
+-rw-r--r--   0        0        0     2131 2023-04-07 21:10:10.229555 chacha20poly1305_reuseable-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1772 2023-04-07 21:10:09.433538 chacha20poly1305_reuseable-0.2.2/src/chacha20poly1305_reuseable/__init__.pxd
+-rw-r--r--   0        0        0     8865 2023-04-07 21:10:10.197554 chacha20poly1305_reuseable-0.2.2/src/chacha20poly1305_reuseable/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:10:09.433538 chacha20poly1305_reuseable-0.2.2/src/chacha20poly1305_reuseable/py.typed
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.2/setup.py
+-rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 chacha20poly1305_reuseable-0.2.2/PKG-INFO
```

### Comparing `chacha20poly1305_reuseable-0.2.1/LICENSE` & `chacha20poly1305_reuseable-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.1/README.md` & `chacha20poly1305_reuseable-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.1/build_ext.py` & `chacha20poly1305_reuseable-0.2.2/build_ext.py`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.1/pyproject.toml` & `chacha20poly1305_reuseable-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chacha20poly1305-reuseable"
-version = "0.2.1"
+version = "0.2.2"
 description = "ChaCha20Poly1305 that is reuseable for asyncio"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/chacha20poly1305-reuseable"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `chacha20poly1305_reuseable-0.2.1/src/chacha20poly1305_reuseable/__init__.pxd` & `chacha20poly1305_reuseable-0.2.2/src/chacha20poly1305_reuseable/__init__.pxd`

 * *Files identical despite different names*

### Comparing `chacha20poly1305_reuseable-0.2.1/src/chacha20poly1305_reuseable/__init__.py` & `chacha20poly1305_reuseable-0.2.2/src/chacha20poly1305_reuseable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 
 import os
```

### Comparing `chacha20poly1305_reuseable-0.2.1/setup.py` & `chacha20poly1305_reuseable-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=36.0.2']
 
 setup_kwargs = {
     'name': 'chacha20poly1305-reuseable',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'ChaCha20Poly1305 that is reuseable for asyncio',
     'long_description': '# chacha20poly1305_reuseable\n\n<p align="center">\n  <a href="https://github.com/bdraco/chacha20poly1305-reuseable/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bdraco/chacha20poly1305-reuseable/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/bdraco/chacha20poly1305-reuseable">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/chacha20poly1305-reuseable.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/chacha20poly1305-reuseable/">\n    <img src="https://img.shields.io/pypi/v/chacha20poly1305-reuseable.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/chacha20poly1305-reuseable.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/chacha20poly1305-reuseable.svg?style=flat-square" alt="License">\n</p>\n\nChaCha20Poly1305 that is reuseable for asyncio\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install chacha20poly1305-reuseable`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/bdraco"><img src="https://avatars.githubusercontent.com/u/663432?v=4?s=80" width="80px;" alt=""/><br /><sub><b>J. Nick Koston</b></sub></a><br /><a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Code">💻</a> <a href="#ideas-bdraco" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/bdraco/chacha20poly1305-reuseable/commits?author=bdraco" title="Documentation">📖</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/chacha20poly1305-reuseable',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['chacha20poly1305_reuseable'] package_data = \ {'': ['*']}
 install_requires = \ ['cryptography>=36.0.2'] setup_kwargs = { 'name':
-'chacha20poly1305-reuseable', 'version': '0.2.1', 'description':
+'chacha20poly1305-reuseable', 'version': '0.2.2', 'description':
 'ChaCha20Poly1305 that is reuseable for asyncio', 'long_description': '#
 chacha20poly1305_reuseable\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `chacha20poly1305_reuseable-0.2.1/PKG-INFO` & `chacha20poly1305_reuseable-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chacha20poly1305-reuseable
-Version: 0.2.1
+Version: 0.2.2
 Summary: ChaCha20Poly1305 that is reuseable for asyncio
 Home-page: https://github.com/bdraco/chacha20poly1305-reuseable
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.2.1 Summary:
+Metadata-Version: 2.1 Name: chacha20poly1305-reuseable Version: 0.2.2 Summary:
 ChaCha20Poly1305 that is reuseable for asyncio Home-page: https://github.com/
 bdraco/chacha20poly1305-reuseable License: Apache Software License 2.0 Author:
 J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

