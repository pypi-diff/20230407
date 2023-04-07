# Comparing `tmp/openschema-0.5.dev1-py3-none-any.whl.zip` & `tmp/openschema-0.6.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 13451 bytes, number of entries: 11
+Zip file size: 14645 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      836 b- defN 20-Feb-02 00:00 openschema/__init__.py
--rw-r--r--  2.0 unx      909 b- defN 20-Feb-02 00:00 openschema/kaggle/__init__.py
+-rw-r--r--  2.0 unx      944 b- defN 20-Feb-02 00:00 openschema/kaggle/__init__.py
+-rw-r--r--  2.0 unx     3067 b- defN 20-Feb-02 00:00 openschema/kaggle/_avazu.py
 -rw-r--r--  2.0 unx     2732 b- defN 20-Feb-02 00:00 openschema/kaggle/_titanic.py
 -rw-r--r--  2.0 unx     1010 b- defN 20-Feb-02 00:00 openschema/sklearn/__init__.py
 -rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 openschema/sklearn/_breast_cancer.py
 -rw-r--r--  2.0 unx     2458 b- defN 20-Feb-02 00:00 openschema/sklearn/_iris.py
-?rw-r--r--  2.0 unx     3729 b- defN 20-Feb-02 00:00 openschema-0.5.dev1.dist-info/METADATA
-?rw-r--r--  2.0 unx       86 b- defN 20-Feb-02 00:00 openschema-0.5.dev1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.5.dev1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.5.dev1.dist-info/licenses/NOTICE
-?rw-r--r--  2.0 unx      942 b- defN 20-Feb-02 00:00 openschema-0.5.dev1.dist-info/RECORD
-11 files, 30952 bytes uncompressed, 11847 bytes compressed:  61.7%
+?rw-r--r--  2.0 unx     3783 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11358 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      124 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/licenses/NOTICE
+?rw-r--r--  2.0 unx     1026 b- defN 20-Feb-02 00:00 openschema-0.6.dev1.dist-info/RECORD
+12 files, 34193 bytes uncompressed, 12911 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
 Filename: openschema/__init__.py
 Comment: 
 
 Filename: openschema/kaggle/__init__.py
 Comment: 
 
+Filename: openschema/kaggle/_avazu.py
+Comment: 
+
 Filename: openschema/kaggle/_titanic.py
 Comment: 
 
 Filename: openschema/sklearn/__init__.py
 Comment: 
 
 Filename: openschema/sklearn/_breast_cancer.py
 Comment: 
 
 Filename: openschema/sklearn/_iris.py
 Comment: 
 
-Filename: openschema-0.5.dev1.dist-info/METADATA
+Filename: openschema-0.6.dev1.dist-info/METADATA
 Comment: 
 
-Filename: openschema-0.5.dev1.dist-info/WHEEL
+Filename: openschema-0.6.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: openschema-0.5.dev1.dist-info/licenses/LICENSE
+Filename: openschema-0.6.dev1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: openschema-0.5.dev1.dist-info/licenses/NOTICE
+Filename: openschema-0.6.dev1.dist-info/licenses/NOTICE
 Comment: 
 
-Filename: openschema-0.5.dev1.dist-info/RECORD
+Filename: openschema-0.6.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openschema/__init__.py

```diff
@@ -15,8 +15,8 @@
 # specific language governing permissions and limitations
 # under the License.
 
 """
 Schema catalog.
 """
 
-__version__ = '0.5.dev1'
+__version__ = '0.6.dev1'
```

## openschema/kaggle/__init__.py

```diff
@@ -15,10 +15,11 @@
 # specific language governing permissions and limitations
 # under the License.
 
 """
 `Kaggle <https://www.kaggle.com/>`_ datasets schema catalog.
 """
 
+from ._avazu import Avazu
 from ._titanic import Titanic
 
-__all__ = ['Titanic']
+__all__ = ['Avazu', 'Titanic']
```

## Comparing `openschema-0.5.dev1.dist-info/METADATA` & `openschema-0.6.dev1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: openschema
-Version: 0.5.dev1
+Version: 0.6.dev1
 Summary: Programmatic catalog of public dataset schemas.
 Project-URL: Source, https://github.com/formlio/openschema/
 Project-URL: Documentation, https://openschema.readthedocs.io/
 Project-URL: Issues, https://github.com/formlio/openschema/issues/
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
@@ -61,15 +63,15 @@
  specific language governing permissions and limitations
  under the License.
 -->
 
 Openschema
 ==========
 
-[![GitHub Build](https://img.shields.io/github/workflow/status/formlio/openschema/CI%20Build/main)](https://github.com/formlio/openschema/actions/)
+[![GitHub Build](https://img.shields.io/github/actions/workflow/status/formlio/openschema/ci.yml?branch=main)](https://github.com/formlio/openschema/actions/)
 
 [![Documentation Status](https://readthedocs.org/projects/openschema/badge/?version=latest)](https://openschema.readthedocs.io/en/latest/)
 [![License](https://img.shields.io/pypi/l/openschema)](http://www.apache.org/licenses/LICENSE-2.0.txt)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/openschema)
 [![PyPI Version](https://img.shields.io/pypi/v/openschema)](https://pypi.org/project/openschema/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/openschema)](https://pypi.org/project/openschema/)
```

## Comparing `openschema-0.5.dev1.dist-info/licenses/LICENSE` & `openschema-0.6.dev1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `openschema-0.5.dev1.dist-info/RECORD` & `openschema-0.6.dev1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-openschema/__init__.py,sha256=bGYAK-zerIZfrnSEIFncS8tmZJtire-LXGh2G70l29o,836
-openschema/kaggle/__init__.py,sha256=Fa3b0M-xRhPj77DRaUH2rhAWtCiQDhkB4OXxYO-kscU,909
+openschema/__init__.py,sha256=fyar--jNiw0TPXVc4o3pFSZmX_xJvilAlc8rkeAhQcw,836
+openschema/kaggle/__init__.py,sha256=wGr9J5JWX7EZvJNrAW9zcD0vEFBKQ8O4ZbIzG5xHQbs,944
+openschema/kaggle/_avazu.py,sha256=QjI6YUQEzoxeHj-zXx2hJofs7KonHPpWQY5j-khAC3w,3067
 openschema/kaggle/_titanic.py,sha256=d43oRYDq-VXvEpqnaZe9ugUEvT_UPNBArq2gjZi-zBE,2732
 openschema/sklearn/__init__.py,sha256=NVfnTf6KWexY35GPauRsquV2EDJqutQR4yiaFRkUeGU,1010
 openschema/sklearn/_breast_cancer.py,sha256=20GHdNMBiFRrXfyRD7JZqmI8mHGwh59XVVuc7v9NSSU,6768
 openschema/sklearn/_iris.py,sha256=7tzpnlR1aB2mlRGtNjGkKmASi3NXpg86ew3NZHTN7eQ,2458
-openschema-0.5.dev1.dist-info/METADATA,sha256=WBTKQExWAChtpDMg1HalRwtlD3unPUSCUF6JL6FAFEs,3729
-openschema-0.5.dev1.dist-info/WHEEL,sha256=09RFlvY3aVzvCNk4AXPZt-N-AI7GY_KktGsTb2IqIBU,86
-openschema-0.5.dev1.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-openschema-0.5.dev1.dist-info/licenses/NOTICE,sha256=T6XsijfZh4z6h1yyQg-V8-6B5wRvdcFgOOf-dRrPRoE,124
-openschema-0.5.dev1.dist-info/RECORD,,
+openschema-0.6.dev1.dist-info/METADATA,sha256=zN1YAyDsN68eJ_TFZGnJ9cjb9lvfCXt1_Qdl_IvS6p8,3783
+openschema-0.6.dev1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
+openschema-0.6.dev1.dist-info/licenses/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+openschema-0.6.dev1.dist-info/licenses/NOTICE,sha256=T6XsijfZh4z6h1yyQg-V8-6B5wRvdcFgOOf-dRrPRoE,124
+openschema-0.6.dev1.dist-info/RECORD,,
```

