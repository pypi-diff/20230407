# Comparing `tmp/pandas-indexing-0.1.2.tar.gz` & `tmp/pandas-indexing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.1.2.tar", last modified: Mon Feb 27 23:15:37 2023, max compression
+gzip compressed data, was "pandas-indexing-0.2.tar", last modified: Fri Apr  7 21:36:25 2023, max compression
```

## Comparing `pandas-indexing-0.1.2.tar` & `pandas-indexing-0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.549020 pandas-indexing-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.549020 pandas-indexing-0.1.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   220293 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/notebooks/introduction.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.549020 pandas-indexing-0.1.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/reference/accessors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.545020 pandas-indexing-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-27 23:15:18.000000 pandas-indexing-0.1.2/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 23:15:37.553020 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-27 23:15:37.000000 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-27 23:15:37.000000 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 23:15:37.000000 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-27 23:15:37.000000 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-27 23:15:37.000000 pandas-indexing-0.1.2/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.518439 pandas-indexing-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-07 21:36:07.000000 pandas-indexing-0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-07 21:36:07.000000 pandas-indexing-0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-07 21:36:07.000000 pandas-indexing-0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-07 21:36:07.000000 pandas-indexing-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-07 21:36:07.000000 pandas-indexing-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-07 21:36:25.518439 pandas-indexing-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-07 21:36:07.000000 pandas-indexing-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.514439 pandas-indexing-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.514439 pandas-indexing-0.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   221702 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 21:36:07.000000 pandas-indexing-0.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-07 21:36:07.000000 pandas-indexing-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-07 21:36:07.000000 pandas-indexing-0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:36:25.518439 pandas-indexing-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.514439 pandas-indexing-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.514439 pandas-indexing-0.2/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.518439 pandas-indexing-0.2/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-07 21:36:07.000000 pandas-indexing-0.2/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:36:25.518439 pandas-indexing-0.2/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-07 21:36:25.000000 pandas-indexing-0.2/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-07 21:36:25.000000 pandas-indexing-0.2/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:36:25.000000 pandas-indexing-0.2/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 21:36:25.000000 pandas-indexing-0.2/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 21:36:25.000000 pandas-indexing-0.2/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.1.2/CODE_OF_CONDUCT.md` & `pandas-indexing-0.2/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,8 +127,7 @@
 [https://www.contributor-covenant.org/translations][translations].
 
 [homepage]: https://www.contributor-covenant.org
 [v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
 [Mozilla CoC]: https://github.com/mozilla/diversity
 [FAQ]: https://www.contributor-covenant.org/faq
 [translations]: https://www.contributor-covenant.org/translations
-
```

### Comparing `pandas-indexing-0.1.2/CONTRIBUTING.rst` & `pandas-indexing-0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/LICENSE` & `pandas-indexing-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/PKG-INFO` & `pandas-indexing-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.1.2
+Version: 0.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
@@ -12,22 +12,21 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: lint
 License-File: LICENSE
 
 pandas-indexing helper
```

### Comparing `pandas-indexing-0.1.2/README.rst` & `pandas-indexing-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/docs/conf.py` & `pandas-indexing-0.2/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,16 +52,19 @@
     spelling_word_list_filename = ["spelling_wordlist.txt"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["."]
 
 
 extlinks = {
-    "issue": ("https://github.com/coroa/pandas-indexing/issues/%s", "#"),  # noqa: E501
-    "pr": ("https://github.com/coroa/pandas-indexing/pull/%s", "PR #"),  # noqa: E501
+    "issue": (
+        "https://github.com/coroa/pandas-indexing/issues/%s",
+        "GH%s",
+    ),
+    "pull": ("https://github.com/coroa/pandas-indexing/pull/%s", "PR%s"),
 }
 
 # codecov io closes connection if host is accessed too repetitively.
 # codecov links are ignored here for the same reason there's a sleep
 # in the .travis.yml file
 # see https://github.com/codecov/codecov-python/issues/158
 linkcheck_ignore = [
@@ -93,14 +96,16 @@
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for coverage extension ------------------------------------------
 coverage_write_headline = False  # do not write headlines.
 
 # -- Options for autodoc extension -------------------------------------------
 
+# Do not add module names in the doc to hide the internal package structure of SeisBench
+add_module_names = False
 autodoc_default_options = {
     "members": True,
     "undoc-members": False,
     "private-members": False,
     "special-members": False,
     "inherited-members": True,
     "show-inheritance": True,
```

### Comparing `pandas-indexing-0.1.2/docs/notebooks/introduction.ipynb` & `pandas-indexing-0.2/docs/notebooks/introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874862351190477%*

 * *Differences: {"'cells'": "{14: {'source': ['Under the hood `isin` and `ismatch` generate `Selector` objects "*

 * *            'that can be called with data to generate boolean masks. They can be composed into '*

 * *            'complex queries intuitively, which are kept as a hierarchical structure of '*

 * *            "objects.']}, 15: {'outputs': {0: {'data': {'text/plain': "*

 * *            '["And(a=Isin(filters={\'variable\': [\'Coal\', \'Gas\', \'Nuclear\'], \'unit\': '*

 * *            '\'GW\'}), b=Not(a=Ismatch(filters={\'variable\': […]*

```diff
@@ -1110,52 +1110,106 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "b4d501a3",
             "metadata": {},
             "source": [
-                "Under the hood `isin` and `ismatch` generate boolean masks that can be used for more complex queries, but the dataframe needs to be handed into the method as first argument then:"
+                "Under the hood `isin` and `ismatch` generate `Selector` objects that can be called with data to generate boolean masks. They can be composed into complex queries intuitively, which are kept as a hierarchical structure of objects."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "4197be7d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
+                            "And(a=Isin(filters={'variable': ['Coal', 'Gas', 'Nuclear'], 'unit': 'GW'}), b=Not(a=Ismatch(filters={'variable': 'S*'}, regex=False)))"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "query = isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & ~ismatch(variable=\"S*\")\n",
+                "query"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "f137127f",
+            "metadata": {},
+            "source": [
+                "For evaluating the query one needs to pass in a data object to produce a boolean mask. Since pandas `.loc` indexer does exactly that, these queries work as expected.\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "18401aa0",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
                             "model                  scenario                      region  variable    unit\n",
                             "REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   Biomass     GW      False\n",
-                            "                                                             Coal        GW      False\n",
+                            "                                                             Coal        GW       True\n",
                             "                                                             Gas         GW       True\n",
                             "                                                             Geothermal  GW      False\n",
                             "                                                             Hydro       GW      False\n",
                             "                                                             Nuclear     GW       True\n",
                             "                                                             Oil         GW      False\n",
                             "                                                             Other       GW      False\n",
                             "                                                             Solar       GW      False\n",
                             "                                                             Wind        GW      False\n",
-                            "Name: 2030, dtype: bool"
+                            "dtype: bool"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "isin(capacity, variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & (capacity[2030] > 250)"
+                "query(capacity)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "7e1d4f00",
+            "metadata": {},
+            "source": [
+                "<div class=\"alert alert-warning\">\n",
+                "\n",
+                "WARNING\n",
+                "\n",
+                "It is currently impossible to use a pandas boolean series **in front of** a selector; ie.\n",
+                "\n",
+                "```python\n",
+                "(capacity[2030] > 250) & isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\")\n",
+                "```\n",
+                "will **fail**, it needs to be\n",
+                "```python\n",
+                "isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & (capacity[2030] > 250)\n",
+                "```\n",
+                "\n",
+                "</div>"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "8b421dba",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1275,23 +1329,22 @@
                             "\n",
                             "                                                                              2040  \n",
                             "model                 scenario                     region variable unit             \n",
                             "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Gas      GW    1289.4777  \n",
                             "                                                          Nuclear  GW     214.4376  "
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "high_capacity_fossil = capacity.loc[\n",
-                "    isin(capacity, variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\")\n",
-                "    & (capacity[2030] > 250),\n",
+                "    isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"], unit=\"GW\") & (capacity[2030] > 250),\n",
                 "    :2041,\n",
                 "]\n",
                 "high_capacity_fossil"
             ]
         },
         {
             "attachments": {},
@@ -1300,15 +1353,15 @@
             "metadata": {},
             "source": [
                 "The simple fact that this is an operation on `[]`, means that we can also use it to modify values in-place:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "71d7aa7d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1428,15 +1481,15 @@
                             "\n",
                             "                                                                              2040  \n",
                             "model                 scenario                     region variable unit             \n",
                             "REMIND-MAgPIE 2.1-4.3 DeepElec_SSP2_HighRE_Budg900 World  Gas      GW    1000.0000  \n",
                             "                                                          Nuclear  GW     214.4376  "
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "high_capacity_fossil.loc[isin(variable=\"Gas\"), 2030:] = 1000.0\n",
                 "high_capacity_fossil"
@@ -1449,15 +1502,15 @@
             "metadata": {},
             "source": [
                 "Most methods in `pandas_indexing` do not care whether they are run on an index, a series or a dataframe, but will transiently take care of handing them down to the appropriate level:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "id": "e0ff32d5",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable  unit  year\n",
@@ -1472,15 +1525,15 @@
                             "                                                             Nuclear   GW    2030     275.5920\n",
                             "                                                                             2040     214.4376\n",
                             "                                                                             2050     156.7766\n",
                             "                                                                             2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fossil_series = (\n",
                 "    capacity.loc[isin(variable=[\"Coal\", \"Gas\", \"Nuclear\"]), [2030, 2040, 2050, 2060]]\n",
@@ -1488,15 +1541,15 @@
                 "    .stack()\n",
                 ")\n",
                 "fossil_series"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "id": "6d4686e6",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                      region  variable  unit  year\n",
@@ -1505,37 +1558,37 @@
                             "                                                             Gas       GW    2030    1584.4033\n",
                             "                                                                             2050     562.8482\n",
                             "                                                             Nuclear   GW    2030     275.5920\n",
                             "                                                                             2050     156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fossil_series.loc[isin(year=[2030, 2050])]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "id": "8d4e91fb",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([False, False, False, False, False, False, False, False,  True,\n",
                             "        True,  True,  True])"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "isin(fossil_series.index, variable=\"Nuclear\")"
             ]
@@ -1549,59 +1602,59 @@
                 "## Selecting based on a multi-index\n",
                 "\n",
                 "If we need pairs of data like `Coal` in 2030 and `Gas` in 2040 and `Nuclear` in 2040 and 2050, based on a given multiindex, then this defines right-oriented `semijoin` like:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "id": "cde4ff9f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([(   'Coal', 2030),\n",
                             "            (    'Gas', 2035),\n",
                             "            ('Nuclear', 2040),\n",
                             "            ('Nuclear', 2050)],\n",
                             "           names=['variable', 'year'])"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "idx = pd.MultiIndex.from_tuples(\n",
                 "    [(\"Coal\", 2030), (\"Gas\", 2035), (\"Nuclear\", 2040), (\"Nuclear\", 2050)],\n",
                 "    names=[\"variable\", \"year\"],\n",
                 ")\n",
                 "idx"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "id": "dc294f2f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year  model                  scenario                      region  unit\n",
                             "Coal      2030  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      182.0149\n",
                             "Gas       2035  NaN                    NaN                           NaN     NaN          NaN\n",
                             "Nuclear   2040  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      214.4376\n",
                             "          2050  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import semijoin\n",
                 "\n",
@@ -1615,29 +1668,29 @@
             "metadata": {},
             "source": [
                 "Since the `(\"Gas\", 2035)` is not part of the original `fossil_series` it shows up as `NaN`s here, an inner join will skip it silently:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "id": "f82d6bf4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year  model                  scenario                      region  unit\n",
                             "Coal      2030  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      182.0149\n",
                             "Nuclear   2040  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      214.4376\n",
                             "          2050  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  World   GW      156.7766\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "semijoin(fossil_series, idx, how=\"inner\")"
             ]
@@ -1651,15 +1704,15 @@
                 "## Projecting levels\n",
                 "\n",
                 "Often after selecting the right subsets, ie the interesting `model` or `scenario` it makes sense to consolidate the data to a given set of `levels`. That is what `projectlevel` is used for:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "id": "6d0000aa",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year\n",
@@ -1674,15 +1727,15 @@
                             "Nuclear   2030     275.5920\n",
                             "          2040     214.4376\n",
                             "          2050     156.7766\n",
                             "          2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import projectlevel\n",
                 "\n",
@@ -1697,15 +1750,15 @@
             "metadata": {},
             "source": [
                 "`projectlevel` reduces the levels attached to a multiindex to the ones explicitly named. It is basically the complement to `droplevel` which removes the listed names"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "id": "308fb920",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "model                  scenario                    \n",
@@ -1720,15 +1773,15 @@
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "                       DeepElec_SSP2_HighRE_Budg900    True\n",
                             "dtype: bool"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series, [\"model\", \"scenario\"]) == fossil_series.droplevel(\n",
                 "    [\"variable\", \"unit\", \"region\", \"year\"]\n",
@@ -1743,15 +1796,15 @@
                 "## Assigning to levels\n",
                 "\n",
                 "`assignlevel` allows to modify individual values with helpful keyword arguments:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 20,
             "id": "4f52e21a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Index(['Updated|Capacity|Electricity|Biomass',\n",
@@ -1772,26 +1825,26 @@
                             "       'Updated|Secondary Energy|Electricity|Oil',\n",
                             "       'Updated|Secondary Energy|Electricity|Other',\n",
                             "       'Updated|Secondary Energy|Electricity|Solar',\n",
                             "       'Updated|Secondary Energy|Electricity|Wind'],\n",
                             "      dtype='object', name='variable')"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "\"Updated|\" + projectlevel(df.index, \"variable\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 21,
             "id": "ca2a3c70",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2631,15 +2684,15 @@
                             "                                                          Updated|Secondary Energy|Electricity|Nuclear    bla   1.388889e+02  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Oil        bla   2.777778e+01  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Other      bla   7.547194e+06  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Solar      bla   9.270394e+07  \n",
                             "                                                          Updated|Secondary Energy|Electricity|Wind       bla   4.123369e+07  "
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from pandas_indexing import assignlevel\n",
                 "\n",
@@ -2652,15 +2705,15 @@
             "metadata": {},
             "source": [
                 "and as such avoids having to rely on `reset_index`, `set_index` pairs, which are painful for large data, since `set_index` is expensive!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 22,
             "id": "72d60d5e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3481,15 +3534,15 @@
                             "                                                                   GWh/yr  1.388889e+02  \n",
                             "                                                                   GWh/yr  2.777778e+01  \n",
                             "                                                                   GWh/yr  7.547194e+06  \n",
                             "                                                                   GWh/yr  9.270394e+07  \n",
                             "                                                                   GWh/yr  4.123369e+07  "
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.reset_index().assign(variable=\"Capacity\").set_index(df.index.names)"
             ]
@@ -3508,15 +3561,15 @@
             "metadata": {},
             "source": [
                 "`concat` ignores level order, so make sure to `reorder_levels` them"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 23,
             "id": "24d42af8-ffd3-4281-9d75-1449046fd6fd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year   \n",
@@ -3543,26 +3596,26 @@
                             "2030      Nuclear     275.5920\n",
                             "2040      Nuclear     214.4376\n",
                             "2050      Nuclear     156.7766\n",
                             "2060      Nuclear      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pd.concat([simple_fossil_series, simple_fossil_series.swaplevel()])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 24,
             "id": "254197c5-8498-4c69-a30d-044e7edb7b53",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "variable  year\n",
@@ -3589,15 +3642,15 @@
                             "Nuclear   2030     275.5920\n",
                             "          2040     214.4376\n",
                             "          2050     156.7766\n",
                             "          2060      92.0667\n",
                             "dtype: float64"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "pd.concat(\n",
                 "    [\n",
@@ -3618,50 +3671,50 @@
                 "# Additional helpful multi-index helpers\n",
                 "\n",
                 "To know which labels exist in a given `level` the index's `unique` method is helpful:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 25,
             "id": "a8300699",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([('REMIND-MAgPIE 2.1-4.3', 2030),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 2040),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 2050),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 2060)],\n",
                             "           names=['model', 'year'])"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series, [\"model\", \"year\"]).index.unique()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 26,
             "id": "187e2a70",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Int64Index([2030, 2040, 2050, 2060], dtype='int64', name='year')"
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fossil_series.index.unique(\"year\")"
             ]
@@ -3672,15 +3725,15 @@
             "metadata": {},
             "source": [
                 "MultiIndex rendering is often annoying to read, since the important information might get abbreviated away, then converting it into a dataframe is helpful"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 27,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MultiIndex([('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
@@ -3694,26 +3747,26 @@
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...),\n",
                             "            ('REMIND-MAgPIE 2.1-4.3', 'DeepElec_SSP2_HighRE_Budg900', ...)],\n",
                             "           names=['model', 'scenario', 'variable'])"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 28,
             "id": "5b7cb7db",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -3828,15 +3881,15 @@
                             "7   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900      Gas\n",
                             "8   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "9   REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "10  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear\n",
                             "11  REMIND-MAgPIE 2.1-4.3  DeepElec_SSP2_HighRE_Budg900  Nuclear"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "projectlevel(fossil_series.index, [\"model\", \"scenario\", \"variable\"]).to_frame(\n",
                 "    index=False\n",
```

### Comparing `pandas-indexing-0.1.2/pyproject.toml` & `pandas-indexing-0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,33 @@
     # 'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Science/Research',
     'Natural Language :: English',
     'Operating System :: POSIX',
     'Operating System :: MacOS',
     'Operating System :: Microsoft',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
 keywords=[
-    'pandas'
+    'pandas',
     # eg: 'keyword1', 'keyword2', 'keyword3',
 ]
 
-requires-python = ">=3.8, <4"
+requires-python = ">=3.9, <4"
 dependencies = [
     # https://stackoverflow.com/questions/14399534
     'pandas>=1.2',
     'deprecated',
+    "attrs",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/coroa/pandas-indexing"
 documentation = "https://pandas-indexing.readthedocs.io/en/latest/"
@@ -57,20 +57,20 @@
     "ipython",
 ]
 
 test = [
     "coverage",
     "pytest",
     "pytest-cov",
-    "hypothesis"
+    "hypothesis",
 ]
 
 lint = [
     "black",
-    "ruff"
+    "ruff",
 ]
 
 [project.scripts]
 
 [tool.pytest.ini_options]
 # If a pytest section is found in one of the possible config files
 # (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
@@ -106,15 +106,15 @@
 # E501: line too long - let black worry about that
 # E731: do not assign a lambda expression, use a def
 # E741: ambiguous variable names
 ignore = [
     "E402",
     "E501",
     "E731",
-    "E741"
+    "E741",
 ]
 select = [
     # Pyflakes
     "F",
     # Pycodestyle
     "E",
     "W",
```

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing/accessors.py` & `pandas-indexing-0.2/src/pandas_indexing/accessors.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 """
 
 from typing import Any, Literal, Sequence, Union
 
 import pandas as pd
 from pandas import DataFrame, Index, MultiIndex, Series
 
+from . import arithmetics
 from .core import assignlevel, projectlevel, semijoin
 
 
 class _IdxAccessor:
     """
     Convenience accessor for accessing `pandas-indexing` functions.
     """
@@ -116,14 +117,26 @@
 
         See also
         --------
         pandas.Index.join
         """
         return semijoin(self._obj, other, how=how, level=level, sort=sort, axis=axis)
 
+    def multiply(self, other, **align_kwds):
+        return arithmetics.multiply(self._obj, other, **align_kwds)
+
+    def divide(self, other, **align_kwds):
+        return arithmetics.divide(self._obj, other, **align_kwds)
+
+    def add(self, other, **align_kwds):
+        return arithmetics.add(self._obj, other, **align_kwds)
+
+    def subtract(self, other, **align_kwds):
+        return arithmetics.subtract(self._obj, other, **align_kwds)
+
 
 @pd.api.extensions.register_dataframe_accessor("idx")
 class DataFrameIdxAccessor(_DataIdxAccessor):
     pass
 
 
 @pd.api.extensions.register_series_accessor("idx")
```

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing/core.py` & `pandas-indexing-0.2/src/pandas_indexing/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Core module.
 """
-from functools import reduce
-from operator import and_
 from typing import Any, Literal, Sequence, Union
 
 import numpy as np
 from pandas import DataFrame, Index, MultiIndex, Series
 from pandas.core.indexes.frozen import FrozenList
 
-from .utils import shell_pattern_to_regex
+
+Data = Union[Series, DataFrame]
 
 
 def _assignlevel(index: Index, order: bool = False, **labels: Any) -> MultiIndex:
     if isinstance(index, MultiIndex):
         new_levels = list(index.levels)
         new_codes = list(index.codes)
         new_names = list(index.names)
@@ -268,94 +267,7 @@
         data = np.where(left_idx != -1, df_or_series.values[left_idx], np.nan)
     else:
         raise TypeError(
             f"df_or_series must derive from DataFrame or Series, but is {type(df_or_series)}"
         )
 
     return cls(data, *axes).__finalize__(df_or_series)
-
-
-def isin(df=None, **filters):
-    """
-    Constructs a MultiIndex selector.
-
-    Usage
-    -----
-    >>> df.loc[isin(region="World", gas=["CO2", "N2O"])]
-
-    or with explicit df to get a boolean mask
-
-    >>> isin(df, region="World", gas=["CO2", "N2O"])
-    """
-
-    def tester(df):
-        if isinstance(df, Index):
-            index = df
-        else:
-            index = df.index
-        tests = (index.isin(np.atleast_1d(v), level=k) for k, v in filters.items())
-        return reduce(and_, tests)
-
-    return tester if df is None else tester(df)
-
-
-def ismatch(df=None, singlefilter=None, regex=False, **filters):
-    """
-    Constructs an Index or MultiIndex selector based on pattern matching.
-
-    Usage
-    -----
-    for a multiindex:
-
-    >>> df.loc[ismatch(variable="Emissions|*|Fossil Fuel and Industry")]
-
-    for a single index:
-
-    >>> df.loc[ismatch("*bla*")]
-    """
-
-    def index_match(index, patterns):
-        matches = np.zeros((len(index),), dtype=bool)
-        for pat in patterns:
-            if isinstance(pat, str):
-                if not regex:
-                    pat = shell_pattern_to_regex(pat) + "$"
-                matches |= index.str.match(pat, na=False)
-            else:
-                matches |= index == pat
-        return matches
-
-    def multiindex_match(index, patterns, level):
-        level_num = index.names.index(level)
-        levels = index.levels[level_num]
-
-        matches = index_match(levels, patterns)
-
-        (indices,) = np.where(matches)
-        return np.in1d(index.codes[level_num], indices)
-
-    def tester(df):
-        if isinstance(df, Index):
-            index = df
-        else:
-            index = df.index
-
-        if singlefilter is not None:
-            matches = index_match(index, np.atleast_1d(singlefilter))
-        else:
-            tests = (
-                multiindex_match(index, np.atleast_1d(v), level=k)
-                for k, v in filters.items()
-            )
-            matches = reduce(and_, tests)
-
-        return Series(matches, index=index)
-
-    if df is None:
-        return tester
-    elif not isinstance(df, (DataFrame, Series)):
-        # Special case: a pattern was passed in through `df` which wants to be applied to
-        # hopefully a non-MultiIndex based Series or dataframe that we get afterwards
-        singlefilter = df
-        return tester
-    else:
-        return tester(df)
```

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing/datasets/__init__.py` & `pandas-indexing-0.2/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas-indexing-0.2/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing/utils.py` & `pandas-indexing-0.2/src/pandas_indexing/utils.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing.egg-info/PKG-INFO` & `pandas-indexing-0.2/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.1.2
+Version: 0.2
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
@@ -12,22 +12,21 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: lint
 License-File: LICENSE
 
 pandas-indexing helper
```

### Comparing `pandas-indexing-0.1.2/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas-indexing-0.2/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 docs/AUTHORS.rst
+docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/notebooks/introduction.ipynb
-docs/reference/accessors.rst
-docs/reference/core.rst
 src/pandas_indexing/__init__.py
 src/pandas_indexing/accessors.py
+src/pandas_indexing/arithmetics.py
 src/pandas_indexing/core.py
+src/pandas_indexing/selectors.py
 src/pandas_indexing/utils.py
 src/pandas_indexing.egg-info/PKG-INFO
 src/pandas_indexing.egg-info/SOURCES.txt
 src/pandas_indexing.egg-info/dependency_links.txt
 src/pandas_indexing.egg-info/requires.txt
 src/pandas_indexing.egg-info/top_level.txt
 src/pandas_indexing/datasets/__init__.py
```

