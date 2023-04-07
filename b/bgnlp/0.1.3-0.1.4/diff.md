# Comparing `tmp/bgnlp-0.1.3.tar.gz` & `tmp/bgnlp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgnlp-0.1.3.tar", last modified: Fri Apr  7 15:19:40 2023, max compression
+gzip compressed data, was "bgnlp-0.1.4.tar", last modified: Fri Apr  7 15:29:30 2023, max compression
```

## Comparing `bgnlp-0.1.3.tar` & `bgnlp-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.554924 bgnlp-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 15:16:58.000000 bgnlp-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 15:16:58.000000 bgnlp-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:19:40.550924 bgnlp-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-07 15:16:58.000000 bgnlp-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.542924 bgnlp-0.1.3/bgnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.546924 bgnlp-0.1.3/bgnlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/models/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.546924 bgnlp-0.1.3/bgnlp/serialized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/serialized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.546924 bgnlp-0.1.3/bgnlp/serialized/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/serialized/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.546924 bgnlp-0.1.3/bgnlp/serialized/vocabs/
--rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/serialized/vocabs/cb-vocab.pt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.550924 bgnlp-0.1.3/bgnlp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-07 15:16:58.000000 bgnlp-0.1.3/bgnlp/tools/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:19:40.546924 bgnlp-0.1.3/bgnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:19:40.000000 bgnlp-0.1.3/bgnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-07 15:19:40.000000 bgnlp-0.1.3/bgnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:19:40.000000 bgnlp-0.1.3/bgnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 15:19:40.000000 bgnlp-0.1.3/bgnlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 15:16:58.000000 bgnlp-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:19:40.554924 bgnlp-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-07 15:16:58.000000 bgnlp-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.676992 bgnlp-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 15:29:19.000000 bgnlp-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 15:29:19.000000 bgnlp-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:29:30.672992 bgnlp-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-07 15:29:19.000000 bgnlp-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/models/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/serialized/vocabs/
+-rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/serialized/vocabs/cb-vocab.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-07 15:29:19.000000 bgnlp-0.1.4/bgnlp/tools/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:29:30.672992 bgnlp-0.1.4/bgnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 15:29:30.000000 bgnlp-0.1.4/bgnlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 15:29:19.000000 bgnlp-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:29:30.676992 bgnlp-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-07 15:29:19.000000 bgnlp-0.1.4/setup.py
```

### Comparing `bgnlp-0.1.3/LICENSE` & `bgnlp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/PKG-INFO` & `bgnlp-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.1.3 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.1.4 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `bgnlp-0.1.3/README.md` & `bgnlp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/models/bert.py` & `bgnlp-0.1.4/bgnlp/models/bert.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/models/seq2seq.py` & `bgnlp-0.1.4/bgnlp/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/serialized/vocabs/cb-vocab.pt` & `bgnlp-0.1.4/bgnlp/serialized/vocabs/cb-vocab.pt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/tools/configs.py` & `bgnlp-0.1.4/bgnlp/tools/configs.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/tools/mappings.py` & `bgnlp-0.1.4/bgnlp/tools/mappings.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/tools/mixins.py` & `bgnlp-0.1.4/bgnlp/tools/mixins.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/tools/taggers.py` & `bgnlp-0.1.4/bgnlp/tools/taggers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp/tools/tokenizers.py` & `bgnlp-0.1.4/bgnlp/tools/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.1.3/bgnlp.egg-info/PKG-INFO` & `bgnlp-0.1.4/bgnlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.1.3 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.1.4 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `bgnlp-0.1.3/setup.py` & `bgnlp-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 ROOT = os.path.abspath(os.path.dirname(__file__))
 README_PATH = os.path.join(ROOT, "README.md")
 REQUIREMENTS_PATH = os.path.join(ROOT, "requirements.txt")
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Package for Bulgarian Natural Language Processing (NLP)'
 
 
 def _get_requirements(path):
     with open(path, "r") as f:
         requirements_str = f.read()
-        packages = re.findall(r"(.+==[^\n]+)\n", requirements_str)
+        packages = re.findall(r"(.+=?=?[^\n]+)\n", requirements_str)
         return packages
 
 
 if __name__ == "__main__":
     setup(
         name="bgnlp",
         version=VERSION,
```

