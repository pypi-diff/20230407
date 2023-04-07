# Comparing `tmp/bobspdf-1.1.tar.gz` & `tmp/bobspdf-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bobspdf-1.1.tar", last modified: Fri Apr  7 18:23:35 2023, max compression
+gzip compressed data, was "bobspdf-1.2.tar", last modified: Fri Apr  7 18:37:28 2023, max compression
```

## Comparing `bobspdf-1.1.tar` & `bobspdf-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 18:23:35.831204 bobspdf-1.1/
-drwxrwxrwx   0        0        0        0 2023-04-07 18:23:35.761796 bobspdf-1.1/8bobspdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 23:20:17.000000 bobspdf-1.1/8bobspdf/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-06 23:21:22.000000 bobspdf-1.1/8bobspdf/pdf2image.py
--rw-rw-rw-   0        0        0       39 2023-04-06 23:23:27.000000 bobspdf-1.1/8bobspdf/pdf2text.py
--rw-rw-rw-   0        0        0    35821 2023-04-07 04:23:19.000000 bobspdf-1.1/LICENSE
--rw-rw-rw-   0        0        0      115 2023-04-07 18:23:35.824211 bobspdf-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-04-07 03:27:31.000000 bobspdf-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 18:23:35.812209 bobspdf-1.1/bobspdf.egg-info/
--rw-rw-rw-   0        0        0      115 2023-04-07 18:23:35.000000 bobspdf-1.1/bobspdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-07 18:23:35.000000 bobspdf-1.1/bobspdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 18:23:35.000000 bobspdf-1.1/bobspdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 18:23:35.000000 bobspdf-1.1/bobspdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 18:23:35.832206 bobspdf-1.1/setup.cfg
--rw-rw-rw-   0        0        0      246 2023-04-07 18:14:18.000000 bobspdf-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:37:28.973146 bobspdf-1.2/
+-rw-rw-rw-   0        0        0    35821 2023-04-07 04:23:19.000000 bobspdf-1.2/LICENSE
+-rw-rw-rw-   0        0        0      115 2023-04-07 18:37:28.965140 bobspdf-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2023-04-07 03:27:31.000000 bobspdf-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 18:37:28.872145 bobspdf-1.2/bobspdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 23:20:17.000000 bobspdf-1.2/bobspdf/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-06 23:21:22.000000 bobspdf-1.2/bobspdf/pdf2image.py
+-rw-rw-rw-   0        0        0       39 2023-04-06 23:23:27.000000 bobspdf-1.2/bobspdf/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-04-07 18:37:28.956140 bobspdf-1.2/bobspdf.egg-info/
+-rw-rw-rw-   0        0        0      115 2023-04-07 18:37:28.000000 bobspdf-1.2/bobspdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-07 18:37:28.000000 bobspdf-1.2/bobspdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 18:37:28.000000 bobspdf-1.2/bobspdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-07 18:37:28.000000 bobspdf-1.2/bobspdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 18:37:28.974141 bobspdf-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      246 2023-04-07 18:35:57.000000 bobspdf-1.2/setup.py
```

### Comparing `bobspdf-1.1/LICENSE` & `bobspdf-1.2/LICENSE`

 * *Files identical despite different names*

