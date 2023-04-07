# Comparing `tmp/hf4q-0.0.6.tar.gz` & `tmp/hf4q-0.0.7.tar.gz`

## Comparing `hf4q-0.0.6.tar` & `hf4q-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,16 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 hf4q-0.0.6/Embedding Images in HTMLs.url
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hf4q-0.0.6/Packaging.url
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hf4q-0.0.6/certutil -encode mypicture.png mypicture.txt.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 hf4q-0.0.6/up8c18p01.png
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 hf4q-0.0.6/up8c18p01.txt
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hf4q-0.0.6/updatePackage.txt
--rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/yyy.py
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/checkups1/checkups1/checkups10.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/checkups1/checkups1/index.html
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/__init__.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/_common.py
--rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/_generateEm.py
--rw-r--r--   0        0        0    17850 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/_generateMakeHTMLs.py
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/_scoreEm.py
--rw-r--r--   0        0        0    14836 2020-02-02 00:00:00.000000 hf4q-0.0.6/src/quizhtml/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hf4q-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 hf4q-0.0.6/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 hf4q-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hf4q-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 hf4q-0.0.7/Embedding Images in HTMLs.url
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hf4q-0.0.7/Packaging.url
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hf4q-0.0.7/certutil -encode mypicture.png mypicture.txt.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 hf4q-0.0.7/up8c18p01.png
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 hf4q-0.0.7/up8c18p01.txt
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hf4q-0.0.7/updatePackage.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/__init__.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/_common.py
+-rw-r--r--   0        0        0     9263 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/_generateEm.py
+-rw-r--r--   0        0        0    17850 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/_generateMakeHTMLs.py
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/_scoreEm.py
+-rw-r--r--   0        0        0    14836 2020-02-02 00:00:00.000000 hf4q-0.0.7/src/hf4q/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 hf4q-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 hf4q-0.0.7/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 hf4q-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hf4q-0.0.7/PKG-INFO
```

### Comparing `hf4q-0.0.6/up8c18p01.png` & `hf4q-0.0.7/up8c18p01.png`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/up8c18p01.txt` & `hf4q-0.0.7/up8c18p01.txt`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/updatePackage.txt` & `hf4q-0.0.7/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/src/quizhtml/_common.py` & `hf4q-0.0.7/src/hf4q/_common.py`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/src/quizhtml/_generateEm.py` & `hf4q-0.0.7/src/hf4q/_generateEm.py`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/src/quizhtml/_generateMakeHTMLs.py` & `hf4q-0.0.7/src/hf4q/_generateMakeHTMLs.py`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/src/quizhtml/_scoreEm.py` & `hf4q-0.0.7/src/hf4q/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/src/quizhtml/makeChoices.py` & `hf4q-0.0.7/src/hf4q/makeChoices.py`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/LICENSE.txt` & `hf4q-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/README.md` & `hf4q-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hf4q-0.0.6/pyproject.toml` & `hf4q-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hf4q"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hf4q-0.0.6/PKG-INFO` & `hf4q-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf4q
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/hf4q
 Project-URL: Bug Tracker, https://github.com/generateNscore/hf4q/issues
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hf4q Version: 0.0.6 Summary: A package that
+Metadata-Version: 2.1 Name: hf4q Version: 0.0.7 Summary: A package that
 generates question papers as HTML files to be distributed over the network and
 grades the answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/hf4q Project-URL: Bug Tracker, https://
 github.com/generateNscore/hf4q/issues Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Education Classifier: Intended Audience
 :: End Users/Desktop Classifier: License :: OSI Approved :: MIT License
```

