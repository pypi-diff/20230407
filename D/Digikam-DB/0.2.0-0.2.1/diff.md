# Comparing `tmp/Digikam-DB-0.2.0.tar.gz` & `tmp/Digikam-DB-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digikam-DB-0.2.0.tar", last modified: Mon Apr  3 17:29:32 2023, max compression
+gzip compressed data, was "Digikam-DB-0.2.1.tar", last modified: Fri Apr  7 16:47:15 2023, max compression
```

## Comparing `Digikam-DB-0.2.0.tar` & `Digikam-DB-0.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.798212 Digikam-DB-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.802212 Digikam-DB-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/CHANGELOG.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.802212 Digikam-DB-0.2.0/Digikam_DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/Digikam_DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.802212 Digikam-DB-0.2.0/digikamdb/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 17:29:32.000000 Digikam-DB-0.2.0/digikamdb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/albumroots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/albums.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/image_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18067 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/image_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    23386 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/digikamdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/_ext/_sqla.py
--rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/_ext/digikam4.db
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/api_albums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/api_images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/api_tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/meta.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:29:32.806212 Digikam-DB-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/digikamrc.mysql
--rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/digikamrc.mysql-internal
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/digikamrc.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/empty.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/empty.tar.xz
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/testdb.sql.xz
--rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data/testdb.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/digikamrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/imagedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/newdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-03 17:29:22.000000 Digikam-DB-0.2.0/tests/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.700128 Digikam-DB-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.700128 Digikam-DB-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/CHANGELOG.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/Digikam_DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/Digikam_DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/digikamdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 16:47:15.000000 Digikam-DB-0.2.1/digikamdb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/albumroots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/image_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/image_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23386 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/digikamdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.704128 Digikam-DB-0.2.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/_ext/_sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/_ext/digikam4.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_albums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/api_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:47:15.708129 Digikam-DB-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.mysql
+-rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.mysql-internal
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/digikamrc.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/empty.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/empty.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/testdb.sql.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data/testdb.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/digikamrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/imagedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32756 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/newdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-07 16:47:04.000000 Digikam-DB-0.2.1/tests/sqlite.py
```

### Comparing `Digikam-DB-0.2.0/.github/workflows/release.yml` & `Digikam-DB-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/.github/workflows/test.yml` & `Digikam-DB-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/Digikam_DB.egg-info/PKG-INFO` & `Digikam-DB-0.2.1/Digikam_DB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.0/Digikam_DB.egg-info/SOURCES.txt` & `Digikam-DB-0.2.1/Digikam_DB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/LICENSE` & `Digikam-DB-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/PKG-INFO` & `Digikam-DB-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Digikam-DB
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to access Digikam metadata
 Author-email: rcw-2 <mail@rcw-2.de>
 Project-URL: documentation, https://digikam-db.readthedocs.io
 Project-URL: homepage, https://github.com/rcw-2/python-digikamdb
 Keywords: digikam
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `Digikam-DB-0.2.0/README.rst` & `Digikam-DB-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/albumroots.py` & `Digikam-DB-0.2.1/digikamdb/albumroots.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/albums.py` & `Digikam-DB-0.2.1/digikamdb/albums.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/conn.py` & `Digikam-DB-0.2.1/digikamdb/conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Defines the ``Digikam`` class for database access.
 """
 
 import logging
 import os
+import re
 from typing import Mapping, Optional, Union
 
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, declarative_base
 from sqlalchemy.ext.declarative import DeferredReflection
 
@@ -63,24 +64,29 @@
         database: Union[str, Engine],
         root_override: Optional[Mapping] = None,
         sql_echo: bool = False
     ):
         """
         Constructor
         """
-        log.info(
-            'Initializing Digikam object from %s',
-            database
-        )
         if isinstance(database, Engine):
+            log.info(
+                'Initializing Digikam object from %s',
+                database
+            )
             self._engine = database
         elif isinstance(database, str):
             if database == 'digikamrc':
+                log.info('Initializing Digikam object from digikamrc')
                 self._engine = Digikam.db_from_config(sql_echo = sql_echo)
             else:
+                log.info(
+                    'Initializing Digikam object from %s',
+                    re.sub(r':.*@', ':XXX@', database)
+                )
                 self._engine = create_engine(
                     database,
                     future = True,
                     echo = sql_echo)
         else:
             raise TypeError('Database specification must be Engine or str')
```

### Comparing `Digikam-DB-0.2.0/digikamdb/exceptions.py` & `Digikam-DB-0.2.1/digikamdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/image_comments.py` & `Digikam-DB-0.2.1/digikamdb/image_comments.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/image_helpers.py` & `Digikam-DB-0.2.1/digikamdb/image_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,17 +317,20 @@
         
         @property
         def digitizationDate(self) -> datetime:
             """The image's digitization date (read-only)"""
             return self._digitizationDate
         
         @property
-        def orientation(self) -> Orientation:
+        def orientation(self) -> Optional[Orientation]:
             """The image's orientation (read-only)"""
-            return Orientation(self._orientation)
+            if self._orientation:
+                return Orientation(self._orientation)
+            else:
+                return None
         
         @property
         def width(self) -> int:
             """The image's width (read-only)"""
             return self._width
         
         @property
@@ -342,17 +345,20 @@
         
         @property
         def colorDepth(self) -> int:
             """The image's color depth (read-only)"""
             return self._colorDepth
         
         @property
-        def colorModel(self) -> ColorModel:
+        def colorModel(self) -> Optional[ColorModel]:
             """The image's color model (read-only)"""
-            return ColorModel(self._colorModel)
+            if self._colorModel is None:
+                return None
+            else:
+                return ColorModel(self._colorModel)
         
         @validates('_orientation', '_colorModel')
         def _convert_to_int(self, key, value):
             return int(value)
     
     class ImageMetadata(dk.base):
         """
```

### Comparing `Digikam-DB-0.2.0/digikamdb/images.py` & `Digikam-DB-0.2.1/digikamdb/images.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/properties.py` & `Digikam-DB-0.2.1/digikamdb/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,28 @@
             self._session.add(self.Class(**attrs))
     
     def __iter__(self) -> Iterable:
         """Iterates over all properties of parent"""
         log.debug('%s: iterating over objects', self.__class__.__name__)
         yield from self._select_self()
     
+    def get(
+        self,
+        prop: Union[str, int, Sequence],
+        default: Any = None
+    ) -> str:
+        """
+        Works similar to :meth:`dict.get`.
+        """
+        ret = self._select_prop(prop).one_or_none()
+        if ret is None:
+            return default
+        else:
+            return self._post_process_value(ret)
+    
     def items(self) -> Iterable[Tuple]:
         """
         Returns the properties as an iterable yielding (key, value) tuples.
         """
         log.debug('%s: iterating over items', self.__class__.__name__)
         for row in self._select_self():
             if isinstance(self._key_col, str):
```

### Comparing `Digikam-DB-0.2.0/digikamdb/settings.py` & `Digikam-DB-0.2.1/digikamdb/settings.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/table.py` & `Digikam-DB-0.2.1/digikamdb/table.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/tags.py` & `Digikam-DB-0.2.1/digikamdb/tags.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/digikamdb/types.py` & `Digikam-DB-0.2.1/digikamdb/types.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/Makefile` & `Digikam-DB-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/_ext/_sqla.py` & `Digikam-DB-0.2.1/docs/_ext/_sqla.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/_ext/digikam4.db` & `Digikam-DB-0.2.1/docs/_ext/digikam4.db`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/api.rst` & `Digikam-DB-0.2.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/api_albums.rst` & `Digikam-DB-0.2.1/docs/api_albums.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/api_images.rst` & `Digikam-DB-0.2.1/docs/api_images.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/conf.py` & `Digikam-DB-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/intro.rst` & `Digikam-DB-0.2.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/docs/tutorial.rst` & `Digikam-DB-0.2.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/pyproject.toml` & `Digikam-DB-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/__init__.py` & `Digikam-DB-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/base.py` & `Digikam-DB-0.2.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/digikamrc.mysql` & `Digikam-DB-0.2.1/tests/data/digikamrc.mysql`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/digikamrc.mysql-internal` & `Digikam-DB-0.2.1/tests/data/digikamrc.mysql-internal`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/digikamrc.sqlite` & `Digikam-DB-0.2.1/tests/data/digikamrc.sqlite`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/empty.sql.xz` & `Digikam-DB-0.2.1/tests/data/empty.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/empty.tar.xz` & `Digikam-DB-0.2.1/tests/data/empty.tar.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/testdb.sql.xz` & `Digikam-DB-0.2.1/tests/data/testdb.sql.xz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data/testdb.tar.gz` & `Digikam-DB-0.2.1/tests/data/testdb.tar.gz`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/data.py` & `Digikam-DB-0.2.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/digikamrc.py` & `Digikam-DB-0.2.1/tests/digikamrc.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/imagedata.py` & `Digikam-DB-0.2.1/tests/imagedata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/mysql.py` & `Digikam-DB-0.2.1/tests/mysql.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/newdata.py` & `Digikam-DB-0.2.1/tests/newdata.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/sanity.py` & `Digikam-DB-0.2.1/tests/sanity.py`

 * *Files identical despite different names*

### Comparing `Digikam-DB-0.2.0/tests/sqlite.py` & `Digikam-DB-0.2.1/tests/sqlite.py`

 * *Files identical despite different names*

