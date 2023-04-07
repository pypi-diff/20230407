# Comparing `tmp/bq_tools_dirupload-0.8.9-py3-none-any.whl.zip` & `tmp/bq_tools_dirupload-0.8.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15810 bytes, number of entries: 10
+Zip file size: 15837 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       65 b- defN 21-Mar-03 20:44 bq/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 21-Mar-03 20:44 bq/tools/__init__.py
 -rw-r--r--  2.0 unx     7488 b- defN 21-Apr-22 21:41 bq/tools/fetchdir.py
 -rw-r--r--  2.0 unx     5054 b- defN 21-Mar-03 20:44 bq/tools/pool.py
--rw-r--r--  2.0 unx    22587 b- defN 21-Sep-03 17:30 bq/tools/uploaddirp.py
--rw-r--r--  2.0 unx     8692 b- defN 21-Sep-03 17:32 bq_tools_dirupload-0.8.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-03 17:32 bq_tools_dirupload-0.8.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       96 b- defN 21-Sep-03 17:32 bq_tools_dirupload-0.8.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        3 b- defN 21-Sep-03 17:32 bq_tools_dirupload-0.8.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      821 b- defN 21-Sep-03 17:32 bq_tools_dirupload-0.8.9.dist-info/RECORD
-10 files, 44963 bytes uncompressed, 14398 bytes compressed:  68.0%
+-rw-r--r--  2.0 unx    22588 b- defN 21-Sep-03 17:50 bq/tools/uploaddirp.py
+-rw-r--r--  2.0 unx     8694 b- defN 21-Sep-03 17:51 bq_tools_dirupload-0.8.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Sep-03 17:51 bq_tools_dirupload-0.8.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       96 b- defN 21-Sep-03 17:51 bq_tools_dirupload-0.8.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        3 b- defN 21-Sep-03 17:51 bq_tools_dirupload-0.8.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      831 b- defN 21-Sep-03 17:51 bq_tools_dirupload-0.8.9.1.dist-info/RECORD
+10 files, 44976 bytes uncompressed, 14405 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: bq/tools/pool.py
 Comment: 
 
 Filename: bq/tools/uploaddirp.py
 Comment: 
 
-Filename: bq_tools_dirupload-0.8.9.dist-info/METADATA
+Filename: bq_tools_dirupload-0.8.9.1.dist-info/METADATA
 Comment: 
 
-Filename: bq_tools_dirupload-0.8.9.dist-info/WHEEL
+Filename: bq_tools_dirupload-0.8.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: bq_tools_dirupload-0.8.9.dist-info/entry_points.txt
+Filename: bq_tools_dirupload-0.8.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: bq_tools_dirupload-0.8.9.dist-info/top_level.txt
+Filename: bq_tools_dirupload-0.8.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bq_tools_dirupload-0.8.9.dist-info/RECORD
+Filename: bq_tools_dirupload-0.8.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bq/tools/uploaddirp.py

```diff
@@ -190,15 +190,15 @@
     new_resource_tags =copy.deepcopy (resource_tags)
     for tag, value in resource_tags.items():
         if tag in fixedtags:
             fixedtable = fixedtags[tag].get(value, None)
             if fixedtable is None:
                 args.log.warn ('%s not in fixedtable %s', value, tag)
             else:
-                args.log.debug("TABLE %s", fixedtable)
+                #args.log.debug("TABLE %s", fixedtable)
                 for ftag, fvalue in fixedtable.items():
                     new_resource_tags[ftag]=fvalue
     #new_resource_tags = apply_fixed_tags(args, filename, image_path, resource_tags, fixedtags)
     if resource_tags != new_resource_tags:
         args.log.info("Found new fixed tags after mapping %s", new_resource_tags)
         resource_tags = new_resource_tags
```

## Comparing `bq_tools_dirupload-0.8.9.dist-info/METADATA` & `bq_tools_dirupload-0.8.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-tools-dirupload
-Version: 0.8.9
+Version: 0.8.9.1
 Summary: Upload/Download files to bisque/ViQi in parallel
 Home-page: https://www.viqi.org
 Author: ViQi Inc
 Author-email: support@viqi.org
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bq_tools_dirupload-0.8.9.dist-info/RECORD` & `bq_tools_dirupload-0.8.9.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 bq/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 bq/tools/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 bq/tools/fetchdir.py,sha256=XlIoptarz4scM2OjezON1wLrGK1mG7cPS5Bp6mxhoQw,7488
 bq/tools/pool.py,sha256=tga44r3SWMuE6r3_-1Z8LMLd7_i2_NpuvFQq4wgQbTI,5054
-bq/tools/uploaddirp.py,sha256=pdbIV5d207r_AsdOHkqwVcaCcc4rwLP8ZStE8rEz_r0,22587
-bq_tools_dirupload-0.8.9.dist-info/METADATA,sha256=ePWUgEKs94z5X6s1iEL7Tuz-YeRZ0hjLPttYEd_q52g,8692
-bq_tools_dirupload-0.8.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-bq_tools_dirupload-0.8.9.dist-info/entry_points.txt,sha256=UzQ0B3t5yhnW4nNSwSr_C4WV-7Ws4g9Y-CrWWBo2azY,96
-bq_tools_dirupload-0.8.9.dist-info/top_level.txt,sha256=w5z7Un4-v3yqVMurNio-Srl-AUvtPOxZ3tZh4Eb8RHo,3
-bq_tools_dirupload-0.8.9.dist-info/RECORD,,
+bq/tools/uploaddirp.py,sha256=qPXKI0ZVUUXuTnZaoUZjWpsj5v9fTKt-ELct4mwNwa0,22588
+bq_tools_dirupload-0.8.9.1.dist-info/METADATA,sha256=hdtjeURkzVsL7uB41BhhuWuzcJoEokBYpP6K4B3UR6E,8694
+bq_tools_dirupload-0.8.9.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+bq_tools_dirupload-0.8.9.1.dist-info/entry_points.txt,sha256=UzQ0B3t5yhnW4nNSwSr_C4WV-7Ws4g9Y-CrWWBo2azY,96
+bq_tools_dirupload-0.8.9.1.dist-info/top_level.txt,sha256=w5z7Un4-v3yqVMurNio-Srl-AUvtPOxZ3tZh4Eb8RHo,3
+bq_tools_dirupload-0.8.9.1.dist-info/RECORD,,
```

