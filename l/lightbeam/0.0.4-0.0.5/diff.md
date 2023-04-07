# Comparing `tmp/lightbeam-0.0.4-py3-none-any.whl.zip` & `tmp/lightbeam-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 28319 bytes, number of entries: 17
+Zip file size: 28325 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 20:03 lightbeam/__init__.py
--rw-r--r--  2.0 unx     4596 b- defN 22-Sep-21 15:21 lightbeam/__main__.py
--rw-r--r--  2.0 unx    17607 b- defN 23-Jan-25 19:00 lightbeam/api.py
+-rw-r--r--  2.0 unx     4590 b- defN 23-Apr-07 18:45 lightbeam/__main__.py
+-rw-r--r--  2.0 unx    18423 b- defN 23-Apr-07 18:43 lightbeam/api.py
 -rw-r--r--  2.0 unx     8914 b- defN 23-Jan-25 19:00 lightbeam/delete.py
 -rw-r--r--  2.0 unx      672 b- defN 22-Sep-19 14:49 lightbeam/hashlog.py
 -rw-r--r--  2.0 unx    10168 b- defN 22-Sep-22 13:34 lightbeam/lightbeam.py
--rw-r--r--  2.0 unx     6219 b- defN 23-Jan-25 19:00 lightbeam/send.py
+-rw-r--r--  2.0 unx     6329 b- defN 23-Apr-07 18:43 lightbeam/send.py
 -rw-r--r--  2.0 unx     1329 b- defN 22-Sep-21 16:31 lightbeam/util.py
 -rw-r--r--  2.0 unx     5888 b- defN 22-Sep-20 13:42 lightbeam/validate.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-28 14:58 lightbeam/resources/__init__.py
--rwxrwxrwx  2.0 unx    11349 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    13228 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      132 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       54 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1367 b- defN 23-Jan-25 19:00 lightbeam-0.0.4.dist-info/RECORD
-17 files, 81625 bytes uncompressed, 26081 bytes compressed:  68.0%
+-rwxrwxrwx  2.0 unx    11349 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12761 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      132 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx       54 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1367 b- defN 23-Apr-07 18:54 lightbeam-0.0.5.dist-info/RECORD
+17 files, 82078 bytes uncompressed, 26087 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: lightbeam/validate.py
 Comment: 
 
 Filename: lightbeam/resources/__init__.py
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/LICENSE
+Filename: lightbeam-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/METADATA
+Filename: lightbeam-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/WHEEL
+Filename: lightbeam-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/dependency_links.txt
+Filename: lightbeam-0.0.5.dist-info/dependency_links.txt
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/entry_points.txt
+Filename: lightbeam-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/top_level.txt
+Filename: lightbeam-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: lightbeam-0.0.4.dist-info/RECORD
+Filename: lightbeam-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lightbeam/__main__.py

```diff
@@ -77,15 +77,15 @@
         )
     defaults = { "selector":"*", "params": "", "older_than": "", "newer_than": "", "resend_status_codes": "" }
     parser.set_defaults(**defaults)
     args, remaining_argv = parser.parse_known_args()
     
     if args.version:
         lb_dir = os.path.dirname(os.path.abspath(__file__))
-        version_file = os.path.join(lb_dir, '..', 'VERSION.txt')
+        version_file = os.path.join(lb_dir, 'VERSION.txt')
         with open(version_file, 'r') as f:
             VERSION = f.read().strip()
             print(f"lightbeam, version {VERSION}")
         exit(0)
 
     if args.command not in ['validate', 'send', 'validate+send', 'delete']:
         logger.error("Please specify a command to run: `validate`, `send`, `validate+send`, or `delete`. (Try the -h flag for help.)")
```

## lightbeam/api.py

```diff
@@ -143,30 +143,36 @@
         return url
     
     # Sorts endpoints by Ed-Fi dependency-order
     def get_sorted_endpoints(self):
         self.logger.debug("fetching resource dependencies...")
         try:
             response = requests.get(self.config["dependencies_url"],
-                                    verify=self.lightbeam.config["connection"]["verify_ssl"]).json()
+                                    verify=self.lightbeam.config["connection"]["verify_ssl"])
+            if response.status_code not in [ 200, 201 ]:
+                raise Exception("Dependencies URL returned status {0} ({1})".format(response.status_code, (response.body[:75] + "...") if len(response.body)>75 else response.body))
+            data = response.json()
         except Exception as e:
             self.logger.critical("Unable to load dependencies from API... terminating. Check API connectivity. ({0})".format(str(e)))
         
         ordered_endpoints = []
-        for e in response:
+        for e in data:
             ordered_endpoints.append(e["resource"].replace('/' + self.lightbeam.config["namespace"] + '/', ""))
         return ordered_endpoints
     
     # Loads the Swagger JSON from the Ed-Fi API
     def load_swagger_docs(self):
         # grab Descriptors and Resources swagger URLs
         try:
             self.logger.debug("fetching swagger docs...")
             response = requests.get(self.config["open_api_metadata_url"],
                                     verify=self.lightbeam.config["connection"]["verify_ssl"]).json()
+            if response.status_code not in [ 200, 201 ]:
+                raise Exception("OpenAPI metadata URL returned status {0} ({1})".format(response.status_code, (response.body[:75] + "...") if len(response.body)>75 else response.body))
+
         except Exception as e:
             self.logger.critical("Unable to load Swagger docs from API... terminating. Check API connectivity.")
 
         # load (or re-use cached) Descriptors and Resources swagger
         self.descriptors_swagger = None
         self.resources_swagger = None
         
@@ -191,17 +197,21 @@
                 ):
                     self.logger.debug(f"re-using cached {endpoint_type} swagger doc (from {file})...")
                     with open(file) as f:
                         swagger = json.load(f)
                 else:
                     self.logger.debug(f"fetching {endpoint_type} swagger doc...")
                     try:
-                        swagger = requests.get(swagger_url,
+                        response = requests.get(swagger_url,
                                                     verify=self.lightbeam.config["connection"]["verify_ssl"]
-                                                    ).json()
+                                                    )
+                        if response.status_code not in [ 200, 201 ]:
+                            raise Exception("OpenAPI metadata URL returned status {0} ({1})".format(response.status_code, (response.body[:75] + "...") if len(response.body)>75 else response.body))
+                        swagger = response.json()
+
                     except Exception as e:
                         self.logger.critical(f"Unable to load {endpoint_type} Swagger from API... terminating. Check API connectivity.")
 
                     if self.lightbeam.track_state:
                         self.logger.debug(f"(saving to {file})")
                         with open(file, 'w') as f:
                             json.dump(swagger, f)
```

## lightbeam/send.py

```diff
@@ -107,19 +107,22 @@
                         self.lightbeam.num_finished += 1
                         
                         # warn about errors
                         if response.status not in [ 200, 201 ]:
                             message = str(response.status) + ": " + util.linearize(body)
                             self.lightbeam.increment_status_reason(message)
                             self.lightbeam.num_errors += 1
+                            if response.status==400:
+                                raise Exception(message)
+
                         
                         # update hashlog
                         if self.lightbeam.track_state:
                             self.hashlog_data[hash] = (round(time.time()), response.status)
 
                     else:
                         self.lightbeam.api.update_oauth()
         
         except Exception as e:
             self.lightbeam.num_errors += 1
-            self.logger.error("{0}  (at line {1} of {2} )".format(str(e), line, file_name))
+            self.logger.warn("{0}  (at line {1} of {2} )".format(str(e), line, file_name))
```

## Comparing `lightbeam-0.0.4.dist-info/LICENSE` & `lightbeam-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lightbeam-0.0.4.dist-info/METADATA` & `lightbeam-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightbeam
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sends JSONL data into an Ed-Fi API
 Home-page: https://github.com/edanalytics/lightbeam
 Download-URL: https://github.com/edanalytics/lightbeam/archive/0.0.1.tar.gz
 Author: Tom Reitz
 Author-email: treitz@edanalytics.org
 License: Apache 2.0
 Keywords: data,transmission,api,edfi
@@ -68,15 +68,15 @@
 # Setup
 Running the tool requires
 1. a folder of JSONL files, one for each Ed-Fi Resource and Descriptor to populate
 1. a YAML configuration file
 An example YAML configuration is below, followed by documentation of each option.
 
 ```yaml
-state_dir: ~/.lighbeam/
+state_dir: ~/.lightbeam/
 data_dir: ./
 namespace: ed-fi
 edfi_api:
   base_url: https://api.schooldistrict.org/v5.3/api
   version: 3
   mode: year_specific
   year: 2021
@@ -252,42 +252,16 @@
 # Performance & Limitations
 Tool performance depends on primarily on the performance of the Ed-Fi API, which in turn depends on the compute resources which back it. Typically the bottleneck is write performance to the database backend (SQL server or Postgres). If you use `lightbeam` to ingest a large amount of data into an Ed-Fi API (not the recommended use-case, by the way), consider temporarily scaling up your database backend.
 
 For reference, we have achieved throughput rates in excess of 100 requests/second against an Ed-Fi ODS & API running in Docker on a laptop.
 
 
 # Changelog
+See [CHANGELOG](CHANGELOG.md).
 
-### v0.0.4
-<details>
-<summary>Released 2023-01-25</summary>
-
-* bugfix: fetching descriptor values for all namespaces, not just `ed-fi`
-</details>
-
-### v0.0.3
-<details>
-<summary>Released 2023-01-12</summary>
-
-* bugfix: add pagination when fetching descriptor values
-</details>
-
-### v0.0.2
-<details>
-<summary>Released 2022-12-16</summary>
-
-* un-pin requirements.txt dependencies from fixed versions
-</details>
-
-### v0.0.1
-<details>
-<summary>Released 2022-09-22</summary>
-
-* initial release
-</details>
 
 
 # Contributing
 Bugfixes and new features (such as additional transformation operations) are gratefully accepted via pull requests here on GitHub.
 
 ## Contributions
 * Cover image created with [DALL &bull; E mini](https://huggingface.co/spaces/dalle-mini/dalle-mini)
```

## Comparing `lightbeam-0.0.4.dist-info/RECORD` & `lightbeam-0.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 lightbeam/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lightbeam/__main__.py,sha256=7n7yB2a7xdF4QJDuUhPf_1KmrF1zQ9alQauVHIjkdSw,4596
-lightbeam/api.py,sha256=scY7yk-uVNPBzlnDdkGsqjyk1bcHgvBV71xjimS-7sE,17607
+lightbeam/__main__.py,sha256=lZbT__6sBLy_Rxs-WPsGegmeqRjx9oKuAIDHS6kcHcg,4590
+lightbeam/api.py,sha256=7yZiCSWV7fyFRvgikdYyAQRC3n2sP7imzeMoaFY76fI,18423
 lightbeam/delete.py,sha256=_2AfXRswfFsV3dhd0ZYHFnEPJMxCmWaUwSK8a_vF8os,8914
 lightbeam/hashlog.py,sha256=K6A0xXhkoWgOpjg6WlF5_bp-YvinH27lOhPb815shrs,672
 lightbeam/lightbeam.py,sha256=9w-LfAKEE-8Yef8h2T5nMaWR4Q8St9RsD-VVighCNAY,10168
-lightbeam/send.py,sha256=SGWB9pLpla8zjwG8ocFqXiV5QQ5qXpyIVc3QvKecR3Y,6219
+lightbeam/send.py,sha256=2Q4ZkOrK-pAzpeyfvIgy46rX3KyFtYKumYZhXIWGNIA,6329
 lightbeam/util.py,sha256=Nem1rzVdcPya1g6rY_fxGm3QRQnrqHR4PAHy9KOdE9I,1329
 lightbeam/validate.py,sha256=96fcQAMT8jAcp_pz3uDTAoc9YHbQJbSE_GYc88siFO4,5888
 lightbeam/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lightbeam-0.0.4.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
-lightbeam-0.0.4.dist-info/METADATA,sha256=-8nTu6svUrYrS_ROA6qZC7VkwH5wrxRxogKnvBAFCKI,13228
-lightbeam-0.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-lightbeam-0.0.4.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
-lightbeam-0.0.4.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
-lightbeam-0.0.4.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
-lightbeam-0.0.4.dist-info/RECORD,,
+lightbeam-0.0.5.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
+lightbeam-0.0.5.dist-info/METADATA,sha256=E2SLuh1Hbzg70hswM6LMny4UFIt3UW-wM168-PXbgXo,12761
+lightbeam-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+lightbeam-0.0.5.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
+lightbeam-0.0.5.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
+lightbeam-0.0.5.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
+lightbeam-0.0.5.dist-info/RECORD,,
```

