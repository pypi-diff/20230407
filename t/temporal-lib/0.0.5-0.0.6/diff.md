# Comparing `tmp/temporal-lib-0.0.5.tar.gz` & `tmp/temporal-lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temporal-lib-0.0.5.tar", last modified: Fri Apr  7 01:52:54 2023, max compression
+gzip compressed data, was "temporal-lib-0.0.6.tar", last modified: Fri Apr  7 20:37:59 2023, max compression
```

## Comparing `temporal-lib-0.0.5.tar` & `temporal-lib-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/
--rw-r--r--   0 sysop     (1000) sysop     (1000)     1070 2023-03-11 23:45:16.000000 temporal-lib-0.0.5/LICENSE
--rw-r--r--   0 sysop     (1000) sysop     (1000)     2221 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/PKG-INFO
--rw-r--r--   0 sysop     (1000) sysop     (1000)     1850 2023-03-08 16:52:08.000000 temporal-lib-0.0.5/README.md
--rw-r--r--   0 sysop     (1000) sysop     (1000)     1112 2023-04-07 01:41:39.000000 temporal-lib-0.0.5/pyproject.toml
--rw-r--r--   0 sysop     (1000) sysop     (1000)       38 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/setup.cfg
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.307198 temporal-lib-0.0.5/src/
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/src/temporal_lib/
--rw-r--r--   0 sysop     (1000) sysop     (1000)     4058 2023-03-20 15:34:46.000000 temporal-lib-0.0.5/src/temporal_lib/__init__.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     6329 2023-03-19 23:43:59.000000 temporal-lib-0.0.5/src/temporal_lib/calendar.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     7844 2023-04-07 01:43:41.000000 temporal-lib-0.0.5/src/temporal_lib/core.py
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/src/temporal_lib/cron/
--rw-r--r--   0 sysop     (1000) sysop     (1000)     5899 2023-03-20 15:25:39.000000 temporal-lib-0.0.5/src/temporal_lib/cron/__init__.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     5966 2023-03-19 23:49:09.000000 temporal-lib-0.0.5/src/temporal_lib/tlib_date.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     9489 2023-03-20 15:29:47.000000 temporal-lib-0.0.5/src/temporal_lib/tlib_types.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     6964 2023-03-20 15:33:51.000000 temporal-lib-0.0.5/src/temporal_lib/tlib_week.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     2800 2023-03-19 23:26:05.000000 temporal-lib-0.0.5/src/temporal_lib/tlib_weekday.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     1040 2023-03-19 23:39:57.000000 temporal-lib-0.0.5/src/temporal_lib/tlib_year.py
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/src/temporal_lib.egg-info/
--rw-r--r--   0 sysop     (1000) sysop     (1000)     2221 2023-04-07 01:52:54.000000 temporal-lib-0.0.5/src/temporal_lib.egg-info/PKG-INFO
--rw-r--r--   0 sysop     (1000) sysop     (1000)      562 2023-04-07 01:52:54.000000 temporal-lib-0.0.5/src/temporal_lib.egg-info/SOURCES.txt
--rw-r--r--   0 sysop     (1000) sysop     (1000)        1 2023-04-07 01:52:54.000000 temporal-lib-0.0.5/src/temporal_lib.egg-info/dependency_links.txt
--rw-r--r--   0 sysop     (1000) sysop     (1000)      211 2023-04-07 01:52:54.000000 temporal-lib-0.0.5/src/temporal_lib.egg-info/requires.txt
--rw-r--r--   0 sysop     (1000) sysop     (1000)       13 2023-04-07 01:52:54.000000 temporal-lib-0.0.5/src/temporal_lib.egg-info/top_level.txt
-drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 01:52:54.311199 temporal-lib-0.0.5/tests/
--rw-r--r--   0 sysop     (1000) sysop     (1000)     2137 2023-03-19 22:14:07.000000 temporal-lib-0.0.5/tests/test_basics.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     2258 2023-03-19 23:48:00.000000 temporal-lib-0.0.5/tests/test_cron.py
--rw-r--r--   0 sysop     (1000) sysop     (1000)     4590 2023-03-19 23:49:43.000000 temporal-lib-0.0.5/tests/test_weeks.py
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     1070 2023-03-11 23:45:16.000000 temporal-lib-0.0.6/LICENSE
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     2221 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/PKG-INFO
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     1850 2023-03-08 16:52:08.000000 temporal-lib-0.0.6/README.md
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     1112 2023-04-07 20:33:17.000000 temporal-lib-0.0.6/pyproject.toml
+-rw-r--r--   0 sysop     (1000) sysop     (1000)       38 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/setup.cfg
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.347562 temporal-lib-0.0.6/src/
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/src/temporal_lib/
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     4058 2023-03-20 15:34:46.000000 temporal-lib-0.0.6/src/temporal_lib/__init__.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     6329 2023-03-19 23:43:59.000000 temporal-lib-0.0.6/src/temporal_lib/calendar.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     7844 2023-04-07 01:43:41.000000 temporal-lib-0.0.6/src/temporal_lib/core.py
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/src/temporal_lib/cron/
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     5899 2023-03-20 15:25:39.000000 temporal-lib-0.0.6/src/temporal_lib/cron/__init__.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     5966 2023-03-19 23:49:09.000000 temporal-lib-0.0.6/src/temporal_lib/tlib_date.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     9577 2023-04-07 20:31:16.000000 temporal-lib-0.0.6/src/temporal_lib/tlib_types.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     6964 2023-03-20 15:33:51.000000 temporal-lib-0.0.6/src/temporal_lib/tlib_week.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     2800 2023-03-19 23:26:05.000000 temporal-lib-0.0.6/src/temporal_lib/tlib_weekday.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     1040 2023-03-19 23:39:57.000000 temporal-lib-0.0.6/src/temporal_lib/tlib_year.py
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/src/temporal_lib.egg-info/
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     2221 2023-04-07 20:37:59.000000 temporal-lib-0.0.6/src/temporal_lib.egg-info/PKG-INFO
+-rw-r--r--   0 sysop     (1000) sysop     (1000)      581 2023-04-07 20:37:59.000000 temporal-lib-0.0.6/src/temporal_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 sysop     (1000) sysop     (1000)        1 2023-04-07 20:37:59.000000 temporal-lib-0.0.6/src/temporal_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 sysop     (1000) sysop     (1000)      211 2023-04-07 20:37:59.000000 temporal-lib-0.0.6/src/temporal_lib.egg-info/requires.txt
+-rw-r--r--   0 sysop     (1000) sysop     (1000)       13 2023-04-07 20:37:59.000000 temporal-lib-0.0.6/src/temporal_lib.egg-info/top_level.txt
+drwxr-xr-x   0 sysop     (1000) sysop     (1000)        0 2023-04-07 20:37:59.351562 temporal-lib-0.0.6/tests/
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     2137 2023-03-19 22:14:07.000000 temporal-lib-0.0.6/tests/test_basics.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     2258 2023-03-19 23:48:00.000000 temporal-lib-0.0.6/tests/test_cron.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)      892 2023-04-07 20:31:59.000000 temporal-lib-0.0.6/tests/test_time.py
+-rw-r--r--   0 sysop     (1000) sysop     (1000)     4590 2023-03-19 23:49:43.000000 temporal-lib-0.0.6/tests/test_weeks.py
```

### Comparing `temporal-lib-0.0.5/LICENSE` & `temporal-lib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/PKG-INFO` & `temporal-lib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporal-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for working with datetime and other temporal concepts.
 Author-email: Datahenge LLC <brian@datahenge.com>
 License: MIT
 Keywords: datetime,cron
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `temporal-lib-0.0.5/README.md` & `temporal-lib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/pyproject.toml` & `temporal-lib-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 description = "A library for working with datetime and other temporal concepts."
 # dynamic =["version" ]
 keywords = ["datetime", "cron"]
 license = {text = "MIT"}
 requires-python = ">=3.7"
 readme = "README.md"
-version = "0.0.5"
+version = "0.0.6"
 
 
 dependencies = [
     "cron-converter",
     "cron-descriptor",
     "local-crontab",
     "python-dateutil>=2.8.2",
```

### Comparing `temporal-lib-0.0.5/src/temporal_lib/__init__.py` & `temporal-lib-0.0.6/src/temporal_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/calendar.py` & `temporal-lib-0.0.6/src/temporal_lib/calendar.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/core.py` & `temporal-lib-0.0.6/src/temporal_lib/core.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/cron/__init__.py` & `temporal-lib-0.0.6/src/temporal_lib/cron/__init__.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/tlib_date.py` & `temporal-lib-0.0.6/src/temporal_lib/tlib_date.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/tlib_types.py` & `temporal-lib-0.0.6/src/temporal_lib/tlib_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,37 +208,40 @@
 		am_pm = 'pm'
 		time_as_string = time_as_string.replace('pm', '')
 	time_as_string = time_as_string.replace(' ', '')
 
 	# Based on length of string, make some assumptions:
 	if len(time_as_string) == 0:
 		raise ValueError(f"Invalid time string '{time_as_string}'")
-	if len(time_as_string) == 1:
-		hour = time_as_string
+	if len(time_as_string) in (1,2):
+		hour = int(time_as_string)
 		minute = 0
-	elif len(time_as_string) == 2:
-		raise ValueError(f"Invalid time string '{time_as_string}'")
 	elif len(time_as_string) == 3:
-		hour = time_as_string[0]
-		minute = time_as_string[1:3]  # NOTE: Python string splicing; last index is not included.
+		hour = int(time_as_string[0])
+		minute = int(time_as_string[1:3])  # NOTE: Python string splicing; last index is not included.
 	elif len(time_as_string) == 4:
-		hour = time_as_string[0:2]  # NOTE: Python string splicing; last index is not included.
-		minute = time_as_string[2:4] # NOTE: Python string splicing; last index is not included.
-		if int(hour) > 12 and am_pm == 'am':
-			raise ValueError(f"Invalid time string '{time_as_string}'")
+		hour = int(time_as_string[0:2])  # NOTE: Python string splicing; last index is not included.
+		minute = int(time_as_string[2:4]) # NOTE: Python string splicing; last index is not included.
 	else:
 		raise ValueError(f"Invalid time string '{time_as_string}'")
 
+	if hour > 23:
+		raise ValueError(f"Invalid time string '{time_as_string}'")
+	if minute > 59:
+		raise ValueError(f"Invalid time string '{time_as_string}'")
+	if int(hour) > 12 and am_pm == 'am':
+		raise ValueError(f"Invalid time string '{time_as_string}'")
+
 	if not am_pm:
-		if int(hour) > 12:
+		if hour > 12:
 			am_pm = 'pm'
 		else:
 			am_pm = 'am'
-	if am_pm == 'pm':
-		hour = int(hour) + 12
+	if am_pm == 'pm' and hour < 12:
+		hour += 12
 
 	return TimeType(int(hour), int(minute), 0)
 
 # ----------------
 # DATETIMES
 # ----------------
```

### Comparing `temporal-lib-0.0.5/src/temporal_lib/tlib_week.py` & `temporal-lib-0.0.6/src/temporal_lib/tlib_week.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/tlib_weekday.py` & `temporal-lib-0.0.6/src/temporal_lib/tlib_weekday.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib/tlib_year.py` & `temporal-lib-0.0.6/src/temporal_lib/tlib_year.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/src/temporal_lib.egg-info/PKG-INFO` & `temporal-lib-0.0.6/src/temporal_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temporal-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for working with datetime and other temporal concepts.
 Author-email: Datahenge LLC <brian@datahenge.com>
 License: MIT
 Keywords: datetime,cron
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `temporal-lib-0.0.5/src/temporal_lib.egg-info/SOURCES.txt` & `temporal-lib-0.0.6/src/temporal_lib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/temporal_lib.egg-info/SOURCES.txt
 src/temporal_lib.egg-info/dependency_links.txt
 src/temporal_lib.egg-info/requires.txt
 src/temporal_lib.egg-info/top_level.txt
 src/temporal_lib/cron/__init__.py
 tests/test_basics.py
 tests/test_cron.py
+tests/test_time.py
 tests/test_weeks.py
```

### Comparing `temporal-lib-0.0.5/tests/test_basics.py` & `temporal-lib-0.0.6/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/tests/test_cron.py` & `temporal-lib-0.0.6/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `temporal-lib-0.0.5/tests/test_weeks.py` & `temporal-lib-0.0.6/tests/test_weeks.py`

 * *Files identical despite different names*

