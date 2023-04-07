# Comparing `tmp/openlake-0.4.dev1-py3-none-any.whl.zip` & `tmp/openlake-0.5.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15021 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1816 b- defN 20-Feb-02 00:00 openlake/__init__.py
--rw-r--r--  2.0 unx     1570 b- defN 20-Feb-02 00:00 openlake/cache.py
+Zip file size: 15316 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1832 b- defN 20-Feb-02 00:00 openlake/__init__.py
+-rw-r--r--  2.0 unx     1581 b- defN 20-Feb-02 00:00 openlake/cache.py
 -rw-r--r--  2.0 unx     1884 b- defN 20-Feb-02 00:00 openlake/fetcher.py
 -rw-r--r--  2.0 unx     2031 b- defN 20-Feb-02 00:00 openlake/parser.py
 -rw-r--r--  2.0 unx     3372 b- defN 20-Feb-02 00:00 openlake/provider/__init__.py
--rw-r--r--  2.0 unx     3346 b- defN 20-Feb-02 00:00 openlake/provider/kaggle.py
+-rw-r--r--  2.0 unx     4782 b- defN 20-Feb-02 00:00 openlake/provider/kaggle.py
 -rw-r--r--  2.0 unx     2213 b- defN 20-Feb-02 00:00 openlake/provider/sklearn.py
-?rw-r--r--  2.0 unx     3871 b- defN 20-Feb-02 00:00 openlake-0.4.dev1.dist-info/METADATA
-?rw-r--r--  2.0 unx       86 b- defN 20-Feb-02 00:00 openlake-0.4.dev1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openlake-0.4.dev1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 openlake-0.4.dev1.dist-info/licenses/NOTICE
-?rw-r--r--  2.0 unx      976 b- defN 20-Feb-02 00:00 openlake-0.4.dev1.dist-info/RECORD
-12 files, 32645 bytes uncompressed, 13391 bytes compressed:  59.0%
+?rw-r--r--  2.0 unx     3911 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      122 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/licenses/NOTICE
+?rw-r--r--  2.0 unx      976 b- defN 20-Feb-02 00:00 openlake-0.5.dev1.dist-info/RECORD
+12 files, 34149 bytes uncompressed, 13686 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: openlake/provider/kaggle.py
 Comment: 
 
 Filename: openlake/provider/sklearn.py
 Comment: 
 
-Filename: openlake-0.4.dev1.dist-info/METADATA
+Filename: openlake-0.5.dev1.dist-info/METADATA
 Comment: 
 
-Filename: openlake-0.4.dev1.dist-info/WHEEL
+Filename: openlake-0.5.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: openlake-0.4.dev1.dist-info/licenses/LICENSE
+Filename: openlake-0.5.dev1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: openlake-0.4.dev1.dist-info/licenses/NOTICE
+Filename: openlake-0.5.dev1.dist-info/licenses/NOTICE
 Comment: 
 
-Filename: openlake-0.4.dev1.dist-info/RECORD
+Filename: openlake-0.5.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openlake/__init__.py

```diff
@@ -13,24 +13,24 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Openlake ForML feed."""
 
-__version__ = '0.4.dev1'
+__version__ = '0.5.dev1'
 
 import typing
 
 from forml.provider.feed import lazy
 
 from openlake.provider import kaggle, sklearn
 
 #: Default list of origin integrations.
-ORIGINS: typing.Collection[lazy.Origin] = {kaggle.Titanic(), sklearn.BreastCancer(), sklearn.Iris()}
+ORIGINS: typing.Collection[lazy.Origin] = {kaggle.Avazu(), kaggle.Titanic(), sklearn.BreastCancer(), sklearn.Iris()}
 
 
 class Lite(lazy.Feed):
     """ForML feed providing access to a number of public datasets.
 
     External data sources are fetched using the Openlake integrations and cached locally.
```

## openlake/cache.py

```diff
@@ -20,15 +20,15 @@
 import logging
 import pathlib
 import typing
 
 import pandas
 from forml import setup
 
-DIR = setup.USRDIR / 'openlake'
+DIR = setup.USRDIR / '.cache' / 'openlake'
 
 LOGGER = logging.getLogger(__name__)
 
 
 def dataframe(
     key: str, loader: typing.Callable[[], pandas.DataFrame], cachedir: pathlib.Path = DIR
 ) -> pandas.DataFrame:
```

## openlake/provider/kaggle.py

```diff
@@ -16,14 +16,15 @@
 # under the License.
 """
 Kaggle datasets providers.
 """
 import abc
 import collections
 import functools
+import logging
 import os
 import pathlib
 import typing
 
 import forml
 from forml import setup
 from forml.io import dsl
@@ -33,14 +34,17 @@
 
 try:
     import kaggle
 except Exception as err:  # pylint: disable=broad-except
     kaggle = provider.Unavailable('kaggle', err)
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 class Partition(provider.Partition, collections.namedtuple('Partition', 'columns, filename')):
     """Kaggle data partition representation."""
 
     columns: tuple[dsl.Column]
     filename: str
 
     def __new__(cls, columns: typing.Sequence[dsl.Column], filename: str):
@@ -63,16 +67,17 @@
         columns = set(columns)
         for partition in self.PARTITIONS:
             if columns.issubset(partition.columns):
                 return tuple([partition])
         raise forml.MissingError('No partition satisfy the column requirement')
 
     def fetch(self, partition: typing.Optional[Partition]) -> typing.IO:
+        LOGGER.info('Fetching %s from %s', partition.filename, self.COMPETITION)
         kaggle.api.competition_download_file(self.COMPETITION, partition.filename, setup.tmpdir, force=True, quiet=True)
-        return open(os.path.join(setup.tmpdir, partition.filename), encoding='utf8')
+        return open(os.path.join(setup.tmpdir, partition.filename), 'rb')
 
 
 class Titanic(File, parser.CSV, provider.Origin):
     """Titanic dataset."""
 
     COMPETITION = 'titanic'
     PARTITIONS = (
@@ -94,7 +99,49 @@
         ),  # Testset partition
         Partition(schema.Titanic.features, 'train.csv'),  # Trainset partition
     )
 
     @property
     def source(self) -> dsl.Source:
         return schema.Titanic
+
+
+class Avazu(File, parser.CSV, provider.Origin):
+    """Avazu dataset."""
+
+    COMPETITION = 'avazu-ctr-prediction'
+    PARTITIONS = (
+        Partition(
+            (
+                schema.Avazu.id,
+                schema.Avazu.hour,
+                schema.Avazu.C1,
+                schema.Avazu.banner_pos,
+                schema.Avazu.site_id,
+                schema.Avazu.site_domain,
+                schema.Avazu.site_category,
+                schema.Avazu.app_id,
+                schema.Avazu.app_domain,
+                schema.Avazu.app_category,
+                schema.Avazu.device_id,
+                schema.Avazu.device_ip,
+                schema.Avazu.device_model,
+                schema.Avazu.device_type,
+                schema.Avazu.device_conn_type,
+                schema.Avazu.C14,
+                schema.Avazu.C15,
+                schema.Avazu.C16,
+                schema.Avazu.C17,
+                schema.Avazu.C18,
+                schema.Avazu.C19,
+                schema.Avazu.C20,
+                schema.Avazu.C21,
+            ),
+            'test.gz',
+        ),  # Testset partition
+        Partition(schema.Avazu.features, 'train.gz'),  # Trainset partition
+    )
+    CSV_PARAMS = {'compression': 'gzip'}
+
+    @property
+    def source(self) -> dsl.Source:
+        return schema.Avazu
```

## Comparing `openlake-0.4.dev1.dist-info/METADATA` & `openlake-0.5.dev1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: openlake
-Version: 0.4.dev1
+Version: 0.5.dev1
 Summary: Public dataset feed.
 Project-URL: Source, https://github.com/formlio/openlake/
 Project-URL: Documentation, https://openlake.readthedocs.io/
 Project-URL: Issues, https://github.com/formlio/openlake/issues/
 Maintainer-email: ForML Development Team <info@forml.io>
 License: Apache License 2.0
+License-File: LICENSE
+License-File: NOTICE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3
 Requires-Dist: forml[sql]
 Requires-Dist: openschema
-Requires-Dist: pandas
-Requires-Dist: pyarrow
+Requires-Dist: pandas[parquet]
 Requires-Dist: sqlalchemy
 Provides-Extra: all
 Requires-Dist: openlake[kaggle,sklearn]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8-bugbear; extra == 'dev'
 Requires-Dist: flake8-colors; extra == 'dev'
@@ -66,15 +67,15 @@
  specific language governing permissions and limitations
  under the License.
 -->
 
 Openlake
 ========
 
-[![GitHub Build](https://img.shields.io/github/workflow/status/formlio/openlake/CI%20Build/main)](https://github.com/formlio/openlake/actions/)
+[![GitHub Build](https://img.shields.io/github/actions/workflow/status/formlio/openlake/ci.yml?branch=main)](https://github.com/formlio/openlake/actions/)
 
 [![Documentation Status](https://readthedocs.org/projects/openlake/badge/?version=latest)](https://openlake.readthedocs.io/en/latest/)
 [![License](https://img.shields.io/pypi/l/openlake)](http://www.apache.org/licenses/LICENSE-2.0.txt)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/openlake)
 [![PyPI Version](https://img.shields.io/pypi/v/openlake)](https://pypi.org/project/openlake/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/openlake)](https://pypi.org/project/openlake/)
```

## Comparing `openlake-0.4.dev1.dist-info/licenses/LICENSE` & `openlake-0.5.dev1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

