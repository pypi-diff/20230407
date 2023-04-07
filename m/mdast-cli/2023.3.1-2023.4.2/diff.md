# Comparing `tmp/mdast_cli-2023.3.1.tar.gz` & `tmp/mdast_cli-2023.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdast_cli-2023.3.1.tar", last modified: Fri Mar 17 12:47:58 2023, max compression
+gzip compressed data, was "mdast_cli-2023.4.2.tar", last modified: Fri Apr  7 19:29:33 2023, max compression
```

## Comparing `mdast_cli-2023.3.1.tar` & `mdast_cli-2023.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.141823 mdast_cli-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)    29676 2023-03-17 12:47:58.141823 mdast_cli-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    29312 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.129823 mdast_cli-2023.3.1/mdast_cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.133823 mdast_cli-2023.3.1/mdast_cli/distribution_systems/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/app_center.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appgallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.133823 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.137823 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
--rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
--rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
--rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5646 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/store.py
--rw-r--r--   0 runner    (1001) docker     (122)     3413 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/firebase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5094 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/google_play.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.137823 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/config.py
--rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/device.properties
--rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/googleplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/nexus2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/distribution_systems/rustore.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.141823 mdast_cli-2023.3.1/mdast_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/helpers/const.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    39533 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli/mdast_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.129823 mdast_cli-2023.3.1/mdast_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29676 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-17 12:47:58.000000 mdast_cli-2023.3.1/mdast_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:58.141823 mdast_cli-2023.3.1/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    23452 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/mdast_cli_core/token.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-17 12:47:58.141823 mdast_cli-2023.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-03-17 12:47:30.000000 mdast_cli-2023.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    28048 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.656478 mdast_cli-2023.4.2/mdast_cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3714 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/app_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appgallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7464 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    99797 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27325 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)   217008 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5001 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)   150706 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5628 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/firebase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5093 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/google_play.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.660478 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9033 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)   305712 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/device.properties
+-rw-r--r--   0 runner    (1001) docker     (122)    15468 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65347 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3380 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/distribution_systems/rustore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/mdast_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36537 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli/mdast_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.656478 mdast_cli-2023.4.2/mdast_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28412 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-07 19:29:33.000000 mdast_cli-2023.4.2/mdast_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24046 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/mdast_cli_core/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 19:29:33.664478 mdast_cli-2023.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-04-07 19:29:07.000000 mdast_cli-2023.4.2/setup.py
```

### Comparing `mdast_cli-2023.3.1/PKG-INFO` & `mdast_cli-2023.4.2/mdast_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mdast_cli
-Version: 2023.3.1
+Name: mdast-cli
+Version: 2023.4.2
 Summary: Dynamic-Mobile-Security
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
@@ -106,16 +106,18 @@
 
 Required parameters:
  * `url` - network address for system (the path to the root without the final /)
  * `token` - CI/CD access token (refer to our documentation for ways to retrieve the token)
  * `company_id` - identifier of the company within which the scan will be performed
 
 Optional parameters:
- * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - project and profile will be created automatically
+ * `project_id` - optional parameter, ID of the project for scan, Use only if you want to autocreate profile in existing project
+ * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - profile will be created automatically
  * `testcase_id` - ID of the test case to be executed. This is an optional parameter, if not set - manual scan with 20 seconds delay until finish will be executed;
+ * `appium_script_path` - path to appium script to be executed for autoscan via appium.
  * `architecture_id` - optional parameter, identifier of the operating system architecture on which the scan will be performed. If not set - architecture will be selected automatically (Android 11/iOS 14)
  * `nowait` - an optional parameter specifying whether to wait for the scan to complete. If this flag is set, the script will not wait for the scan to complete but will exit immediately after starting. If the flag is not selected, the script will wait for the completion of the analysis process and generate a report.
  * `summary_report_json_file_name` - an optional parameter defining the name of the json file into which the scanning information in json format is uploaded. If the parameter is absent, the information will not be saved.
  * `pdf_report_file_name` - an optional parameter that specifies the name of the pdf file into which information on scanning in pdf format is uploaded. If the parameter is absent, the report will not be saved.
  * `download_path` - an optional parameter that specifies the path to folder with downloaded apps. Default value: *downloaded_apps*
  * `long_wait` - increase wait time for scan to 1 week, boolean parameter
 
@@ -280,69 +282,41 @@
 "Logging in to the App Store. To open app, log in with the Apple ID with which you made the purchase."
 
 Then contact the support team to agree on an Apple ID, which will be used for AppStore integration, you will be offered a solution to this problem.
 
 While creating AppStore integration [ipatool](https://github.com/majd/ipatool) helped a lot, huge thanks for everyone who contributed to this nice open-source tool.
 
 ### Firebase
-To download the application from firebase platform you need to know some cookies for Google SSO authentication and project_id, app_id, app_code, api_key and file_extension parameters from firebase project.  
-You need to select the `--distribution_system firebase` and specify mandatory parameters.  
+To download the application latest release from firebase platform you need to know project_number, app_id, app_code, api_key and file_extension parameters from firebase project.  
+You need to select the `--distribution_system firebase` and specify following mandatory parameters.  
 
-First, you should log in via Google SSO to [Firebase](https://console.firebase.google.com/u/0/) and get necessary cookies from your Chrome session local storage(F12 -> Application -> Cookies)  
-And copy SID, SSID, APISID, SAPISID, HSID to your launch command. The lifetime of them are 2 years, so you don't have to do it often :)  
-
-Screenshot of cookie storage:
-![cookie_storage](https://user-images.githubusercontent.com/46852358/149788352-d453dd78-547f-4989-8132-b94a6f020a81.png)
-
-#### Parameters
-
- * `firebase_SID_cookie` - SID
- * `firebase_HSID_cookie` - HSID
- * `firebase_SSID_cookie` - SSID
- * `firebase_APISID_cookie` - APISID
- * `firebase_SAPISID_cookie` - SAPISID
-
-Now you need project_id, app_id, app_code, api_key to complete parameters for the scan. To get them go to:
-
-App Project home page, url looks like this `https://console.firebase.google.com/u/0/project/{project_name}/overview` ->
-![app_project](https://user-images.githubusercontent.com/46852358/149789837-2787cb52-355d-4ef0-9440-89053764db78.png)
-
-to `Release & Monitor -> App Distribution` ->
-![distr_page](https://user-images.githubusercontent.com/46852358/149791304-2658f1be-9ee0-422e-94ce-59f1ba1858df.png)  
-
-Open network console(F12 -> Network -> Clear) and click `Download`
-
-You will get this request in DevTools:
-![download_req](https://user-images.githubusercontent.com/46852358/149792212-512d33ab-2323-45b6-a25c-6a8d817cde1f.png)  
-
-And url will be like:  
-
-`https://firebaseappdistribution-pa.clients6.google.com/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
-So, you just extract missing parameters from this request and your launch command for CI/CD mobile applications' security analysis is ready!
-Request url will match this pattern, you should extract 4 parameters from url.
-`/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
- * `firebase_project_id` - project id of your Firebase project
+ * `firebase_project_number` - project number of your Firebase project
  * `firebase_app_id` - application id
- * `firebase_app_code` - application code
- * `firebase_api_key` - your api key
+ * `firebase_account_json_path` - path to json key file that contains the credentials for the service account.
  * `firebase_app_extension` - your app extension, it can be `apk` for android and `ipa` for iOS
 
 You can specify the downloaded app file name with an optional parameter
 
  * `firebase_file_name` - file name for app to be saved with
 
+To find `project_number` from Firebase homepage(https://console.firebase.google.com/project/PROJECT_NAME/overview) go to `Project overview -> settings image ->Project settings` In general tab there will be project number in integer format.
+
+To find `app_id` scroll down to 'Your apps'. There will be your app id.
+
+You'll need to obtain an json file that can be used to authenticate request. To do so, you'll need to use a Service Account. A Service Account is a special type of account that is used by applications and services to access Google APIs. To create a Service Account, go to the `GCP Console` and navigate to the `IAM & admin > Service accounts` page. You should enable `scope /auth/cloud-platform` to this account. From there, you can create a new Service Account and download a JSON key file that contains the credentials for the account.
+
+Once you have a Service Account, you can use it to download apps from Firebase via mdast_cli. 
+
 #### Launch example
 
 To start the manual scan analysis of the application, that was downloaded from Firebase, you need to run the following command:
 ```
-python mdast_cli/mdast_scan.py --profile_id 468 --architecture_id 2 --distribution_system firebase --firebase_project_id 2834204**** --firebase_app_id 1:283***3642:android:8b0a0***56ac40c1a43 --firebase_app_code 2b***sltr0 --firebase_api_key AIzaSyDov*****qKdbj-geRWyzMTrg --firebase_SID_cookie FgiA*****ZiQakQ-_C-5ZaEHvbDMFGkrgriAByQ9P9fv7LfRrYJ5suXgrCwIQBoOjA. --firebase_HSID_cookie AsiL****OjPI --firebase_SSID_cookie A****dwcZk1Z-1pE --firebase_APISID_cookie Z-FmS1aPB****djK/AjmG0h2Hc-GG9g2Ac --firebase_SAPISID_cookie XYR2tnf****0zOt/AEvVZ8JVEuCnE6pxm --url "https://saas.mobile.appsec.world" --company_id 1 --token 2fac9652a2fbe4****9f44af59c3381772f --firebase_file_name your_app_file_name  --firebase_file_extension apk
+python mdast_cli/mdast_scan.py -d --distribution_system firebase --firebase_project_number 1231231337 --firebase_app_id 1:1337:android:123123 --firebase_account_json_path service_acc0unt_file.json --firebase_file_extension apk --firebase_file_name b3st_app
 ```
-As a result in the `downloaded_apps` repository will be application with name `your_app_file_name.apk` and manual scan will be started.
+As a result in the `downloaded_apps` repository will be application with name `b3st_app.apk`.
 
 ### AppCenter
 
 #### Parameters
 
 To download the application from AppCenter distribution system you need to select the `distribution_system appcenter` parameter. Also, you need to specify the following mandatory parameters:
  * `appcenter_token` - API access token. Look in official documentation to [learn how to retrieve it]((https://docs.microsoft.com/en-us/appcenter/api-docs/)).
```

### Comparing `mdast_cli-2023.3.1/README.md` & `mdast_cli-2023.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: mdast_cli
+Version: 2023.4.2
+Summary: Dynamic-Mobile-Security
+Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
+Author: Dynamic-Mobile-Security
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
+
 <h1>Mobile DAST CI/CD</h1>
 
 **Python script for automating security analysis of mobile applications.**
 
 [![Docker Hub](https://img.shields.io/docker/v/mobilesecurity/mdast_cli?label=docker%20hub)](https://hub.docker.com/repository/docker/mobilesecurity/mdast_cli)
 [![PyPi](https://img.shields.io/pypi/v/mdast_cli?color=3)](https://pypi.org/project/mdast-cli/)
 ![GitHub issues](https://img.shields.io/github/issues-raw/Dynamic-Mobile-Security/mdast-cli)
@@ -95,16 +106,18 @@
 
 Required parameters:
  * `url` - network address for system (the path to the root without the final /)
  * `token` - CI/CD access token (refer to our documentation for ways to retrieve the token)
  * `company_id` - identifier of the company within which the scan will be performed
 
 Optional parameters:
- * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - project and profile will be created automatically
+ * `project_id` - optional parameter, ID of the project for scan, Use only if you want to autocreate profile in existing project
+ * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - profile will be created automatically
  * `testcase_id` - ID of the test case to be executed. This is an optional parameter, if not set - manual scan with 20 seconds delay until finish will be executed;
+ * `appium_script_path` - path to appium script to be executed for autoscan via appium.
  * `architecture_id` - optional parameter, identifier of the operating system architecture on which the scan will be performed. If not set - architecture will be selected automatically (Android 11/iOS 14)
  * `nowait` - an optional parameter specifying whether to wait for the scan to complete. If this flag is set, the script will not wait for the scan to complete but will exit immediately after starting. If the flag is not selected, the script will wait for the completion of the analysis process and generate a report.
  * `summary_report_json_file_name` - an optional parameter defining the name of the json file into which the scanning information in json format is uploaded. If the parameter is absent, the information will not be saved.
  * `pdf_report_file_name` - an optional parameter that specifies the name of the pdf file into which information on scanning in pdf format is uploaded. If the parameter is absent, the report will not be saved.
  * `download_path` - an optional parameter that specifies the path to folder with downloaded apps. Default value: *downloaded_apps*
  * `long_wait` - increase wait time for scan to 1 week, boolean parameter
 
@@ -269,69 +282,41 @@
 "Logging in to the App Store. To open app, log in with the Apple ID with which you made the purchase."
 
 Then contact the support team to agree on an Apple ID, which will be used for AppStore integration, you will be offered a solution to this problem.
 
 While creating AppStore integration [ipatool](https://github.com/majd/ipatool) helped a lot, huge thanks for everyone who contributed to this nice open-source tool.
 
 ### Firebase
-To download the application from firebase platform you need to know some cookies for Google SSO authentication and project_id, app_id, app_code, api_key and file_extension parameters from firebase project.  
-You need to select the `--distribution_system firebase` and specify mandatory parameters.  
-
-First, you should log in via Google SSO to [Firebase](https://console.firebase.google.com/u/0/) and get necessary cookies from your Chrome session local storage(F12 -> Application -> Cookies)  
-And copy SID, SSID, APISID, SAPISID, HSID to your launch command. The lifetime of them are 2 years, so you don't have to do it often :)  
-
-Screenshot of cookie storage:
-![cookie_storage](https://user-images.githubusercontent.com/46852358/149788352-d453dd78-547f-4989-8132-b94a6f020a81.png)
-
-#### Parameters
-
- * `firebase_SID_cookie` - SID
- * `firebase_HSID_cookie` - HSID
- * `firebase_SSID_cookie` - SSID
- * `firebase_APISID_cookie` - APISID
- * `firebase_SAPISID_cookie` - SAPISID
-
-Now you need project_id, app_id, app_code, api_key to complete parameters for the scan. To get them go to:
-
-App Project home page, url looks like this `https://console.firebase.google.com/u/0/project/{project_name}/overview` ->
-![app_project](https://user-images.githubusercontent.com/46852358/149789837-2787cb52-355d-4ef0-9440-89053764db78.png)
-
-to `Release & Monitor -> App Distribution` ->
-![distr_page](https://user-images.githubusercontent.com/46852358/149791304-2658f1be-9ee0-422e-94ce-59f1ba1858df.png)  
+To download the application latest release from firebase platform you need to know project_number, app_id, app_code, api_key and file_extension parameters from firebase project.  
+You need to select the `--distribution_system firebase` and specify following mandatory parameters.  
 
-Open network console(F12 -> Network -> Clear) and click `Download`
-
-You will get this request in DevTools:
-![download_req](https://user-images.githubusercontent.com/46852358/149792212-512d33ab-2323-45b6-a25c-6a8d817cde1f.png)  
-
-And url will be like:  
-
-`https://firebaseappdistribution-pa.clients6.google.com/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
-So, you just extract missing parameters from this request and your launch command for CI/CD mobile applications' security analysis is ready!
-Request url will match this pattern, you should extract 4 parameters from url.
-`/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
- * `firebase_project_id` - project id of your Firebase project
+ * `firebase_project_number` - project number of your Firebase project
  * `firebase_app_id` - application id
- * `firebase_app_code` - application code
- * `firebase_api_key` - your api key
+ * `firebase_account_json_path` - path to json key file that contains the credentials for the service account.
  * `firebase_app_extension` - your app extension, it can be `apk` for android and `ipa` for iOS
 
 You can specify the downloaded app file name with an optional parameter
 
  * `firebase_file_name` - file name for app to be saved with
 
+To find `project_number` from Firebase homepage(https://console.firebase.google.com/project/PROJECT_NAME/overview) go to `Project overview -> settings image ->Project settings` In general tab there will be project number in integer format.
+
+To find `app_id` scroll down to 'Your apps'. There will be your app id.
+
+You'll need to obtain an json file that can be used to authenticate request. To do so, you'll need to use a Service Account. A Service Account is a special type of account that is used by applications and services to access Google APIs. To create a Service Account, go to the `GCP Console` and navigate to the `IAM & admin > Service accounts` page. You should enable `scope /auth/cloud-platform` to this account. From there, you can create a new Service Account and download a JSON key file that contains the credentials for the account.
+
+Once you have a Service Account, you can use it to download apps from Firebase via mdast_cli. 
+
 #### Launch example
 
 To start the manual scan analysis of the application, that was downloaded from Firebase, you need to run the following command:
 ```
-python mdast_cli/mdast_scan.py --profile_id 468 --architecture_id 2 --distribution_system firebase --firebase_project_id 2834204**** --firebase_app_id 1:283***3642:android:8b0a0***56ac40c1a43 --firebase_app_code 2b***sltr0 --firebase_api_key AIzaSyDov*****qKdbj-geRWyzMTrg --firebase_SID_cookie FgiA*****ZiQakQ-_C-5ZaEHvbDMFGkrgriAByQ9P9fv7LfRrYJ5suXgrCwIQBoOjA. --firebase_HSID_cookie AsiL****OjPI --firebase_SSID_cookie A****dwcZk1Z-1pE --firebase_APISID_cookie Z-FmS1aPB****djK/AjmG0h2Hc-GG9g2Ac --firebase_SAPISID_cookie XYR2tnf****0zOt/AEvVZ8JVEuCnE6pxm --url "https://saas.mobile.appsec.world" --company_id 1 --token 2fac9652a2fbe4****9f44af59c3381772f --firebase_file_name your_app_file_name  --firebase_file_extension apk
+python mdast_cli/mdast_scan.py -d --distribution_system firebase --firebase_project_number 1231231337 --firebase_app_id 1:1337:android:123123 --firebase_account_json_path service_acc0unt_file.json --firebase_file_extension apk --firebase_file_name b3st_app
 ```
-As a result in the `downloaded_apps` repository will be application with name `your_app_file_name.apk` and manual scan will be started.
+As a result in the `downloaded_apps` repository will be application with name `b3st_app.apk`.
 
 ### AppCenter
 
 #### Parameters
 
 To download the application from AppCenter distribution system you need to select the `distribution_system appcenter` parameter. Also, you need to specify the following mandatory parameters:
  * `appcenter_token` - API access token. Look in official documentation to [learn how to retrieve it]((https://docs.microsoft.com/en-us/appcenter/api-docs/)).
```

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/app_center.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/app_center.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appgallery.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appgallery.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_authenticate_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_buyproduct_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_req.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/schemas/store_download_resp.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/appstore_client/store.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/appstore_client/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         while True:
             r = self.sess.post(url,
                                headers={
                                    "Accept": "*/*",
                                    "Content-Type": "application/x-www-form-urlencoded",
                                    "User-Agent":
                                        "Configurator/2.0 (Macintosh; OS X 10.12.6; 16G29) AppleWebKit/2603.3.8",
-                                        },
+                               },
                                data=plistlib.dumps(req.as_dict()), allow_redirects=False,
                                verify=False)
             if r.status_code == 302:
                 url = r.headers['Location']
                 continue
             break
         resp = StoreAuthenticateResp.from_dict(plistlib.loads(r.content))
@@ -53,27 +53,27 @@
         self.sess.headers['X-Dsid'] = self.sess.headers['iCloud-Dsid'] = str(resp.download_queue_info.dsid)
         self.sess.headers['X-Apple-Store-Front'] = r.headers.get('x-set-apple-store-front')
         self.sess.headers['X-Token'] = resp.passwordToken
 
         self.account_name = resp.accountInfo.address.firstName + " " + resp.accountInfo.address.lastName
         return resp
 
-    def find_app(self, app_id=None,  bundle_id=None, country="US"):
+    def find_app(self, app_id=None, bundle_id=None, country="US"):
         return self.sess.get("https://itunes.apple.com/lookup?",
                              params={
                                  "bundleId": bundle_id,
                                  "id": app_id,
                                  "term": None,
                                  "country": country,
                                  "limit": 1,
                                  "media": "software",
                              },
                              headers={
                                  "Content-Type": "application/x-www-form-urlencoded",
-                                     },
+                             },
                              verify=False)
 
     def purchase(self, app_id, productType='C'):
         url = "https://buy.itunes.apple.com/WebObjects/MZBuy.woa/wa/buyProduct"
         req = StoreBuyproductReq(
             guid=self.guid,
             salableAdamId=str(app_id),
```

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/google_play.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/google_play.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def get_app_info(self, package_name):
         self.login()
         app_data = self.gp_api.details(package_name)
         return {
             'integration_type': 'google_play',
             'package_name': app_data['details']['appDetails']['packageName'],
-            'version_name':  app_data['details']['appDetails']['versionString'],
+            'version_name': app_data['details']['appDetails']['versionString'],
             'version_code': app_data['details']['appDetails']['versionCode'],
             'file_size': app_data['details']['appDetails']['installationSize'],
             'icon_url': app_data['image'][0]['imageUrl']
         }
 
     def download_app(self, download_path, package_name, file_name=None):
         file_name = file_name or package_name
```

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/config.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/config.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/device.properties` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/device.properties`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/googleplay.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/gpapi/googleplay_pb2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/nexus.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         download_url = ''
         file_name = ''
         component_search_result = self.search_component(repo_name, group_id, artifact_id, version)
         for asset in component_search_result.get('assets', {}):
             if asset.get('contentType', '') in ('application/vnd.android.package-archive', 'application/x-itunes-ipa'):
                 download_url = asset.get('downloadUrl')
                 file_name = download_url.split('/')[-1] if download_url.split('/')[
-                                                                   -1] != '' else f'{group_id}-{version}.apk'
+                                                               -1] != '' else f'{group_id}-{version}.apk'
                 break
         if not download_url:
             logger.error(f'NexusRepo: Unable to find download URL: {len(component_search_result)}')
         response = self.session.get(download_url, allow_redirects=True)
         if response.status_code != 200:
             raise RuntimeError(f'NexusRepo: Failed to download application. '
                                f'Request return status code: {response.status_code}')
```

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/nexus2.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/nexus2.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/distribution_systems/rustore.py` & `mdast_cli-2023.4.2/mdast_cli/distribution_systems/rustore.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/helpers/const.py` & `mdast_cli-2023.4.2/mdast_cli/helpers/const.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli/mdast_scan.py` & `mdast_cli-2023.4.2/mdast_cli/mdast_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 
 import urllib3
 
 from mdast_cli.distribution_systems.app_center import AppCenter
 from mdast_cli.distribution_systems.appgallery import appgallery_download_app
 from mdast_cli.distribution_systems.appstore import AppStore
-from mdast_cli.distribution_systems.firebase import Firebase
+from mdast_cli.distribution_systems.firebase import firebase_download_app
 from mdast_cli.distribution_systems.google_play import GooglePlay
 from mdast_cli.distribution_systems.nexus import NexusRepository
 from mdast_cli.distribution_systems.nexus2 import Nexus2Repository
 from mdast_cli.distribution_systems.rustore import rustore_download_app
 from mdast_cli.helpers.const import (ANDROID_EXTENSIONS, END_SCAN_TIMEOUT, LONG_TRY, SLEEP_TIMEOUT, TRY, DastState,
                                      DastStateDict)
 from mdast_cli.helpers.helpers import check_app_md5
@@ -78,41 +78,23 @@
                         help='Artifact id for mobile application. '
                              'This argument is required if distribution system set to "appcenter"')
     parser.add_argument('--nexus_version', type=str,
                         help='Version to download from Nexus. '
                              'This argument is required if distribution system set to "appcenter"')
 
     # Arguments for Firebase
-    parser.add_argument('--firebase_project_id', type=str,
-                        help='Project id for firebase where mobile application is located.'
+    parser.add_argument('--firebase_project_number', type=int,
+                        help='Project number for firebase where mobile application is located.'
                              ' This argument is required if distribution system set to "firebase"')
     parser.add_argument('--firebase_app_id', type=str,
                         help='Application id for firebase where mobile application is located.'
                              ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_app_code', type=str,
-                        help='Application code for firebase where mobile application is located.'
+    parser.add_argument('--firebase_account_json_path', type=str,
+                        help='json.'
                              ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_api_key', type=str,
-                        help='Api code for firebase where mobile application is located.'
-                             ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_SID_cookie', type=str,
-                        help='SID cookie for firebase authentication  via google sso.'
-                             ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_HSID_cookie', type=str,
-                        help='HSID cookie for firebase authentication  via google sso.'
-                             ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_SSID_cookie', type=str,
-                        help='SSID cookie for firebase authentication  via google sso.'
-                             ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_APISID_cookie', type=str,
-                        help='APISID cookie for firebase authentication  via google sso.'
-                             ' This argument is required if distribution system set to "firebase"')
-    parser.add_argument('--firebase_SAPISID_cookie', type=str,
-                        help='SAPISID cookie for firebase authentication  via google sso.'
-                             ' This argument required if distribution system set to "firebase"')
     parser.add_argument('--firebase_file_extension', type=str,
                         help='File extension(apk or ipa) for downloaded application.'
                              ' This argument is required if distribution system set to "firebase"',
                         choices=['ipa', 'apk'])
     parser.add_argument('--firebase_file_name', type=str,
                         help='File name for downloaded application.'
                              ' This argument is optional if distribution system set to "firebase"')
@@ -210,17 +192,20 @@
                              'This argument is optional if distribution system set to "appcenter"')
 
     # Main arguments
     parser.add_argument('--url', type=str, help='System url', required=(not '-d'))
     parser.add_argument('--company_id', type=int, help='Company id for starting scan', required=(not '-d'))
     parser.add_argument('--token', type=str, help='CI/CD Token for start scan and get results', required=(not '-d'))
     parser.add_argument('--architecture_id', type=int, help='Architecture id to perform scan')
-    parser.add_argument('--profile_id', type=int,
-                        help='Profile id for scan. If not set - autocreate project and profile')
+    parser.add_argument('--profile_id', type=int, default=None,
+                        help='Profile id for scan. If not set - autocreate profile')
+    parser.add_argument('--project_id', type=int, default=None,
+                        help='Project id for scan. Only if you want to autocreate profile in existing project')
     parser.add_argument('--testcase_id', type=int, help='Testcase id. If not set - manual scan')
+    parser.add_argument('--appium_script_path', type=str, help='Appium script path for autoscan with Stingray appium')
     parser.add_argument('--summary_report_json_file_name', type=str,
                         help='Name for the json file with summary results in structured format')
     parser.add_argument('--pdf_report_file_name', type=str, help='Name for the pdf report file.')
     parser.add_argument('--nowait', '-nw', action='store_true',
                         help='Wait before scan ends and get results if set to True. If set to False - just start scan '
                              'and exit')
     parser.add_argument('--download_path', '-p', type=str, help='Path to folder with downloaded apps',
@@ -262,28 +247,20 @@
             args.nexus2_version is None or
             args.nexus2_extension is None):
         parser.error('"--distribution_system nexus2" requires "--nexus2_url", "--nexus2_login", "--nexus2_password",'
                      ' "--nexus2_repo_name", "--nexus2_group_id", "--nexus2_artifact_id", "--nexus2_extension" '
                      'arguments to be set')
 
     elif args.distribution_system == 'firebase' and (
-            args.firebase_project_id is None or
+            args.firebase_project_number is None or
             args.firebase_app_id is None or
-            args.firebase_app_code is None or
-            args.firebase_api_key is None or
-            args.firebase_SID_cookie is None or
-            args.firebase_HSID_cookie is None or
-            args.firebase_SSID_cookie is None or
-            args.firebase_APISID_cookie is None or
-            args.firebase_SAPISID_cookie is None or
+            args.firebase_account_json_path is None or
             args.firebase_file_extension is None):
-        parser.error('"--distribution_system nexus" requires "--firebase_project_id", "--firebase_app_id", '
-                     '"--firebase_app_code", "--firebase_api_key", "--firebase_api_key", "--firebase_SID_cookie", '
-                     '"--firebase_HSID_cookie", "--firebase_SSID_cookie", "--firebase_APISID_cookie", '
-                     '"--firebase_SAPISID_cookie", "--firebase_file_extension" arguments to be set')
+        parser.error('"--distribution_system firebase" requires "--firebase_project_number", "--firebase_app_id", '
+                     '"--firebase_account_json_path", "--firebase_file_extension" arguments to be set')
 
     elif args.distribution_system == 'appstore' and (
             (args.appstore_app_id is None and args.appstore_bundle_id is None) or
             args.appstore_apple_id is None or
             (args.appstore_password is None or args.appstore_2FA is None) and args.appstore_password2FA is None):
         parser.error('"--distribution_system appstore" requires either "--appstore_app_id" or "--appstore_bundle_id", '
                      '"--appstore_apple_id" and ("--appstore_password" + "--appstore_2FA")/'
@@ -316,15 +293,17 @@
 
     if arguments.download_only is False:
         url = arguments.url
         company_id = arguments.company_id
         architecture = arguments.architecture_id
         token = arguments.token
         profile_id = arguments.profile_id
+        project_id = arguments.project_id
         testcase_id = arguments.testcase_id
+        appium_script_path = arguments.appium_script_path
         json_summary_file_name = arguments.summary_report_json_file_name
         pdf_report_file_name = arguments.pdf_report_file_name
         not_wait_scan_end = arguments.nowait
         long_wait = arguments.long_wait
 
         url = url if url.endswith('/') else f'{url}/'
         url = url if url.endswith('rest/') else f'{url}rest'
@@ -362,26 +341,20 @@
                                                       arguments.nexus2_group_id,
                                                       arguments.nexus2_artifact_id,
                                                       arguments.nexus2_version,
                                                       arguments.nexus2_extension,
                                                       arguments.nexus2_file_name)
 
         elif distribution_system == 'firebase':
-            firebase = Firebase(arguments.firebase_api_key,
-                                arguments.firebase_SID_cookie,
-                                arguments.firebase_HSID_cookie,
-                                arguments.firebase_SSID_cookie,
-                                arguments.firebase_APISID_cookie,
-                                arguments.firebase_SAPISID_cookie)
-            app_file = firebase.download_app(download_path,
-                                             arguments.firebase_project_id,
+            app_file = firebase_download_app(download_path,
+                                             arguments.firebase_project_number,
                                              arguments.firebase_app_id,
-                                             arguments.firebase_app_code,
-                                             arguments.firebase_file_extension,
-                                             arguments.firebase_file_name)
+                                             arguments.firebase_account_json_path,
+                                             arguments.firebase_file_name,
+                                             arguments.firebase_file_extension)
 
         elif distribution_system == 'appstore':
             if arguments.appstore_password and arguments.appstore_2FA:
                 password2FA = arguments.appstore_password + arguments.appstore_2FA
             else:
                 password2FA = arguments.appstore_password2FA
             appstore = AppStore(arguments.appstore_apple_id,
@@ -448,20 +421,23 @@
         get_testcase_resp = mdast.get_testcase(testcase_id)
         if get_testcase_resp.status_code == 200:
             architecture = get_testcase_resp.json()['architecture']['id']
         else:
             logger.warning("Testcase with this id does not exist or you use old version of system. Trying to use "
                            "architecture from command line params.")
 
-    if testcase_id is None:
-        logger.info(f'Manual scan with profile id: {profile_id} and file located in {app_file},'
+    if testcase_id:
+        logger.info(f'Autoscan(Stingray) with test case id: '
+                    f'{testcase_id}, profile id: {profile_id} and file: {app_file}, architecture id is {architecture}')
+    elif appium_script_path:
+        logger.info(f'Autoscan(Appium) with  profile id: {profile_id} and file: {app_file},'
                     f' architecture id is {architecture}')
     else:
-        logger.info(f'Auto scan with test case id: '
-                    f'{testcase_id}, profile id: {profile_id} and file: {app_file}, architecture id is {architecture}')
+        logger.info(f'Manual scan with profile id: {profile_id} and file located in {app_file},'
+                    f' architecture id is {architecture}')
 
     logger.info('Check if this version of application was already uploaded..')
     if appstore_app_md5:
         check_app_already_uploaded = mdast.check_app_md5(mdast.company_id, appstore_app_md5).json()
     else:
         check_app_already_uploaded = mdast.check_app_md5(mdast.company_id, check_app_md5(app_file)).json()
     if check_app_already_uploaded:
@@ -476,61 +452,41 @@
         if upload_application_resp.status_code != 201:
             logger.error(f'Error while uploading application to server: {upload_application_resp.text}')
             sys.exit(1)
         application = upload_application_resp.json()
         logger.info(f"Application uploaded successfully. Application id: {application['id']}")
 
     logger.info(f"Creating scan for application {application['id']}")
-
-    if 'Android' in architecture_type.get('name', ''):
-        if not testcase_id:
-            if profile_id:
-                create_dast_resp = mdast.create_manual_scan(profile_id=profile_id,
-                                                            app_id=application['id'],
-                                                            arch_id=architecture)
-            else:
-                create_dast_resp = mdast.create_manual_scan_autocreate_profile(app_id=application['id'],
-                                                                               arch_id=architecture)
-                dast_info = create_dast_resp.json()
-                logger.info(f"Project and profile was created/found successfully."
-                            f" Project id: {dast_info['project']['id']}, profile id: {dast_info['profile']['id']}")
-            scan_type = 'manual'
-        else:
-            create_dast_resp = mdast.create_auto_scan(profile_id=profile_id,
-                                                      app_id=application['id'],
-                                                      arch_id=architecture,
-                                                      test_case_id=testcase_id)
-            scan_type = 'auto'
-    elif 'iOS' in architecture_type.get('name', ''):
-        if profile_id:
-            create_dast_resp = mdast.create_manual_scan(profile_id=profile_id,
-                                                        app_id=application['id'],
-                                                        arch_id=architecture)
-        else:
-            create_dast_resp = mdast.create_manual_scan_autocreate_profile(app_id=application['id'],
-                                                                           arch_id=architecture)
-            dast_info = create_dast_resp.json()
-            logger.info(f"Project and profile was created/found successfully."
-                        f" Project id: {dast_info['project']['id']}, profile id: {dast_info['profile']['id']}")
-        scan_type = 'manual'
+    if testcase_id:
+        create_dast_resp = mdast.create_auto_scan(project_id, profile_id, application['id'], architecture, testcase_id)
+        scan_type = 'auto_stingray'
+    elif appium_script_path:
+        create_dast_resp = mdast.create_appium_scan(project_id, profile_id, application['id'], architecture,
+                                                    appium_script_path)
+        scan_type = 'auto_appium'
     else:
-        logger.error("Cannot create scan - unknown architecture")
-        sys.exit(1)
-
+        create_dast_resp = mdast.create_manual_scan(project_id, profile_id, application['id'], architecture)
+        scan_type = 'manual'
     if create_dast_resp.status_code != 201:
         logger.error(f'Error while creating scan: {create_dast_resp.text}')
         sys.exit(1)
 
+    dast_info = create_dast_resp.json()
+    logger.info(f"Project and profile was created/found successfully."
+                f" Project id: {dast_info['project']['id']}, profile id: {dast_info['profile']['id']}")
+
     dast = create_dast_resp.json()
     if 'id' not in dast and dast.get('id', '') != '':
         logger.error(f'Something went wrong while creating scan: {dast}')
         sys.exit(1)
 
-    if scan_type == 'auto':
-        logger.info(f"Autoscan was created successfully. Scan id: {dast['id']}")
+    if scan_type == 'auto_stingray':
+        logger.info(f"Autoscan(Stingray) was created successfully. Scan id: {dast['id']}")
+    elif scan_type == 'auto_appium':
+        logger.info(f"Autoscan(Appium) was created successfully. Scan id: {dast['id']}")
     else:
         logger.info(f"Manual scan was created successfully. Scan id: {dast['id']}")
 
     logger.info(f"Start scan with id {dast['id']}")
     start_dast_resp = mdast.start_scan(dast['id'])
     if start_dast_resp.status_code != 200:
         logger.error(f"Error while starting scan with id {dast['id']}: {start_dast_resp.text}")
```

### Comparing `mdast_cli-2023.3.1/mdast_cli.egg-info/PKG-INFO` & `mdast_cli-2023.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: mdast-cli
-Version: 2023.3.1
-Summary: Dynamic-Mobile-Security
-Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli
-Author: Dynamic-Mobile-Security
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-
 <h1>Mobile DAST CI/CD</h1>
 
 **Python script for automating security analysis of mobile applications.**
 
 [![Docker Hub](https://img.shields.io/docker/v/mobilesecurity/mdast_cli?label=docker%20hub)](https://hub.docker.com/repository/docker/mobilesecurity/mdast_cli)
 [![PyPi](https://img.shields.io/pypi/v/mdast_cli?color=3)](https://pypi.org/project/mdast-cli/)
 ![GitHub issues](https://img.shields.io/github/issues-raw/Dynamic-Mobile-Security/mdast-cli)
@@ -106,16 +95,18 @@
 
 Required parameters:
  * `url` - network address for system (the path to the root without the final /)
  * `token` - CI/CD access token (refer to our documentation for ways to retrieve the token)
  * `company_id` - identifier of the company within which the scan will be performed
 
 Optional parameters:
- * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - project and profile will be created automatically
+ * `project_id` - optional parameter, ID of the project for scan, Use only if you want to autocreate profile in existing project
+ * `profile_id` - optional parameter, ID of the profile to be analyzed, If not set - profile will be created automatically
  * `testcase_id` - ID of the test case to be executed. This is an optional parameter, if not set - manual scan with 20 seconds delay until finish will be executed;
+ * `appium_script_path` - path to appium script to be executed for autoscan via appium.
  * `architecture_id` - optional parameter, identifier of the operating system architecture on which the scan will be performed. If not set - architecture will be selected automatically (Android 11/iOS 14)
  * `nowait` - an optional parameter specifying whether to wait for the scan to complete. If this flag is set, the script will not wait for the scan to complete but will exit immediately after starting. If the flag is not selected, the script will wait for the completion of the analysis process and generate a report.
  * `summary_report_json_file_name` - an optional parameter defining the name of the json file into which the scanning information in json format is uploaded. If the parameter is absent, the information will not be saved.
  * `pdf_report_file_name` - an optional parameter that specifies the name of the pdf file into which information on scanning in pdf format is uploaded. If the parameter is absent, the report will not be saved.
  * `download_path` - an optional parameter that specifies the path to folder with downloaded apps. Default value: *downloaded_apps*
  * `long_wait` - increase wait time for scan to 1 week, boolean parameter
 
@@ -280,69 +271,41 @@
 "Logging in to the App Store. To open app, log in with the Apple ID with which you made the purchase."
 
 Then contact the support team to agree on an Apple ID, which will be used for AppStore integration, you will be offered a solution to this problem.
 
 While creating AppStore integration [ipatool](https://github.com/majd/ipatool) helped a lot, huge thanks for everyone who contributed to this nice open-source tool.
 
 ### Firebase
-To download the application from firebase platform you need to know some cookies for Google SSO authentication and project_id, app_id, app_code, api_key and file_extension parameters from firebase project.  
-You need to select the `--distribution_system firebase` and specify mandatory parameters.  
-
-First, you should log in via Google SSO to [Firebase](https://console.firebase.google.com/u/0/) and get necessary cookies from your Chrome session local storage(F12 -> Application -> Cookies)  
-And copy SID, SSID, APISID, SAPISID, HSID to your launch command. The lifetime of them are 2 years, so you don't have to do it often :)  
-
-Screenshot of cookie storage:
-![cookie_storage](https://user-images.githubusercontent.com/46852358/149788352-d453dd78-547f-4989-8132-b94a6f020a81.png)
-
-#### Parameters
-
- * `firebase_SID_cookie` - SID
- * `firebase_HSID_cookie` - HSID
- * `firebase_SSID_cookie` - SSID
- * `firebase_APISID_cookie` - APISID
- * `firebase_SAPISID_cookie` - SAPISID
-
-Now you need project_id, app_id, app_code, api_key to complete parameters for the scan. To get them go to:
-
-App Project home page, url looks like this `https://console.firebase.google.com/u/0/project/{project_name}/overview` ->
-![app_project](https://user-images.githubusercontent.com/46852358/149789837-2787cb52-355d-4ef0-9440-89053764db78.png)
-
-to `Release & Monitor -> App Distribution` ->
-![distr_page](https://user-images.githubusercontent.com/46852358/149791304-2658f1be-9ee0-422e-94ce-59f1ba1858df.png)  
+To download the application latest release from firebase platform you need to know project_number, app_id, app_code, api_key and file_extension parameters from firebase project.  
+You need to select the `--distribution_system firebase` and specify following mandatory parameters.  
 
-Open network console(F12 -> Network -> Clear) and click `Download`
-
-You will get this request in DevTools:
-![download_req](https://user-images.githubusercontent.com/46852358/149792212-512d33ab-2323-45b6-a25c-6a8d817cde1f.png)  
-
-And url will be like:  
-
-`https://firebaseappdistribution-pa.clients6.google.com/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
-So, you just extract missing parameters from this request and your launch command for CI/CD mobile applications' security analysis is ready!
-Request url will match this pattern, you should extract 4 parameters from url.
-`/v1/projects/{project_id}/apps/{app_id}/releases/{app_code}:getLatestBinary?alt=json&key={api_key}`  
-
- * `firebase_project_id` - project id of your Firebase project
+ * `firebase_project_number` - project number of your Firebase project
  * `firebase_app_id` - application id
- * `firebase_app_code` - application code
- * `firebase_api_key` - your api key
+ * `firebase_account_json_path` - path to json key file that contains the credentials for the service account.
  * `firebase_app_extension` - your app extension, it can be `apk` for android and `ipa` for iOS
 
 You can specify the downloaded app file name with an optional parameter
 
  * `firebase_file_name` - file name for app to be saved with
 
+To find `project_number` from Firebase homepage(https://console.firebase.google.com/project/PROJECT_NAME/overview) go to `Project overview -> settings image ->Project settings` In general tab there will be project number in integer format.
+
+To find `app_id` scroll down to 'Your apps'. There will be your app id.
+
+You'll need to obtain an json file that can be used to authenticate request. To do so, you'll need to use a Service Account. A Service Account is a special type of account that is used by applications and services to access Google APIs. To create a Service Account, go to the `GCP Console` and navigate to the `IAM & admin > Service accounts` page. You should enable `scope /auth/cloud-platform` to this account. From there, you can create a new Service Account and download a JSON key file that contains the credentials for the account.
+
+Once you have a Service Account, you can use it to download apps from Firebase via mdast_cli. 
+
 #### Launch example
 
 To start the manual scan analysis of the application, that was downloaded from Firebase, you need to run the following command:
 ```
-python mdast_cli/mdast_scan.py --profile_id 468 --architecture_id 2 --distribution_system firebase --firebase_project_id 2834204**** --firebase_app_id 1:283***3642:android:8b0a0***56ac40c1a43 --firebase_app_code 2b***sltr0 --firebase_api_key AIzaSyDov*****qKdbj-geRWyzMTrg --firebase_SID_cookie FgiA*****ZiQakQ-_C-5ZaEHvbDMFGkrgriAByQ9P9fv7LfRrYJ5suXgrCwIQBoOjA. --firebase_HSID_cookie AsiL****OjPI --firebase_SSID_cookie A****dwcZk1Z-1pE --firebase_APISID_cookie Z-FmS1aPB****djK/AjmG0h2Hc-GG9g2Ac --firebase_SAPISID_cookie XYR2tnf****0zOt/AEvVZ8JVEuCnE6pxm --url "https://saas.mobile.appsec.world" --company_id 1 --token 2fac9652a2fbe4****9f44af59c3381772f --firebase_file_name your_app_file_name  --firebase_file_extension apk
+python mdast_cli/mdast_scan.py -d --distribution_system firebase --firebase_project_number 1231231337 --firebase_app_id 1:1337:android:123123 --firebase_account_json_path service_acc0unt_file.json --firebase_file_extension apk --firebase_file_name b3st_app
 ```
-As a result in the `downloaded_apps` repository will be application with name `your_app_file_name.apk` and manual scan will be started.
+As a result in the `downloaded_apps` repository will be application with name `b3st_app.apk`.
 
 ### AppCenter
 
 #### Parameters
 
 To download the application from AppCenter distribution system you need to select the `distribution_system appcenter` parameter. Also, you need to specify the following mandatory parameters:
  * `appcenter_token` - API access token. Look in official documentation to [learn how to retrieve it]((https://docs.microsoft.com/en-us/appcenter/api-docs/)).
```

### Comparing `mdast_cli-2023.3.1/mdast_cli.egg-info/SOURCES.txt` & `mdast_cli-2023.4.2/mdast_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli.egg-info/requires.txt` & `mdast_cli-2023.4.2/mdast_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli_core/api.py` & `mdast_cli-2023.4.2/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/mdast_cli_core/base.py` & `mdast_cli-2023.4.2/mdast_cli_core/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,49 +298,66 @@
         }
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/applications/',
                              headers=headers_multipart,
                              files=multipart_form_data,
                              data={'architecture_type': architecture_type},
                              verify=False)
 
-    def create_manual_scan(self, profile_id, app_id, arch_id):
+    def create_manual_scan(self, project_id, profile_id, app_id, arch_id):
         data = {
-            'profile_id': profile_id,
             'application_id': app_id,
             'architecture_id': arch_id,
             'type': 0
         }
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
                              headers=self.headers,
                              data=json.dumps(data),
                              verify=False)
 
-    def create_manual_scan_autocreate_profile(self, app_id, arch_id):
+    def create_auto_scan(self, project_id, profile_id, app_id, arch_id, test_case_id):
         data = {
             'application_id': app_id,
             'architecture_id': arch_id,
-            'type': 0
+            'test_case_id': test_case_id,
+            'type': 1
         }
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
         return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
                              headers=self.headers,
                              data=json.dumps(data),
                              verify=False)
 
-    def create_auto_scan(self, profile_id, app_id, arch_id, test_case_id):
+    def create_appium_scan(self, project_id, profile_id, app_id, arch_id, appium_script_path):
         data = {
-            'profile_id': profile_id,
             'application_id': app_id,
             'architecture_id': arch_id,
-            'test_case_id': test_case_id,
-            'type': 1
+            'type': 2
         }
-        return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
-                             headers=self.headers,
-                             data=json.dumps(data),
-                             verify=False)
+        headers = {
+            'Authorization': self.headers['Authorization']
+        }
+
+        if project_id:
+            data['project_id'] = project_id
+        if profile_id:
+            data['profile_id'] = profile_id
+        with open(appium_script_path, 'rb') as f:
+            files = {'script': f}
+            return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/dasts/',
+                                 headers=headers,
+                                 data=data,
+                                 files=files,
+                                 verify=False)
 
     def start_scan(self, dast_id):
         """
         Start automated scan through REST API
         :return: scan info resp(dict)
         """
         return requests.post(f'{self.url}/dasts/{dast_id}/start/',
```

### Comparing `mdast_cli-2023.3.1/mdast_cli_core/token.py` & `mdast_cli-2023.4.2/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli-2023.3.1/setup.py` & `mdast_cli-2023.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli",
 
 
-    version='2023.03.01',
+    version='2023.04.02',
+
 
 
     author="Dynamic-Mobile-Security",
     description="Dynamic-Mobile-Security",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dynamic-Mobile-Security/mdast-cli",
```

