# Comparing `tmp/mypy-boto3-redshift-data-1.26.30.tar.gz` & `tmp/mypy-boto3-redshift-data-1.26.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-data-1.26.30.tar", last modified: Wed Dec 14 20:47:11 2022, max compression
+gzip compressed data, was "mypy-boto3-redshift-data-1.26.88.tar", last modified: Thu Mar  9 20:38:41 2023, max compression
```

## Comparing `mypy-boto3-redshift-data-1.26.30.tar` & `mypy-boto3-redshift-data-1.26.88.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.689211 mypy-boto3-redshift-data-1.26.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2022-12-14 20:47:11.689211 mypy-boto3-redshift-data-1.26.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.689211 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16684 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 20:47:11.689211 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-14 20:47:11.000000 mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 20:47:11.689211 mypy-boto3-redshift-data-1.26.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-14 20:47:02.000000 mypy-boto3-redshift-data-1.26.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-09 20:37:54.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 20:38:41.000000 mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 20:38:41.678347 mypy-boto3-redshift-data-1.26.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-09 20:37:53.000000 mypy-boto3-redshift-data-1.26.88/setup.py
```

### Comparing `mypy-boto3-redshift-data-1.26.30/LICENSE` & `mypy-boto3-redshift-data-1.26.88/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/PKG-INFO` & `mypy-boto3-redshift-data-1.26.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.26.30
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.88
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-data-1.26.30/README.md` & `mypy-boto3-redshift-data-1.26.88/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__init__.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__init__.pyi` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/__main__.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftDataAPIService 1.26.30\nVersion:        "
-        " 1.26.30\nBuilder version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.RedshiftDataAPIService 1.26.88\nVersion:        "
+        " 1.26.88\nBuilder version: 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.30")
+    print("1.26.88")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/client.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/client.pyi` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/literals.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,24 +85,26 @@
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -188,14 +190,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -210,30 +213,33 @@
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
@@ -361,14 +367,15 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/literals.pyi` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,24 +83,26 @@
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
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -186,14 +188,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -208,30 +211,33 @@
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
@@ -359,14 +365,15 @@
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

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/paginator.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/paginator.pyi` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/type_defs.py` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data/type_defs.pyi` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/PKG-INFO` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.26.30
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.30 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.88
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-data?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.26.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.26.88](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-data-1.26.30/mypy_boto3_redshift_data.egg-info/SOURCES.txt` & `mypy-boto3-redshift-data-1.26.88/mypy_boto3_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.26.30/setup.py` & `mypy-boto3-redshift-data-1.26.88/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-redshift-data",
-    version="1.26.30",
+    version="1.26.88",
     packages=["mypy_boto3_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftDataAPIService 1.26.30 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.RedshiftDataAPIService 1.26.88 service generated with"
+        " mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

