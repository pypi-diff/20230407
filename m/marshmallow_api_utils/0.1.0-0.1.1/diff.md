# Comparing `tmp/marshmallow_api_utils-0.1.0.tar.gz` & `tmp/marshmallow_api_utils-0.1.1.tar.gz`

## Comparing `marshmallow_api_utils-0.1.0.tar` & `marshmallow_api_utils-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/.editorconfig
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/local.ipynb
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/fields.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/flask_blueprint.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/ma_dataclass.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/package_finder.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/middleware/__init__.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/middleware/flask_logging_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/__init__.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/date_time_filter.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/pageable.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/sortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/tests/test_date_filter_parsing.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/tests/test_date_filter_sql_generator.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/tests/utils.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/LICENSE.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/README.md
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/local.ipynb
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/fields.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/flask_blueprint.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/ma_dataclass.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/package_finder.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/middleware/__init__.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/middleware/flask_logging_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/__init__.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/date_time_filter.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/pageable.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/sortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/tests/test_date_filter_parsing.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/tests/test_date_filter_sql_generator.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/README.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 marshmallow_api_utils-0.1.1/PKG-INFO
```

### Comparing `marshmallow_api_utils-0.1.0/.pre-commit-config.yaml` & `marshmallow_api_utils-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/local.ipynb` & `marshmallow_api_utils-0.1.1/local.ipynb`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/fields.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/flask_blueprint.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/ma_dataclass.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/ma_dataclass.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/package_finder.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/package_finder.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/middleware/flask_logging_middleware.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/middleware/flask_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/date_time_filter.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/date_time_filter.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/pageable.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/pageable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/marshmallow_api_utils/models/sortable.py` & `marshmallow_api_utils-0.1.1/marshmallow_api_utils/models/sortable.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/tests/test_date_filter_parsing.py` & `marshmallow_api_utils-0.1.1/tests/test_date_filter_parsing.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/tests/test_date_filter_sql_generator.py` & `marshmallow_api_utils-0.1.1/tests/test_date_filter_sql_generator.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/tests/utils.py` & `marshmallow_api_utils-0.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/.gitignore` & `marshmallow_api_utils-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/LICENSE.md` & `marshmallow_api_utils-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `marshmallow_api_utils-0.1.0/pyproject.toml` & `marshmallow_api_utils-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "sqlalchemy >=2.0.0,<3",
   "python-multipart >=0.0.5,<0.0.7",
   "pyyaml >=5.4.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/mvanderlee/starmallow"
+Homepage = "https://github.com/mvanderlee/marshmallow_api_utils"
 
 
 [project.optional-dependencies]
 test = [
   "coverage[toml] >= 6.5.0,< 8.0",
   "isort >=5.0.6,<6.0.0",
   "mypy>=1.1.1,<2",
```

### Comparing `marshmallow_api_utils-0.1.0/PKG-INFO` & `marshmallow_api_utils-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: marshmallow_api_utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Marshmallow API Utilities
-Project-URL: Homepage, https://github.com/mvanderlee/starmallow
+Project-URL: Homepage, https://github.com/mvanderlee/marshmallow_api_utils
 Author-email: Michiel Vanderlee <jmt.vanderlee@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

