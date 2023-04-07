# Comparing `tmp/submit_cgap-3.1.0.1b1.tar.gz` & `tmp/submit_cgap-3.1.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "submit_cgap-3.1.0.1b1.tar", max compression
+gzip compressed data, was "submit_cgap-3.1.0.1b2.tar", max compression
```

## Comparing `submit_cgap-3.1.0.1b1.tar` & `submit_cgap-3.1.0.1b2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1071 2023-03-28 09:59:05.076193 submit_cgap-3.1.0.1b1/LICENSE
--rw-r--r--   0        0        0     1893 2023-03-28 09:59:05.076193 submit_cgap-3.1.0.1b1/README.rst
--rw-r--r--   0        0        0     2741 2023-03-28 09:59:05.076193 submit_cgap-3.1.0.1b1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 09:59:05.076193 submit_cgap-3.1.0.1b1/submit_cgap/__init__.py
--rw-r--r--   0        0        0     2189 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/base.py
--rw-r--r--   0        0        0      292 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/__init__.py
--rw-r--r--   0        0        0      924 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     1567 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/resume_uploads.py
--rw-r--r--   0        0        0      898 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1563 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_genelist.py
--rw-r--r--   0        0        0     2932 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     2205 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1243 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/scripts/upload_item_data.py
--rw-r--r--   0        0        0    44452 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/submission.py
--rw-r--r--   0        0        0        0 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/__init__.py
--rw-r--r--   0        0        0    10870 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_simple.xlsx
--rw-r--r--   0        0        0    10875 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_simple2.xlsx
--rw-r--r--   0        0        0    13306 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_test.xlsx
--rw-r--r--   0        0        0    13192 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_test_with_errors.xlsx
--rw-r--r--   0        0        0      163 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0      169 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     3535 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_base.py
--rw-r--r--   0        0        0      543 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     9678 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2904 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   150101 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submission.py
--rw-r--r--   0        0        0     3291 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6869 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3223 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3836 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     5131 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_utils.py
--rw-r--r--   0        0        0      363 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/test_version.py
--rw-r--r--   0        0        0      684 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/tests/testing_helpers.py
--rw-r--r--   0        0        0     2436 2023-03-28 09:59:05.080194 submit_cgap-3.1.0.1b1/submit_cgap/utils.py
--rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 submit_cgap-3.1.0.1b1/setup.py
--rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 submit_cgap-3.1.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/LICENSE
+-rw-r--r--   0        0        0     1893 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/README.rst
+-rw-r--r--   0        0        0     2909 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/__init__.py
+-rw-r--r--   0        0        0     2189 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/base.py
+-rw-r--r--   0        0        0      292 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/__init__.py
+-rw-r--r--   0        0        0      924 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1567 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/resume_uploads.py
+-rw-r--r--   0        0        0      898 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1563 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_genelist.py
+-rw-r--r--   0        0        0     2932 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     2205 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1243 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    44452 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/submission.py
+-rw-r--r--   0        0        0        0 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/tests/__init__.py
+-rw-r--r--   0        0        0    10870 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_simple.xlsx
+-rw-r--r--   0        0        0    10875 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2023-04-07 21:12:52.830515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_test.xlsx
+-rw-r--r--   0        0        0    13192 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_test_with_errors.xlsx
+-rw-r--r--   0        0        0      163 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0      169 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     3535 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_base.py
+-rw-r--r--   0        0        0      543 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     9678 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2904 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   150101 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submission.py
+-rw-r--r--   0        0        0     3291 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6869 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3223 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3836 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     5131 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_utils.py
+-rw-r--r--   0        0        0      363 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/test_version.py
+-rw-r--r--   0        0        0      684 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/tests/testing_helpers.py
+-rw-r--r--   0        0        0     2436 2023-04-07 21:12:52.834515 submit_cgap-3.1.0.1b2/submit_cgap/utils.py
+-rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 submit_cgap-3.1.0.1b2/setup.py
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 submit_cgap-3.1.0.1b2/PKG-INFO
```

### Comparing `submit_cgap-3.1.0.1b1/LICENSE` & `submit_cgap-3.1.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/README.rst` & `submit_cgap-3.1.0.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/pyproject.toml` & `submit_cgap-3.1.0.1b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "submit_cgap"
-version = "3.1.0.1b1"  # to become 4.0.0
+version = "3.1.0.1b2"  # to become 4.0.0
 description = "Support for uploading file submissions to the Clinical Genomics Analysis Platform (CGAP)."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submit-cgap"]
 homepage = "https://github.com/dbmi-bgm/SubmitCGAP"
 repository = "https://github.com/dbmi-bgm/SubmitCGAP.git"
@@ -55,15 +55,17 @@
 
 # PyCharm says boto3-stubs contains useful type hints
 # boto3-stubs = "^1.26.79"
 
 # Coverage
 codacy-coverage = ">=1.3.11"
 coverage = ">=6.5.0"
-coveralls = ">=3.3.1"
+# Loaded manually in GA workflow for coverage because a dependency on 2to3
+# in its docopts dependency makes a problem for laoding it here in poetry. -kmp 7-Apr-2023
+# coveralls = ">=3.3.1"
 
 # Linting generally
 flake8 = ">=3.9.2"
 
 # pygments is used by PyCharm
 pygments = ">=2.14.0"
```

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/base.py` & `submit_cgap-3.1.0.1b2/submit_cgap/base.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/make_sample_fastq_file.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/resume_uploads.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/show_upload_info.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_genelist.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_metadata_bundle.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/submit_ontology.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/scripts/upload_item_data.py` & `submit_cgap-3.1.0.1b2/submit_cgap/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/submission.py` & `submit_cgap-3.1.0.1b2/submit_cgap/submission.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_simple.xlsx` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_simple.xlsx`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_simple2.xlsx` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_test.xlsx` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_test.xlsx`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/data/cgap_submit_test_with_errors.xlsx` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/data/cgap_submit_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_base.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_exceptions.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_make_sample_fastq_file.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_resume_uploads.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_show_upload_info.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submission.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_genelist.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_metadata_bundle.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_submit_ontology.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_testing_helpers.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_upload_item_data.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/test_utils.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/tests/testing_helpers.py` & `submit_cgap-3.1.0.1b2/submit_cgap/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/submit_cgap/utils.py` & `submit_cgap-3.1.0.1b2/submit_cgap/utils.py`

 * *Files identical despite different names*

### Comparing `submit_cgap-3.1.0.1b1/setup.py` & `submit_cgap-3.1.0.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                      'submit-ontology = '
                      'submit_cgap.scripts.submit_ontology:main',
                      'upload-item-data = '
                      'submit_cgap.scripts.upload_item_data:main']}
 
 setup_kwargs = {
     'name': 'submit-cgap',
-    'version': '3.1.0.1b1',
+    'version': '3.1.0.1b2',
     'description': 'Support for uploading file submissions to the Clinical Genomics Analysis Platform (CGAP).',
     'long_description': '==========\nSubmitCGAP\n==========\n\n\nA file submission tool for CGAP\n===============================\n\n.. image:: https://travis-ci.org/dbmi-bgm/SubmitCGAP.svg\n   :target: https://travis-ci.org/dbmi-bgm/SubmitCGAP\n   :alt: Build Status\n\n.. image:: https://coveralls.io/repos/github/dbmi-bgm/SubmitCGAP/badge.svg\n   :target: https://coveralls.io/github/dbmi-bgm/SubmitCGAP\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/submitcgap/badge/?version=latest\n   :target: https://submitcgap.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n\nDescription\n===========\n\nThis is a tool for uploading certain kinds of files to CGAP.\n\nCurrent support is for submission of new cases, family histories, and gene lists.\n\n\nInstallation\n============\n\nInstalling this system involves these steps:\n\n1. Create, install, and activate a virtual environment.\n2. *Only if you are a developer*, install poetry and select the source repository.\n   Others will not have a source repository to select,\n   so should skip this step.\n3. If you are an end user, do "``pip install submit_cgap``".\n   Otherwise, do "``make build``".\n4. Set up a ``~/.cgap-keys.json`` credentials file.\n\nFor detailed information about these installation steps, see\n`Installing SubmitCGAP <https://submitcgap.readthedocs.io/en/latest/installation.html>`_.\n\n\nTesting\n=======\n\nTo run unit tests, do::\n\n   $ make test\n\nAdditional notes on testing these scripts for release can be found in\n`Testing SubmitCGAP <TESTING.rst>`__.\n\n\nGetting Started\n===============\n\nOnce you have finished installing this library into your virtual environment,\nyou should have access to the ``submit-metadata-bundle`` and the ``submit-genelist``\ncommands. For more information about how to format files for submission and how to\nuse these commands, see `Getting Started <https://submitcgap.readthedocs.io/en/latest/getting_started.html>`_.\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dbmi-bgm/SubmitCGAP',
```

### Comparing `submit_cgap-3.1.0.1b1/PKG-INFO` & `submit_cgap-3.1.0.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: submit-cgap
-Version: 3.1.0.1b1
+Version: 3.1.0.1b2
 Summary: Support for uploading file submissions to the Clinical Genomics Analysis Platform (CGAP).
 Home-page: https://github.com/dbmi-bgm/SubmitCGAP
 License: MIT
 Keywords: submit-cgap
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.0,<3.10
```

