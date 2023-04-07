# Comparing `tmp/importlib_metadata-6.1.0.tar.gz` & `tmp/importlib_metadata-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.1.0.tar", last modified: Sat Mar 18 17:10:38 2023, max compression
+gzip compressed data, was "importlib_metadata-6.2.0.tar", last modified: Fri Apr  7 17:13:17 2023, max compression
```

## Comparing `importlib_metadata-6.1.0.tar` & `importlib_metadata-6.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.770994 importlib_metadata-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.762994 importlib_metadata-6.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.762994 importlib_metadata-6.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20188 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-18 17:10:38.770994 importlib_metadata-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    26518 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-18 17:10:38.000000 importlib_metadata-6.1.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-18 17:10:38.000000 importlib_metadata-6.1.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 17:10:38.000000 importlib_metadata-6.1.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-18 17:10:38.000000 importlib_metadata-6.1.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-18 17:10:38.000000 importlib_metadata-6.1.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.758994 importlib_metadata-6.1.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.766994 importlib_metadata-6.1.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-18 17:10:38.770994 importlib_metadata-6.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.770994 importlib_metadata-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:38.770994 importlib_metadata-6.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-18 17:10:20.000000 importlib_metadata-6.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    26518 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tox.ini
```

### Comparing `importlib_metadata-6.1.0/.github/workflows/main.yml` & `importlib_metadata-6.2.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -126,14 +129,16 @@
           python -m pip install tox
       - name: Evaluate coverage
         run: tox
         env:
           TOXENV: diffcov
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `importlib_metadata-6.1.0/CHANGES.rst` & `importlib_metadata-6.2.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v6.2.0
+======
+
+* #384: ``PackageMetadata`` now stipulates an additional ``get``
+  method allowing for easy querying of metadata keys that may not
+  be present.
+
 v6.1.0
 ======
 
 * #428: ``packages_distributions`` now honors packages and modules
   with Python modules that not ``.py`` sources (e.g. ``.pyc``,
   ``.so``).
```

### Comparing `importlib_metadata-6.1.0/LICENSE` & `importlib_metadata-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/PKG-INFO` & `importlib_metadata-6.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.1.0
+Version: 6.2.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.1.0/README.rst` & `importlib_metadata-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/conftest.py` & `importlib_metadata-6.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/docs/conf.py` & `importlib_metadata-6.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/docs/index.rst` & `importlib_metadata-6.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/docs/migration.rst` & `importlib_metadata-6.2.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/docs/using.rst` & `importlib_metadata-6.2.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/exercises.py` & `importlib_metadata-6.2.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/__init__.py` & `importlib_metadata-6.2.0/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.2.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_collections.py` & `importlib_metadata-6.2.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_compat.py` & `importlib_metadata-6.2.0/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_functools.py` & `importlib_metadata-6.2.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.2.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.2.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata/_text.py` & `importlib_metadata-6.2.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.2.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.1.0
+Version: 6.2.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.1.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.2.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/pytest.ini` & `importlib_metadata-6.2.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/setup.cfg` & `importlib_metadata-6.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.2.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.2.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.2.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/fixtures.py` & `importlib_metadata-6.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/test_api.py` & `importlib_metadata-6.2.0/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,28 @@
         """
         Requesting a missing key will still return None, but warn.
         """
         md = metadata('distinfo-pkg')
         with suppress_known_deprecation():
             assert md['does-not-exist'] is None
 
+    def test_get_key(self):
+        """
+        Getting a key gets the key.
+        """
+        md = metadata('egginfo-pkg')
+        assert md.get('Name') == 'egginfo-pkg'
+
+    def test_get_missing_key(self):
+        """
+        Requesting a missing key will return None.
+        """
+        md = metadata('distinfo-pkg')
+        assert md.get('does-not-exist') is None
+
     @staticmethod
     def _test_files(files):
         root = files[0].root
         for file in files:
             assert file.root == root
             assert not file.hash or file.hash.value
             assert not file.hash or file.hash.mode == 'sha256'
```

### Comparing `importlib_metadata-6.1.0/tests/test_integration.py` & `importlib_metadata-6.2.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/test_main.py` & `importlib_metadata-6.2.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/test_py39compat.py` & `importlib_metadata-6.2.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tests/test_zip.py` & `importlib_metadata-6.2.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.1.0/tox.ini` & `importlib_metadata-6.2.0/tox.ini`

 * *Files identical despite different names*

