# Comparing `tmp/robotcode_debugger-0.32.2.tar.gz` & `tmp/robotcode_debugger-0.32.3.tar.gz`

## Comparing `robotcode_debugger-0.32.2.tar` & `robotcode_debugger-0.32.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/client.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/__main__.py
--rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0    12645 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/README.md
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/pyproject.toml
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/client.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0    14877 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/__main__.py
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0    12645 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/README.md
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/pyproject.toml
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 robotcode_debugger-0.32.3/PKG-INFO
```

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/__main__.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/client.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/server.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/__main__.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.32.3/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/.gitignore` & `robotcode_debugger-0.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/LICENSE.txt` & `robotcode_debugger-0.32.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/README.md` & `robotcode_debugger-0.32.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/pyproject.toml` & `robotcode_debugger-0.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.32.2/PKG-INFO` & `robotcode_debugger-0.32.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.32.2
+Version: 0.32.3
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

