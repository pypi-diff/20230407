# Comparing `tmp/hdmf-3.5.2.tar.gz` & `tmp/hdmf-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdmf-3.5.2.tar", last modified: Tue Mar 14 17:43:26 2023, max compression
+gzip compressed data, was "hdmf-3.5.4.tar", last modified: Fri Apr  7 20:40:59 2023, max compression
```

## Comparing `hdmf-3.5.2.tar` & `hdmf-3.5.4.tar`

### file list

```diff
@@ -1,220 +1,158 @@
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.473903 hdmf-3.5.2/
--rw-r--r--   0 mavaylon   (501) staff       (20)      838 2023-02-25 18:27:20.000000 hdmf-3.5.2/Legal.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      206 2023-02-23 17:02:20.000000 hdmf-3.5.2/MANIFEST.in
--rw-r--r--   0 mavaylon   (501) staff       (20)     7774 2023-03-14 17:43:26.474072 hdmf-3.5.2/PKG-INFO
--rw-r--r--   0 mavaylon   (501) staff       (20)     6728 2023-02-25 18:27:20.000000 hdmf-3.5.2/README.rst
--rw-r--r--   0 mavaylon   (501) staff       (20)     2407 2023-02-25 18:27:20.000000 hdmf-3.5.2/license.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      321 2023-02-23 17:02:20.000000 hdmf-3.5.2/requirements-dev.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      207 2023-02-23 17:02:20.000000 hdmf-3.5.2/requirements-doc.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      390 2023-03-13 16:04:51.000000 hdmf-3.5.2/requirements-min.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      566 2023-03-13 16:04:51.000000 hdmf-3.5.2/requirements.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)      760 2023-03-14 17:43:26.474918 hdmf-3.5.2/setup.cfg
--rwxr-xr-x   0 mavaylon   (501) staff       (20)     2348 2023-02-23 17:02:20.000000 hdmf-3.5.2/setup.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.316042 hdmf-3.5.2/src/
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.475264 hdmf-3.5.2/src/hdmf/
--rw-r--r--   0 mavaylon   (501) staff       (20)     1613 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2018 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/_due.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      497 2023-03-14 17:43:26.475354 hdmf-3.5.2/src/hdmf/_version.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     5420 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/array.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.346515 hdmf-3.5.2/src/hdmf/backends/
--rw-r--r--   0 mavaylon   (501) staff       (20)       19 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/backends/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)       87 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/backends/errors.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.348816 hdmf-3.5.2/src/hdmf/backends/hdf5/
--rw-r--r--   0 mavaylon   (501) staff       (20)      135 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/backends/hdf5/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    23735 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/backends/hdf5/h5_utils.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    72886 2023-03-13 16:04:51.000000 hdmf-3.5.2/src/hdmf/backends/hdf5/h5tools.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     5947 2023-02-25 18:27:20.000000 hdmf-3.5.2/src/hdmf/backends/io.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     4517 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/backends/utils.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      116 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/backends/warnings.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.354835 hdmf-3.5.2/src/hdmf/build/
--rw-r--r--   0 mavaylon   (501) staff       (20)      604 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    17265 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/builders.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    20440 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/classgenerator.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2208 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/errors.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    39613 2023-03-13 16:04:51.000000 hdmf-3.5.2/src/hdmf/build/manager.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      394 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/map.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    65654 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/objectmapper.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      907 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/build/warnings.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.362488 hdmf-3.5.2/src/hdmf/common/
--rw-r--r--   0 mavaylon   (501) staff       (20)     8877 2023-03-13 22:46:27.000000 hdmf-3.5.2/src/hdmf/common/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    22928 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/common/alignedtable.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.317338 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.368892 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/
--rw-r--r--   0 mavaylon   (501) staff       (20)      644 2023-02-23 17:02:21.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/base.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)      429 2023-02-23 17:02:21.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/experimental.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)     1264 2023-02-23 17:02:21.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/namespace.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)     2779 2023-03-06 16:16:15.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/resources.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)      921 2023-02-23 17:02:21.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/sparse.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)     6652 2023-02-23 17:02:21.000000 hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/table.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)    14523 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/hierarchicaltable.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.372005 hdmf-3.5.2/src/hdmf/common/io/
--rw-r--r--   0 mavaylon   (501) staff       (20)      147 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/io/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      602 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/io/alignedtable.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      949 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/io/multi.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     1764 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/io/resources.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     7878 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/io/table.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      832 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/multi.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    44284 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/common/resources.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2834 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/common/sparse.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    73500 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/common/table.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    47444 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/container.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    49488 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/data_utils.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2238 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/monitor.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     6322 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/query.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2710 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/region.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.376530 hdmf-3.5.2/src/hdmf/spec/
--rw-r--r--   0 mavaylon   (501) staff       (20)      302 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/spec/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     9280 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/spec/catalog.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    24617 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/spec/namespace.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    60591 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/spec/spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    11148 2023-03-06 16:15:34.000000 hdmf-3.5.2/src/hdmf/spec/write.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.379468 hdmf-3.5.2/src/hdmf/testing/
--rw-r--r--   0 mavaylon   (501) staff       (20)      113 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/testing/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    17977 2023-02-25 18:27:20.000000 hdmf-3.5.2/src/hdmf/testing/testcase.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      451 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/testing/utils.py
--rwxr-xr-x   0 mavaylon   (501) staff       (20)     1794 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/testing/validate_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    48832 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/utils.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.381357 hdmf-3.5.2/src/hdmf/validate/
--rw-r--r--   0 mavaylon   (501) staff       (20)      158 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/validate/__init__.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     8899 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/validate/errors.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    28044 2023-02-23 17:02:20.000000 hdmf-3.5.2/src/hdmf/validate/validator.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.343546 hdmf-3.5.2/src/hdmf.egg-info/
--rw-r--r--   0 mavaylon   (501) staff       (20)     7774 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/PKG-INFO
--rw-r--r--   0 mavaylon   (501) staff       (20)     8234 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/SOURCES.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)        1 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/dependency_links.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)       71 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/entry_points.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)        1 2023-02-23 17:02:33.000000 hdmf-3.5.2/src/hdmf.egg-info/not-zip-safe
--rw-r--r--   0 mavaylon   (501) staff       (20)      116 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/requires.txt
--rw-r--r--   0 mavaylon   (501) staff       (20)        5 2023-03-14 17:43:26.000000 hdmf-3.5.2/src/hdmf.egg-info/top_level.txt
--rwxr-xr-x   0 mavaylon   (501) staff       (20)     5107 2023-02-23 17:02:20.000000 hdmf-3.5.2/test.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.382315 hdmf-3.5.2/tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.382653 hdmf-3.5.2/tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      142 2023-03-02 23:42:28.000000 hdmf-3.5.2/tests/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.389581 hdmf-3.5.2/tests/unit/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.397722 hdmf-3.5.2/tests/unit/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      147 2023-03-02 23:42:28.000000 hdmf-3.5.2/tests/unit/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    25391 2023-03-13 16:05:34.000000 hdmf-3.5.2/tests/unit/__pycache__/test_container.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     8321 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/__pycache__/test_io_hdf5.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)   118184 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/__pycache__/test_io_hdf5_h5tools.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    21693 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/__pycache__/test_multicontainerinterface.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     5532 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/__pycache__/test_query.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     4879 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/__pycache__/test_table.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    20296 2023-03-02 23:42:30.000000 hdmf-3.5.2/tests/unit/__pycache__/utils.cpython-39.pyc
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.399751 hdmf-3.5.2/tests/unit/back_compat_tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)    18000 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/back_compat_tests/1.0.5.h5
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/back_compat_tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.400922 hdmf-3.5.2/tests/unit/back_compat_tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      165 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/back_compat_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     2277 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/back_compat_tests/__pycache__/test_1_1_0.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     1906 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/back_compat_tests/test_1_1_0.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.405912 hdmf-3.5.2/tests/unit/build_tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.414111 hdmf-3.5.2/tests/unit/build_tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      159 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    17114 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_builder.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    34562 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_classgenerator.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    17775 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_convert_dtype.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    13266 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_io_manager.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    31920 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_io_map.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    16151 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/__pycache__/test_io_map_data.cpython-39-pytest-7.1.2.pyc
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.416899 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.420038 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      172 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    17715 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/__pycache__/test_build.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    30383 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/__pycache__/test_build_quantity.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    23395 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/test_build.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    46424 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/mapper_tests/test_build_quantity.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    14154 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/test_builder.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    47400 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/test_classgenerator.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    25679 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/test_convert_dtype.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    13994 2023-03-13 16:04:51.000000 hdmf-3.5.2/tests/unit/build_tests/test_io_manager.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    41135 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/test_io_map.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    19803 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/build_tests/test_io_map_data.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.427446 hdmf-3.5.2/tests/unit/common/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.435787 hdmf-3.5.2/tests/unit/common/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      154 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    26368 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_alignedtable.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)      857 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_common.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     4633 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_common_io.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     8157 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_generate_table.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    23845 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_linkedtables.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     1024 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_multi.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    23911 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_resources.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     7945 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_sparse.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)   100808 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/common/__pycache__/test_table.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    33128 2023-03-06 16:15:34.000000 hdmf-3.5.2/tests/unit/common/test_alignedtable.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      399 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_common.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     3647 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_common_io.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    11531 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_generate_table.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    48786 2023-03-06 16:15:34.000000 hdmf-3.5.2/tests/unit/common/test_linkedtables.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      558 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_multi.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    36063 2023-03-13 22:46:27.000000 hdmf-3.5.2/tests/unit/common/test_resources.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     8393 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_sparse.py
--rw-r--r--   0 mavaylon   (501) staff       (20)   110730 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/common/test_table.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.444759 hdmf-3.5.2/tests/unit/spec_tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.451632 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      158 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     3639 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_attribute_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     8333 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_dataset_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     4702 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_dtype_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    23419 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_group_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     2476 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_link_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    13498 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_load_namespace.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     1309 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_ref_spec.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     6710 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_spec_catalog.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     7754 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/spec_tests/__pycache__/test_spec_write.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)      392 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test-ext.base.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)      301 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test-ext.namespace.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)      382 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test.base.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)      345 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test.namespace.yaml
--rw-r--r--   0 mavaylon   (501) staff       (20)     3787 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_attribute_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    11458 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_dataset_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     3360 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_dtype_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    32100 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_group_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2227 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_link_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    16604 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_load_namespace.py
--rw-r--r--   0 mavaylon   (501) staff       (20)      702 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_ref_spec.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    10378 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_spec_catalog.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     8145 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/spec_tests/test_spec_write.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    24297 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/test_container.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     8952 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/test_io_hdf5.py
--rw-r--r--   0 mavaylon   (501) staff       (20)   147101 2023-03-13 22:46:27.000000 hdmf-3.5.2/tests/unit/test_io_hdf5_h5tools.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    19807 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/test_multicontainerinterface.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     4744 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/test_query.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     4040 2023-03-06 16:15:34.000000 hdmf-3.5.2/tests/unit/test_table.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    21544 2023-02-25 18:27:20.000000 hdmf-3.5.2/tests/unit/utils.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.458325 hdmf-3.5.2/tests/unit/utils_test/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.469180 hdmf-3.5.2/tests/unit/utils_test/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      158 2023-03-13 16:05:38.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     1866 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_core_DataChunk.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    16272 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_core_DataChunkIterator.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     3336 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_core_DataIO.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    16807 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_core_GenericDataChunkIterator.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     8670 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_core_ShapeValidator.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    51984 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_docval.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    12941 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_labelleddict.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     8089 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/utils_test/__pycache__/test_utils.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     1154 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_core_DataChunk.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    18929 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_core_DataChunkIterator.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     2386 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_core_DataIO.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    16200 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_core_GenericDataChunkIterator.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     9171 2023-03-06 16:15:34.000000 hdmf-3.5.2/tests/unit/utils_test/test_core_ShapeValidator.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    49444 2023-03-13 16:04:51.000000 hdmf-3.5.2/tests/unit/utils_test/test_docval.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    10605 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_labelleddict.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     7047 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/utils_test/test_utils.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.470961 hdmf-3.5.2/tests/unit/validator_tests/
--rw-r--r--   0 mavaylon   (501) staff       (20)        0 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/validator_tests/__init__.py
-drwxr-xr-x   0 mavaylon   (501) staff       (20)        0 2023-03-14 17:43:26.473202 hdmf-3.5.2/tests/unit/validator_tests/__pycache__/
--rw-r--r--   0 mavaylon   (501) staff       (20)      163 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/validator_tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     3040 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/validator_tests/__pycache__/test_errors.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)    46995 2023-03-13 16:05:39.000000 hdmf-3.5.2/tests/unit/validator_tests/__pycache__/test_validate.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 mavaylon   (501) staff       (20)     2203 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/validator_tests/test_errors.py
--rw-r--r--   0 mavaylon   (501) staff       (20)    52983 2023-02-23 17:02:20.000000 hdmf-3.5.2/tests/unit/validator_tests/test_validate.py
--rw-r--r--   0 mavaylon   (501) staff       (20)     4845 2023-02-23 17:02:20.000000 hdmf-3.5.2/tox.ini
--rw-r--r--   0 mavaylon   (501) staff       (20)    83607 2023-02-23 17:02:20.000000 hdmf-3.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.680945 hdmf-3.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-07 20:39:25.000000 hdmf-3.5.4/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 20:39:25.000000 hdmf-3.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 20:40:59.680945 hdmf-3.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-07 20:39:25.000000 hdmf-3.5.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-07 20:39:25.000000 hdmf-3.5.4/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 20:40:59.680945 hdmf-3.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-04-07 20:39:25.000000 hdmf-3.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.660944 hdmf-3.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.680945 hdmf-3.5.4/src/hdmf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/_due.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 20:40:59.680945 hdmf-3.5.4/src/hdmf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.664944 hdmf-3.5.4/src/hdmf/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/backends/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/h5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72886 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/h5tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/classgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65654 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/objectmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/alignedtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.660944 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/experimental.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/sparse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/hierarchicaltable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/alignedtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73532 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47444 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49701 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24617 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60591 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/validate_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48832 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.664944 hdmf-3.5.4/src/hdmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:39:53.000000 hdmf-3.5.4/src/hdmf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-04-07 20:39:25.000000 hdmf-3.5.4/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/back_compat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/1.0.5.h5
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/test_1_1_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/build_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46424 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48994 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_classgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25679 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_convert_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_map_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33128 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_alignedtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_common_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_generate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_linkedtables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36063 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110730 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/spec_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test-ext.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test-ext.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_attribute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_dataset_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_dtype_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32100 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_group_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_link_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_load_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_ref_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_spec_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_spec_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_io_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147101 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_io_hdf5_h5tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_multicontainerinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21544 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunkIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_GenericDataChunkIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_ShapeValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49444 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_docval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_labelleddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/validator_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52983 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-07 20:39:25.000000 hdmf-3.5.4/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-07 20:39:25.000000 hdmf-3.5.4/versioneer.py
```

### Comparing `hdmf-3.5.2/Legal.txt` & `hdmf-3.5.4/Legal.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/PKG-INFO` & `hdmf-3.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: hdmf
-Version: 3.5.2
+Version: 3.5.4
 Summary: A package for standardizing hierarchical object data
 Home-page: https://github.com/hdmf-dev/hdmf
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `hdmf-3.5.2/README.rst` & `hdmf-3.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/license.txt` & `hdmf-3.5.4/license.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/requirements.txt` & `hdmf-3.5.4/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # pinned dependencies to reproduce an entire development environment to use HDMF
-# note that python 3.7 end of life is 27 Jun 2023
-h5py==3.7.0
+h5py==3.8.0
 jsonschema==4.9.1
 numpy==1.23.3;python_version>='3.8'
 numpy==1.21.5;python_version<'3.8'  # note that numpy 1.22 dropped python 3.7 support
 pandas==1.5.0;python_version>='3.8'
 pandas==1.3.5;python_version<'3.8'  # note that pandas 1.4 dropped python 3.7 support
 ruamel.yaml==0.17.21
 scipy==1.9.3;python_version>='3.8'
```

### Comparing `hdmf-3.5.2/setup.cfg` & `hdmf-3.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/setup.py` & `hdmf-3.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 pkgs = find_packages('src', exclude=['data'])
 print('found these packages:', pkgs)
 
 schema_dir = 'common/hdmf-common-schema/common'
 
 reqs = [
-    'h5py>=2.10,<4',
-    'jsonschema>=2.6.0,<5',
-    'numpy>=1.16,<1.24',
-    'pandas>=1.0.5,<2',
-    'ruamel.yaml>=0.16,<1',
-    'scipy>=1.1,<2',
+    'h5py>=2.10',
+    'jsonschema>=2.6.0',
+    'numpy>=1.16',
+    'pandas>=1.0.5',
+    'ruamel.yaml>=0.16',
+    'scipy>=1.1',
     'setuptools',
 ]
 
 print(reqs)
 
 setup_args = {
     'name': 'hdmf',
@@ -47,14 +47,15 @@
     'python_requires': '>=3.7',
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
```

### Comparing `hdmf-3.5.2/src/hdmf/__init__.py` & `hdmf-3.5.4/src/hdmf/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/_due.py` & `hdmf-3.5.4/src/hdmf/_due.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/array.py` & `hdmf-3.5.4/src/hdmf/array.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/backends/hdf5/h5_utils.py` & `hdmf-3.5.4/src/hdmf/backends/hdf5/h5_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/backends/hdf5/h5tools.py` & `hdmf-3.5.4/src/hdmf/backends/hdf5/h5tools.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/backends/io.py` & `hdmf-3.5.4/src/hdmf/backends/io.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/backends/utils.py` & `hdmf-3.5.4/src/hdmf/backends/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/__init__.py` & `hdmf-3.5.4/src/hdmf/build/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/builders.py` & `hdmf-3.5.4/src/hdmf/build/builders.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/classgenerator.py` & `hdmf-3.5.4/src/hdmf/build/classgenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,14 +403,19 @@
                     new_kwarg = dict(
                         attr_name=attr_name,
                         value=popargs(attr_name, kwargs),
                         add_method_name=add_method_name
                     )
                     new_kwargs.append(new_kwarg)
 
+                    # pass an empty list to previous_init in case attr_name field is required
+                    # (one or many). we do not want previous_init to set the attribute directly.
+                    # instead, we will use the add_method after previous_init is finished.
+                    kwargs[attr_name] = list()
+
                 # call the parent class init without the MCI attribute
                 previous_init(self, **kwargs)
 
                 # call the add method for each MCI attribute
                 for new_kwarg in new_kwargs:
                     add_method = getattr(self, new_kwarg['add_method_name'])
                     add_method(new_kwarg['value'])
```

### Comparing `hdmf-3.5.2/src/hdmf/build/errors.py` & `hdmf-3.5.4/src/hdmf/build/errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/manager.py` & `hdmf-3.5.4/src/hdmf/build/manager.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/objectmapper.py` & `hdmf-3.5.4/src/hdmf/build/objectmapper.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/build/warnings.py` & `hdmf-3.5.4/src/hdmf/build/warnings.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/__init__.py` & `hdmf-3.5.4/src/hdmf/common/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/alignedtable.py` & `hdmf-3.5.4/src/hdmf/common/alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/base.yaml` & `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/base.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/namespace.yaml` & `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/namespace.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/resources.yaml` & `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/resources.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/sparse.yaml` & `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/sparse.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hdmf-common-schema/common/table.yaml` & `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/table.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/hierarchicaltable.py` & `hdmf-3.5.4/src/hdmf/common/hierarchicaltable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/io/alignedtable.py` & `hdmf-3.5.4/src/hdmf/common/io/alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/io/multi.py` & `hdmf-3.5.4/src/hdmf/common/io/multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/io/resources.py` & `hdmf-3.5.4/src/hdmf/common/io/resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/io/table.py` & `hdmf-3.5.4/src/hdmf/common/io/table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/multi.py` & `hdmf-3.5.4/src/hdmf/common/multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/resources.py` & `hdmf-3.5.4/src/hdmf/common/resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/sparse.py` & `hdmf-3.5.4/src/hdmf/common/sparse.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/common/table.py` & `hdmf-3.5.4/src/hdmf/common/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -988,15 +988,15 @@
         for k in coldata:  # for each column
             if isinstance(coldata[k], (np.ndarray, list, tuple, pd.DataFrame)):
                 # wrap in a list because coldata[k] may be an array/list/tuple with multiple elements (ragged or
                 # multi-dim column) and pandas needs to have one element per index row (=1 in this case)
                 df_input[k] = [coldata[k]]
             else:  # scalar, don't wrap
                 df_input[k] = coldata[k]
-        ret = pd.DataFrame(df_input, index=pd.Index(name=self.id.name, data=id_index))
+        ret = pd.DataFrame(df_input, index=pd.Index(name=self.id.name, data=id_index, dtype=np.int64))
         ret.name = self.name
         return ret
 
     def __get_selection_as_df(self, coldata):
         """Return a pandas dataframe for the given rows and columns with the id column as the index.
 
         This is used when multiple row indices are selected (or a list/array/slice of a single index is passed to get).
@@ -1013,15 +1013,15 @@
             elif isinstance(coldata[k], pd.DataFrame):
                 # multiple rows were selected and collapsed into a dataframe
                 # split up the rows of the df into a list of dataframes, one per row
                 # TODO make this more efficient
                 df_input[k] = [coldata[k].iloc[[i]] for i in range(len(coldata[k]))]
             else:
                 df_input[k] = coldata[k]
-        ret = pd.DataFrame(df_input, index=pd.Index(name=self.id.name, data=id_index))
+        ret = pd.DataFrame(df_input, index=pd.Index(name=self.id.name, data=id_index, dtype=np.int64))
         ret.name = self.name
         return ret
 
     def __contains__(self, val):
         """
         Check if the given value (i.e., column) exists in this table
         """
```

### Comparing `hdmf-3.5.2/src/hdmf/container.py` & `hdmf-3.5.4/src/hdmf/container.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/data_utils.py` & `hdmf-3.5.4/src/hdmf/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import math
-import functools  # TODO: remove when Python 3.7 support is dropped
+import functools  # TODO: remove when Python 3.7 support is dropped - see #785
 import operator  # TODO: remove when Python 3.7 support is dropped
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable
 from warnings import warn
 from typing import Tuple
 from itertools import product, chain
 
@@ -233,15 +233,17 @@
             for chunk_axis, buffer_axis, maxshape_axis in zip(self.chunk_shape, self.buffer_shape, self.maxshape)
             if buffer_axis != maxshape_axis
         ), (
             f"Some dimensions of chunk_shape ({self.chunk_shape}) do not "
             f"evenly divide the buffer shape ({self.buffer_shape})!"
         )
 
-        self.num_buffers = functools.reduce(  # TODO: replace with math.prod when Python 3.7 support is dropped
+        # TODO: replace with below when Python 3.7 support is dropped
+        # self.num_buffers = math.prod(
+        self.num_buffers = functools.reduce(
             operator.mul,
             [
                 math.ceil(maxshape_axis / buffer_axis)
                 for buffer_axis, maxshape_axis in zip(self.buffer_shape, self.maxshape)
             ],
             1,
         )
@@ -305,19 +307,22 @@
 
         n_dims = len(self.maxshape)
         itemsize = self.dtype.itemsize
         chunk_bytes = chunk_mb * 1e6
 
         min_maxshape = min(self.maxshape)
         v = tuple(math.floor(maxshape_axis / min_maxshape) for maxshape_axis in self.maxshape)
-        prod_v = functools.reduce(operator.mul, v, 1)  # TODO: replace with math.prod when Python 3.7 support is dropped
+        # TODO: replace with below when Python 3.7 support is dropped
+        # prod_v = math.prod(v)
+        prod_v = functools.reduce(operator.mul, v, 1)
         while prod_v * itemsize > chunk_bytes and prod_v != 1:
             non_unit_min_v = min(x for x in v if x != 1)
             v = tuple(math.floor(x / non_unit_min_v) if x != 1 else x for x in v)
-            # TODO: replace with math.prod when Python 3.7 support is dropped
+            # TODO: replace with below when Python 3.7 support is dropped
+            # prod_v = math.prod(v)
             prod_v = functools.reduce(operator.mul, v, 1)
         k = math.floor((chunk_bytes / (prod_v * itemsize)) ** (1 / n_dims))
         return tuple([min(k * x, self.maxshape[dim]) for dim, x in enumerate(v)])
 
     @docval(
         dict(
             name="buffer_gb",
@@ -335,17 +340,18 @@
         """
         buffer_gb = getargs("buffer_gb", kwargs)
         assert buffer_gb > 0, f"buffer_gb ({buffer_gb}) must be greater than zero!"
         assert all(chunk_axis > 0 for chunk_axis in self.chunk_shape), (
             f"Some dimensions of chunk_shape ({self.chunk_shape}) are less than zero!"
         )
 
-        # TODO: replace with math.prod when Python 3.7 support is dropped
         k = math.floor(
             (
+                # TODO: replace with below when Python 3.7 support is dropped
+                # buffer_gb * 1e9 / (math.prod(self.chunk_shape) * self.dtype.itemsize)
                 buffer_gb * 1e9 / (functools.reduce(operator.mul, self.chunk_shape, 1) * self.dtype.itemsize)
             ) ** (1 / len(self.chunk_shape))
         )
         return tuple(
             [
                 min(max(k * x, self.chunk_shape[j]), self.maxshape[j])
                 for j, x in enumerate(self.chunk_shape)
```

### Comparing `hdmf-3.5.2/src/hdmf/monitor.py` & `hdmf-3.5.4/src/hdmf/monitor.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/query.py` & `hdmf-3.5.4/src/hdmf/query.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/region.py` & `hdmf-3.5.4/src/hdmf/region.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/spec/catalog.py` & `hdmf-3.5.4/src/hdmf/spec/catalog.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/spec/namespace.py` & `hdmf-3.5.4/src/hdmf/spec/namespace.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/spec/spec.py` & `hdmf-3.5.4/src/hdmf/spec/spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/spec/write.py` & `hdmf-3.5.4/src/hdmf/spec/write.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/testing/testcase.py` & `hdmf-3.5.4/src/hdmf/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/testing/validate_spec.py` & `hdmf-3.5.4/src/hdmf/testing/validate_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/utils.py` & `hdmf-3.5.4/src/hdmf/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/validate/errors.py` & `hdmf-3.5.4/src/hdmf/validate/errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf/validate/validator.py` & `hdmf-3.5.4/src/hdmf/validate/validator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/src/hdmf.egg-info/PKG-INFO` & `hdmf-3.5.4/src/hdmf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: hdmf
-Version: 3.5.2
+Version: 3.5.4
 Summary: A package for standardizing hierarchical object data
 Home-page: https://github.com/hdmf-dev/hdmf
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
```

### Comparing `hdmf-3.5.2/test.py` & `hdmf-3.5.4/test.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/back_compat_tests/1.0.5.h5` & `hdmf-3.5.4/tests/unit/back_compat_tests/1.0.5.h5`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/back_compat_tests/test_1_1_0.py` & `hdmf-3.5.4/tests/unit/back_compat_tests/test_1_1_0.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/mapper_tests/test_build.py` & `hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/mapper_tests/test_build_quantity.py` & `hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build_quantity.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_builder.py` & `hdmf-3.5.4/tests/unit/build_tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_classgenerator.py` & `hdmf-3.5.4/tests/unit/build_tests/test_classgenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         )
         assert multi.data == list(range(10))
         assert multi.attr1 == 'value1'
         assert multi.attr2 == 10
         assert multi.bars['my_bar'] == Bar(name='my_bar', data=list(range(10)), attr1='value1', attr2=10)
         assert multi.attr3 == 5.
 
-    def test_multi_container_spec_optional(self):
+    def test_multi_container_spec_zero_or_more(self):
         multi_spec = GroupSpec(
             doc='A test extension that contains a multi',
             data_type_def='Multi',
             groups=[
                 GroupSpec(data_type_inc=self.bar_spec, doc='test multi', quantity='*')
             ],
             attributes=[
@@ -387,14 +387,53 @@
         Multi = self.type_map.get_dt_container_cls('Multi', CORE_NAMESPACE)
         multi = Multi(
             name='my_multi',
             attr3=5.
         )
         assert len(multi.bars) == 0
 
+    def test_multi_container_spec_one_or_more_missing(self):
+        multi_spec = GroupSpec(
+            doc='A test extension that contains a multi',
+            data_type_def='Multi',
+            groups=[
+                GroupSpec(data_type_inc=self.bar_spec, doc='test multi', quantity='+')
+            ],
+            attributes=[
+                AttributeSpec(name='attr3', doc='a float attribute', dtype='float')
+            ]
+        )
+        self.spec_catalog.register_spec(multi_spec, 'extension.yaml')
+        Multi = self.type_map.get_dt_container_cls('Multi', CORE_NAMESPACE)
+        with self.assertRaisesWith(TypeError, "MCIClassGenerator.set_init.<locals>.__init__: missing argument 'bars'"):
+            Multi(
+                name='my_multi',
+                attr3=5.
+            )
+
+    def test_multi_container_spec_one_or_more_ok(self):
+        multi_spec = GroupSpec(
+            doc='A test extension that contains a multi',
+            data_type_def='Multi',
+            groups=[
+                GroupSpec(data_type_inc=self.bar_spec, doc='test multi', quantity='+')
+            ],
+            attributes=[
+                AttributeSpec(name='attr3', doc='a float attribute', dtype='float')
+            ]
+        )
+        self.spec_catalog.register_spec(multi_spec, 'extension.yaml')
+        Multi = self.type_map.get_dt_container_cls('Multi', CORE_NAMESPACE)
+        multi = Multi(
+            name='my_multi',
+            bars=[Bar(name='my_bar', data=list(range(10)), attr1='value1', attr2=10)],
+            attr3=5.
+        )
+        assert len(multi.bars) == 1
+
 
 class TestGetClassSeparateNamespace(TestCase):
 
     def setUp(self):
         self.test_dir = tempfile.mkdtemp()
         if os.path.exists(self.test_dir):  # start clean
             self.tearDown()
```

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_convert_dtype.py` & `hdmf-3.5.4/tests/unit/build_tests/test_convert_dtype.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_io_manager.py` & `hdmf-3.5.4/tests/unit/build_tests/test_io_manager.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_io_map.py` & `hdmf-3.5.4/tests/unit/build_tests/test_io_map.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/build_tests/test_io_map_data.py` & `hdmf-3.5.4/tests/unit/build_tests/test_io_map_data.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_alignedtable.py` & `hdmf-3.5.4/tests/unit/common/test_alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_common_io.py` & `hdmf-3.5.4/tests/unit/common/test_common_io.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_generate_table.py` & `hdmf-3.5.4/tests/unit/common/test_generate_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_linkedtables.py` & `hdmf-3.5.4/tests/unit/common/test_linkedtables.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_multi.py` & `hdmf-3.5.4/tests/unit/common/test_multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_resources.py` & `hdmf-3.5.4/tests/unit/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_sparse.py` & `hdmf-3.5.4/tests/unit/common/test_sparse.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/common/test_table.py` & `hdmf-3.5.4/tests/unit/common/test_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_attribute_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_attribute_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_dataset_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_dataset_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_dtype_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_dtype_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_group_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_group_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_link_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_link_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_load_namespace.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_load_namespace.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_ref_spec.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_ref_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_spec_catalog.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_spec_catalog.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/spec_tests/test_spec_write.py` & `hdmf-3.5.4/tests/unit/spec_tests/test_spec_write.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_container.py` & `hdmf-3.5.4/tests/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_io_hdf5.py` & `hdmf-3.5.4/tests/unit/test_io_hdf5.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_io_hdf5_h5tools.py` & `hdmf-3.5.4/tests/unit/test_io_hdf5_h5tools.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_multicontainerinterface.py` & `hdmf-3.5.4/tests/unit/test_multicontainerinterface.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_query.py` & `hdmf-3.5.4/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/test_table.py` & `hdmf-3.5.4/tests/unit/test_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils.py` & `hdmf-3.5.4/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_core_DataChunk.py` & `hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunk.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_core_DataChunkIterator.py` & `hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunkIterator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_core_DataIO.py` & `hdmf-3.5.4/tests/unit/utils_test/test_core_DataIO.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_core_GenericDataChunkIterator.py` & `hdmf-3.5.4/tests/unit/utils_test/test_core_GenericDataChunkIterator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_core_ShapeValidator.py` & `hdmf-3.5.4/tests/unit/utils_test/test_core_ShapeValidator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_docval.py` & `hdmf-3.5.4/tests/unit/utils_test/test_docval.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_labelleddict.py` & `hdmf-3.5.4/tests/unit/utils_test/test_labelleddict.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/utils_test/test_utils.py` & `hdmf-3.5.4/tests/unit/utils_test/test_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/validator_tests/test_errors.py` & `hdmf-3.5.4/tests/unit/validator_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tests/unit/validator_tests/test_validate.py` & `hdmf-3.5.4/tests/unit/validator_tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.2/tox.ini` & `hdmf-3.5.4/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py37, py38, py39, py310
+envlist = py37, py38, py39, py310, py311
 requires = pip >= 22.0
 
 [testenv]
 download = True
 usedevelop = True
 setenv =
   PYTHONDONTWRITEBYTECODE = 1
@@ -22,42 +22,42 @@
 commands =
     python -m pip check  # Check for conflicting packages
     python -m pip list
     pytest -v
 
 # Env to create coverage report locally
 [testenv:localcoverage]
-basepython = python3.10
+basepython = python3.11
 commands =
     pytest --cov=hdmf
     coverage html -d tests/coverage/htmlcov
 
-# Test with python 3.10; pinned dev and optional reqs
-[testenv:py310-optional]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs
+[testenv:py311-optional]
+basepython = python3.11
 install_command =
     python -m pip install {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.10; pinned dev and optional reqs; upgraded run reqs
-[testenv:py310-upgraded]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs; upgraded run reqs
+[testenv:py311-upgraded]
+basepython = python3.11
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.10; pinned dev and optional reqs; upgraded, pre-release run reqs
-[testenv:py310-prerelease]
-basepython = python3.10
+# Test with python 3.11; pinned dev and optional reqs; upgraded, pre-release run reqs
+[testenv:py311-prerelease]
+basepython = python3.11
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
@@ -87,32 +87,36 @@
 basepython = python3.9
 commands = {[testenv:build]commands}
 
 [testenv:build-py310]
 basepython = python3.10
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-optional]
-basepython = python3.10
+[testenv:build-py311]
+basepython = python3.11
+commands = {[testenv:build]commands}
+
+[testenv:build-py311-optional]
+basepython = python3.11
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-upgraded]
-basepython = python3.10
+[testenv:build-py311-upgraded]
+basepython = python3.11
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py310-prerelease]
-basepython = python3.10
+[testenv:build-py311-prerelease]
+basepython = python3.11
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
@@ -137,19 +141,14 @@
     -rrequirements-dev.txt
     -rrequirements.txt
     -rrequirements-doc.txt
 
 commands =
     python test_gallery.py
 
-[testenv:gallery-py37]
-basepython = python3.7
-deps = {[testenv:gallery]deps}
-commands = {[testenv:gallery]commands}
-
 [testenv:gallery-py38]
 basepython = python3.8
 deps = {[testenv:gallery]deps}
 commands = {[testenv:gallery]commands}
 
 [testenv:gallery-py39]
 basepython = python3.9
@@ -157,28 +156,33 @@
 commands = {[testenv:gallery]commands}
 
 [testenv:gallery-py310]
 basepython = python3.10
 deps = {[testenv:gallery]deps}
 commands = {[testenv:gallery]commands}
 
-# Test with python 3.10; pinned dev, doc, and optional reqs; upgraded run reqs
-[testenv:gallery-py310-upgraded]
-basepython = python3.10
+[testenv:gallery-py311]
+basepython = python3.11
+deps = {[testenv:gallery]deps}
+commands = {[testenv:gallery]commands}
+
+# Test with python 3.11; pinned dev, doc, and optional reqs; upgraded run reqs
+[testenv:gallery-py311-upgraded]
+basepython = python3.11
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-doc.txt
     -rrequirements-opt.txt
 commands = {[testenv:gallery]commands}
 
-# Test with python 3.10; pinned dev, doc, and optional reqs; pre-release run reqs
-[testenv:gallery-py310-prerelease]
-basepython = python3.10
+# Test with python 3.11; pinned dev, doc, and optional reqs; pre-release run reqs
+[testenv:gallery-py311-prerelease]
+basepython = python3.11
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-doc.txt
     -rrequirements-opt.txt
 commands = {[testenv:gallery]commands}
```

### Comparing `hdmf-3.5.2/versioneer.py` & `hdmf-3.5.4/versioneer.py`

 * *Files identical despite different names*

