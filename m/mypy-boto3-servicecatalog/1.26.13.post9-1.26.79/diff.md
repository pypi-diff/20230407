# Comparing `tmp/mypy-boto3-servicecatalog-1.26.13.post9.tar.gz` & `tmp/mypy-boto3-servicecatalog-1.26.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-1.26.13.post9.tar", last modified: Fri Nov 18 23:30:00 2022, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-1.26.13.post9.tar` & `mypy-boto3-servicecatalog-1.26.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.608253 mypy-boto3-servicecatalog-1.26.13.post9/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    27306 2022-11-18 23:30:00.608253 mypy-boto3-servicecatalog-1.26.13.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25835 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.604253 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4569 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    73597 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    73487 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13903 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    13901 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    21847 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)    21828 2022-11-18 23:29:42.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    99234 2022-11-18 23:29:44.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    99095 2022-11-18 23:29:43.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 23:30:00.608253 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    27306 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-18 23:30:00.000000 mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 23:30:00.608253 mypy-boto3-servicecatalog-1.26.13.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-11-18 23:29:41.000000 mypy-boto3-servicecatalog-1.26.13.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-servicecatalog-1.26.79/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-02-24 21:22:49.733199 mypy-boto3-servicecatalog-1.26.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25834 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73597 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73487 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99234 2023-02-24 21:22:38.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99095 2023-02-24 21:22:36.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.733199 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.737199 mypy-boto3-servicecatalog-1.26.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/setup.py
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/LICENSE` & `mypy-boto3-servicecatalog-1.26.79/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/PKG-INFO` & `mypy-boto3-servicecatalog-1.26.79/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.26.13.post9
-Summary: Type annotations for boto3.ServiceCatalog 1.26.13 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.79
+Summary: Type annotations for boto3.ServiceCatalog 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/README.md` & `mypy-boto3-servicecatalog-1.26.79/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__init__.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__init__.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/__main__.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceCatalog 1.26.13\nVersion:         1.26.13.post9\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.ServiceCatalog 1.26.79\nVersion:         1.26.79\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.13.post9")
+    print("1.26.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/client.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/client.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/literals.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -194,27 +195,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -243,14 +247,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -317,30 +322,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -372,28 +380,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -421,30 +433,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -460,14 +476,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/literals.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -192,27 +193,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -241,14 +245,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -315,30 +320,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -370,28 +378,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -419,30 +431,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -458,14 +474,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/paginator.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/paginator.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/type_defs.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog/type_defs.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.26.13.post9
-Summary: Type annotations for boto3.ServiceCatalog 1.26.13 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.79
+Summary: Type annotations for boto3.ServiceCatalog 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.13](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/mypy_boto3_servicecatalog.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.13.post9/setup.py` & `mypy-boto3-servicecatalog-1.26.79/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-servicecatalog",
-    version="1.26.13.post9",
+    version="1.26.79",
     packages=["mypy_boto3_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceCatalog 1.26.13 service generated with"
-        " mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.ServiceCatalog 1.26.79 service generated with"
+        " mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 servicecatalog type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_servicecatalog": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_servicecatalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

