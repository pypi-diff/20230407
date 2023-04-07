# Comparing `tmp/omnidep-0.3.3.tar.gz` & `tmp/omnidep-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnidep-0.3.3.tar", max compression
+gzip compressed data, was "omnidep-0.3.4.tar", max compression
```

## Comparing `omnidep-0.3.3.tar` & `omnidep-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.3/LICENSE
--rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.3/omnidep/__init__.py
--rw-r--r--   0        0        0     5128 2022-12-13 00:57:08.000000 omnidep-0.3.3/omnidep/command.py
--rw-r--r--   0        0        0     3349 2022-11-29 18:45:06.000000 omnidep-0.3.3/omnidep/errors.py
--rw-r--r--   0        0        0     2083 2022-06-12 12:45:12.000000 omnidep-0.3.3/omnidep/imports.py
--rw-r--r--   0        0        0     1413 2022-12-24 13:49:00.000000 omnidep-0.3.3/omnidep/main.py
--rw-r--r--   0        0        0     3046 2022-11-28 18:05:04.000000 omnidep-0.3.3/omnidep/packages.py
--rw-r--r--   0        0        0     7612 2022-12-24 13:37:44.000000 omnidep-0.3.3/omnidep/project.py
--rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.3/omnidep/tst/__init__.py
--rw-r--r--   0        0        0     9636 2022-12-24 13:36:52.000000 omnidep-0.3.3/omnidep/tst/errors_test.py
--rw-r--r--   0        0        0     1504 2022-06-12 12:45:12.000000 omnidep-0.3.3/omnidep/tst/imports_test.py
--rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.3/omnidep/tst/packages_test.py
--rw-r--r--   0        0        0     1692 2022-12-24 13:49:46.000000 omnidep-0.3.3/omnidep/tst/project_test.py
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.3/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.3/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
--rw-r--r--   0        0        0      257 2022-12-13 00:37:56.000000 omnidep-0.3.3/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
--rw-r--r--   0        0        0      138 2022-12-13 01:05:38.000000 omnidep-0.3.3/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
--rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.3/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
--rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.3/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
--rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.3/omnidep/tst/test_cases/every_import.py~
--rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.3/omnidep/tst/test_cases/unsorted/pyproject.toml
--rw-r--r--   0        0        0     1613 2022-12-24 16:47:12.000000 omnidep-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    13267 2022-12-24 16:56:36.000000 omnidep-0.3.3/README.rst
--rw-r--r--   0        0        0    15081 2022-12-24 16:57:36.790341 omnidep-0.3.3/setup.py
--rw-r--r--   0        0        0    14081 2022-12-24 16:57:36.790341 omnidep-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-06-11 17:48:28.000000 omnidep-0.3.4/LICENSE
+-rw-r--r--   0        0        0        0 2022-06-11 16:57:02.840000 omnidep-0.3.4/omnidep/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/__main__.py
+-rw-r--r--   0        0        0     5128 2022-12-13 00:57:08.000000 omnidep-0.3.4/omnidep/command.py
+-rw-r--r--   0        0        0     3349 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/errors.py
+-rw-r--r--   0        0        0     2083 2022-06-12 12:45:12.000000 omnidep-0.3.4/omnidep/imports.py
+-rw-r--r--   0        0        0     1413 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/main.py
+-rw-r--r--   0        0        0     3046 2022-11-28 18:05:04.000000 omnidep-0.3.4/omnidep/packages.py
+-rw-r--r--   0        0        0     7620 2023-04-07 18:02:26.000000 omnidep-0.3.4/omnidep/project.py
+-rw-r--r--   0        0        0        0 2022-11-28 18:05:02.570000 omnidep-0.3.4/omnidep/tst/__init__.py
+-rw-r--r--   0        0        0     9636 2022-12-24 13:36:52.000000 omnidep-0.3.4/omnidep/tst/errors_test.py
+-rw-r--r--   0        0        0     1504 2022-06-12 12:45:12.000000 omnidep-0.3.4/omnidep/tst/imports_test.py
+-rw-r--r--   0        0        0     2602 2022-06-11 17:48:28.000000 omnidep-0.3.4/omnidep/tst/packages_test.py
+-rw-r--r--   0        0        0     1692 2022-12-24 13:49:46.000000 omnidep-0.3.4/omnidep/tst/project_test.py
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/case_insensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      314 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/case_sensitive_sorted/pyproject.toml
+-rw-r--r--   0        0        0      257 2022-12-13 00:37:56.000000 omnidep-0.3.4/omnidep/tst/test_cases/dependency_in_test_code/pyproject.toml
+-rw-r--r--   0        0        0      138 2022-12-13 01:05:38.000000 omnidep-0.3.4/omnidep/tst/test_cases/dependency_in_test_code/tests/test_code.py
+-rw-r--r--   0        0        0      291 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/dev_dependencies_new/pyproject.toml
+-rw-r--r--   0        0        0      285 2022-11-29 18:45:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/dev_dependencies_old/pyproject.toml
+-rw-r--r--   0        0        0     2266 2022-06-11 17:48:28.000000 omnidep-0.3.4/omnidep/tst/test_cases/every_import.py~
+-rw-r--r--   0        0        0      293 2022-10-07 14:23:06.000000 omnidep-0.3.4/omnidep/tst/test_cases/unsorted/pyproject.toml
+-rw-r--r--   0        0        0     1529 2023-04-07 18:02:26.000000 omnidep-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    13401 2023-04-07 18:02:26.000000 omnidep-0.3.4/README.rst
+-rw-r--r--   0        0        0    14216 1970-01-01 00:00:00.000000 omnidep-0.3.4/PKG-INFO
```

### Comparing `omnidep-0.3.3/LICENSE` & `omnidep-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/command.py` & `omnidep-0.3.4/omnidep/command.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/errors.py` & `omnidep-0.3.4/omnidep/errors.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/imports.py` & `omnidep-0.3.4/omnidep/imports.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/main.py` & `omnidep-0.3.4/omnidep/main.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/packages.py` & `omnidep-0.3.4/omnidep/packages.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/project.py` & `omnidep-0.3.4/omnidep/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                     yield V.ODEP003(f"Namespace package found: any of {found} might provide {module!r}")
                     used.update(found)
                 else:
                     yield V.ODEP004(f"Namespace package found: any of {found} might provide {module!r}, and there are no dependencies on any of them", module)
         if check_unused:
             unused = set(packages) - used - set(self.config.ignore_dependencies)
             if unused:
-                yield V.ODEP005(f'Unused {label} in project file: {unused}')
+                yield V.ODEP005(f'Unused {label} in project file: {sorted(unused)}')
 
     def ignore_import(self, module: str) -> bool:
         return bool(self.config) and module in self.config.ignore_imports
 
     def required(self, package: str, packages: Container[str]) -> bool:
         def mentioned(pkg: str) -> bool:
             return pkg in packages or pkg in self.local_packages
```

### Comparing `omnidep-0.3.3/omnidep/tst/errors_test.py` & `omnidep-0.3.4/omnidep/tst/errors_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/tst/imports_test.py` & `omnidep-0.3.4/omnidep/tst/imports_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/tst/packages_test.py` & `omnidep-0.3.4/omnidep/tst/packages_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/tst/project_test.py` & `omnidep-0.3.4/omnidep/tst/project_test.py`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/omnidep/tst/test_cases/every_import.py~` & `omnidep-0.3.4/omnidep/tst/test_cases/every_import.py~`

 * *Files identical despite different names*

### Comparing `omnidep-0.3.3/pyproject.toml` & `omnidep-0.3.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [tool.poetry]
 name = "omnidep"
-version = "0.3.3"
+version = "0.3.4"
 description = "Linter to compare project dependencies against imports in source code"
 readme = "README.rst"
 authors = ["Steve Jessop <68118527+sjjessop@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/sjjessop/omnidep"
 packages = [{ include = "omnidep" }]
-# Temporary until I'm using Poetry 1.2.2+ and poetry-core 1.3.2+ for publishing.
-classifiers = ["Programming Language :: Python :: 3.11"]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0"
 
-importlib-metadata = ">=1.1.0"  # 1.1.0 required by flake8
+importlib-metadata = ">=1.1.0"
 isort = { version = ">=5.0.1", python = "<3.10" }  # 5.0.1 fixes some issue importing vendored toml
 tomli = ">=1.1.0"  # 1.1.0 adds support for binary filehandles
 
 [tool.poetry.dev-dependencies]
 coverage = { version = "*", extras = ["toml"] }
-flake8 = ">=5"
-isort = "*"
+isort = "<5.12"
 mypy = "*"
 pyOpenSSL = "*"  # Used as a test case
 pytest = "*"
 pytest-cov = "*"
+ruff = "0.0.261"
 
 [tool.poetry.scripts]
 omnidep = 'omnidep.main:script_entry_point'
 
 
 [tool.omnidep]
 local-test-paths = ["omnidep/tst/"]
@@ -58,10 +56,16 @@
 ]
 
 
 [tool.pytest.ini_options]
 filterwarnings = ["error"]
 
 
+[tool.ruff]
+select = ["E", "F"]
+ignore = ["E501"]
+target-version = "py37"
+
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `omnidep-0.3.3/README.rst` & `omnidep-0.3.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,19 @@
 * If you know what you're doing, and users of your project will know how to
   supply the code that you're importing, then ignore the import with
   ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
 
 Changelog
 =========
 
+0.3.4
+-----
+* Report unused dependencies as a sorted list
+* Allow `python -m omnidep` (https://github.com/sjjessop/omnidep/issues/2)
+
 0.3.3
 -----
 
 * Treat local-test-paths config more like --tests option.
 * Non-zero exit code if there are any errors reported.
 * Documentation improvements.
```

### Comparing `omnidep-0.3.3/setup.py` & `omnidep-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,409 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: omnidep
+Version: 0.3.4
+Summary: Linter to compare project dependencies against imports in source code
+Home-page: https://github.com/sjjessop/omnidep
+License: MIT
+Author: Steve Jessop
+Author-email: 68118527+sjjessop@users.noreply.github.com
+Requires-Python: >=3.7.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=1.1.0)
+Requires-Dist: isort (>=5.0.1) ; python_version < "3.10"
+Requires-Dist: tomli (>=1.1.0)
+Description-Content-Type: text/x-rst
 
-packages = \
-['omnidep',
- 'omnidep.tst',
- 'omnidep.tst.test_cases.dependency_in_test_code.tests']
-
-package_data = \
-{'': ['*'],
- 'omnidep.tst': ['test_cases/*',
-                 'test_cases/case_insensitive_sorted/*',
-                 'test_cases/case_sensitive_sorted/*',
-                 'test_cases/dependency_in_test_code/*',
-                 'test_cases/dev_dependencies_new/*',
-                 'test_cases/dev_dependencies_old/*',
-                 'test_cases/unsorted/*']}
-
-install_requires = \
-['importlib-metadata>=1.1.0', 'tomli>=1.1.0']
-
-extras_require = \
-{':python_version < "3.10"': ['isort>=5.0.1']}
-
-entry_points = \
-{'console_scripts': ['omnidep = omnidep.main:script_entry_point']}
-
-setup_kwargs = {
-    'name': 'omnidep',
-    'version': '0.3.3',
-    'description': 'Linter to compare project dependencies against imports in source code',
-    'long_description': '=======\nOmnidep\n=======\n\nA Python linter to compare a project\'s declared dependencies against the import\nstatements in its source code.\n\n.. image:: https://github.com/sjjessop/omnidep/workflows/tests/badge.svg?branch=develop\n   :alt: Test status\n   :target: https://github.com/sjjessop/omnidep/actions?query=workflow%3Atests+branch%3Adevelop\n\n.. image:: https://img.shields.io/badge/CI%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg\n   :alt: Tested with Python versions 3.7 3.8 3.9 3.10 3.11\n   :target: https://www.python.org/downloads/\n\n.. image:: https://img.shields.io/pypi/pyversions/omnidep\n   :alt: PyPI project\n   :target: https://pypi.org/project/omnidep/\n\n.. image:: https://img.shields.io/badge/badges-4-green.svg\n   :alt: 4 badges\n   :target: https://shields.io/\n\nPurpose\n=======\n\nProvides warnings when a project imports packages that it doesn\'t declare a\ndependency on, plus some related linting of the project dependency data.\n\nCurrently only poetry projects are supported (configured in pyproject.toml).\nThe projects that your project depends on can be packaged using any tools, but\nyour project (that omnidep analyses) currently must use poetry.\n\nInstallation\n------------\n\n.. code-block:: bash\n\n    pip install omnidep\n\nOptionally, you can also run the test suite. This would be a good idea if\nyou\'re using a new (or pre-release) version of Python not included in this\nrepo\'s CI testing.\n\n.. code-block:: bash\n\n    pip install pyOpenSSL pytest\n    pytest --pyargs omnidep.tst\n\nUsage\n-----\n\n.. code-block:: bash\n\n    omnidep pyproject.toml\n\n\nConfiguration\n-------------\n\nomnidep uses your project\'s poetry configuration to work out:\n\n* What source files to search for imports, from ``tool.poetry.packages``.\n* What dependencies your project declares, from ``tool.poetry.dependencies``.\n* What dev-dependencies your project declares, from\n  ``tool.poetry.dev-dependencies`` and ``tool.poetry.group.dev.dependencies``.\n\nIf you have test code that you want omnidep to search for imports, then:\n\n* If you keep your test code "inside" your project, then list it in\n  ``local-test-paths`` in the ``[tool.omnidep]`` section described below,\n  otherwise omnidep treats it as regular code.\n* If you keep your test code "outside" your project, then either use the\n  ``--tests`` command-line option to locate it, or list it in\n  ``local-test-paths`` in ``[tool.omnidep]``, otherwise omnidep ignores it. You\n  also need to configure ``local-test-packages`` if some of your test files\n  import other test files, for example if you have shared helper functions.\n\nomnidep is configured using the ``pyproject.toml`` file, and specifically the\n``[tool.omnidep]`` section. Unrecognised keys are rejected and omnidep will not\nrun (so, if you want to use a particular key then you should require at least\nthe minimum version of omnidep that recognises it). The following config keys\nare recognised:\n\nignore-imports\n^^^^^^^^^^^^^^\n\nExample: ``ignore-imports = ["X"]``\n\nSince: 0.2.0\n\nCauses omnidep to ignore all import statements from X, for example\n``import X``, ``from X.Y import Z``. omnidep will behave as if your code does\nnot use package X, even if it does. X must be a top-level package. It is not\ncurrently possible to selectively ignore a sub-package (like X.Y), nor is it\ncurrently possible to ignore imports from some files but not others.\n\nchild-packages\n^^^^^^^^^^^^^^\n\nExample: ``child-packages = {boto3 = ["botocore"]}``\n\nSince: 0.2.0\n\nCauses omnidep to consider a dependency on boto3 to also supply botocore. This\nsaves you having to explictly list the child as a dependency of your project.\nYou chould only do this when the child is inherant to the parent, not just\nbecause by chance you pull in a package you need via an indirect dependency.\nThe reason is that indirect dependencies can change, and the project that you\ndo depend on might not require the same version of the child that your usage\nrequires. Only if the projects are closely related can you assume that the\nversion you require of one will provide the features you need from the other.\n\nignore-dependencies\n^^^^^^^^^^^^^^^^^^^\n\nExample: ``ignore-dependencies = ["X"]``\n\nSince: 0.2.0\n\nCauses omnidep to ignore the project X listed in your project\'s dependencies.\nomnidep will behave as if your project does not depend on X, even if it does.\n\nignore-dependencies-order\n^^^^^^^^^^^^^^^^^^^^^^^^^\n\nExample: ``ignore-dependencies-order = true``\n\nSince: 0.2.0\n\nCauses omnidep to skip the check that your dependencies are alphabetically\nordered.\n\nignore-dev-dependencies-order\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nExample: ``ignore-dev-dependencies-order = true``\n\nSince: 0.2.0\n\nCauses omnidep to skip the check that your dev-dependencies are alphabetically\nordered.\n\nlocal-test-paths\n^^^^^^^^^^^^^^^^\n\nExample: ``local-test-paths = ["myproject/tests/"]``\n\nSince: 0.2.0\n\nCauses omnidep to treat all code in ``myproject.tests`` as test code, meaning\nthat anything it imports can be provided either by your projects dependencies\nor by its dev-dependencies. Imports from code that is not test code must be\nprovided by non-dev dependencies.\n\nlocal-test-packages\n^^^^^^^^^^^^^^^^^^^\n\nExample: ``local-test-packages = ["tests"]``\n\nSince: 0.2.0\n\nCauses omnidep to treat ``tests`` as part of the current project, but only when\nconsidering imports that appear in test code. Use this when your test code is\nnot shipped as part of your project.\n\nError codes explained\n---------------------\n\nX, Y, P, Q, R, represent the names of imports or dependencies, depending on the\nmessage.\n\nODEP001\n^^^^^^^\n\n| ``package \'X\' is imported but not listed in dependencies``\n| ``package \'X\' is imported but not listed in dev-dependencies``\n|\n\nX is the name you imported, which is not necessarily the same as the name of\nthe project you have to install (for example the project ``beautifulsoup4``\ninstalls the package ``bs4``). omnidep does its best to find what project your\ndesired package comes from, but if it fails, or if you don\'t have a suitable\ndependency, then this is the result.\n\nTo fix, choose one of the following:\n\n* List the project name in your dependencies. If the package is used from test\n  code, then the dependency can be either dev or non-dev. If the package is\n  used from non-test code, then the dependency needs to be non-dev.\n* To ignore the import, add it to the list of ignored imports in your\n  ``[tool.omnidep]`` config, like ``ignore-imports = ["X"]``.\n* The package might come from a dependency of a dependency, and you might\n  prefer not to explicitly list it as a direct dependency too, so you can list\n  X as a child of some other dependency that you do list. You should only do\n  this when the indirect dependency is inherent to the direct dependency, for\n  example ``boto3`` provides ``botocore``. Add\n  ``child-packages = {something = ["X"]}`` to your ``[tool.omnidep]`` config,\n  meaning that the project named "something" provides "X", and so a dependency\n  on "something" is acceptable in place of a dependency on "X".\n\nODEP002\n^^^^^^^\n\n``module \'X\' is imported but not installed``\n\nNot only is there no dependency found that provides X, but X isn\'t even\ncurrently installed. omnidep relies on locally installed metadata to help it\nfind what dependencies correspond to what imports.\n\nTo fix, choose one of the following:\n\n* If your project has X as a dependency, but you haven\'t installed your\n  project then install your project, bringing in its dependencies.\n* Add a dependency that provides X.\n* Ignore the import by listing it in your in your ``[tool.omnidep]`` config,\n  like ``ignore-imports = ["X"]``.\n\nODEP003\n^^^^^^^\n\n``Namespace package found: any of [\'P\', \'Q\', \'R\'] might provide \'X\'``\n\nIf projects P, Q, and R all provide code in the Python package X, then omnidep\ndoesn\'t know which one you need in order to satisfy a given import. If you\ndeclare dependencies on all of them (that is, all the ones you currently have\ninstalled), then omnidep is satisfied. If you depend on some but not others,\nthen you get this message.\n\nTo fix, choose one of the following:\n\n* If you don\'t need the ones you don\'t declare dependencies on, and they are\n  installed accidentally, then uninstall them.\n* If appropriate, declare dependencies on all of P, Q, and R. However, this\n  might not be appropriate because P and Q might be genuine direct dependencies\n  of your code, whereas R was pulled in indirectly via something else. You\n  don\'t want to have to list indirect dependencies as direct dependencies.\n* Otherwise you have to resolve for yourself whether your dependencies are\n  adequate, then ignore the import with ``ignore-imports = ["X"]`` in your\n  ``[tool.omnidep]`` config.\n\n\nODEP004\n^^^^^^^\n\n``Namespace package found: any of [\'P\', \'Q\', \'R\'] might provide \'X\', and there are no dependencies on any of them``\n\nIf projects P, Q, and R all provide code in the Python package X, then omnidep\ndoesn\'t know which one you need in order to satisfy a given import. If you\ndeclare dependencies on all of them (that is, all the ones you currently have\ninstalled), then omnidep is satisfied. If you depend on none of them,\nthen you get this message.\n\nTo fix, choose one of the following:\n\n* If appropriate, declare dependencies on all of P, Q, and R. However, this\n  might not be appropriate because P and Q might be genuine direct dependencies\n  of your code, whereas R was pulled in indirectly via something else. You\n  don\'t want to have to list indirect dependencies as direct dependencies.\n* Otherwise you have to resolve for yourself whether your dependencies are\n  adequate, then ignore the import with ``ignore-imports = ["X"]`` in your\n  ``[tool.omnidep]`` config.\n\n\nODEP005\n^^^^^^^\n\n``unused dependencies in project file: {\'X\', \'Y\'}``\n\nomnidep expects you not to list any dependencies that you don\'t import. This\nmight be completely legitimate, for example:\n\n* the dependency is a plugin to some framework and will be used via some means\n  other than an explicit ``import`` in your code;\n* you are controlling the version of an indirect dependency, to deal with\n  some problem caused by unexpected breaking changes.\n\nUnused dev-dependencies are always ignored, since they tend to include linters\nand suchlike.\n\nTo fix, choose one of the following:\n\n* Remove the dependency.\n* List the dependency in your ``[tool.omnidep]`` config like\n  ``ignore-dependencies = ["X"]``.\n\nODEP006\n^^^^^^^\n\n| ``dependencies are not sorted: \'Y\' before \'X\'``\n| ``dev-dependencies are not sorted: \'Y\' before \'X\'``\n|\n\nIgnoring ``python``, which is allowed to come first, omnidep expects you to\nlist dependencies in case-insensitive alphabetical order within each section\n(dev and non-dev).\n\nTo fix, choose one of the following:\n\n* List your dependencies alphabetically.\n* Set ``ignore-dependencies-order = true`` or\n  ``ignore-dev-dependencies-order = true`` in your ``[tool.omnidep]`` config.\n\nODEP007\n^^^^^^^\n\n``dependency \'X\' is not the preferred name: consider \'Y\'``\n\nomnidep expects you to use either of two formats to name dependencies in your\nproject file: the "Normalized Name" as defined in\n`PEP 503 <https://peps.python.org/pep-0503/>`_ or the name the dependency uses\nfor itself in its metadata. Any name that normalizes to the same value will\nwork, but inconsistent naming tends to lead to confusion, or to failing to find\nmentions when you search for them.\n\nTo fix:\n\n* Use the name omnidep suggests, or the normalized name.\n\nODEP008\n^^^^^^^\n\n``Module \'X\' not under package management but found on python path``\n\nomnidep cannot find any project that provides X, but it is available to import.\nThis can happen for example if you have set up the ``PYTHONPATH`` to find the\ncode, instead of installing it as a dependency.\n\nTo fix, choose one of the following:\n\n* If this is an error, list a suitable dependency.\n* If this occors when your test code is importing other modules also within\n  your test code (for example helper utilities) then you can configure\n  ``local-test-packages = ["X"]`` in your ``[tool.omnidep]`` config, and/or\n  ``local-test-paths`` with the location of the test source.\n* If you know what you\'re doing, and users of your project will know how to\n  supply the code that you\'re importing, then ignore the import with\n  ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.\n\nChangelog\n=========\n\n0.3.3\n-----\n\n* Treat local-test-paths config more like --tests option.\n* Non-zero exit code if there are any errors reported.\n* Documentation improvements.\n\n0.3.2\n-----\n\n* Read dev dependencies from the new location used by Poetry 1.2.0+\n* Add Python 3.11 to PyPI classifiers.\n\n0.3.1\n-----\n\n* Add Python 3.11 to the test matrix, and use separate badges in the README\n  for what is tagged on PyPI vs. what is tested.\n* Documentation improvements.\n* Uncap Python dependency. If Python ever reaches version 4, you are free to\n  install omnidep on it and see what happens!\n\n0.3.0\n-----\n\n* Breaking: When testing that dependencies are sorted, do it case-insensitive.\n* Deal with some build issues.\n\n0.2.1\n-----\n\n* Refer to online docs insted of long message in terminal.\n* Publish to PyPI.\n\n0.2.0\n-----\n\n* Minor documentation improvements.\n* Lower bounds for dependencies importlib-metadata, isort, and tomli.\n* CI test of the lower-bound versions.\n',
-    'author': 'Steve Jessop',
-    'author_email': '68118527+sjjessop@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/sjjessop/omnidep',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.0',
-}
+=======
+Omnidep
+=======
 
+A Python linter to compare a project's declared dependencies against the import
+statements in its source code.
+
+.. image:: https://github.com/sjjessop/omnidep/workflows/tests/badge.svg?branch=develop
+   :alt: Test status
+   :target: https://github.com/sjjessop/omnidep/actions?query=workflow%3Atests+branch%3Adevelop
+
+.. image:: https://img.shields.io/badge/CI%20python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg
+   :alt: Tested with Python versions 3.7 3.8 3.9 3.10 3.11
+   :target: https://www.python.org/downloads/
+
+.. image:: https://img.shields.io/pypi/pyversions/omnidep
+   :alt: PyPI project
+   :target: https://pypi.org/project/omnidep/
+
+.. image:: https://img.shields.io/badge/badges-4-green.svg
+   :alt: 4 badges
+   :target: https://shields.io/
+
+Purpose
+=======
+
+Provides warnings when a project imports packages that it doesn't declare a
+dependency on, plus some related linting of the project dependency data.
+
+Currently only poetry projects are supported (configured in pyproject.toml).
+The projects that your project depends on can be packaged using any tools, but
+your project (that omnidep analyses) currently must use poetry.
+
+Installation
+------------
+
+.. code-block:: bash
+
+    pip install omnidep
+
+Optionally, you can also run the test suite. This would be a good idea if
+you're using a new (or pre-release) version of Python not included in this
+repo's CI testing.
+
+.. code-block:: bash
+
+    pip install pyOpenSSL pytest
+    pytest --pyargs omnidep.tst
+
+Usage
+-----
+
+.. code-block:: bash
+
+    omnidep pyproject.toml
+
+
+Configuration
+-------------
+
+omnidep uses your project's poetry configuration to work out:
+
+* What source files to search for imports, from ``tool.poetry.packages``.
+* What dependencies your project declares, from ``tool.poetry.dependencies``.
+* What dev-dependencies your project declares, from
+  ``tool.poetry.dev-dependencies`` and ``tool.poetry.group.dev.dependencies``.
+
+If you have test code that you want omnidep to search for imports, then:
+
+* If you keep your test code "inside" your project, then list it in
+  ``local-test-paths`` in the ``[tool.omnidep]`` section described below,
+  otherwise omnidep treats it as regular code.
+* If you keep your test code "outside" your project, then either use the
+  ``--tests`` command-line option to locate it, or list it in
+  ``local-test-paths`` in ``[tool.omnidep]``, otherwise omnidep ignores it. You
+  also need to configure ``local-test-packages`` if some of your test files
+  import other test files, for example if you have shared helper functions.
+
+omnidep is configured using the ``pyproject.toml`` file, and specifically the
+``[tool.omnidep]`` section. Unrecognised keys are rejected and omnidep will not
+run (so, if you want to use a particular key then you should require at least
+the minimum version of omnidep that recognises it). The following config keys
+are recognised:
+
+ignore-imports
+^^^^^^^^^^^^^^
+
+Example: ``ignore-imports = ["X"]``
+
+Since: 0.2.0
+
+Causes omnidep to ignore all import statements from X, for example
+``import X``, ``from X.Y import Z``. omnidep will behave as if your code does
+not use package X, even if it does. X must be a top-level package. It is not
+currently possible to selectively ignore a sub-package (like X.Y), nor is it
+currently possible to ignore imports from some files but not others.
+
+child-packages
+^^^^^^^^^^^^^^
+
+Example: ``child-packages = {boto3 = ["botocore"]}``
+
+Since: 0.2.0
+
+Causes omnidep to consider a dependency on boto3 to also supply botocore. This
+saves you having to explictly list the child as a dependency of your project.
+You chould only do this when the child is inherant to the parent, not just
+because by chance you pull in a package you need via an indirect dependency.
+The reason is that indirect dependencies can change, and the project that you
+do depend on might not require the same version of the child that your usage
+requires. Only if the projects are closely related can you assume that the
+version you require of one will provide the features you need from the other.
+
+ignore-dependencies
+^^^^^^^^^^^^^^^^^^^
+
+Example: ``ignore-dependencies = ["X"]``
+
+Since: 0.2.0
+
+Causes omnidep to ignore the project X listed in your project's dependencies.
+omnidep will behave as if your project does not depend on X, even if it does.
+
+ignore-dependencies-order
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Example: ``ignore-dependencies-order = true``
+
+Since: 0.2.0
+
+Causes omnidep to skip the check that your dependencies are alphabetically
+ordered.
+
+ignore-dev-dependencies-order
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Example: ``ignore-dev-dependencies-order = true``
+
+Since: 0.2.0
+
+Causes omnidep to skip the check that your dev-dependencies are alphabetically
+ordered.
+
+local-test-paths
+^^^^^^^^^^^^^^^^
+
+Example: ``local-test-paths = ["myproject/tests/"]``
+
+Since: 0.2.0
+
+Causes omnidep to treat all code in ``myproject.tests`` as test code, meaning
+that anything it imports can be provided either by your projects dependencies
+or by its dev-dependencies. Imports from code that is not test code must be
+provided by non-dev dependencies.
+
+local-test-packages
+^^^^^^^^^^^^^^^^^^^
+
+Example: ``local-test-packages = ["tests"]``
+
+Since: 0.2.0
+
+Causes omnidep to treat ``tests`` as part of the current project, but only when
+considering imports that appear in test code. Use this when your test code is
+not shipped as part of your project.
+
+Error codes explained
+---------------------
+
+X, Y, P, Q, R, represent the names of imports or dependencies, depending on the
+message.
+
+ODEP001
+^^^^^^^
+
+| ``package 'X' is imported but not listed in dependencies``
+| ``package 'X' is imported but not listed in dev-dependencies``
+|
+
+X is the name you imported, which is not necessarily the same as the name of
+the project you have to install (for example the project ``beautifulsoup4``
+installs the package ``bs4``). omnidep does its best to find what project your
+desired package comes from, but if it fails, or if you don't have a suitable
+dependency, then this is the result.
+
+To fix, choose one of the following:
+
+* List the project name in your dependencies. If the package is used from test
+  code, then the dependency can be either dev or non-dev. If the package is
+  used from non-test code, then the dependency needs to be non-dev.
+* To ignore the import, add it to the list of ignored imports in your
+  ``[tool.omnidep]`` config, like ``ignore-imports = ["X"]``.
+* The package might come from a dependency of a dependency, and you might
+  prefer not to explicitly list it as a direct dependency too, so you can list
+  X as a child of some other dependency that you do list. You should only do
+  this when the indirect dependency is inherent to the direct dependency, for
+  example ``boto3`` provides ``botocore``. Add
+  ``child-packages = {something = ["X"]}`` to your ``[tool.omnidep]`` config,
+  meaning that the project named "something" provides "X", and so a dependency
+  on "something" is acceptable in place of a dependency on "X".
+
+ODEP002
+^^^^^^^
+
+``module 'X' is imported but not installed``
+
+Not only is there no dependency found that provides X, but X isn't even
+currently installed. omnidep relies on locally installed metadata to help it
+find what dependencies correspond to what imports.
+
+To fix, choose one of the following:
+
+* If your project has X as a dependency, but you haven't installed your
+  project then install your project, bringing in its dependencies.
+* Add a dependency that provides X.
+* Ignore the import by listing it in your in your ``[tool.omnidep]`` config,
+  like ``ignore-imports = ["X"]``.
+
+ODEP003
+^^^^^^^
+
+``Namespace package found: any of ['P', 'Q', 'R'] might provide 'X'``
+
+If projects P, Q, and R all provide code in the Python package X, then omnidep
+doesn't know which one you need in order to satisfy a given import. If you
+declare dependencies on all of them (that is, all the ones you currently have
+installed), then omnidep is satisfied. If you depend on some but not others,
+then you get this message.
+
+To fix, choose one of the following:
+
+* If you don't need the ones you don't declare dependencies on, and they are
+  installed accidentally, then uninstall them.
+* If appropriate, declare dependencies on all of P, Q, and R. However, this
+  might not be appropriate because P and Q might be genuine direct dependencies
+  of your code, whereas R was pulled in indirectly via something else. You
+  don't want to have to list indirect dependencies as direct dependencies.
+* Otherwise you have to resolve for yourself whether your dependencies are
+  adequate, then ignore the import with ``ignore-imports = ["X"]`` in your
+  ``[tool.omnidep]`` config.
+
+
+ODEP004
+^^^^^^^
+
+``Namespace package found: any of ['P', 'Q', 'R'] might provide 'X', and there are no dependencies on any of them``
+
+If projects P, Q, and R all provide code in the Python package X, then omnidep
+doesn't know which one you need in order to satisfy a given import. If you
+declare dependencies on all of them (that is, all the ones you currently have
+installed), then omnidep is satisfied. If you depend on none of them,
+then you get this message.
+
+To fix, choose one of the following:
+
+* If appropriate, declare dependencies on all of P, Q, and R. However, this
+  might not be appropriate because P and Q might be genuine direct dependencies
+  of your code, whereas R was pulled in indirectly via something else. You
+  don't want to have to list indirect dependencies as direct dependencies.
+* Otherwise you have to resolve for yourself whether your dependencies are
+  adequate, then ignore the import with ``ignore-imports = ["X"]`` in your
+  ``[tool.omnidep]`` config.
+
+
+ODEP005
+^^^^^^^
+
+``unused dependencies in project file: {'X', 'Y'}``
+
+omnidep expects you not to list any dependencies that you don't import. This
+might be completely legitimate, for example:
+
+* the dependency is a plugin to some framework and will be used via some means
+  other than an explicit ``import`` in your code;
+* you are controlling the version of an indirect dependency, to deal with
+  some problem caused by unexpected breaking changes.
+
+Unused dev-dependencies are always ignored, since they tend to include linters
+and suchlike.
+
+To fix, choose one of the following:
+
+* Remove the dependency.
+* List the dependency in your ``[tool.omnidep]`` config like
+  ``ignore-dependencies = ["X"]``.
+
+ODEP006
+^^^^^^^
+
+| ``dependencies are not sorted: 'Y' before 'X'``
+| ``dev-dependencies are not sorted: 'Y' before 'X'``
+|
+
+Ignoring ``python``, which is allowed to come first, omnidep expects you to
+list dependencies in case-insensitive alphabetical order within each section
+(dev and non-dev).
+
+To fix, choose one of the following:
+
+* List your dependencies alphabetically.
+* Set ``ignore-dependencies-order = true`` or
+  ``ignore-dev-dependencies-order = true`` in your ``[tool.omnidep]`` config.
+
+ODEP007
+^^^^^^^
+
+``dependency 'X' is not the preferred name: consider 'Y'``
+
+omnidep expects you to use either of two formats to name dependencies in your
+project file: the "Normalized Name" as defined in
+`PEP 503 <https://peps.python.org/pep-0503/>`_ or the name the dependency uses
+for itself in its metadata. Any name that normalizes to the same value will
+work, but inconsistent naming tends to lead to confusion, or to failing to find
+mentions when you search for them.
+
+To fix:
+
+* Use the name omnidep suggests, or the normalized name.
+
+ODEP008
+^^^^^^^
+
+``Module 'X' not under package management but found on python path``
+
+omnidep cannot find any project that provides X, but it is available to import.
+This can happen for example if you have set up the ``PYTHONPATH`` to find the
+code, instead of installing it as a dependency.
+
+To fix, choose one of the following:
+
+* If this is an error, list a suitable dependency.
+* If this occors when your test code is importing other modules also within
+  your test code (for example helper utilities) then you can configure
+  ``local-test-packages = ["X"]`` in your ``[tool.omnidep]`` config, and/or
+  ``local-test-paths`` with the location of the test source.
+* If you know what you're doing, and users of your project will know how to
+  supply the code that you're importing, then ignore the import with
+  ``ignore-imports = ["X"]`` in your ``[tool.omnidep]`` config.
+
+Changelog
+=========
+
+0.3.4
+-----
+* Report unused dependencies as a sorted list
+* Allow `python -m omnidep` (https://github.com/sjjessop/omnidep/issues/2)
+
+0.3.3
+-----
+
+* Treat local-test-paths config more like --tests option.
+* Non-zero exit code if there are any errors reported.
+* Documentation improvements.
+
+0.3.2
+-----
+
+* Read dev dependencies from the new location used by Poetry 1.2.0+
+* Add Python 3.11 to PyPI classifiers.
+
+0.3.1
+-----
+
+* Add Python 3.11 to the test matrix, and use separate badges in the README
+  for what is tagged on PyPI vs. what is tested.
+* Documentation improvements.
+* Uncap Python dependency. If Python ever reaches version 4, you are free to
+  install omnidep on it and see what happens!
+
+0.3.0
+-----
+
+* Breaking: When testing that dependencies are sorted, do it case-insensitive.
+* Deal with some build issues.
+
+0.2.1
+-----
+
+* Refer to online docs insted of long message in terminal.
+* Publish to PyPI.
+
+0.2.0
+-----
+
+* Minor documentation improvements.
+* Lower bounds for dependencies importlib-metadata, isort, and tomli.
+* CI test of the lower-bound versions.
 
-setup(**setup_kwargs)
```

