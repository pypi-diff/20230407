# Comparing `tmp/kokos-1.9.2.tar.gz` & `tmp/kokos-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kokos-1.9.2.tar", last modified: Sat Feb  6 10:11:33 2021, max compression
+gzip compressed data, was "kokos-1.9.3.tar", last modified: Sat Feb  6 21:54:08 2021, max compression
```

## Comparing `kokos-1.9.2.tar` & `kokos-1.9.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.046748 kokos-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)       30 2021-02-06 10:11:16.000000 kokos-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8539 2021-02-06 10:11:33.046748 kokos-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6722 2021-02-06 10:11:16.000000 kokos-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.034748 kokos-1.9.2/kks/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3540 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/binary.py
--rw-r--r--   0 runner    (1001) docker     (116)     1495 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.038748 kokos-1.9.2/kks/cmd/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2078 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/convert.py
--rw-r--r--   0 runner    (1001) docker     (116)     5482 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/gen.py
--rw-r--r--   0 runner    (1001) docker     (116)     2191 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/hide.py
--rw-r--r--   0 runner    (1001) docker     (116)     4178 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     2296 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/lint.py
--rw-r--r--   0 runner    (1001) docker     (116)      831 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/open.py
--rw-r--r--   0 runner    (1001) docker     (116)     3218 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/run.py
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/status.py
--rw-r--r--   0 runner    (1001) docker     (116)     1977 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/submit.py
--rw-r--r--   0 runner    (1001) docker     (116)     7654 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     7517 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     6941 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/top.py
--rw-r--r--   0 runner    (1001) docker     (116)      484 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/cmd/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.038748 kokos-1.9.2/kks/data/
--rw-r--r--   0 runner    (1001) docker     (116)     2198 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/data/targets.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    15466 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/ejudge.py
--rw-r--r--   0 runner    (1001) docker     (116)     3443 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/ejudge_submit.py
--rw-r--r--   0 runner    (1001) docker     (116)       80 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.042748 kokos-1.9.2/kks/util/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2755 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/click.py
--rw-r--r--   0 runner    (1001) docker     (116)     5719 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     6835 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     4855 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/ejudge.py
--rw-r--r--   0 runner    (1001) docker     (116)    10037 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/h2t.py
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/script.py
--rw-r--r--   0 runner    (1001) docker     (116)     5258 2021-02-06 10:11:16.000000 kokos-1.9.2/kks/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 10:11:33.046748 kokos-1.9.2/kokos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8539 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      738 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2021-02-06 10:11:32.000000 kokos-1.9.2/kokos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-06 10:11:33.046748 kokos-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      702 2021-02-06 10:11:16.000000 kokos-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.949482 kokos-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2021-02-06 21:53:47.000000 kokos-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8539 2021-02-06 21:54:08.949482 kokos-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6722 2021-02-06 21:53:47.000000 kokos-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.945482 kokos-1.9.3/kks/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3540 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/binary.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1495 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.949482 kokos-1.9.3/kks/cmd/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2078 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1609 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/convert.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5482 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/gen.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2191 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/hide.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4178 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/init.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2296 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/lint.py
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/open.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3218 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1977 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/submit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7654 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7517 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6941 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/top.py
+-rw-r--r--   0 runner    (1001) docker     (116)      484 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/cmd/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.949482 kokos-1.9.3/kks/data/
+-rw-r--r--   0 runner    (1001) docker     (116)     2198 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/data/targets.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    15682 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/ejudge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3443 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/ejudge_submit.py
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.949482 kokos-1.9.3/kks/util/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2755 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2816 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5719 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6835 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4855 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/ejudge.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10037 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/h2t.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2314 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/script.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5258 2021-02-06 21:53:47.000000 kokos-1.9.3/kks/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-06 21:54:08.949482 kokos-1.9.3/kokos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8539 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      738 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2021-02-06 21:54:08.000000 kokos-1.9.3/kokos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-06 21:54:08.949482 kokos-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      702 2021-02-06 21:53:47.000000 kokos-1.9.3/setup.py
```

### Comparing `kokos-1.9.2/PKG-INFO` & `kokos-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kokos
-Version: 1.9.2
+Version: 1.9.3
 Summary: KoKoS helper tool
 Home-page: https://github.com/DarkKeks/kks
 Author: Vyacheslav Boben
 License: UNKNOWN
 Description: # KoKoS
         
         Утилита для удобного решения задач курса АКОС.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kokos Version: 1.9.2 Summary: KoKoS helper tool
+Metadata-Version: 2.1 Name: kokos Version: 1.9.3 Summary: KoKoS helper tool
 Home-page: https://github.com/DarkKeks/kks Author: Vyacheslav Boben License:
 UNKNOWN Description: # KoKoS Ð£ÑÐ¸Ð»Ð¸ÑÐ° Ð´Ð»Ñ ÑÐ´Ð¾Ð±Ð½Ð¾Ð³Ð¾
 ÑÐµÑÐµÐ½Ð¸Ñ Ð·Ð°Ð´Ð°Ñ ÐºÑÑÑÐ° ÐÐÐÐ¡. Ð¤Ð¸Ð´Ð±ÐµÐº Ð¼Ð¾Ð¶Ð½Ð¾
 Ð¿Ð¸ÑÐ°ÑÑ Ð² issue, Ð»Ð¸Ð±Ð¾ Ð² ÑÐµÐ»ÐµÐ³ÑÐ°Ð¼ [@darkkeks](https://t.me/
 darkkeks). Inspired by - [DoomzD/caos-reborn](https://github.com/DoomzD/caos-
 reborn) - [petuhovskiy/acos](https://github.com/petuhovskiy/acos) - [BigRedEye/
 cacos](https://github.com/BigRedEye/cacos) ## Installation ### ÐÐ· PyPi
```

### Comparing `kokos-1.9.2/README.md` & `kokos-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/binary.py` & `kokos-1.9.3/kks/binary.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cli.py` & `kokos-1.9.3/kks/cli.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/auth.py` & `kokos-1.9.3/kks/cmd/auth.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/convert.py` & `kokos-1.9.3/kks/cmd/convert.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/gen.py` & `kokos-1.9.3/kks/cmd/gen.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/hide.py` & `kokos-1.9.3/kks/cmd/hide.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/init.py` & `kokos-1.9.3/kks/cmd/init.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/lint.py` & `kokos-1.9.3/kks/cmd/lint.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/open.py` & `kokos-1.9.3/kks/cmd/open.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/run.py` & `kokos-1.9.3/kks/cmd/run.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/status.py` & `kokos-1.9.3/kks/cmd/status.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/submit.py` & `kokos-1.9.3/kks/cmd/submit.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/sync.py` & `kokos-1.9.3/kks/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/test.py` & `kokos-1.9.3/kks/cmd/test.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/cmd/top.py` & `kokos-1.9.3/kks/cmd/top.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/data/targets.yaml` & `kokos-1.9.3/kks/data/targets.yaml`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/ejudge.py` & `kokos-1.9.3/kks/ejudge.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,22 +127,25 @@
         self.score = score
         self.status = status
 
     def color(self):
         return 'green' if self.status == Status.REVIEW \
             else 'green' if self.status == Status.OK \
             else 'bright_yellow' if self.status == Status.TESTING \
+            else 'yellow' if self.status == Status.REJECTED \
             else 'red' if self.status == Status.PARTIAL \
             else 'white'
+        # in standings CHECK has the same style as TESTING
 
     def bold(self):
-        return self.status == Status.OK
+        # TESTING is bold for more contrast with REJECTED
+        return self.status in [Status.OK, Status.TESTING]
 
     def table_score(self):
-        if self.status == Status.TESTING and self.score is None:
+        if self.status in [Status.TESTING, Status.REJECTED] and self.score is None:
             return '??'
         return self.score
 
 
 class Standings:
     def __init__(self, task_names, rows):
         self.task_names = task_names
```

### Comparing `kokos-1.9.2/kks/ejudge_submit.py` & `kokos-1.9.3/kks/ejudge_submit.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/cache.py` & `kokos-1.9.3/kks/util/cache.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/click.py` & `kokos-1.9.3/kks/util/click.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/common.py` & `kokos-1.9.3/kks/util/common.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/config.py` & `kokos-1.9.3/kks/util/config.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/ejudge.py` & `kokos-1.9.3/kks/util/ejudge.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/h2t.py` & `kokos-1.9.3/kks/util/h2t.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/script.py` & `kokos-1.9.3/kks/util/script.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kks/util/testing.py` & `kokos-1.9.3/kks/util/testing.py`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/kokos.egg-info/PKG-INFO` & `kokos-1.9.3/kokos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kokos
-Version: 1.9.2
+Version: 1.9.3
 Summary: KoKoS helper tool
 Home-page: https://github.com/DarkKeks/kks
 Author: Vyacheslav Boben
 License: UNKNOWN
 Description: # KoKoS
         
         Утилита для удобного решения задач курса АКОС.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kokos Version: 1.9.2 Summary: KoKoS helper tool
+Metadata-Version: 2.1 Name: kokos Version: 1.9.3 Summary: KoKoS helper tool
 Home-page: https://github.com/DarkKeks/kks Author: Vyacheslav Boben License:
 UNKNOWN Description: # KoKoS Ð£ÑÐ¸Ð»Ð¸ÑÐ° Ð´Ð»Ñ ÑÐ´Ð¾Ð±Ð½Ð¾Ð³Ð¾
 ÑÐµÑÐµÐ½Ð¸Ñ Ð·Ð°Ð´Ð°Ñ ÐºÑÑÑÐ° ÐÐÐÐ¡. Ð¤Ð¸Ð´Ð±ÐµÐº Ð¼Ð¾Ð¶Ð½Ð¾
 Ð¿Ð¸ÑÐ°ÑÑ Ð² issue, Ð»Ð¸Ð±Ð¾ Ð² ÑÐµÐ»ÐµÐ³ÑÐ°Ð¼ [@darkkeks](https://t.me/
 darkkeks). Inspired by - [DoomzD/caos-reborn](https://github.com/DoomzD/caos-
 reborn) - [petuhovskiy/acos](https://github.com/petuhovskiy/acos) - [BigRedEye/
 cacos](https://github.com/BigRedEye/cacos) ## Installation ### ÐÐ· PyPi
```

### Comparing `kokos-1.9.2/kokos.egg-info/SOURCES.txt` & `kokos-1.9.3/kokos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kokos-1.9.2/setup.py` & `kokos-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     name='kokos',
     description='KoKoS helper tool',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Vyacheslav Boben',
     url='https://github.com/DarkKeks/kks',
-    version='1.9.2',
+    version='1.9.3',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click',
         'requests',
         'configparser',
         'colorama',
```

