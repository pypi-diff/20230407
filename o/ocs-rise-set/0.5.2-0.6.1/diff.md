# Comparing `tmp/ocs-rise-set-0.5.2.tar.gz` & `tmp/ocs_rise_set-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocs-rise-set-0.5.2.tar", last modified: Fri May 13 06:41:26 2022, max compression
+gzip compressed data, was "ocs_rise_set-0.6.1.tar", max compression
```

## Comparing `ocs-rise-set-0.5.2.tar` & `ocs_rise_set-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,15 @@
-drwxrwxr-x   0 jnation   (1000) jnation   (1000)        0 2022-05-13 06:41:26.670609 ocs-rise-set-0.5.2/
--rw-rw-r--   0 jnation   (1000) jnation   (1000)      480 2022-05-13 06:41:26.669609 ocs-rise-set-0.5.2/PKG-INFO
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     1938 2022-05-03 22:52:20.000000 ocs-rise-set-0.5.2/README.md
-drwxrwxr-x   0 jnation   (1000) jnation   (1000)        0 2022-05-13 06:41:26.666609 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/
--rw-rw-r--   0 jnation   (1000) jnation   (1000)      480 2022-05-13 06:41:26.000000 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/PKG-INFO
--rw-rw-r--   0 jnation   (1000) jnation   (1000)      458 2022-05-13 06:41:26.000000 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/SOURCES.txt
--rw-rw-r--   0 jnation   (1000) jnation   (1000)        1 2022-05-13 06:41:26.000000 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/dependency_links.txt
--rw-rw-r--   0 jnation   (1000) jnation   (1000)       22 2022-05-13 06:41:26.000000 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/requires.txt
--rw-rw-r--   0 jnation   (1000) jnation   (1000)        9 2022-05-13 06:41:26.000000 ocs-rise-set-0.5.2/ocs_rise_set.egg-info/top_level.txt
-drwxrwxr-x   0 jnation   (1000) jnation   (1000)        0 2022-05-13 06:41:26.669609 ocs-rise-set-0.5.2/rise_set/
--rw-rw-r--   0 jnation   (1000) jnation   (1000)        0 2019-08-02 03:59:39.000000 ocs-rise-set-0.5.2/rise_set/__init__.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     5078 2020-06-05 06:43:05.000000 ocs-rise-set-0.5.2/rise_set/angle.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)    52413 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/rise_set/astrometry.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     1189 2020-06-05 06:43:05.000000 ocs-rise-set-0.5.2/rise_set/exceptions.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)      745 2019-08-02 03:59:39.000000 ocs-rise-set-0.5.2/rise_set/logging.conf
--rw-rw-r--   0 jnation   (1000) jnation   (1000)    13677 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/rise_set/moving_objects.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     2425 2020-06-05 06:43:05.000000 ocs-rise-set-0.5.2/rise_set/rates.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     1940 2019-08-02 03:59:39.000000 ocs-rise-set-0.5.2/rise_set/sky_coordinates.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)    27911 2020-06-05 07:08:26.000000 ocs-rise-set-0.5.2/rise_set/transits.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     4128 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/rise_set/utils.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)    29825 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/rise_set/visibility.py
--rw-rw-r--   0 jnation   (1000) jnation   (1000)       38 2022-05-13 06:41:26.670609 ocs-rise-set-0.5.2/setup.cfg
--rw-rw-r--   0 jnation   (1000) jnation   (1000)     1057 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/setup.py
-drwxrwxr-x   0 jnation   (1000) jnation   (1000)        0 2022-05-13 06:41:26.669609 ocs-rise-set-0.5.2/test/
--rw-rw-r--   0 jnation   (1000) jnation   (1000)    11331 2022-05-13 00:09:41.000000 ocs-rise-set-0.5.2/test/test_utils.py
+-rw-r--r--   0        0        0    35147 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2043 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/README.md
+-rw-r--r--   0        0        0      702 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/__init__.py
+-rw-r--r--   0        0        0     5078 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/angle.py
+-rw-r--r--   0        0        0    52413 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/astrometry.py
+-rw-r--r--   0        0        0     1189 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/exceptions.py
+-rw-r--r--   0        0        0      745 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/logging.conf
+-rw-r--r--   0        0        0    13677 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/moving_objects.py
+-rw-r--r--   0        0        0     2425 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/rates.py
+-rw-r--r--   0        0        0     1940 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/sky_coordinates.py
+-rw-r--r--   0        0        0    27911 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/transits.py
+-rw-r--r--   0        0        0     4128 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/utils.py
+-rw-r--r--   0        0        0    29825 2023-04-07 17:14:49.180901 ocs_rise_set-0.6.1/rise_set/visibility.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 ocs_rise_set-0.6.1/PKG-INFO
```

### Comparing `ocs-rise-set-0.5.2/README.md` & `ocs_rise_set-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Rise-set Library
 
 ![Build](https://github.com/observatorycontrolsystem/rise_set/workflows/Build/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/observatorycontrolsystem/rise_set/badge.svg?branch=master)](https://coveralls.io/github/observatorycontrolsystem/rise_set?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8b05ac4107534c7297dfff464360af57)](https://www.codacy.com/gh/observatorycontrolsystem/rise_set/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=observatorycontrolsystem/rise_set&amp;utm_campaign=Badge_Grade)
+[![PyPI](https://img.shields.io/pypi/v/ocs-rise-set?style=flat)](https://pypi.org/project/ocs-rise-set/)
 
 ***WARNING: The API of this library will be updated in the near future***
 
 This library provides Python routines for finding the positions of astronomical bodies to reasonable precision. It is primarily used to calculate target uptime and sunrise, sunset and twilight times, accurate to 30s-1m. It also supports calculating target airmass over time. The library depends on Fortran SLALIB to perform the computations. The rise/set/transit algorithms are implementations of Astronomical Algorithms, Ch. 14 (Jean Meeus). This library was initially authored by [Eric Saunders](https://github.com/ire-and-curses).
 
 ## Prerequisites
 
--   Python >= 3.6
+-   Python >= 3.7
 -   Ability to compile fortran (gfortran installed)
 
 ## Installation
 
 It is highly recommended that you install and run your python code inside a dedicated python
 [virtual environment](https://docs.python.org/3/tutorial/venv.html).
 
@@ -24,13 +25,13 @@
 (venv) $ pip install numpy; pip install ocs_rise_set
 ```
 
 ## For Developers
 
 ### Running the Tests
 
-The unit tests are currently using nosetests, so there are a few tests dependencies to install. After cloning this project, from the project root and inside your virtual environment:
+The unit tests are currently using nosetests, so there are a few tests dependencies to install. After cloning this project, from the project root and inside your virtual environment (using Poetry):
 
 ```bash
-(venv) $ pip install -r test_requirements.pip
-(venv) $ nosetests
+$ poetry env use python3.9
+$ poetry run nosetests
 ```
```

### Comparing `ocs-rise-set-0.5.2/rise_set/angle.py` & `ocs_rise_set-0.6.1/rise_set/angle.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/astrometry.py` & `ocs_rise_set-0.6.1/rise_set/astrometry.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/exceptions.py` & `ocs_rise_set-0.6.1/rise_set/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/logging.conf` & `ocs_rise_set-0.6.1/rise_set/logging.conf`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/moving_objects.py` & `ocs_rise_set-0.6.1/rise_set/moving_objects.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/rates.py` & `ocs_rise_set-0.6.1/rise_set/rates.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/sky_coordinates.py` & `ocs_rise_set-0.6.1/rise_set/sky_coordinates.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/transits.py` & `ocs_rise_set-0.6.1/rise_set/transits.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/utils.py` & `ocs_rise_set-0.6.1/rise_set/utils.py`

 * *Files identical despite different names*

### Comparing `ocs-rise-set-0.5.2/rise_set/visibility.py` & `ocs_rise_set-0.6.1/rise_set/visibility.py`

 * *Files identical despite different names*

