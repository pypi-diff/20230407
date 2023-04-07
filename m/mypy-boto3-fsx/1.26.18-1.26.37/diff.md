# Comparing `tmp/mypy-boto3-fsx-1.26.18.tar.gz` & `tmp/mypy-boto3-fsx-1.26.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.26.18.tar", last modified: Tue Nov 29 06:12:18 2022, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.26.37.tar", last modified: Fri Dec 23 20:32:30 2022, max compression
```

## Comparing `mypy-boto3-fsx-1.26.18.tar` & `mypy-boto3-fsx-1.26.37.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.249822 mypy-boto3-fsx-1.26.18/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    21911 2022-11-29 06:12:18.241821 mypy-boto3-fsx-1.26.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20490 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.241821 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38793 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    38740 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14047 2022-11-29 06:10:08.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14045 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6578 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    78987 2022-11-29 06:10:10.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    78890 2022-11-29 06:10:08.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.241821 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21911 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-29 06:12:18.000000 mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:12:18.249822 mypy-boto3-fsx-1.26.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2022-11-29 06:10:07.000000 mypy-boto3-fsx-1.26.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.588941 mypy-boto3-fsx-1.26.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21998 2022-12-23 20:32:30.584941 mypy-boto3-fsx-1.26.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.580941 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38793 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79078 2022-12-23 20:32:18.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78981 2022-12-23 20:32:17.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 20:32:30.584941 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21998 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2022-12-23 20:32:30.000000 mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 20:32:30.588941 mypy-boto3-fsx-1.26.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2022-12-23 20:32:16.000000 mypy-boto3-fsx-1.26.37/setup.py
```

### Comparing `mypy-boto3-fsx-1.26.18/LICENSE` & `mypy-boto3-fsx-1.26.37/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/PKG-INFO` & `mypy-boto3-fsx-1.26.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.26.18
-Summary: Type annotations for boto3.FSx 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.37
+Summary: Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,14 +361,15 @@
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
+    StorageVirtualMachineSubtypeType,
     TieringPolicyNameType,
     VolumeFilterNameType,
     VolumeLifecycleType,
     VolumeTypeType,
     WindowsAccessAuditLogLevelType,
     WindowsDeploymentTypeType,
     FSxServiceName,
```

### Comparing `mypy-boto3-fsx-1.26.18/README.md` & `mypy-boto3-fsx-1.26.37/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,14 +329,15 @@
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
+    StorageVirtualMachineSubtypeType,
     TieringPolicyNameType,
     VolumeFilterNameType,
     VolumeLifecycleType,
     VolumeTypeType,
     WindowsAccessAuditLogLevelType,
     WindowsDeploymentTypeType,
     FSxServiceName,
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.26.18\nVersion:         1.26.18\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.FSx 1.26.37\nVersion:         1.26.37\nBuilder version:"
+        " 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.18")
+    print("1.26.37")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
@@ -66,28 +65,28 @@
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
+    "StorageVirtualMachineSubtypeType",
     "TieringPolicyNameType",
     "VolumeFilterNameType",
     "VolumeLifecycleType",
     "VolumeTypeType",
     "WindowsAccessAuditLogLevelType",
     "WindowsDeploymentTypeType",
     "FSxServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdministrativeActionTypeType = Literal[
     "FILE_SYSTEM_ALIAS_ASSOCIATION",
     "FILE_SYSTEM_ALIAS_DISASSOCIATION",
     "FILE_SYSTEM_UPDATE",
     "RELEASE_NFS_V3_LOCKS",
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
@@ -170,14 +169,17 @@
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
 ]
 StorageVirtualMachineRootVolumeSecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+StorageVirtualMachineSubtypeType = Literal[
+    "DEFAULT", "DP_DESTINATION", "SYNC_DESTINATION", "SYNC_SOURCE"
+]
 TieringPolicyNameType = Literal["ALL", "AUTO", "NONE", "SNAPSHOT_ONLY"]
 VolumeFilterNameType = Literal["file-system-id", "storage-virtual-machine-id"]
 VolumeLifecycleType = Literal[
     "AVAILABLE", "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
 ]
 VolumeTypeType = Literal["ONTAP", "OPENZFS"]
 WindowsAccessAuditLogLevelType = Literal[
@@ -237,14 +239,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
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
@@ -273,14 +276,15 @@
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
@@ -352,25 +356,27 @@
     "kafkaconnect",
     "kendra",
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
@@ -403,28 +409,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -452,30 +461,34 @@
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
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
     "DataCompressionTypeType",
@@ -65,27 +66,29 @@
     "SnapshotFilterNameType",
     "SnapshotLifecycleType",
     "StatusType",
     "StorageTypeType",
     "StorageVirtualMachineFilterNameType",
     "StorageVirtualMachineLifecycleType",
     "StorageVirtualMachineRootVolumeSecurityStyleType",
+    "StorageVirtualMachineSubtypeType",
     "TieringPolicyNameType",
     "VolumeFilterNameType",
     "VolumeLifecycleType",
     "VolumeTypeType",
     "WindowsAccessAuditLogLevelType",
     "WindowsDeploymentTypeType",
     "FSxServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdministrativeActionTypeType = Literal[
     "FILE_SYSTEM_ALIAS_ASSOCIATION",
     "FILE_SYSTEM_ALIAS_DISASSOCIATION",
     "FILE_SYSTEM_UPDATE",
     "RELEASE_NFS_V3_LOCKS",
     "SNAPSHOT_UPDATE",
     "STORAGE_OPTIMIZATION",
@@ -168,14 +171,17 @@
 StatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "UPDATED_OPTIMIZING"]
 StorageTypeType = Literal["HDD", "SSD"]
 StorageVirtualMachineFilterNameType = Literal["file-system-id"]
 StorageVirtualMachineLifecycleType = Literal[
     "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
 ]
 StorageVirtualMachineRootVolumeSecurityStyleType = Literal["MIXED", "NTFS", "UNIX"]
+StorageVirtualMachineSubtypeType = Literal[
+    "DEFAULT", "DP_DESTINATION", "SYNC_DESTINATION", "SYNC_SOURCE"
+]
 TieringPolicyNameType = Literal["ALL", "AUTO", "NONE", "SNAPSHOT_ONLY"]
 VolumeFilterNameType = Literal["file-system-id", "storage-virtual-machine-id"]
 VolumeLifecycleType = Literal[
     "AVAILABLE", "CREATED", "CREATING", "DELETING", "FAILED", "MISCONFIGURED", "PENDING"
 ]
 VolumeTypeType = Literal["ONTAP", "OPENZFS"]
 WindowsAccessAuditLogLevelType = Literal[
@@ -235,14 +241,15 @@
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
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
@@ -271,14 +278,15 @@
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
@@ -350,25 +358,27 @@
     "kafkaconnect",
     "kendra",
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
@@ -401,28 +411,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -450,30 +463,34 @@
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
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     SecurityStyleType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
+    StorageVirtualMachineSubtypeType,
     TieringPolicyNameType,
     VolumeFilterNameType,
     VolumeLifecycleType,
     VolumeTypeType,
     WindowsAccessAuditLogLevelType,
     WindowsDeploymentTypeType,
 )
@@ -66,15 +67,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
@@ -287,22 +287,20 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -361,19 +359,17 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
-
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
-
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -387,21 +383,19 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
-
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
     total=False,
@@ -430,22 +424,20 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -453,22 +445,20 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
-
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -538,21 +528,19 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -560,86 +548,78 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
-
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -685,22 +665,20 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -745,22 +723,20 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -775,42 +751,38 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
-
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
-
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
-
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -843,22 +815,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": List[str],
     },
 )
@@ -882,22 +852,20 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -906,22 +874,20 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
-
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -976,21 +942,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -998,21 +962,19 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
-
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
-
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1151,21 +1113,19 @@
     {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
-
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
-
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1185,21 +1145,19 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
-
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1219,21 +1177,19 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1335,22 +1291,20 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
-
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1359,22 +1313,20 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
-
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1424,22 +1376,20 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1491,22 +1441,20 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1522,22 +1470,20 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -1551,21 +1497,19 @@
         "OntapVolumeType": InputOntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
     },
     total=False,
 )
 
-
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
-
 OntapVolumeConfigurationTypeDef = TypedDict(
     "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
@@ -1642,21 +1586,19 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
-
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
-
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1704,22 +1646,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1781,22 +1721,20 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
-
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1822,15 +1760,15 @@
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
     },
     total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
@@ -1890,21 +1828,19 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1938,22 +1874,20 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 DataRepositoryAssociationTypeDef = TypedDict(
     "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
@@ -1985,22 +1919,20 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -2010,21 +1942,19 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -2045,21 +1975,19 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
-
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2081,22 +2009,20 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
-
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2106,22 +2032,20 @@
         "ClientRequestToken": str,
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVolumeFromBackupRequestRequestTypeDef(
     _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
     _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
 ):
     pass
 
-
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
@@ -2173,21 +2097,19 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
-
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
-
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2292,22 +2214,20 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
-
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
-
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
@@ -2367,21 +2287,19 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2390,33 +2308,32 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
-
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
+        "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagTypeDef],
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
@@ -2487,15 +2404,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2513,21 +2430,19 @@
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2541,22 +2456,20 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "CreationTime": datetime,
         "FileSystemId": str,
         "Lifecycle": VolumeLifecycleType,
         "Name": str,
@@ -2585,21 +2498,19 @@
         "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
         "Name": str,
         "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
-
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2641,22 +2552,20 @@
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
         "StorageCapacity": int,
     },
     total=False,
 )
 
-
 class CreateFileSystemFromBackupRequestRequestTypeDef(
     _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
     _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "FileSystemType": FileSystemTypeType,
         "StorageCapacity": int,
         "SubnetIds": Sequence[str],
     },
@@ -2674,21 +2583,19 @@
         "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
@@ -2724,19 +2631,17 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
-
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
-
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     SecurityStyleType,
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
+    StorageVirtualMachineSubtypeType,
     TieringPolicyNameType,
     VolumeFilterNameType,
     VolumeLifecycleType,
     VolumeTypeType,
     WindowsAccessAuditLogLevelType,
     WindowsDeploymentTypeType,
 )
@@ -66,14 +67,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutoExportPolicyTypeDef",
@@ -286,20 +288,22 @@
     "_OptionalAssociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -358,17 +362,19 @@
         "Path": str,
         "Format": Literal["REPORT_CSV_20191124"],
         "Scope": Literal["FAILED_FILES_ONLY"],
     },
     total=False,
 )
 
+
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
+
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
@@ -382,19 +388,21 @@
     "_OptionalLustreLogCreateConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogCreateConfigurationTypeDef(
     _RequiredLustreLogCreateConfigurationTypeDef, _OptionalLustreLogCreateConfigurationTypeDef
 ):
     pass
 
+
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
         "NoSquashNids": List[str],
     },
     total=False,
@@ -423,20 +431,22 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
+
 class SelfManagedActiveDirectoryConfigurationTypeDef(
     _RequiredSelfManagedActiveDirectoryConfigurationTypeDef,
     _OptionalSelfManagedActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredWindowsAuditLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogCreateConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -444,20 +454,22 @@
     "_OptionalWindowsAuditLogCreateConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogCreateConfigurationTypeDef(
     _RequiredWindowsAuditLogCreateConfigurationTypeDef,
     _OptionalWindowsAuditLogCreateConfigurationTypeDef,
 ):
     pass
 
+
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
     total=False,
@@ -527,19 +539,21 @@
     "_OptionalDeleteBackupRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -547,78 +561,86 @@
     {
         "ClientRequestToken": str,
         "DeleteDataInFileSystem": bool,
     },
     total=False,
 )
 
+
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
     },
 )
 _OptionalDeleteFileCacheRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteFileCacheRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 _OptionalDeleteSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStorageVirtualMachineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteVolumeOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     {
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
@@ -664,20 +686,22 @@
         "ClientRequestToken": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeFileSystemAliasesRequestRequestTypeDef(
     _RequiredDescribeFileSystemAliasesRequestRequestTypeDef,
     _OptionalDescribeFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -722,20 +746,22 @@
     "_OptionalDisassociateFileSystemAliasesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+
 FileCacheFailureDetailsTypeDef = TypedDict(
     "FileCacheFailureDetailsTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
@@ -750,38 +776,42 @@
     "_OptionalFileCacheNFSConfigurationTypeDef",
     {
         "DnsIps": Sequence[str],
     },
     total=False,
 )
 
+
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
+
 _RequiredLustreLogConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogConfigurationTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
     },
 )
 _OptionalLustreLogConfigurationTypeDef = TypedDict(
     "_OptionalLustreLogConfigurationTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
+
 class LustreLogConfigurationTypeDef(
     _RequiredLustreLogConfigurationTypeDef, _OptionalLustreLogConfigurationTypeDef
 ):
     pass
 
+
 FileSystemEndpointTypeDef = TypedDict(
     "FileSystemEndpointTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
     total=False,
@@ -814,20 +844,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
         "Options": List[str],
     },
 )
@@ -851,20 +883,22 @@
     "_OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef",
     {
         "VolumeId": str,
         "SnapshotId": str,
     },
 )
@@ -873,20 +907,22 @@
     {
         "ClientRequestToken": str,
         "Options": Sequence[RestoreOpenZFSVolumeOptionType],
     },
     total=False,
 )
 
+
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
+
 SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
     "SelfManagedActiveDirectoryAttributesTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
@@ -941,19 +977,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWindowsAuditLogConfigurationTypeDef = TypedDict(
     "_RequiredWindowsAuditLogConfigurationTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
     },
 )
@@ -961,19 +999,21 @@
     "_OptionalWindowsAuditLogConfigurationTypeDef",
     {
         "AuditLogDestination": str,
     },
     total=False,
 )
 
+
 class WindowsAuditLogConfigurationTypeDef(
     _RequiredWindowsAuditLogConfigurationTypeDef, _OptionalWindowsAuditLogConfigurationTypeDef
 ):
     pass
 
+
 AssociateFileSystemAliasesResponseTypeDef = TypedDict(
     "AssociateFileSystemAliasesResponseTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1112,19 +1152,21 @@
     {
         "DnsIps": List[str],
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
+
 class NFSDataRepositoryConfigurationTypeDef(
     _RequiredNFSDataRepositoryConfigurationTypeDef, _OptionalNFSDataRepositoryConfigurationTypeDef
 ):
     pass
 
+
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
@@ -1144,19 +1186,21 @@
         "KmsKeyId": str,
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyBackupRequestRequestTypeDef(
     _RequiredCopyBackupRequestRequestTypeDef, _OptionalCopyBackupRequestRequestTypeDef
 ):
     pass
 
+
 CreateBackupRequestRequestTypeDef = TypedDict(
     "CreateBackupRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
@@ -1176,19 +1220,21 @@
     {
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemLustreConfigurationTypeDef = TypedDict(
     "DeleteFileSystemLustreConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
@@ -1290,20 +1336,22 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "CapacityToRelease": int,
     },
     total=False,
 )
 
+
 class CreateDataRepositoryTaskRequestRequestTypeDef(
     _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
     _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1312,20 +1360,22 @@
     "_OptionalCreateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileCacheLustreConfigurationTypeDef(
     _RequiredCreateFileCacheLustreConfigurationTypeDef,
     _OptionalCreateFileCacheLustreConfigurationTypeDef,
 ):
     pass
 
+
 CreateFileSystemLustreConfigurationTypeDef = TypedDict(
     "CreateFileSystemLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
@@ -1375,20 +1425,22 @@
         "PreferredSubnetId": str,
         "RouteTableIds": Sequence[str],
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
+
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSFileSystemConfigurationTypeDef = TypedDict(
     "OpenZFSFileSystemConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "CopyTagsToVolumes": bool,
         "DailyAutomaticBackupStartTime": str,
@@ -1440,20 +1492,22 @@
     "_OptionalCreateSvmActiveDirectoryConfigurationTypeDef",
     {
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateSvmActiveDirectoryConfigurationTypeDef(
     _RequiredCreateSvmActiveDirectoryConfigurationTypeDef,
     _OptionalCreateSvmActiveDirectoryConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemWindowsConfigurationTypeDef",
     {
         "ThroughputCapacity": int,
     },
 )
 _OptionalCreateFileSystemWindowsConfigurationTypeDef = TypedDict(
@@ -1469,20 +1523,22 @@
         "CopyTagsToBackups": bool,
         "Aliases": Sequence[str],
         "AuditLogConfiguration": WindowsAuditLogCreateConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -1496,19 +1552,21 @@
         "OntapVolumeType": InputOntapVolumeTypeType,
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
     },
     total=False,
 )
 
+
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
+
 OntapVolumeConfigurationTypeDef = TypedDict(
     "OntapVolumeConfigurationTypeDef",
     {
         "FlexCacheEndpointType": FlexCacheEndpointTypeType,
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
@@ -1585,19 +1643,21 @@
         "Report": CompletionReportTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
     total=False,
 )
 
+
 class DataRepositoryTaskTypeDef(
     _RequiredDataRepositoryTaskTypeDef, _OptionalDataRepositoryTaskTypeDef
 ):
     pass
 
+
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
         "BackupIds": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1645,20 +1705,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "SnapshotIds": Sequence[str],
         "Filters": Sequence[SnapshotFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
@@ -1720,20 +1782,22 @@
     {
         "DataRepositorySubdirectories": Sequence[str],
         "NFS": FileCacheNFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
+
 FileCacheLustreConfigurationTypeDef = TypedDict(
     "FileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1759,15 +1823,15 @@
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "Tags": List[TagTypeDef],
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
     },
     total=False,
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
@@ -1827,19 +1891,21 @@
     {
         "ClientRequestToken": str,
         "LustreConfiguration": UpdateFileCacheLustreConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 WindowsFileSystemConfigurationTypeDef = TypedDict(
     "WindowsFileSystemConfigurationTypeDef",
     {
         "ActiveDirectoryId": str,
         "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
@@ -1873,20 +1939,22 @@
         "S3": S3DataRepositoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 DataRepositoryAssociationTypeDef = TypedDict(
     "DataRepositoryAssociationTypeDef",
     {
         "AssociationId": str,
         "ResourceARN": str,
         "FileSystemId": str,
         "Lifecycle": DataRepositoryLifecycleType,
@@ -1918,20 +1986,22 @@
         "ClientRequestToken": str,
         "ImportedFileChunkSize": int,
         "S3": S3DataRepositoryConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -1941,19 +2011,21 @@
         "WindowsConfiguration": DeleteFileSystemWindowsConfigurationTypeDef,
         "LustreConfiguration": DeleteFileSystemLustreConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 DeleteFileSystemResponseTypeDef = TypedDict(
     "DeleteFileSystemResponseTypeDef",
     {
         "FileSystemId": str,
         "Lifecycle": FileSystemLifecycleType,
         "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
         "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
@@ -1974,19 +2046,21 @@
         "ClientRequestToken": str,
         "OntapConfiguration": DeleteVolumeOntapConfigurationTypeDef,
         "OpenZFSConfiguration": DeleteVolumeOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
+
 DeleteVolumeResponseTypeDef = TypedDict(
     "DeleteVolumeResponseTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
         "OntapResponse": DeleteVolumeOntapResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2008,20 +2082,22 @@
         "SvmAdminPassword": str,
         "Tags": Sequence[TagTypeDef],
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
 
+
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2031,20 +2107,22 @@
         "ClientRequestToken": str,
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVolumeFromBackupRequestRequestTypeDef(
     _RequiredCreateVolumeFromBackupRequestRequestTypeDef,
     _OptionalCreateVolumeFromBackupRequestRequestTypeDef,
 ):
     pass
 
+
 LustreFileSystemConfigurationTypeDef = TypedDict(
     "LustreFileSystemConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
         "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
@@ -2096,19 +2174,21 @@
         "KmsKeyId": str,
         "LustreConfiguration": CreateFileCacheLustreConfigurationTypeDef,
         "DataRepositoryAssociations": Sequence[FileCacheDataRepositoryAssociationTypeDef],
     },
     total=False,
 )
 
+
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
+
 FileCacheCreatingTypeDef = TypedDict(
     "FileCacheCreatingTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
@@ -2213,20 +2293,22 @@
         "ReadOnly": bool,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
     },
     total=False,
 )
 
+
 class CreateOpenZFSVolumeConfigurationTypeDef(
     _RequiredCreateOpenZFSVolumeConfigurationTypeDef,
     _OptionalCreateOpenZFSVolumeConfigurationTypeDef,
 ):
     pass
 
+
 OpenZFSCreateRootVolumeConfigurationTypeDef = TypedDict(
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
     {
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
@@ -2286,19 +2368,21 @@
         "LustreConfiguration": UpdateFileSystemLustreConfigurationTypeDef,
         "OntapConfiguration": UpdateFileSystemOntapConfigurationTypeDef,
         "OpenZFSConfiguration": UpdateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageVirtualMachineRequestRequestTypeDef",
     {
         "StorageVirtualMachineId": str,
     },
 )
 _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
@@ -2307,31 +2391,34 @@
         "ActiveDirectoryConfiguration": UpdateSvmActiveDirectoryConfigurationTypeDef,
         "ClientRequestToken": str,
         "SvmAdminPassword": str,
     },
     total=False,
 )
 
+
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
+
 StorageVirtualMachineTypeDef = TypedDict(
     "StorageVirtualMachineTypeDef",
     {
         "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
         "CreationTime": datetime,
         "Endpoints": SvmEndpointsTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
+        "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
         "Tags": List[TagTypeDef],
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
     total=False,
 )
@@ -2402,15 +2489,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2428,19 +2515,21 @@
         "OntapConfiguration": CreateOntapVolumeConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
         "OpenZFSConfiguration": CreateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
         "ThroughputCapacity": int,
     },
 )
@@ -2454,20 +2543,22 @@
         "WeeklyMaintenanceStartTime": str,
         "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
         "RootVolumeConfiguration": OpenZFSCreateRootVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
+
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "CreationTime": datetime,
         "FileSystemId": str,
         "Lifecycle": VolumeLifecycleType,
         "Name": str,
@@ -2496,19 +2587,21 @@
         "OntapConfiguration": UpdateOntapVolumeConfigurationTypeDef,
         "Name": str,
         "OpenZFSConfiguration": UpdateOpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
+
 CreateStorageVirtualMachineResponseTypeDef = TypedDict(
     "CreateStorageVirtualMachineResponseTypeDef",
     {
         "StorageVirtualMachine": StorageVirtualMachineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2550,20 +2643,22 @@
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
         "StorageCapacity": int,
     },
     total=False,
 )
 
+
 class CreateFileSystemFromBackupRequestRequestTypeDef(
     _RequiredCreateFileSystemFromBackupRequestRequestTypeDef,
     _OptionalCreateFileSystemFromBackupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "FileSystemType": FileSystemTypeType,
         "StorageCapacity": int,
         "SubnetIds": Sequence[str],
     },
@@ -2581,19 +2676,21 @@
         "OntapConfiguration": CreateFileSystemOntapConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": CreateFileSystemOpenZFSConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 AdministrativeActionTypeDef = TypedDict(
     "AdministrativeActionTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
@@ -2629,17 +2726,19 @@
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
         "Volume": VolumeTypeDef,
     },
     total=False,
 )
 
+
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+
 CreateVolumeFromBackupResponseTypeDef = TypedDict(
     "CreateVolumeFromBackupResponseTypeDef",
     {
         "Volume": VolumeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.26.18
-Summary: Type annotations for boto3.FSx 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.37
+Summary: Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.26.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,14 +361,15 @@
     SnapshotFilterNameType,
     SnapshotLifecycleType,
     StatusType,
     StorageTypeType,
     StorageVirtualMachineFilterNameType,
     StorageVirtualMachineLifecycleType,
     StorageVirtualMachineRootVolumeSecurityStyleType,
+    StorageVirtualMachineSubtypeType,
     TieringPolicyNameType,
     VolumeFilterNameType,
     VolumeLifecycleType,
     VolumeTypeType,
     WindowsAccessAuditLogLevelType,
     WindowsDeploymentTypeType,
     FSxServiceName,
```

### Comparing `mypy-boto3-fsx-1.26.18/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.26.37/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.26.18/setup.py` & `mypy-boto3-fsx-1.26.37/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.26.18",
+    version="1.26.37",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.26.18 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.FSx 1.26.37 service generated with mypy-boto3-builder 7.12.2"
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
     keywords="boto3 fsx type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_fsx": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_fsx": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

