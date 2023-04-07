# Comparing `tmp/mtsql-1.3.202303251820-py3-none-any.whl.zip` & `tmp/mtsql-1.3.202304072016-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18942 bytes, number of entries: 11
+Zip file size: 18946 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
 -rw-r--r--  2.0 unx     9605 b- defN 23-Feb-28 20:18 mt/sql/base.py
 -rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
--rw-r--r--  2.0 unx    61149 b- defN 23-Mar-25 18:20 mt/sql/psql.py
+-rw-r--r--  2.0 unx    61173 b- defN 23-Apr-07 20:16 mt/sql/psql.py
 -rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Mar-25 18:20 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Mar-25 18:20 mtsql-1.3.202303251820.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-Mar-25 18:20 mtsql-1.3.202303251820.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-25 18:20 mtsql-1.3.202303251820.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Mar-25 18:20 mtsql-1.3.202303251820.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-Mar-25 18:20 mtsql-1.3.202303251820.dist-info/RECORD
-11 files, 87391 bytes uncompressed, 17488 bytes compressed:  80.0%
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-07 20:16 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/RECORD
+11 files, 87415 bytes uncompressed, 17492 bytes compressed:  80.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.3.202303251820.dist-info/LICENSE
+Filename: mtsql-1.3.202304072016.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.3.202303251820.dist-info/METADATA
+Filename: mtsql-1.3.202304072016.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.3.202303251820.dist-info/WHEEL
+Filename: mtsql-1.3.202304072016.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.3.202303251820.dist-info/top_level.txt
+Filename: mtsql-1.3.202304072016.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.3.202303251820.dist-info/RECORD
+Filename: mtsql-1.3.202304072016.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/psql.py

```diff
@@ -1,11 +1,12 @@
 """Useful modules for accessing PostgreSQL"""
 
 from typing import Optional
 
+import sqlalchemy as sa
 import re
 import psycopg2 as ps
 import sqlalchemy.exc as se
 from tqdm import tqdm  # nice progress bar
 
 from mt import pd, np
 import mt.base.path as _p
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('03')
-VERSION_DAY = int('25')
-VERSION_HOUR = int('18')
-VERSION_MINUTE = int('20')
+VERSION_MONTH = int('04')
+VERSION_DAY = int('07')
+VERSION_HOUR = int('20')
+VERSION_MINUTE = int('16')
 MAJOR_VERSION = 1
 MINOR_VERSION = 3
-PATCH_VERSION = 202303251820
-version_date = '2023/03/25 18:20'
+PATCH_VERSION = 202304072016
+version_date = '2023/04/07 20:16'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.3.202303251820.dist-info/LICENSE` & `mtsql-1.3.202304072016.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.3.202303251820.dist-info/METADATA` & `mtsql-1.3.202304072016.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.3.202303251820
+Version: 1.3.202304072016
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

## Comparing `mtsql-1.3.202303251820.dist-info/RECORD` & `mtsql-1.3.202304072016.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mt/sql/__init__.py,sha256=b7zO50apZxt9Hg2eOkJhRLrXgACR8eS5b-Rphdn5qNQ,44
 mt/sql/base.py,sha256=j0M3f7Z5UxexwDzSUsdm_45bsOfkUt5uZh1kLk89wQs,9605
 mt/sql/mysql.py,sha256=n2ENDctdUqZuSaDAcrqZYtPtawq3Wx4dOPCRsCB5Q4w,4894
-mt/sql/psql.py,sha256=1QSdfuSNAaJBueI7AxOfURABqvs8cT6bRIfiGGgG36A,61149
+mt/sql/psql.py,sha256=E79TdH6Bpwz09uhVq0xXbfINtebFPS8hsKw9_Q0cE5M,61173
 mt/sql/sqlite.py,sha256=T2ak_hhNi_zRfpg_gp8JhNHn7D2kl4i-Ey6-9ANMtz0,8678
-mt/sql/version.py,sha256=bxmNdFWlyPPojfJLhT8aci2pmROKH9t80jRaKp4imWU,396
-mtsql-1.3.202303251820.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
-mtsql-1.3.202303251820.dist-info/METADATA,sha256=om6LiHFfEV4Cve76XAgJogrJynZs6SVcTxhwTYL8lDY,597
-mtsql-1.3.202303251820.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mtsql-1.3.202303251820.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
-mtsql-1.3.202303251820.dist-info/RECORD,,
+mt/sql/version.py,sha256=ouijTUttXWymxAsJQ6GDhliCKCDPTo6wKKXQMJW1lV0,396
+mtsql-1.3.202304072016.dist-info/LICENSE,sha256=PojkRlQzTT5Eg6Nj03XoIVEefN3u8iiIFf1p4rqe_t4,1070
+mtsql-1.3.202304072016.dist-info/METADATA,sha256=KuH_szigvyFhTuKvKszmM3ClNmtMmql7SFtKN7VFdy8,597
+mtsql-1.3.202304072016.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mtsql-1.3.202304072016.dist-info/top_level.txt,sha256=WcqGFu9cV7iMZg09iam8eNxUvGpLSKKF2Iubf6SJVOo,3
+mtsql-1.3.202304072016.dist-info/RECORD,,
```

