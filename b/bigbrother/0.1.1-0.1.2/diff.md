# Comparing `tmp/bigbrother-0.1.1.tar.gz` & `tmp/bigbrother-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbrother-0.1.1.tar", last modified: Thu Apr  6 03:03:35 2023, max compression
+gzip compressed data, was "bigbrother-0.1.2.tar", last modified: Fri Apr  7 20:15:46 2023, max compression
```

## Comparing `bigbrother-0.1.1.tar` & `bigbrother-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.391080 bigbrother-0.1.1/
--rw-r--r--   0 timkpaine   (501) staff       (20)      299 2023-04-06 03:02:35.000000 bigbrother-0.1.1/.bumpversion.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1920 2023-04-06 02:39:34.000000 bigbrother-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-06 02:39:34.000000 bigbrother-0.1.1/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      509 2023-04-06 02:39:34.000000 bigbrother-0.1.1/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     3323 2023-04-06 02:39:34.000000 bigbrother-0.1.1/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)    14476 2023-04-06 03:03:35.390920 bigbrother-0.1.1/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      631 2023-04-06 02:39:34.000000 bigbrother-0.1.1/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.388582 bigbrother-0.1.1/bigbrother/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1948 2023-04-06 03:02:35.000000 bigbrother-0.1.1/bigbrother/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.389755 bigbrother-0.1.1/bigbrother/builtins/
--rw-r--r--   0 timkpaine   (501) staff       (20)       94 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/builtins/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1167 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/builtins/dict.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1584 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/builtins/list.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1842 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/builtins/set.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      126 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/generic.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.389877 bigbrother-0.1.1/bigbrother/libraries/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/libraries/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.390064 bigbrother-0.1.1/bigbrother/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.390522 bigbrother-0.1.1/bigbrother/tests/builtins/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/builtins/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1188 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/builtins/test_dict.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1827 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/builtins/test_list.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1832 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/builtins/test_set.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      465 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/common.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.390722 bigbrother-0.1.1/bigbrother/tests/libraries/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.1/bigbrother/tests/libraries/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1700 2023-04-06 03:00:20.000000 bigbrother-0.1.1/bigbrother/tests/libraries/test_pydantic.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-06 03:03:35.389135 bigbrother-0.1.1/bigbrother.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)    14476 2023-04-06 03:03:35.000000 bigbrother-0.1.1/bigbrother.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      750 2023-04-06 03:03:35.000000 bigbrother-0.1.1/bigbrother.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-06 03:03:35.000000 bigbrother-0.1.1/bigbrother.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)      163 2023-04-06 03:03:35.000000 bigbrother-0.1.1/bigbrother.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-04-06 03:03:35.000000 bigbrother-0.1.1/bigbrother.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)     2170 2023-04-06 03:02:35.000000 bigbrother-0.1.1/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2023-04-06 03:03:35.391112 bigbrother-0.1.1/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)       39 2023-04-06 02:39:34.000000 bigbrother-0.1.1/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478933 bigbrother-0.1.2/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      299 2023-04-07 20:15:44.000000 bigbrother-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1920 2023-04-06 02:39:34.000000 bigbrother-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-06 02:39:34.000000 bigbrother-0.1.2/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      509 2023-04-06 02:39:34.000000 bigbrother-0.1.2/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3036 2023-04-07 19:12:10.000000 bigbrother-0.1.2/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)    15759 2023-04-07 20:15:46.478727 bigbrother-0.1.2/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1914 2023-04-07 19:12:14.000000 bigbrother-0.1.2/README.md
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.476199 bigbrother-0.1.2/bigbrother/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2355 2023-04-07 20:15:44.000000 bigbrother-0.1.2/bigbrother/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477305 bigbrother-0.1.2/bigbrother/builtins/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      189 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2471 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/dict.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3048 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/list.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3048 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/builtins/set.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      282 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/common.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      126 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/generic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477513 bigbrother-0.1.2/bigbrother/libraries/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/libraries/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1695 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/libraries/pydantic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.477708 bigbrother-0.1.2/bigbrother/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478152 bigbrother-0.1.2/bigbrother/tests/builtins/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/builtins/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1348 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_dict.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2083 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_list.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2088 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/builtins/test_set.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      465 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/common.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.478480 bigbrother-0.1.2/bigbrother/tests/libraries/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-04-06 02:39:34.000000 bigbrother-0.1.2/bigbrother/tests/libraries/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2457 2023-04-07 19:12:10.000000 bigbrother-0.1.2/bigbrother/tests/libraries/test_pydantic.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-07 20:15:46.476846 bigbrother-0.1.2/bigbrother.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)    15759 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      804 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)      163 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-04-07 20:15:46.000000 bigbrother-0.1.2/bigbrother.egg-info/top_level.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2170 2023-04-07 20:15:44.000000 bigbrother-0.1.2/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2023-04-07 20:15:46.478974 bigbrother-0.1.2/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)       39 2023-04-06 02:39:34.000000 bigbrother-0.1.2/setup.py
```

### Comparing `bigbrother-0.1.1/CONTRIBUTING.md` & `bigbrother-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.1/LICENSE` & `bigbrother-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbrother-0.1.1/Makefile` & `bigbrother-0.1.2/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 	python -m black --check bigbrother setup.py
 lint: lint-py  ## run all lints
 
 # Alias
 lints: lint
 
 fix-py:  ## fix python formatting with black
-	python -m ruff bigbrother/ setup.py --fix
 	python -m black bigbrother/ setup.py
+	python -m ruff bigbrother/ setup.py --fix
 fix: fix-py  ## run all autofixers
 
 # alias
 format: fix
 
 ################
 # Other Checks #
@@ -48,24 +48,19 @@
 	python -m mypy ./bigbrother
 
 semgrep: 
 
 #########
 # TESTS #
 #########
-test-py:  ## run python tests
+test:  ## run python tests
 	python -m pytest -v bigbrother/tests --junitxml=junit.xml
 
-coverage-py:  ## run tests and collect test coverage
-	python -m pytest -v bigbrother/tests --junitxml=junit.xml --cov=bigbrother --cov-report=xml:.coverage/coverage.xml --cov-report=html:.coverage/coverage.html --cov-branch --cov-fail-under=80 --cov-report term-missing
-
-show-coverage: coverage-py  ## show interactive python coverage viewer
-	cd .coverage && PYTHONBUFFERED=1 python -m http.server | sec -u "s/0\.0\.0\.0/$$(hostname)/g"
-
-test: test-py  ## run all tests
+coverage:  ## run tests and collect test coverage
+	python -m pytest -v bigbrother/tests --junitxml=junit.xml --cov=bigbrother --cov-branch --cov-fail-under=80 --cov-report term-missing
 
 # Alias
 tests: test
 
 ###########
 # VERSION #
 ###########
@@ -110,8 +105,8 @@
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build-py build-js build build install serverextension labextension lint-py lint-js lint-cpp lint lints fix-py fix-js fix-cpp fix format check-manifest checks check annotate semgrep test-py test-js coverage-py show-coverage test tests docs show-docs show-version patch minor major dist-py dist-py-sdist dist-py-local-wheel dist-check dist publish-py publish-js publish deep-clean clean help 
+.PHONY: develop build-py build-js build build install serverextension labextension lint-py lint-js lint-cpp lint lints fix-py fix-js fix-cpp fix format check-manifest checks check annotate semgrep test-py test-js coverage-py show-coverage test tests docs show-docs show-version patch minor major dist-py dist-py-sdist dist-py-local-wheel dist-check dist publish-py publish-js publish deep-clean clean help
```

### Comparing `bigbrother-0.1.1/PKG-INFO` & `bigbrother-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbrother
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for object observability
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -223,9 +223,67 @@
 License-File: LICENSE
 
 # bigbrother
 An evil, awful, terrible, no-good library for watching objects for mutation. Do not use this library.
 
 [![Build Status](https://github.com/timkpaine/bigbrother/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/bigbrother/actions?query=workflow%3A%22Build+Status%22)
 [![Coverage](https://codecov.io/gh/timkpaine/bigbrother/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/bigbrother)
-[![PyPI](https://img.shields.io/pypi/l/bigbrother.svg)](https://pypi.python.org/pypi/bigbrother)
+[![License](https://img.shields.io/github/license/timkpaine/bigbrother)](https://github.com/timkpaine/bigbrother)
 [![PyPI](https://img.shields.io/pypi/v/bigbrother.svg)](https://pypi.python.org/pypi/bigbrother)
+
+## Overview
+`bigbrother` is a mutation observer library. You can use it to watch your objects for changes. When your object changes, `bigbrother` will trigger your choice of callback. 
+
+
+```python
+x = {1: "a", 2: "b", 3: "c"}
+
+def track_changes(obj, method, *args, **kwargs):
+    print(f"method: {method}, args: {args}, kwargs: {kwargs}")
+
+x = watch(x, track_changes)
+
+x[1] = "x"
+
+# prints: method: setitem, args: (1, 'x'), kwargs: {}
+```
+
+`bigbrother` can also embed itself recursively in your object by passing in argument `deepstate=True`.
+
+
+## Supported types
+
+### Builtins
+Most builtin types are read-only and cannot have their method structure mutated, so we observe via replacement with thin wrappers. 
+
+- `list` via `_ObservedList`
+    - `append`
+    - `clear`
+    - `extend`
+    - `insert`
+    - `pop`
+    - `remove`
+    - `sort`
+    - `__setattr__`
+    - `__setitem__`
+- `dict` via `_ObservedDict`
+    - `clear`
+    - `pop`
+    - `popitem`
+    - `update`
+    - `__setattr__`
+    - `__setitem__`
+- `set` via `_ObservedSet`
+    - `add`
+    - `clear`
+    - `difference_update`
+    - `discard`
+    - `intersection_update`
+    - `pop`
+    - `remove`
+    - `symmetric_difference_update`
+    - `update`
+    - `__setattr__`
+
+
+### Libraries
+- `pydantic.BaseModel`
```

### Comparing `bigbrother-0.1.1/bigbrother/tests/builtins/test_list.py` & `bigbrother-0.1.2/bigbrother/tests/builtins/test_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,58 +8,66 @@
 
 
 class TestList:
     def test_list_append(self, a_list):
         instance, called = create_tester(a_list, "append", (1,), {})
         instance.append(1)
         assert called[0]
+        assert len(called) == 1
         assert instance == [1, 2, 3, 1]
 
     def test_list_clear(self, a_list):
         instance, called = create_tester(a_list, "clear", (), {})
         instance.clear()
         assert called[0]
+        assert len(called) == 1
         assert instance == []
 
     def test_list_extend(self, a_list):
         instance, called = create_tester(a_list, "extend", ([1, 2, 3],), {})
         instance.extend([1, 2, 3])
         assert called[0]
+        assert len(called) == 1
         assert instance == [1, 2, 3, 1, 2, 3]
 
     def test_list_insert(self, a_list):
         instance, called = create_tester(
             a_list,
             "insert",
             (
                 0,
                 1,
             ),
             {},
         )
         instance.insert(0, 1)
         assert called[0]
+        assert len(called) == 1
         assert instance == [1, 1, 2, 3]
 
     def test_list_pop(self, a_list):
         instance, called = create_tester(a_list, "pop", (0,), {})
         instance.pop(0)
         assert called[0]
+        assert len(called) == 1
         assert instance == [2, 3]
 
     def test_list_remove(self, a_list):
         instance, called = create_tester(a_list, "remove", (1,), {})
         instance.remove(1)
         assert called[0]
+        assert len(called) == 1
         assert instance == [2, 3]
 
     def test_list_sort(self, a_list):
         instance, called = create_tester(a_list, "sort", (), {})
         instance.sort()
         assert called[0]
+        assert len(called) == 1
         assert instance == [1, 2, 3]
 
     def test_list___setitem__(self, a_list):
         instance, called = create_tester(a_list, "setitem", (1, 4), {})
         instance[1] = 4
         assert called[0]
+        assert len(called) == 1
         assert instance == [1, 4, 3]
```

### Comparing `bigbrother-0.1.1/bigbrother/tests/builtins/test_set.py` & `bigbrother-0.1.2/bigbrother/tests/builtins/test_set.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,50 +8,58 @@
 
 
 class TestDict:
     def test_set_add(self, a_set):
         instance, called = create_tester(a_set, "add", (4,), {})
         instance.add(4)
         assert called[0]
+        assert len(called) == 1
         assert instance == {1, 2, 3, 4}
 
     def test_set_clear(self, a_set):
         instance, called = create_tester(a_set, "clear", (), {})
         instance.clear()
         assert called[0]
+        assert len(called) == 1
         assert instance == set()
 
     def test_set_difference_update(self, a_set):
         instance, called = create_tester(a_set, "difference_update", ({1, 2, 4},), {})
         instance.difference_update({1, 2, 4})
         assert called[0]
+        assert len(called) == 1
         assert instance == {3}
 
     def test_set_discard(self, a_set):
         instance, called = create_tester(a_set, "discard", (1,), {})
         instance.discard(1)
         assert called[0]
+        assert len(called) == 1
         assert instance == {2, 3}
 
     def test_set_intersection_update(self, a_set):
         instance, called = create_tester(a_set, "intersection_update", ({1, 3},), {})
         instance.intersection_update({1, 3})
         assert called[0]
+        assert len(called) == 1
         assert instance == {1, 3}
 
     def test_set_remove(self, a_set):
         instance, called = create_tester(a_set, "remove", (1,), {})
         instance.remove(1)
         assert called[0]
+        assert len(called) == 1
         assert instance == {2, 3}
 
     def test_set_symmetric_difference_update(self, a_set):
         instance, called = create_tester(a_set, "intersection_update", ({1, 3},), {})
         instance.intersection_update({1, 3})
         assert called[0]
+        assert len(called) == 1
         assert instance == {1, 3}
 
     def test_set_update(self, a_set):
         instance, called = create_tester(a_set, "update", ({4, 5},), {})
         instance.update({4, 5})
         assert called[0]
+        assert len(called) == 1
         assert instance == {1, 2, 3, 4, 5}
```

### Comparing `bigbrother-0.1.1/bigbrother/tests/libraries/test_pydantic.py` & `bigbrother-0.1.2/bigbrother/tests/libraries/test_pydantic.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,35 +35,62 @@
                 my_sub_model,
             ),
             {},
         )
         x.d = my_sub_model
 
         assert called[0]
+        assert len(called) == 1
         assert x.d == my_sub_model
 
     def test_pydantic_setattr_sub(self):
         my_sub_model = MySubModel()
         my_other_sub_model = MyOtherSubModel()
         x = MyModel(a=my_sub_model, b=my_other_sub_model)
 
         called = []
 
-        instance = x.d
+        instance = x
         method_name = "setitem"
         expected_args = ("x", [1])
         expected_kwargs = {}
 
         def track_changes(obj, method, *args, **kwargs):
             called.append(True)
             print(f"method: {method} args: {args} kwargs: {kwargs}")
             assert obj == instance
             assert method == method_name
             assert args == expected_args
             assert kwargs == expected_kwargs
 
-        x = watch(x, track_changes)
+        x = watch(x, track_changes, deepstate=True)
 
         x.d.x = [1]
 
         assert called[0]
+        assert len(called) == 1
         assert x.d.x == [1]
+
+    def test_pydantic_setattr_deep(self):
+        my_sub_model = MySubModel()
+        my_other_sub_model = MyOtherSubModel()
+        x = MyModel(a=my_sub_model, b=my_other_sub_model)
+
+        called = []
+
+        def track_changes(obj, method, *args, **kwargs):
+            called.append(True)
+            print(f"method: {method} args: {args} kwargs: {kwargs}")
+
+        x = watch(x, track_changes, deepstate=True)
+
+        x.d.x = [1]
+        x.d.x.append(2)
+        x.b.y["a"] = 1
+        x.e.append(1)
+
+        print(called)
+        assert x.d.x == [1, 2]
+        assert x.b.y == {"a": 1}
+        assert x.e == [1]
+        assert all(called)
+        assert len(called) == 4
```

### Comparing `bigbrother-0.1.1/bigbrother.egg-info/PKG-INFO` & `bigbrother-0.1.2/bigbrother.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbrother
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for object observability
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -223,9 +223,67 @@
 License-File: LICENSE
 
 # bigbrother
 An evil, awful, terrible, no-good library for watching objects for mutation. Do not use this library.
 
 [![Build Status](https://github.com/timkpaine/bigbrother/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/timkpaine/bigbrother/actions?query=workflow%3A%22Build+Status%22)
 [![Coverage](https://codecov.io/gh/timkpaine/bigbrother/branch/main/graph/badge.svg)](https://codecov.io/gh/timkpaine/bigbrother)
-[![PyPI](https://img.shields.io/pypi/l/bigbrother.svg)](https://pypi.python.org/pypi/bigbrother)
+[![License](https://img.shields.io/github/license/timkpaine/bigbrother)](https://github.com/timkpaine/bigbrother)
 [![PyPI](https://img.shields.io/pypi/v/bigbrother.svg)](https://pypi.python.org/pypi/bigbrother)
+
+## Overview
+`bigbrother` is a mutation observer library. You can use it to watch your objects for changes. When your object changes, `bigbrother` will trigger your choice of callback. 
+
+
+```python
+x = {1: "a", 2: "b", 3: "c"}
+
+def track_changes(obj, method, *args, **kwargs):
+    print(f"method: {method}, args: {args}, kwargs: {kwargs}")
+
+x = watch(x, track_changes)
+
+x[1] = "x"
+
+# prints: method: setitem, args: (1, 'x'), kwargs: {}
+```
+
+`bigbrother` can also embed itself recursively in your object by passing in argument `deepstate=True`.
+
+
+## Supported types
+
+### Builtins
+Most builtin types are read-only and cannot have their method structure mutated, so we observe via replacement with thin wrappers. 
+
+- `list` via `_ObservedList`
+    - `append`
+    - `clear`
+    - `extend`
+    - `insert`
+    - `pop`
+    - `remove`
+    - `sort`
+    - `__setattr__`
+    - `__setitem__`
+- `dict` via `_ObservedDict`
+    - `clear`
+    - `pop`
+    - `popitem`
+    - `update`
+    - `__setattr__`
+    - `__setitem__`
+- `set` via `_ObservedSet`
+    - `add`
+    - `clear`
+    - `difference_update`
+    - `discard`
+    - `intersection_update`
+    - `pop`
+    - `remove`
+    - `symmetric_difference_update`
+    - `update`
+    - `__setattr__`
+
+
+### Libraries
+- `pydantic.BaseModel`
```

### Comparing `bigbrother-0.1.1/bigbrother.egg-info/SOURCES.txt` & `bigbrother-0.1.2/bigbrother.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.py
 bigbrother/__init__.py
+bigbrother/common.py
 bigbrother/generic.py
 bigbrother.egg-info/PKG-INFO
 bigbrother.egg-info/SOURCES.txt
 bigbrother.egg-info/dependency_links.txt
 bigbrother.egg-info/requires.txt
 bigbrother.egg-info/top_level.txt
 bigbrother/builtins/__init__.py
 bigbrother/builtins/dict.py
 bigbrother/builtins/list.py
 bigbrother/builtins/set.py
 bigbrother/libraries/__init__.py
+bigbrother/libraries/pydantic.py
 bigbrother/tests/__init__.py
 bigbrother/tests/common.py
 bigbrother/tests/builtins/__init__.py
 bigbrother/tests/builtins/test_dict.py
 bigbrother/tests/builtins/test_list.py
 bigbrother/tests/builtins/test_set.py
 bigbrother/tests/libraries/__init__.py
```

### Comparing `bigbrother-0.1.1/pyproject.toml` & `bigbrother-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 name = "bigbrother"
 authors = [{name = "Tim Paine", email = "t.paine154@gmail.com"}]
 description="A library for object observability"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.8"
 keywords = ["observer", "observer-pattern"]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -53,25 +53,25 @@
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 [tool.black]
 color = true
-line-length = 120
+line-length = 160
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.check-manifest]
 ignore = [
 ]
 
 
 [tool.ruff]
-line-length = 120
+line-length = 160
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.isort]
 line_length = 120
 known_first_party = 'pydantic'
```

