# Comparing `tmp/psicalc-0.4.3.tar.gz` & `tmp/psicalc-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psicalc-0.4.3.tar", last modified: Fri Feb 10 17:26:44 2023, max compression
+gzip compressed data, was "psicalc-0.4.4.tar", last modified: Fri Apr  7 17:47:39 2023, max compression
```

## Comparing `psicalc-0.4.3.tar` & `psicalc-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-02-10 17:26:44.138139 psicalc-0.4.3/
--rw-r--r--   0 thomastownsley   (501) staff       (20)     1223 2023-02-10 17:26:44.137908 psicalc-0.4.3/PKG-INFO
--rw-r--r--   0 thomastownsley   (501) staff       (20)      721 2021-09-29 20:18:43.000000 psicalc-0.4.3/README.md
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-02-10 17:26:44.135849 psicalc-0.4.3/psicalc/
--rw-r--r--   0 thomastownsley   (501) staff       (20)       23 2021-02-10 15:47:57.000000 psicalc-0.4.3/psicalc/__init__.py
--rw-r--r--   0 thomastownsley   (501) staff       (20)     8816 2021-09-29 20:15:24.000000 psicalc-0.4.3/psicalc/nmi.py
--rwxr-xr-x   0 thomastownsley   (501) staff       (20)    17241 2023-02-10 17:22:19.000000 psicalc-0.4.3/psicalc/psicalc.py
-drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-02-10 17:26:44.137601 psicalc-0.4.3/psicalc.egg-info/
--rw-r--r--   0 thomastownsley   (501) staff       (20)     1223 2023-02-10 17:26:44.000000 psicalc-0.4.3/psicalc.egg-info/PKG-INFO
--rw-r--r--   0 thomastownsley   (501) staff       (20)      226 2023-02-10 17:26:44.000000 psicalc-0.4.3/psicalc.egg-info/SOURCES.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)        1 2023-02-10 17:26:44.000000 psicalc-0.4.3/psicalc.egg-info/dependency_links.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)       20 2023-02-10 17:26:44.000000 psicalc-0.4.3/psicalc.egg-info/requires.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)        8 2023-02-10 17:26:44.000000 psicalc-0.4.3/psicalc.egg-info/top_level.txt
--rw-r--r--   0 thomastownsley   (501) staff       (20)       38 2023-02-10 17:26:44.138218 psicalc-0.4.3/setup.cfg
--rw-r--r--   0 thomastownsley   (501) staff       (20)      909 2023-02-10 17:25:22.000000 psicalc-0.4.3/setup.py
+drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-04-07 17:47:39.883213 psicalc-0.4.4/
+-rw-r--r--   0 thomastownsley   (501) staff       (20)     1223 2023-04-07 17:47:39.882995 psicalc-0.4.4/PKG-INFO
+-rw-r--r--   0 thomastownsley   (501) staff       (20)      721 2021-09-29 20:18:43.000000 psicalc-0.4.4/README.md
+drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-04-07 17:47:39.880504 psicalc-0.4.4/psicalc/
+-rw-r--r--   0 thomastownsley   (501) staff       (20)       23 2021-02-10 15:47:57.000000 psicalc-0.4.4/psicalc/__init__.py
+-rw-r--r--   0 thomastownsley   (501) staff       (20)     8816 2021-09-29 20:15:24.000000 psicalc-0.4.4/psicalc/nmi.py
+-rwxr-xr-x   0 thomastownsley   (501) staff       (20)    16874 2023-04-07 17:44:07.000000 psicalc-0.4.4/psicalc/psicalc.py
+drwxr-xr-x   0 thomastownsley   (501) staff       (20)        0 2023-04-07 17:47:39.882702 psicalc-0.4.4/psicalc.egg-info/
+-rw-r--r--   0 thomastownsley   (501) staff       (20)     1223 2023-04-07 17:47:39.000000 psicalc-0.4.4/psicalc.egg-info/PKG-INFO
+-rw-r--r--   0 thomastownsley   (501) staff       (20)      226 2023-04-07 17:47:39.000000 psicalc-0.4.4/psicalc.egg-info/SOURCES.txt
+-rw-r--r--   0 thomastownsley   (501) staff       (20)        1 2023-04-07 17:47:39.000000 psicalc-0.4.4/psicalc.egg-info/dependency_links.txt
+-rw-r--r--   0 thomastownsley   (501) staff       (20)       20 2023-04-07 17:47:39.000000 psicalc-0.4.4/psicalc.egg-info/requires.txt
+-rw-r--r--   0 thomastownsley   (501) staff       (20)        8 2023-04-07 17:47:39.000000 psicalc-0.4.4/psicalc.egg-info/top_level.txt
+-rw-r--r--   0 thomastownsley   (501) staff       (20)       38 2023-04-07 17:47:39.883288 psicalc-0.4.4/setup.cfg
+-rw-r--r--   0 thomastownsley   (501) staff       (20)      909 2023-04-07 17:47:16.000000 psicalc-0.4.4/setup.py
```

### Comparing `psicalc-0.4.3/PKG-INFO` & `psicalc-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psicalc
-Version: 0.4.3
+Version: 0.4.4
 Summary: Algorithm for clustering protein multiple sequence alignments using normalized mutual information.
 Home-page: https://github.com/mandosoft/psi-calc
 Author: Thomas Townsley
 Author-email: thomas@mandosoft.dev
 Keywords: bioinformatics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psicalc-0.4.3/README.md` & `psicalc-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `psicalc-0.4.3/psicalc/nmi.py` & `psicalc-0.4.4/psicalc/nmi.py`

 * *Files identical despite different names*

### Comparing `psicalc-0.4.3/psicalc/psicalc.py` & `psicalc-0.4.4/psicalc/psicalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,73 +44,59 @@
     label_val = value
     df = df.rename(columns=lambda x: int(x) + label_val)
 
     return df
 
 
 # noinspection PyUnresolvedReferences
-def deweese_schema(df: pd.DataFrame, pattern='^-'):
-    """Labels data based on the range on the row in the MSA with the least insertions.
+def deweese_schema(df: pd.DataFrame, pattern='^-') -> pd.DataFrame:
+    """Labels data based on the range on the first row of the MSA.
+    For example, if the first row is labelled TOP2 YEAST/59-205, then all
+    columns with individuals in the first row are kept and labeled 59-205.
+
     As an option, you can supply a different regex if the MSA uses different
-    symbols to represent insertions. Returns the name of the best row and the resultant
-    MSA in a pandas dataframe."""
+    symbols to represent insertions."""
 
     try:
-        least = None
-        map_row = 0
-        for index, row in df.iterrows():
-            series = row.value_counts()
-            try:
-                null_ct = series['-']
-            except KeyError:
-                null_ct = 0
-                map_row = index
-            if least is None:
-                least = null_ct
-            else:
-                if null_ct < least:
-                    least = null_ct
-                    map_row = index
-        row_ix = map_row
-
-        if '(' in row_ix:
-            ix_label = row_ix.rsplit('(', 1)
-        elif ':' in row_ix:
-            ix_label = row_ix.rsplit(':', 1)
+        first_row_ix = df.index[0]
+        if '(' in first_row_ix:
+            ix_label = first_row_ix.rsplit('(', 1)
+        elif ':' in first_row_ix:
+            ix_label = first_row_ix.rsplit(':', 1)
         else:
-            ix_label = row_ix.rsplit('/', 1)
+            ix_label = first_row_ix.rsplit('/', 1)
         ix_label = ix_label[1]
         ix_label = ix_label.rsplit('-', 1)
         df_label = int(ix_label[0])
         column_lab_dict = dict()
 
         if pattern == 'None':
             for i in df:
-                if df[i].loc[row_ix] is not None:
+                if df[i].iloc[0] is not None:
                     column_lab_dict[df.columns[i]] = df_label
                     df_label += 1
                 else:
                     column_lab_dict[df.columns[i]] = ''
         else:
             for i in df:
-                if not re.search(pattern, df[i].loc[row_ix]):
+                if not re.search(pattern, df[i].iloc[0]):
                     column_lab_dict[df.columns[i]] = df_label
                     df_label += 1
                 else:
                     column_lab_dict[df.columns[i]] = ''
 
         df = df.rename(columns=column_lab_dict)
         if '' in column_lab_dict.values():
             df = df.drop(columns=[''])
         df = df.rename(columns=lambda x: int(x))
 
     except IndexError or KeyError:
         sys.exit(1)
 
-    return row_ix, df
+    return df
 
 
 def check_for_duplicates(df: pd.DataFrame) -> pd.DataFrame:
     """Removes duplicate sequences based on sequence label only."""
     raw_data = len(df.index)
     df = df[~df.index.duplicated(keep='first')]
     dd = len(df.index)
```

### Comparing `psicalc-0.4.3/psicalc.egg-info/PKG-INFO` & `psicalc-0.4.4/psicalc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psicalc
-Version: 0.4.3
+Version: 0.4.4
 Summary: Algorithm for clustering protein multiple sequence alignments using normalized mutual information.
 Home-page: https://github.com/mandosoft/psi-calc
 Author: Thomas Townsley
 Author-email: thomas@mandosoft.dev
 Keywords: bioinformatics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `psicalc-0.4.3/setup.py` & `psicalc-0.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 setuptools.setup(
     name="psicalc",
     keywords=['bioinformatics'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.4.3",
+    version="0.4.4",
     author="Thomas Townsley",
     author_email="thomas@mandosoft.dev",
     description="Algorithm for clustering protein multiple sequence alignments using normalized mutual information.",
     url="https://github.com/mandosoft/psi-calc",
     packages=setuptools.find_packages(),
     install_requires=['pandas', 'scikit-learn'],
     classifiers=[
```

