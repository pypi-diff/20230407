# Comparing `tmp/pysmells-1.0.1.tar.gz` & `tmp/pysmells-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.1.tar", last modified: Thu Jan 12 09:20:18 2023, max compression
+gzip compressed data, was "pysmells-1.0.2.tar", last modified: Fri Apr  7 21:02:43 2023, max compression
```

## Comparing `pysmells-1.0.1.tar` & `pysmells-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 09:20:18.354280 pysmells-1.0.1/
--rw-rw-rw-   0        0        0     1133 2023-01-05 01:08:53.000000 pysmells-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      517 2023-01-12 09:20:18.353281 pysmells-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-01-12 08:03:48.000000 pysmells-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 09:20:18.331294 pysmells-1.0.1/pysmells/
--rw-rw-rw-   0        0        0       19 2023-01-12 08:16:38.000000 pysmells-1.0.1/pysmells/__init__.py
--rw-rw-rw-   0        0        0     1582 2022-12-28 21:35:26.000000 pysmells-1.0.1/pysmells/data_processing.py
--rw-rw-rw-   0        0        0     1182 2023-01-12 09:12:50.000000 pysmells-1.0.1/pysmells/main.py
-drwxrwxrwx   0        0        0        0 2023-01-12 09:20:18.352284 pysmells-1.0.1/pysmells.egg-info/
--rw-rw-rw-   0        0        0      517 2023-01-12 09:20:18.000000 pysmells-1.0.1/pysmells.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-01-12 09:20:18.000000 pysmells-1.0.1/pysmells.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 09:20:18.000000 pysmells-1.0.1/pysmells.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-01-12 09:20:18.000000 pysmells-1.0.1/pysmells.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-12 09:20:18.000000 pysmells-1.0.1/pysmells.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-12 09:20:18.354280 pysmells-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-01-12 09:18:08.000000 pysmells-1.0.1/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-07 21:02:43.528782 pysmells-1.0.2/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 19:20:52.000000 pysmells-1.0.2/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1520 2023-04-07 21:02:43.528088 pysmells-1.0.2/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      691 2023-04-07 19:14:25.000000 pysmells-1.0.2/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-07 21:02:43.520550 pysmells-1.0.2/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 18:55:25.000000 pysmells-1.0.2/pysmells/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-07 21:02:43.527064 pysmells-1.0.2/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1520 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      241 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-07 21:02:43.000000 pysmells-1.0.2/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-07 21:02:43.529037 pysmells-1.0.2/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1213 2023-04-07 21:02:02.000000 pysmells-1.0.2/setup.py
```

### Comparing `pysmells-1.0.1/LICENSE` & `pysmells-1.0.2/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-Copyright (c) 2023 Marco Aurélio Proença Neto, Marcos Paulo Alves de Souza
-
- Permission is hereby granted, free of charge, to any person obtaining a copy
- of this software and associated documentation files (the "Software"), to deal
- in the Software without restriction, including without limitation the rights
- to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
- copies of the Software, and to permit persons to whom the Software is
- furnished to do so, subject to the following conditions:
-
- The above copyright notice and this permission notice shall be included in
- all copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
- IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
- FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
- AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
- LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
- OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
- THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Marcos Paulo Alves de Sousa e Marco Aurélio Proença Neto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

