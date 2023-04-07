# Comparing `tmp/python_ftp_server-1.3.8.tar.gz` & `tmp/python_ftp_server-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ftp_server-1.3.8.tar", max compression
+gzip compressed data, was "python_ftp_server-1.3.9.tar", last modified: Wed Oct 12 10:19:09 2022, max compression
```

## Comparing `python_ftp_server-1.3.8.tar` & `python_ftp_server-1.3.9.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0      951 2022-07-27 08:25:44.037257 python_ftp_server-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      117 2021-11-29 08:48:16.562934 python_ftp_server-1.3.8/python_ftp_server/__init__.py
--rw-r--r--   0        0        0      203 2021-12-01 17:34:43.306152 python_ftp_server-1.3.8/python_ftp_server/__main__.py
--rw-r--r--   0        0        0     4602 2022-07-27 08:23:00.102546 python_ftp_server-1.3.8/python_ftp_server/ftp_server.py
--rw-r--r--   0        0        0      476 2021-12-01 18:21:10.373181 python_ftp_server-1.3.8/README.md
--rw-r--r--   0        0        0     1083 2022-07-27 08:30:55.860877 python_ftp_server-1.3.8/setup.py
--rw-r--r--   0        0        0     1627 2022-07-27 08:30:55.860877 python_ftp_server-1.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-12 10:19:09.021538 python_ftp_server-1.3.9/
+-rw-rw-rw-   0        0        0      503 2022-10-12 10:19:09.022483 python_ftp_server-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2021-12-01 18:21:10.000000 python_ftp_server-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-12 10:19:09.003993 python_ftp_server-1.3.9/python_ftp_server/
+-rw-rw-rw-   0        0        0      117 2021-11-29 08:48:16.000000 python_ftp_server-1.3.9/python_ftp_server/__init__.py
+-rw-rw-rw-   0        0        0      203 2021-12-01 17:34:43.000000 python_ftp_server-1.3.9/python_ftp_server/__main__.py
+-rw-rw-rw-   0        0        0     4602 2022-07-27 08:23:00.000000 python_ftp_server-1.3.9/python_ftp_server/ftp_server.py
+drwxrwxrwx   0        0        0        0 2022-10-12 10:19:09.019480 python_ftp_server-1.3.9/python_ftp_server.egg-info/
+-rw-rw-rw-   0        0        0      503 2022-10-12 10:19:08.000000 python_ftp_server-1.3.9/python_ftp_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2022-10-12 10:19:08.000000 python_ftp_server-1.3.9/python_ftp_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-12 10:19:08.000000 python_ftp_server-1.3.9/python_ftp_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2022-10-12 10:19:08.000000 python_ftp_server-1.3.9/python_ftp_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2022-10-12 10:19:08.000000 python_ftp_server-1.3.9/python_ftp_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2022-10-12 10:19:09.023951 python_ftp_server-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0       37 2022-10-12 10:14:36.000000 python_ftp_server-1.3.9/setup.py
```

### Comparing `python_ftp_server-1.3.8/python_ftp_server/ftp_server.py` & `python_ftp_server-1.3.9/python_ftp_server/ftp_server.py`

 * *Files identical despite different names*

