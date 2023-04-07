# Comparing `tmp/fairscape_cli-0.1.1-py3-none-any.whl.zip` & `tmp/fairscape_cli-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 19351 bytes, number of entries: 32
+Zip file size: 19344 bytes, number of entries: 32
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 fairscape_cli/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/apps/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 80-Jan-01 00:00 fairscape_cli/apps/cache.py
 -rw-r--r--  2.0 unx      510 b- defN 80-Jan-01 00:00 fairscape_cli/apps/describe.py
 -rw-r--r--  2.0 unx      764 b- defN 80-Jan-01 00:00 fairscape_cli/apps/fairscape.py
 -rw-r--r--  2.0 unx       89 b- defN 80-Jan-01 00:00 fairscape_cli/apps/list.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 fairscape_cli/apps/models/__init__.py
 -rw-r--r--  2.0 unx      340 b- defN 80-Jan-01 00:00 fairscape_cli/apps/models/computation.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 fairscape_cli/apps/models/dataset.py
 -rw-r--r--  2.0 unx     1890 b- defN 80-Jan-01 00:00 fairscape_cli/apps/models/software.py
 -rw-r--r--  2.0 unx     8135 b- defN 80-Jan-01 00:00 fairscape_cli/apps/objects.py
 -rw-r--r--  2.0 unx     3369 b- defN 80-Jan-01 00:00 fairscape_cli/apps/rocrate.py
 -rw-r--r--  2.0 unx     2276 b- defN 80-Jan-01 00:00 fairscape_cli/apps/utils.py
 -rw-r--r--  2.0 unx     2677 b- defN 80-Jan-01 00:00 fairscape_cli/apps/validator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/cli.py
+-rw-r--r--  2.0 unx      397 b- defN 80-Jan-01 00:00 fairscape_cli/main.py
 -rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 fairscape_cli/models/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 80-Jan-01 00:00 fairscape_cli/models/computation.py
 -rw-r--r--  2.0 unx      205 b- defN 80-Jan-01 00:00 fairscape_cli/models/dataset.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/models/models.py
 -rw-r--r--  2.0 unx      924 b- defN 80-Jan-01 00:00 fairscape_cli/models/rocrate.py
 -rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 fairscape_cli/models/software.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/rocrate/__init__.py
 -rw-r--r--  2.0 unx    14769 b- defN 80-Jan-01 00:00 fairscape_cli/rocrate/rocrate.py
 -rw-r--r--  2.0 unx     1326 b- defN 80-Jan-01 00:00 fairscape_cli/rocrate/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fairscape_cli/validate/__init__.py
 -rw-r--r--  2.0 unx     1365 b- defN 80-Jan-01 00:00 fairscape_cli/validate/validate_json.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4724 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2767 b- defN 16-Jan-01 00:00 fairscape_cli-0.1.1.dist-info/RECORD
-32 files, 51383 bytes uncompressed, 14835 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4724 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 fairscape_cli-0.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2763 b- defN 16-Jan-01 00:00 fairscape_cli-0.1.2.dist-info/RECORD
+32 files, 51379 bytes uncompressed, 14836 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,13 +1,10 @@
 Filename: fairscape_cli/__init__.py
 Comment: 
 
-Filename: fairscape_cli/__main__.py
-Comment: 
-
 Filename: fairscape_cli/apps/__init__.py
 Comment: 
 
 Filename: fairscape_cli/apps/cache.py
 Comment: 
 
 Filename: fairscape_cli/apps/describe.py
@@ -42,14 +39,17 @@
 
 Filename: fairscape_cli/apps/validator.py
 Comment: 
 
 Filename: fairscape_cli/cli.py
 Comment: 
 
+Filename: fairscape_cli/main.py
+Comment: 
+
 Filename: fairscape_cli/models/__init__.py
 Comment: 
 
 Filename: fairscape_cli/models/computation.py
 Comment: 
 
 Filename: fairscape_cli/models/dataset.py
@@ -75,23 +75,23 @@
 
 Filename: fairscape_cli/validate/__init__.py
 Comment: 
 
 Filename: fairscape_cli/validate/validate_json.py
 Comment: 
 
-Filename: fairscape_cli-0.1.1.dist-info/LICENSE
+Filename: fairscape_cli-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: fairscape_cli-0.1.1.dist-info/METADATA
+Filename: fairscape_cli-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: fairscape_cli-0.1.1.dist-info/WHEEL
+Filename: fairscape_cli-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: fairscape_cli-0.1.1.dist-info/entry_points.txt
+Filename: fairscape_cli-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fairscape_cli-0.1.1.dist-info/RECORD
+Filename: fairscape_cli-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fairscape_cli-0.1.1.dist-info/LICENSE` & `fairscape_cli-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fairscape_cli-0.1.1.dist-info/METADATA` & `fairscape_cli-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: mlev71
 Author-email: max.adam.levinson@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `fairscape_cli-0.1.1.dist-info/RECORD` & `fairscape_cli-0.1.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 fairscape_cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fairscape_cli/__main__.py,sha256=OQah5l1vjnJq0SyBNBIbK-Gj90FdnZSb8ptkZJggW2g,397
 fairscape_cli/apps/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fairscape_cli/apps/cache.py,sha256=0fSBbuTAUW8W7H_5mYEfNV0qOxzpzWPZQUlthH6BW24,274
 fairscape_cli/apps/describe.py,sha256=BLoRpF1_bp1laIXJgpen_aXN4uB4BfMXxu4l6qYlTFg,510
 fairscape_cli/apps/fairscape.py,sha256=t3KngVBUGcVpY_3_uRx73x-YvbWYIJkjrj6-S9leoq8,764
 fairscape_cli/apps/list.py,sha256=EPuSNU8GmYI9W6JwLsUqjkapJcMlKr8MZf__3T02PIM,89
 fairscape_cli/apps/models/__init__.py,sha256=Cs9rVlD_QnwqTck0XlvlaWQplVJqzjs_ZjoONuw_opA,173
 fairscape_cli/apps/models/computation.py,sha256=E0WjOrb46WdAK9caT97paHXULWw11AUmxMjBBRFXCIA,340
 fairscape_cli/apps/models/dataset.py,sha256=enwbt2k5Qwuy5kdzojCaDsr-SU90hfs19PjUCk98D_c,2559
 fairscape_cli/apps/models/software.py,sha256=q9GUNeVMd67CySlFPy9Ko1r-jruh4G6lnhc0VOjtbBg,1890
 fairscape_cli/apps/objects.py,sha256=rMp7Youe8IMnV9RAicqtV0HMzsnJc8e0jl8_ipKbn8g,8135
 fairscape_cli/apps/rocrate.py,sha256=Yw9DWRJW8b2j0_QMVmWg4F4hrT7SD3JzhgprzM45OhU,3369
 fairscape_cli/apps/utils.py,sha256=pPK7-m82GBJTqYMvJhj1gt82P4wimJOzQpUdQxbPyCE,2276
 fairscape_cli/apps/validator.py,sha256=ou--6q37DFOTvuT3m5A07l0E4QIX02YsazcVFeFT39I,2677
 fairscape_cli/cli.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fairscape_cli/main.py,sha256=OQah5l1vjnJq0SyBNBIbK-Gj90FdnZSb8ptkZJggW2g,397
 fairscape_cli/models/__init__.py,sha256=r1BMiUXRH-Ys3sQRjLHfcM12kjEdKksMgLN7Z82STDA,221
 fairscape_cli/models/computation.py,sha256=P0NfON2bJFRwCq0FsnZ7n8hBqiD2sd2xo2v9ttGHlL8,291
 fairscape_cli/models/dataset.py,sha256=1Xyl9-K25PX7LPRuSo7gxVkfZWXn9sNA_wqChla_ZWg,205
 fairscape_cli/models/models.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fairscape_cli/models/rocrate.py,sha256=ugS-6JYTvGRV61__B_Rx-xhR6h2SyyVcT_lxY6UKPSg,924
 fairscape_cli/models/software.py,sha256=ngF1Rs-DphcU4CYgqsLi5g8T7Do50CxJn4yZiIE00aU,128
 fairscape_cli/rocrate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fairscape_cli/rocrate/rocrate.py,sha256=Ghkvd84P47hckRr7uNj858VXZhKUoTfWUYmL9NgkzgU,14769
 fairscape_cli/rocrate/utils.py,sha256=r-BiOwJEAcMAxXGp8cpb1_yRjHcF6VYxG9DAhjI4QWU,1326
 fairscape_cli/validate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fairscape_cli/validate/validate_json.py,sha256=2qkHGMnT2i6wGyhtdkK6a1fSLfzmKNIxWNmfwWweqDM,1365
-fairscape_cli-0.1.1.dist-info/LICENSE,sha256=PcuCQpGxZ1Tb7IcZraQxk5uLEARgk_bvaWhCV1s51Vg,1066
-fairscape_cli-0.1.1.dist-info/METADATA,sha256=0dILohK9DLvJYK0fP5J7husdnPXkrF3ftuJ2y-uYO08,4724
-fairscape_cli-0.1.1.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-fairscape_cli-0.1.1.dist-info/entry_points.txt,sha256=UCTm0OfEk7UB_d9lEpHInZx68ErRZCIcYL8aCZaYBEc,56
-fairscape_cli-0.1.1.dist-info/RECORD,,
+fairscape_cli-0.1.2.dist-info/LICENSE,sha256=PcuCQpGxZ1Tb7IcZraQxk5uLEARgk_bvaWhCV1s51Vg,1066
+fairscape_cli-0.1.2.dist-info/METADATA,sha256=M2TTXgNHfsuaBubzuLeRz2JGDCj1J11TwchWi6tPpaU,4724
+fairscape_cli-0.1.2.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
+fairscape_cli-0.1.2.dist-info/entry_points.txt,sha256=UCTm0OfEk7UB_d9lEpHInZx68ErRZCIcYL8aCZaYBEc,56
+fairscape_cli-0.1.2.dist-info/RECORD,,
```

