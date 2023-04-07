# Comparing `tmp/netunicorn-connector-salt-0.3.0.tar.gz` & `tmp/netunicorn-connector-salt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.0.tar", last modified: Sat Apr  1 04:08:29 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.1.tar", last modified: Fri Apr  7 21:47:54 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.0.tar` & `netunicorn-connector-salt-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.435349 netunicorn-connector-salt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-01 04:08:19.000000 netunicorn-connector-salt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-01 04:08:29.435349 netunicorn-connector-salt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-01 04:08:19.000000 netunicorn-connector-salt-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-01 04:08:19.000000 netunicorn-connector-salt-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 04:08:29.435349 netunicorn-connector-salt-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:19.000000 netunicorn-connector-salt-0.3.0/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-01 04:08:19.000000 netunicorn-connector-salt-0.3.0/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 04:08:29.431349 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-01 04:08:29.000000 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-01 04:08:29.000000 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 04:08:29.000000 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 04:08:29.000000 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-01 04:08:29.000000 netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-04-07 21:47:41.000000 netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:47:54.190308 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 21:47:54.000000 netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.0/LICENSE` & `netunicorn-connector-salt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.0/PKG-INFO` & `netunicorn-connector-salt-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.0
+Version: 0.3.1
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.0/README.md` & `netunicorn-connector-salt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.0/pyproject.toml` & `netunicorn-connector-salt-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
@@ -21,8 +21,8 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
 python_version = "3.10"
 ignore_missing_imports = true
-strict = true
+strict = true
```

### Comparing `netunicorn-connector-salt-0.3.0/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.1/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,17 +212,16 @@
                             "fun": "cmd.run",
                             "arg": [command],
                             "username": self.username,
                             "password": self.password,
                             "eauth": self.eauth,
                             "full_return": True,
                         },
-                    )
+                    ).json()
                 )
-                .json()
                 .get("return", [{}])[0]
                 for command in deployment.environment_definition.commands
             ]
         except Exception as e:
             self.logger.error(
                 f"Exception during deployment of executor {deployment.executor_id}, node {deployment.node}: {e}"
             )
```

### Comparing `netunicorn-connector-salt-0.3.0/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.1/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.0
+Version: 0.3.1
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

