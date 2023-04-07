# Comparing `tmp/ecnet-4.1.0.tar.gz` & `tmp/ecnet-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecnet-4.1.0.tar", last modified: Wed Jun 30 17:34:44 2021, max compression
+gzip compressed data, was "ecnet-4.1.1.tar", last modified: Fri Apr  7 21:11:10 2023, max compression
```

## Comparing `ecnet-4.1.0.tar` & `ecnet-4.1.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.072173 ecnet-4.1.0/
--rw-r--r--   0 tjkessler   (501) staff       (20)      267 2021-06-30 17:34:44.072023 ecnet-4.1.0/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     2811 2021-04-30 18:04:56.000000 ecnet-4.1.0/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.066717 ecnet-4.1.0/ecnet/
--rw-r--r--   0 tjkessler   (501) staff       (20)       47 2021-06-30 17:34:27.000000 ecnet-4.1.0/ecnet/__init__.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.068036 ecnet-4.1.0/ecnet/blends/
--rw-r--r--   0 tjkessler   (501) staff       (20)      189 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/blends/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     3690 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/blends/equations.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     3596 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/blends/predict.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     5232 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/callbacks.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.068566 ecnet-4.1.0/ecnet/datasets/
--rw-r--r--   0 tjkessler   (501) staff       (20)      198 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/__init__.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.071497 ecnet-4.1.0/ecnet/datasets/data/
--rw-r--r--   0 tjkessler   (501) staff       (20)     2873 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/bp.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)      985 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/bp.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     8824 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/cn.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     1712 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/cn.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     1399 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/cp.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)      173 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/cp.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     2686 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/kv.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     1465 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/kv.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     4615 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/lhv.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     1163 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/lhv.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     4018 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/mon.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     1466 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/mon.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     2229 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/mp.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)      866 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/mp.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     2075 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/pp.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)      159 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/pp.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     4018 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/ron.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     1543 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/ron.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     8191 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/ysi.smiles
--rw-r--r--   0 tjkessler   (501) staff       (20)     2851 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/data/ysi.target
--rw-r--r--   0 tjkessler   (501) staff       (20)     9443 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/load_data.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     5463 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/structs.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2261 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/datasets/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    10478 2021-06-30 17:34:27.000000 ecnet-4.1.0/ecnet/model.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.071858 ecnet-4.1.0/ecnet/tasks/
--rw-r--r--   0 tjkessler   (501) staff       (20)      161 2021-06-30 17:34:27.000000 ecnet-4.1.0/ecnet/tasks/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     1425 2021-04-30 18:04:56.000000 ecnet-4.1.0/ecnet/tasks/feature_selection.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    10850 2021-06-30 17:34:27.000000 ecnet-4.1.0/ecnet/tasks/parameter_tuning.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-06-30 17:34:44.067445 ecnet-4.1.0/ecnet.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)      267 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     1119 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       67 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        6 2021-06-30 17:34:44.000000 ecnet-4.1.0/ecnet.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2021-06-30 17:34:44.072219 ecnet-4.1.0/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      585 2021-06-30 17:34:27.000000 ecnet-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.290615 ecnet-4.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-07 20:45:50.000000 ecnet-4.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      263 2023-04-07 21:11:10.290615 ecnet-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2797 2023-04-07 21:09:42.000000 ecnet-4.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.153180 ecnet-4.1.1/ecnet/
+-rw-rw-rw-   0        0        0       47 2023-04-07 21:09:44.000000 ecnet-4.1.1/ecnet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.178637 ecnet-4.1.1/ecnet/blends/
+-rw-rw-rw-   0        0        0      189 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/equations.py
+-rw-rw-rw-   0        0        0     3596 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/blends/predict.py
+-rw-rw-rw-   0        0        0     5232 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.182637 ecnet-4.1.1/ecnet/datasets/
+-rw-rw-rw-   0        0        0      198 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.286615 ecnet-4.1.1/ecnet/datasets/data/
+-rw-rw-rw-   0        0        0     2873 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/bp.smiles
+-rw-rw-rw-   0        0        0      985 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/bp.target
+-rw-rw-rw-   0        0        0     8824 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cn.smiles
+-rw-rw-rw-   0        0        0     1712 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cn.target
+-rw-rw-rw-   0        0        0     1399 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cp.smiles
+-rw-rw-rw-   0        0        0      173 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/cp.target
+-rw-rw-rw-   0        0        0     2686 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/kv.smiles
+-rw-rw-rw-   0        0        0     1465 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/kv.target
+-rw-rw-rw-   0        0        0     4615 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/lhv.smiles
+-rw-rw-rw-   0        0        0     1163 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/lhv.target
+-rw-rw-rw-   0        0        0     4018 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mon.smiles
+-rw-rw-rw-   0        0        0     1466 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mon.target
+-rw-rw-rw-   0        0        0     2229 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mp.smiles
+-rw-rw-rw-   0        0        0      866 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/mp.target
+-rw-rw-rw-   0        0        0     2075 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/pp.smiles
+-rw-rw-rw-   0        0        0      159 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/pp.target
+-rw-rw-rw-   0        0        0     4018 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ron.smiles
+-rw-rw-rw-   0        0        0     1543 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ron.target
+-rw-rw-rw-   0        0        0     8191 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ysi.smiles
+-rw-rw-rw-   0        0        0     2851 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/data/ysi.target
+-rw-rw-rw-   0        0        0     9443 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/load_data.py
+-rw-rw-rw-   0        0        0     7120 2023-04-07 21:09:44.000000 ecnet-4.1.1/ecnet/datasets/structs.py
+-rw-rw-rw-   0        0        0     2261 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/datasets/utils.py
+-rw-rw-rw-   0        0        0    10478 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/model.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.289615 ecnet-4.1.1/ecnet/tasks/
+-rw-rw-rw-   0        0        0      161 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/__init__.py
+-rw-rw-rw-   0        0        0     1425 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/feature_selection.py
+-rw-rw-rw-   0        0        0    10850 2023-04-07 20:45:50.000000 ecnet-4.1.1/ecnet/tasks/parameter_tuning.py
+drwxrwxrwx   0        0        0        0 2023-04-07 21:11:10.175635 ecnet-4.1.1/ecnet.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       80 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-07 21:11:10.000000 ecnet-4.1.1/ecnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 21:11:10.290615 ecnet-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      598 2023-04-07 21:09:44.000000 ecnet-4.1.1/setup.py
```

### Comparing `ecnet-4.1.0/README.md` & `ecnet-4.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![UML Energy & Combustion Research Laboratory](http://faculty.uml.edu/Hunter_Mack/uploads/9/7/1/3/97138798/1481826668_2.png)](http://faculty.uml.edu/Hunter_Mack/)
+[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
 
 # ECNet: machine learning models for fuel property prediction
 
 [![GitHub version](https://badge.fury.io/gh/ecrl%2FECNet.svg)](https://badge.fury.io/gh/ecrl%2FECNet)
 [![PyPI version](https://badge.fury.io/py/ecnet.svg)](https://badge.fury.io/py/ecnet)
 [![status](http://joss.theoj.org/papers/f556afbc97e18e1c1294d98e0f7ff99f/status.svg)](http://joss.theoj.org/papers/f556afbc97e18e1c1294d98e0f7ff99f)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ECRL/ECNet/master/LICENSE.txt)
```

### Comparing `ecnet-4.1.0/ecnet/blends/equations.py` & `ecnet-4.1.1/ecnet/blends/equations.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/blends/predict.py` & `ecnet-4.1.1/ecnet/blends/predict.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/callbacks.py` & `ecnet-4.1.1/ecnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/bp.smiles` & `ecnet-4.1.1/ecnet/datasets/data/bp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/bp.target` & `ecnet-4.1.1/ecnet/datasets/data/bp.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/cn.smiles` & `ecnet-4.1.1/ecnet/datasets/data/cn.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/cn.target` & `ecnet-4.1.1/ecnet/datasets/data/cn.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/kv.smiles` & `ecnet-4.1.1/ecnet/datasets/data/kv.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/kv.target` & `ecnet-4.1.1/ecnet/datasets/data/kv.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/lhv.smiles` & `ecnet-4.1.1/ecnet/datasets/data/lhv.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/lhv.target` & `ecnet-4.1.1/ecnet/datasets/data/lhv.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/mon.smiles` & `ecnet-4.1.1/ecnet/datasets/data/mon.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/mon.target` & `ecnet-4.1.1/ecnet/datasets/data/mon.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/mp.smiles` & `ecnet-4.1.1/ecnet/datasets/data/mp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/mp.target` & `ecnet-4.1.1/ecnet/datasets/data/mp.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/pp.smiles` & `ecnet-4.1.1/ecnet/datasets/data/pp.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/ron.smiles` & `ecnet-4.1.1/ecnet/datasets/data/ron.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/ron.target` & `ecnet-4.1.1/ecnet/datasets/data/ron.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/ysi.smiles` & `ecnet-4.1.1/ecnet/datasets/data/ysi.smiles`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/data/ysi.target` & `ecnet-4.1.1/ecnet/datasets/data/ysi.target`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/load_data.py` & `ecnet-4.1.1/ecnet/datasets/load_data.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/datasets/structs.py` & `ecnet-4.1.1/ecnet/datasets/structs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 r"""PyTorch-iterable/callable data structures"""
 from typing import List, Tuple, Iterable
 import torch
 from torch.utils.data import Dataset
+from sklearn.decomposition import PCA
 
 from .utils import _qspr_from_padel, _qspr_from_alvadesc,\
     _qspr_from_alvadesc_smifile
 
 
 class QSPRDataset(Dataset):
 
@@ -17,17 +18,17 @@
         Args:
             smiles (list[str]): SMILES strings
             target_vals (Iterable[Iterable[float]]): target values of shape (n_samples, n_targets)
             backend (str, optional): backend for QSPR generation, ['padel', 'alvadesc']
         """
 
         self.smiles = smiles
-        self.target_vals = torch.as_tensor(target_vals)
+        self.target_vals = torch.as_tensor(target_vals).type(torch.float32)
         self.desc_vals, self.desc_names = self.smi_to_qspr(smiles, backend)
-        self.desc_vals = torch.as_tensor(self.desc_vals)
+        self.desc_vals = torch.as_tensor(self.desc_vals).type(torch.float32)
 
     @staticmethod
     def smi_to_qspr(smiles: List[str], backend: str) -> Tuple[List[List[float]], List[str]]:
         """
         Generate QSPR descriptors for each supplied SMILES string
 
         Args:
@@ -106,25 +107,25 @@
         Args:
             smiles_fn (str): filename/path of SMILES file
             target_vals (Iterable[Iterable[float]]): target values of shape (n_samples, n_targets)
             backend (str, optional): backend for QSPR generation, ['padel', 'alvadesc']
         """
 
         self.smiles = self._open_smiles_file(smiles_fn)
-        self.target_vals = torch.as_tensor(target_vals)
+        self.target_vals = torch.as_tensor(target_vals).type(torch.float32)
         if backend == 'padel':
             self.desc_vals, self.desc_names = self.smi_to_qspr(
                 self.smiles, backend
             )
-            self.desc_vals = torch.as_tensor(self.desc_vals)
+            self.desc_vals = torch.as_tensor(self.desc_vals).type(torch.float32)
         elif backend == 'alvadesc':
             self.desc_vals, self.desc_names = _qspr_from_alvadesc_smifile(
                 smiles_fn
             )
-            self.desc_vals = torch.as_tensor(self.desc_vals)
+            self.desc_vals = torch.as_tensor(self.desc_vals).type(torch.float32)
 
     @staticmethod
     def _open_smiles_file(smiles_fn: str) -> List[str]:
         """
         Open SMILES file at specified location
 
         Args:
@@ -152,9 +153,39 @@
         Args:
             desc_vals (Iterable[Iterable[float]]): descriptor values, shape (n_samples, n_features)
             target_vals (Iterable[Iterable[float]]): target values, shape (n_samples, n_targets)
         """
 
         self.smiles = ['' for _ in range(len(target_vals))]
         self.desc_names = ['' for _ in range(len(desc_vals[0]))]
-        self.desc_vals = torch.as_tensor(desc_vals)
-        self.target_vals = torch.as_tensor(target_vals)
+        self.desc_vals = torch.as_tensor(desc_vals).type(torch.float32)
+        self.target_vals = torch.as_tensor(target_vals).type(torch.float32)
+
+
+class PCADataset(QSPRDataset):
+
+    def __init__(self, smiles: List[str], target_vals: Iterable[Iterable[float]],
+                 backend: str = 'padel', existing_pca_dataset: 'PCADataset' = None):
+        """
+        PCADataset: creates a torch.utils.data.Dataset given supplied SMILES strings, supplied
+        target values; first generates QSPR descriptors, then transforms them via PCA; an existing
+        PCADataset can be supplied to peform PCA transformation
+
+        Args:
+            smiles (list[str]): SMILES strings
+            target_vals (Iterable[Iterable[float]]): target values of shape (n_samples, n_targets)
+            backend (str, optional): backend for QSPR generation, ['padel', 'alvadesc']
+            existing_pca_dataset (PCADataset, optional): if PCA already trained (e.g. trained
+                using training set, want to use for testing set), the pre-trained PCA can be used
+                to perform PCA for this data
+        """
+
+        self.smiles = smiles
+        self.target_vals = torch.as_tensor(target_vals).type(torch.float32)
+        self.desc_names = None
+        desc_vals, _ = self.smi_to_qspr(smiles, backend)
+        if existing_pca_dataset is None:
+            self.pca = PCA(n_components=min(desc_vals.shape[0], desc_vals.shape[1]))
+            self.pca.fit(desc_vals)
+        else:
+            self.pca = existing_pca_dataset.pca
+        self.desc_vals = torch.as_tensor(self.pca.transform(desc_vals)).type(torch.float32)
```

### Comparing `ecnet-4.1.0/ecnet/datasets/utils.py` & `ecnet-4.1.1/ecnet/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/model.py` & `ecnet-4.1.1/ecnet/model.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/tasks/feature_selection.py` & `ecnet-4.1.1/ecnet/tasks/feature_selection.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet/tasks/parameter_tuning.py` & `ecnet-4.1.1/ecnet/tasks/parameter_tuning.py`

 * *Files identical despite different names*

### Comparing `ecnet-4.1.0/ecnet.egg-info/SOURCES.txt` & `ecnet-4.1.1/ecnet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 ecnet/__init__.py
 ecnet/callbacks.py
 ecnet/model.py
 ecnet.egg-info/PKG-INFO
 ecnet.egg-info/SOURCES.txt
```

### Comparing `ecnet-4.1.0/setup.py` & `ecnet-4.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(
     name='ecnet',
-    version='4.1.0',
+    version='4.1.1',
     description='Fuel property prediction using QSPR descriptors',
     url='https://github.com/ecrl/ecnet',
     author='Travis Kessler',
     author_email='Travis_Kessler@student.uml.edu',
     license='MIT',
     packages=find_packages(),
     install_requires=[
-        'torch==1.8.0',
-        'sklearn',
-        'padelpy==0.1.9',
+        'torch==2.0.0',
+        'scikit-learn==1.2.2',
+        'padelpy==0.1.13',
         'alvadescpy==0.1.2',
         'ecabc==3.0.0'
     ],
     package_data={
         'ecnet': [
             'datasets/data/*'
         ]
```

