# Comparing `tmp/pyBibX-1.7.4.tar.gz` & `tmp/pyBibX-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-1.7.4.tar", last modified: Fri Apr  7 15:23:45 2023, max compression
+gzip compressed data, was "dist\pyBibX-1.7.5.tar", last modified: Fri Apr  7 15:25:24 2023, max compression
```

## Comparing `pyBibX-1.7.4.tar` & `pyBibX-1.7.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 15:23:45.000000 pyBibX-1.7.4/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-1.7.4/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-1.7.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8550 2023-04-07 15:23:45.000000 pyBibX-1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     8116 2023-04-07 14:48:33.000000 pyBibX-1.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 15:23:45.000000 pyBibX-1.7.4/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.4/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:23:45.000000 pyBibX-1.7.4/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-1.7.4/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   240751 2023-04-07 14:35:11.000000 pyBibX-1.7.4/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:23:45.000000 pyBibX-1.7.4/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.4/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 15:23:45.000000 pyBibX-1.7.4/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     8550 2023-04-07 15:23:44.000000 pyBibX-1.7.4/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-07 15:23:45.000000 pyBibX-1.7.4/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 15:23:44.000000 pyBibX-1.7.4/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-04-07 15:23:44.000000 pyBibX-1.7.4/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 15:23:44.000000 pyBibX-1.7.4/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 15:23:44.000000 pyBibX-1.7.4/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-07 15:23:45.000000 pyBibX-1.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-07 15:23:35.000000 pyBibX-1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:25:24.000000 pyBibX-1.7.5/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-1.7.5/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-1.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8357 2023-04-07 15:25:24.000000 pyBibX-1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7926 2023-04-07 15:24:42.000000 pyBibX-1.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 15:25:24.000000 pyBibX-1.7.5/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.5/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:25:24.000000 pyBibX-1.7.5/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-1.7.5/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   240751 2023-04-07 14:35:11.000000 pyBibX-1.7.5/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:25:24.000000 pyBibX-1.7.5/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-1.7.5/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 15:25:24.000000 pyBibX-1.7.5/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     8357 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 15:25:23.000000 pyBibX-1.7.5/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-07 15:25:24.000000 pyBibX-1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-04-07 15:25:09.000000 pyBibX-1.7.5/setup.py
```

### Comparing `pyBibX-1.7.4/LICENSE` & `pyBibX-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/PKG-INFO` & `pyBibX-1.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 1.7.4
+Version: 1.7.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -62,20 +62,17 @@
 ```
 
 2. Try it in **Colab**:
 
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
-- Example 04: Cochrane              ([ Colab Demo ]())
-- Example 05: Dimensions            ([ Colab Demo ]())
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
-- Example 09: Scopus + WOS + Pubmed + Cochrane  + Dimensions ([ Colab Demo ]())
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
```

### Comparing `pyBibX-1.7.4/README.md` & `pyBibX-1.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,17 @@
 ```
 
 2. Try it in **Colab**:
 
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
-- Example 04: Cochrane              ([ Colab Demo ]())
-- Example 05: Dimensions            ([ Colab Demo ]())
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
-- Example 09: Scopus + WOS + Pubmed + Cochrane  + Dimensions ([ Colab Demo ]())
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
```

### Comparing `pyBibX-1.7.4/pyBibX/base/pbx.py` & `pyBibX-1.7.5/pyBibX/base/pbx.py`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-1.7.5/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/pyBibX.egg-info/PKG-INFO` & `pyBibX-1.7.5/pyBibX.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 1.7.4
+Version: 1.7.5
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -62,20 +62,17 @@
 ```
 
 2. Try it in **Colab**:
 
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
-- Example 04: Cochrane              ([ Colab Demo ]())
-- Example 05: Dimensions            ([ Colab Demo ]())
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
-- Example 09: Scopus + WOS + Pubmed + Cochrane  + Dimensions ([ Colab Demo ]())
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
```

### Comparing `pyBibX-1.7.4/pyBibX.egg-info/SOURCES.txt` & `pyBibX-1.7.5/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-1.7.4/setup.py` & `pyBibX-1.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='1.7.4',
+    version='1.7.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

