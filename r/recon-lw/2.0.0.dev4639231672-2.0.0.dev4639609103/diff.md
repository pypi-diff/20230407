# Comparing `tmp/recon_lw-2.0.0.dev4639231672.tar.gz` & `tmp/recon_lw-2.0.0.dev4639609103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4639231672.tar", last modified: Fri Apr  7 15:14:40 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4639609103.tar", last modified: Fri Apr  7 16:13:24 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4639231672.tar` & `recon_lw-2.0.0.dev4639609103.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-07 15:14:25.000000 recon_lw-2.0.0.dev4639231672/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12890 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    12172 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 15:14:40.000000 recon_lw-2.0.0.dev4639231672/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-07 15:14:17.000000 recon_lw-2.0.0.dev4639231672/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-07 16:13:13.000000 recon_lw-2.0.0.dev4639609103/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12172 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 16:13:24.000000 recon_lw-2.0.0.dev4639609103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-07 16:13:07.000000 recon_lw-2.0.0.dev4639609103/setup.py
```

### Comparing `recon_lw-2.0.0.dev4639231672/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4639609103/recon_lw/recon_lw.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         rule_settings["init_func"](rule_settings)
 
     save_events_standalone([r["rule_root_event"] for r in rules_settings_dict.values()],
                            events_buffer,result_events_path)
     if sessions_list is not None and len(sessions_list):
         sessions_set = set(sessions_list)
         streams = open_streams(message_pickle_path,
-                               lambda n: n[:n.index("_IN")] in sessions_set or n[:n.index("_OUT")] in sessions_set)
+                               lambda n: n[:n.rfind('_')] in sessions_set)
     else:
         streams = open_streams(message_pickle_path)
 
     message_buffer = [None]*100
     buffer_len = 100
     while len(streams)>0:
         next_batch_len = get_next_batch(streams, message_buffer, buffer_len)
```

### Comparing `recon_lw-2.0.0.dev4639231672/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4639609103/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4639231672/setup.py` & `recon_lw-2.0.0.dev4639609103/setup.py`

 * *Files identical despite different names*

