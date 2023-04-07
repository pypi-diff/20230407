# Comparing `tmp/pytokei-0.1.2.tar.gz` & `tmp/pytokei-0.2.0.tar.gz`

## Comparing `pytokei-0.1.2.tar` & `pytokei-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 pytokei-0.1.2/Cargo.toml
--rw-r--r--   0     1001      121     5101 2022-11-02 17:52:49.000000 pytokei-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0     1001      121     1853 2022-11-02 17:52:49.000000 pytokei-0.1.2/.gitignore
--rw-r--r--   0     1001      121      616 2022-11-02 17:52:49.000000 pytokei-0.1.2/CHANGELOG.md
--rw-r--r--   0     1001      121     1061 2022-11-02 17:52:49.000000 pytokei-0.1.2/LICENSE
--rw-r--r--   0     1001      121      294 2022-11-02 17:52:49.000000 pytokei-0.1.2/Makefile
--rw-r--r--   0     1001      121     3245 2022-11-02 17:52:49.000000 pytokei-0.1.2/README.md
--rw-r--r--   0     1001      121      130 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/Dockerfile.python
--rw-r--r--   0     1001      121      503 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/README.md
--rw-r--r--   0     1001      121      751 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/bench.rs
--rw-r--r--   0     1001      121      259 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/bench_py.sh
--rw-r--r--   0     1001      121      117 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/bench_rs.sh
--rw-r--r--   0     1001      121      105 2022-11-02 17:52:49.000000 pytokei-0.1.2/bench/run_dockerfile_py.sh
--rw-r--r--   0     1001      121      117 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/config.md
--rw-r--r--   0     1001      121      120 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/language.md
--rw-r--r--   0     1001      121      128 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/language_type.md
--rw-r--r--   0     1001      121      121 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/languages.md
--rw-r--r--   0     1001      121       58 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/sort.md
--rw-r--r--   0     1001      121      164 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/api/stats.md
--rw-r--r--   0     1001      121     2393 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/index.md
--rw-r--r--   0     1001      121     6465 2022-11-02 17:52:49.000000 pytokei-0.1.2/docs/usage.md
--rw-r--r--   0     1001      121     1515 2022-11-02 17:52:49.000000 pytokei-0.1.2/mkdocs.yml
--rw-r--r--   0     1001      121     1125 2022-11-02 17:52:49.000000 pytokei-0.1.2/pyproject.toml
--rw-r--r--   0     1001      121      322 2022-11-02 17:52:49.000000 pytokei-0.1.2/pytokei/__init__.py
--rw-r--r--   0     1001      121    16559 2022-11-02 17:52:49.000000 pytokei-0.1.2/pytokei/_pytokei.pyi
--rw-r--r--   0     1001      121        0 2022-11-02 17:52:49.000000 pytokei-0.1.2/pytokei/py.typed
--rw-r--r--   0     1001      121       47 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/all.txt
--rw-r--r--   0     1001      121       43 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/docs.in
--rw-r--r--   0     1001      121     1584 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/docs.txt
--rw-r--r--   0     1001      121       16 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/linting.in
--rw-r--r--   0     1001      121      526 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/linting.txt
--rw-r--r--   0     1001      121        6 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/test.in
--rw-r--r--   0     1001      121      395 2022-11-02 17:52:49.000000 pytokei-0.1.2/requirements/test.txt
--rw-r--r--   0     1001      121      897 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/lib.rs
--rw-r--r--   0     1001      121     1350 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pyconfig.rs
--rw-r--r--   0     1001      121     3283 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pylanguage.rs
--rw-r--r--   0     1001      121    14300 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pylanguage_type.rs
--rw-r--r--   0     1001      121     4274 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pylanguages.rs
--rw-r--r--   0     1001      121      994 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pysort.rs
--rw-r--r--   0     1001      121     3586 2022-11-02 17:52:49.000000 pytokei-0.1.2/src/pystats.rs
--rw-r--r--   0     1001      121      330 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/data/Dockerfile
--rw-r--r--   0     1001      121      313 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/data/configs/tokei.example.toml
--rw-r--r--   0     1001      121      225 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/data/python1.py
--rw-r--r--   0     1001      121      249 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/data/python2.py
--rw-r--r--   0     1001      121      838 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/data/rust.rs
--rw-r--r--   0     1001      121    12125 2022-11-02 17:52:49.000000 pytokei-0.1.2/tests/test_pytokei.py
--rw-r--r--   0     1001      121    36225 2022-11-02 17:54:35.000000 pytokei-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     4294 1970-01-01 00:00:00.000000 pytokei-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 pytokei-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     5101 2023-04-07 18:15:17.000000 pytokei-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1853 2023-04-07 18:15:17.000000 pytokei-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      682 2023-04-07 18:15:17.000000 pytokei-0.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     1061 2023-04-07 18:15:17.000000 pytokei-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      294 2023-04-07 18:15:17.000000 pytokei-0.2.0/Makefile
+-rw-r--r--   0     1001      123     4726 2023-04-07 18:15:17.000000 pytokei-0.2.0/README.md
+-rw-r--r--   0     1001      123      130 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/Dockerfile.python
+-rw-r--r--   0     1001      123      503 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/README.md
+-rw-r--r--   0     1001      123      751 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/bench.rs
+-rw-r--r--   0     1001      123      259 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/bench_py.sh
+-rw-r--r--   0     1001      123      117 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/bench_rs.sh
+-rw-r--r--   0     1001      123      105 2023-04-07 18:15:17.000000 pytokei-0.2.0/bench/run_dockerfile_py.sh
+-rw-r--r--   0     1001      123      117 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/config.md
+-rw-r--r--   0     1001      123      120 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/language.md
+-rw-r--r--   0     1001      123      128 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/language_type.md
+-rw-r--r--   0     1001      123      121 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/languages.md
+-rw-r--r--   0     1001      123       58 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/sort.md
+-rw-r--r--   0     1001      123      164 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/api/stats.md
+-rw-r--r--   0     1001      123    89048 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/assets/pytokei-help.png
+-rw-r--r--   0     1001      123    38636 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/assets/pytokei-itself.png
+-rw-r--r--   0     1001      123    32151 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/assets/pytokei-no-color.png
+-rw-r--r--   0     1001      123      578 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/cli.md
+-rw-r--r--   0     1001      123     2539 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/index.md
+-rw-r--r--   0     1001      123     6465 2023-04-07 18:15:17.000000 pytokei-0.2.0/docs/usage.md
+-rw-r--r--   0     1001      123     1533 2023-04-07 18:15:17.000000 pytokei-0.2.0/mkdocs.yml
+-rw-r--r--   0     1001      123     1254 2023-04-07 18:15:17.000000 pytokei-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      397 2023-04-07 18:15:17.000000 pytokei-0.2.0/pytokei/__init__.py
+-rw-r--r--   0     1001      123    16559 2023-04-07 18:15:17.000000 pytokei-0.2.0/pytokei/_pytokei.pyi
+-rw-r--r--   0     1001      123     3796 2023-04-07 18:15:17.000000 pytokei-0.2.0/pytokei/cli.py
+-rw-r--r--   0     1001      123        0 2023-04-07 18:15:17.000000 pytokei-0.2.0/pytokei/py.typed
+-rw-r--r--   0     1001      123       47 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/all.txt
+-rw-r--r--   0     1001      123       43 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/docs.in
+-rw-r--r--   0     1001      123     1584 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/docs.txt
+-rw-r--r--   0     1001      123       16 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/linting.in
+-rw-r--r--   0     1001      123      526 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/linting.txt
+-rw-r--r--   0     1001      123        6 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/test.in
+-rw-r--r--   0     1001      123      406 2023-04-07 18:15:17.000000 pytokei-0.2.0/requirements/test.txt
+-rw-r--r--   0     1001      123      897 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     1350 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pyconfig.rs
+-rw-r--r--   0     1001      123     3283 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pylanguage.rs
+-rw-r--r--   0     1001      123    14300 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pylanguage_type.rs
+-rw-r--r--   0     1001      123     4274 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pylanguages.rs
+-rw-r--r--   0     1001      123      994 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pysort.rs
+-rw-r--r--   0     1001      123     3586 2023-04-07 18:15:17.000000 pytokei-0.2.0/src/pystats.rs
+-rw-r--r--   0     1001      123      330 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/data/Dockerfile
+-rw-r--r--   0     1001      123      313 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/data/configs/tokei.example.toml
+-rw-r--r--   0     1001      123      225 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/data/python1.py
+-rw-r--r--   0     1001      123      249 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/data/python2.py
+-rw-r--r--   0     1001      123      838 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/data/rust.rs
+-rw-r--r--   0     1001      123    12147 2023-04-07 18:15:17.000000 pytokei-0.2.0/tests/test_pytokei.py
+-rw-r--r--   0     1001      123    36225 2023-04-07 18:15:17.000000 pytokei-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 pytokei-0.2.0/PKG-INFO
```

### Comparing `pytokei-0.1.2/.github/workflows/ci.yml` & `pytokei-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/.gitignore` & `pytokei-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/CHANGELOG.md` & `pytokei-0.2.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Future changes
 
 Here should be the updates to the project. As they are completed they will be added to the next version.
 
 - Add `pre-commit` to lint and format.
 
+
+# 0.2.0
+
+Added a small CLI to run the program from the console.
+
 # 0.1.2
 
 Fixed:
     - `PyLanguages.report_compact_plain` now counts correctly the
     summarised languages.
```

### Comparing `pytokei-0.1.2/LICENSE` & `pytokei-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/README.md` & `pytokei-0.2.0/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,21 @@
 # pytokei
+Pytokei is a python binding to [tokei](https://github.com/XAMPPRocky/tokei), from their repo:
+
 ---
-Pytokei is a python binding to [tokei](https://github.com/XAMPPRocky/tokei):
 
 <p align="center">
-    Tokei is a program that displays statistics about your code. Tokei will show the number of files, total lines within those files and code, comments, and blanks grouped by language.
+Tokei is a program that displays statistics about your code. Tokei will show the number of files, total lines within those files and code, comments, and blanks grouped by language.
 </p>
 
 --- 
 
 This wrapper allows to obtain the same reports directly from python.
 
-```python
-$ python
->>> import pytokei
->>> from rich import print
->>> langs = pytokei.Languages()
->>> langs.get_statistics(["."], ["tests/data", "requirements"], pytokei.Config())
->>> print(langs.report_compact_plain())
-{
-    'YAML': {'blanks': 6, 'code': 63, 'comments': 0, 'files': 1, 'lines': 69},
-    'Python': {'lines': 376, 'blanks': 89, 'files': 2, 'code': 280, 'comments': 7},
-    'Makefile': {'code': 18, 'lines': 26, 'comments': 0, 'blanks': 8, 'files': 1},
-    'Markdown': {'code': 0, 'blanks': 37, 'files': 10, 'comments': 52, 'lines': 89},
-    'Rust': {'blanks': 23, 'comments': 23, 'code': 317, 'lines': 363, 'files': 7},
-    'TOML': {'code': 14, 'comments': 2, 'lines': 20, 'blanks': 4, 'files': 2}
-}
-```
-
-For more information about `tokei`, please visit the original repo.
-
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytokei.svg)](https://pypi.org/project/pytokei/)
-![example workflow](https://github.com/plaguss/pytokei/actions/workflows/ci.yml/badge.svg)
-[![license](https://img.shields.io/github/license/plaguss/pytokei.svg)](https://github.com/plaguss/pytokei/blob/main/LICENSE)
-
+For more information about `tokei`, please visit its [repo](https://github.com/XAMPPRocky/tokei).
 
 ## Installation
 
 ```bash
 pip install pytokei
 ```
 
@@ -46,27 +25,19 @@
 
 * **Linux**: `x86_64`, `aarch64`, `i686`, `armv7l`, `musl-x86_64` & `musl-aarch64`
 * **MacOS**: `x86_64` & `arm64` (except python 3.7)
 * **Windows**: `amd64` & `win32`
 
 Otherwise, you can install from source which requires Rust stable to be installed.
 
-## Why this library?
-
-Wanted to practice rust, and taking this library to python seemed like a good opportunity. It's awesome, and maybe more people coming from python will find something useful to do with it.
-
-But really? Just for fun :)
-
-## [Documentation](https://plaguss.github.io/pytokei/)
-
-## What times should you expect?
-
-Running `Languages.get_statistics` against [cpython](https://github.com/python/cpython) takes a little less than 200 milliseconds.
+To use the CLI, install with the needed dependencies (maybe with [`pipx`](https://github.com/pypa/pipx)).
 
-Some more info should be found in the [docs](https://plaguss.github.io/pytokei/#time-comparison-tokei-and-pytokei).
+```bash
+pipx install pytokei[cli]
+```
 
 ## Development
 
 You will need:
 
 - [maturin](https://www.maturin.rs/installation.html) to compile the library
 
@@ -74,12 +45,36 @@
 
 From python side:
 
 Run `make install-dev` inside a virtual environment, `make test`, `make mypy` and `make format` to ensure everything is as expected, and `make docs` to build the documentation.
 
 *There are some problems when building the docs with mkdocstrings, a reminder is in the following [github issue](https://github.com/mkdocstrings/mkdocstrings/issues/404). For the moment, it seems that the best option is to remove the .so file and build the docs without it.*
 
-To create a new release:
+## Time comparison `tokei` and `pytokei`
+
+Just to see if the binding makes the code slower, a test was done against the [cpython](https://github.com/python/cpython) repository.
+
+*The timing isn't directly comparable, Rust's version prints the average time, while Python's version shows the minimum, but it should be enough to get an idea. A better test should be defined in the future.*
+
+The python version uses `docker`. A print like the following should appear:
 
-- Update the version in [Cargo.toml](./Cargo.toml).
-- Create a new tag to run the github action workflow.
-- git push --atomic origin main tag-name 
+```bash
+$ sh run_dockerfile_py.sh
+...
+Successfully tagged bench_from_pytokei:latest
+==================
+Timing python run:
+------------------
+100 loops, best of 1: 194 msec per loop
+==================
+```
+
+The rust version needs [rust-script](https://rust-script.org/) installed.
+
+```bash
+$ sh bench_rs.sh         
+================
+Timing rust run:
+----------------
+100 loops, average time was: 0.17748523967000002 sec
+================
+```
```

### Comparing `pytokei-0.1.2/bench/bench.rs` & `pytokei-0.2.0/bench/bench.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/docs/usage.md` & `pytokei-0.2.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/mkdocs.yml` & `pytokei-0.2.0/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             merge_init_into_class: true
             show_signature_annotations: true
             separate_signature: true
 
 nav:
     - Intro: index.md
     - Usage: usage.md
+    - CLI: cli.md
     - API:
         - api/config.md
         - api/language_type.md
         - api/language.md
         - api/languages.md
         - api/sort.md
         - api/stats.md
```

### Comparing `pytokei-0.1.2/pyproject.toml` & `pytokei-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ['maturin>=0.13,<0.14']
+requires = ['maturin>=0.14,<0.15']
 build-backend = 'maturin'
 
 [project]
 name = 'pytokei'
 requires-python = '>=3.7'
 description = 'Python bindings to tokei, the Rust library to count code quickly.'
 authors = [
@@ -20,14 +20,23 @@
     'Operating System :: POSIX :: Linux',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS',
     'Topic :: Software Development :: Libraries :: Python Modules'
 ]
 description-file = "README.md"
 
+[project.optional-dependencies]
+cli = [
+    "typer>=0.7.0",
+    "rich>=13.3.0"
+]
+
+[project.scripts]
+pytokei = "pytokei.cli:app"
+
 [project.urls]
 Homepage = 'https://github.com/plaguss/pytokei'
 Documentation = 'https://plaguss.github.io/pytokei/'
 Source = 'https://github.com/plaguss/pytokei'
 
 [tool.maturin]
 bindings = 'pyo3'
```

### Comparing `pytokei-0.1.2/pytokei/_pytokei.pyi` & `pytokei-0.2.0/pytokei/_pytokei.pyi`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/requirements/docs.txt` & `pytokei-0.2.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/requirements/linting.txt` & `pytokei-0.2.0/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/lib.rs` & `pytokei-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pyconfig.rs` & `pytokei-0.2.0/src/pyconfig.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pylanguage.rs` & `pytokei-0.2.0/src/pylanguage.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pylanguage_type.rs` & `pytokei-0.2.0/src/pylanguage_type.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pylanguages.rs` & `pytokei-0.2.0/src/pylanguages.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pysort.rs` & `pytokei-0.2.0/src/pysort.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/src/pystats.rs` & `pytokei-0.2.0/src/pystats.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/tests/data/rust.rs` & `pytokei-0.2.0/tests/data/rust.rs`

 * *Files identical despite different names*

### Comparing `pytokei-0.1.2/tests/test_pytokei.py` & `pytokei-0.2.0/tests/test_pytokei.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,8 +369,10 @@
 
     def test_languages_default_report_plain(self, languages):
         report = languages.report_compact_plain()
         lang_names = ["TOML", "Dockerfile", "Python", "Rust"]
         stats = ["files", "lines", "code", "comments", "blanks"]
         values_dockerfile = [1, 16, 7, 3, 6]
         assert all([name in report.keys() for name in lang_names])
-        assert all([report["Dockerfile"][k] == v for k, v in zip(stats, values_dockerfile)])
+        assert all(
+            [report["Dockerfile"][k] == v for k, v in zip(stats, values_dockerfile)]
+        )
```

### Comparing `pytokei-0.1.2/Cargo.lock` & `pytokei-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -851,15 +851,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytokei"
-version = "0.1.2"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "tokei",
 ]
 
 [[package]]
 name = "quote"
```

