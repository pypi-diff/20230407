# Comparing `tmp/PyPDFForm-1.2.4.tar.gz` & `tmp/PyPDFForm-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.4.tar", last modified: Thu Feb 23 00:39:19 2023, max compression
+gzip compressed data, was "PyPDFForm-1.2.5.tar", last modified: Fri Apr  7 18:49:55 2023, max compression
```

## Comparing `PyPDFForm-1.2.4.tar` & `PyPDFForm-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:39:19.015204 PyPDFForm-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-02-23 00:39:19.015204 PyPDFForm-1.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:39:19.011204 PyPDFForm-1.2.4/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:39:19.015204 PyPDFForm-1.2.4/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:39:19.015204 PyPDFForm-1.2.4/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 00:39:19.011204 PyPDFForm-1.2.4/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-02-23 00:39:18.000000 PyPDFForm-1.2.4/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-23 00:39:18.000000 PyPDFForm-1.2.4/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 00:39:18.000000 PyPDFForm-1.2.4/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 00:39:18.000000 PyPDFForm-1.2.4/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-23 00:39:18.000000 PyPDFForm-1.2.4/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 00:39:19.015204 PyPDFForm-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-23 00:38:59.000000 PyPDFForm-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 18:49:55.000000 PyPDFForm-1.2.5/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:49:55.382804 PyPDFForm-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 18:49:46.000000 PyPDFForm-1.2.5/setup.py
```

### Comparing `PyPDFForm-1.2.4/LICENSE` & `PyPDFForm-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PKG-INFO` & `PyPDFForm-1.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 5079 5044  : 2.1.Name: PyPD
 00000020: 4646 6f72 6d0a 5665 7273 696f 6e3a 2031  FForm.Version: 1
-00000030: 2e32 2e34 0a53 756d 6d61 7279 3a20 5468  .2.4.Summary: Th
+00000030: 2e32 2e35 0a53 756d 6d61 7279 3a20 5468  .2.5.Summary: Th
 00000040: 6520 5079 7468 6f6e 206c 6962 7261 7279  e Python library
 00000050: 2066 6f72 2050 4446 2066 6f72 6d73 2e0a   for PDF forms..
 00000060: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000070: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
 00000080: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
 00000090: 4646 6f72 6d0a 4175 7468 6f72 3a20 4a69  FForm.Author: Ji
 000000a0: 6e67 6520 4c69 0a43 6c61 7373 6966 6965  nge Li.Classifie
@@ -18,180 +18,214 @@
 00000110: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
 00000120: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 00000130: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
 00000140: 732d 5079 7468 6f6e 3a20 3e3d 332e 370a  s-Python: >=3.7.
 00000150: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000160: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 00000170: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
-00000180: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
-00000190: 2050 7950 4446 466f 726d 2021 5b63 6f64   PyPDFForm ![cod
-000001a0: 6520 666f 726d 6174 7469 6e67 5d28 6874  e formatting](ht
-000001b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000001c0: 2f63 6869 6e61 7061 6e64 616d 616e 2f50  /chinapandaman/P
-000001d0: 7950 4446 466f 726d 2f61 6374 696f 6e73  yPDFForm/actions
-000001e0: 2f77 6f72 6b66 6c6f 7773 2f70 7974 686f  /workflows/pytho
-000001f0: 6e2d 626c 6163 6b2d 6973 6f72 742e 796d  n-black-isort.ym
-00000200: 6c2f 6261 6467 652e 7376 6729 2021 5b74  l/badge.svg) ![t
-00000210: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
-00000220: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
-00000230: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
-00000240: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000250: 7773 2f70 7974 686f 6e2d 7061 636b 6167  ws/python-packag
-00000260: 652e 796d 6c2f 6261 6467 652e 7376 6729  e.yml/badge.svg)
-00000270: 205b 215b 636f 6465 636f 765d 2868 7474   [![codecov](htt
-00000280: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000290: 6768 2f63 6869 6e61 7061 6e64 616d 616e  gh/chinapandaman
-000002a0: 2f50 7950 4446 466f 726d 2f62 7261 6e63  /PyPDFForm/branc
-000002b0: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
-000002c0: 6164 6765 2e73 7667 3f74 6f6b 656e 3d43  adge.svg?token=C
-000002d0: 5352 4c4e 3134 4946 4529 5d28 6874 7470  SRLN14IFE)](http
-000002e0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-000002f0: 682f 6368 696e 6170 616e 6461 6d61 6e2f  h/chinapandaman/
-00000300: 5079 5044 4646 6f72 6d29 2021 5b64 6570  PyPDFForm) ![dep
-00000310: 6c6f 795d 2868 7474 7073 3a2f 2f67 6974  loy](https://git
-00000320: 6875 622e 636f 6d2f 6368 696e 6170 616e  hub.com/chinapan
-00000330: 6461 6d61 6e2f 5079 5044 4646 6f72 6d2f  daman/PyPDFForm/
-00000340: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000350: 732f 7079 7468 6f6e 2d70 7562 6c69 7368  s/python-publish
-00000360: 2e79 6d6c 2f62 6164 6765 2e73 7667 290a  .yml/badge.svg).
-00000370: 0a50 7950 4446 466f 726d 2069 7320 6120  .PyPDFForm is a 
-00000380: 7075 7265 2050 7974 686f 6e20 6c69 6272  pure Python libr
-00000390: 6172 7920 666f 7220 5044 4620 666f 726d  ary for PDF form
-000003a0: 2070 726f 6365 7373 696e 672e 200a 4974   processing. .It
-000003b0: 2061 6c6c 6f77 7320 6669 6c6c 696e 6720   allows filling 
-000003c0: 6120 5044 4620 666f 726d 2070 726f 6772  a PDF form progr
-000003d0: 616d 6d61 7469 6361 6c6c 7920 6279 2063  ammatically by c
-000003e0: 7265 6174 696e 6720 0a61 2050 7974 686f  reating .a Pytho
-000003f0: 6e20 6469 6374 696f 6e61 7279 2077 6974  n dictionary wit
-00000400: 6820 6b65 7973 206d 6174 6368 696e 6720  h keys matching 
-00000410: 6974 7320 616e 6e6f 7461 7465 6420 6e61  its annotated na
-00000420: 6d65 7320 0a66 6f72 2065 6c65 6d65 6e74  mes .for element
-00000430: 7320 6c69 6b65 2074 6578 7420 6669 656c  s like text fiel
-00000440: 6473 2061 6e64 2063 6865 636b 626f 7865  ds and checkboxe
-00000450: 732e 2049 7420 616c 736f 2073 7570 706f  s. It also suppo
-00000460: 7274 7320 6f74 6865 7220 6675 6e63 7469  rts other functi
-00000470: 6f6e 616c 6974 6965 7320 7375 6368 2061  onalities such a
-00000480: 7320 0a64 7261 7769 6e67 2069 6d61 6765  s .drawing image
-00000490: 2061 6e64 206d 6572 6769 6e67 206d 756c   and merging mul
-000004a0: 7469 706c 6520 5044 4673 2074 6f67 6574  tiple PDFs toget
-000004b0: 6865 722e 0a0a 2323 2049 6e73 7461 6c6c  her...## Install
-000004c0: 696e 670a 0a49 6e73 7461 6c6c 2075 7369  ing..Install usi
-000004d0: 6e67 205b 7069 705d 2868 7474 7073 3a2f  ng [pip](https:/
-000004e0: 2f70 6970 2e70 7970 612e 696f 2f65 6e2f  /pip.pypa.io/en/
-000004f0: 7374 6162 6c65 2f29 3a0a 0a60 6060 7368  stable/):..```sh
-00000500: 656c 6c20 7363 7269 7074 0a70 6970 2069  ell script.pip i
-00000510: 6e73 7461 6c6c 2050 7950 4446 466f 726d  nstall PyPDFForm
-00000520: 0a60 6060 0a0a 2323 2051 7569 636b 2045  .```..## Quick E
-00000530: 7861 6d70 6c65 0a0a 4120 7361 6d70 6c65  xample..A sample
-00000540: 2050 4446 2066 6f72 6d20 6361 6e20 6265   PDF form can be
-00000550: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
-00000560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000570: 2f63 6869 6e61 7061 6e64 616d 616e 2f50  /chinapandaman/P
-00000580: 7950 4446 466f 726d 2f62 6c6f 622f 6d61  yPDFForm/blob/ma
-00000590: 7374 6572 2f70 6466 5f73 616d 706c 6573  ster/pdf_samples
-000005a0: 2f73 616d 706c 655f 7465 6d70 6c61 7465  /sample_template
-000005b0: 2e70 6466 292e 2044 6f77 6e6c 6f61 6420  .pdf). Download 
-000005c0: 6974 2061 6e64 2074 7279 3a0a 0a60 6060  it and try:..```
-000005d0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f73  python.import os
-000005e0: 0a0a 6672 6f6d 2050 7950 4446 466f 726d  ..from PyPDFForm
-000005f0: 2069 6d70 6f72 7420 5079 5044 4646 6f72   import PyPDFFor
-00000600: 6d0a 0a50 4154 485f 544f 5f44 4f57 4e4c  m..PATH_TO_DOWNL
-00000610: 4f41 4445 445f 5341 4d50 4c45 5f50 4446  OADED_SAMPLE_PDF
-00000620: 5f46 4f52 4d20 3d20 6f73 2e70 6174 682e  _FORM = os.path.
-00000630: 6a6f 696e 280a 2020 2020 6f73 2e70 6174  join(.    os.pat
-00000640: 682e 6578 7061 6e64 7573 6572 2822 7e2f  h.expanduser("~/
-00000650: 446f 776e 6c6f 6164 7322 292c 2022 7361  Downloads"), "sa
-00000660: 6d70 6c65 5f74 656d 706c 6174 652e 7064  mple_template.pd
-00000670: 6622 0a29 2020 2320 4368 616e 6765 2074  f".)  # Change t
-00000680: 6869 7320 746f 2077 6865 7265 2079 6f75  his to where you
-00000690: 2064 6f77 6e6c 6f61 6465 6420 7468 6520   downloaded the 
-000006a0: 7361 6d70 6c65 2050 4446 2066 6f72 6d0a  sample PDF form.
-000006b0: 0a50 4154 485f 544f 5f46 494c 4c45 445f  .PATH_TO_FILLED_
-000006c0: 5044 465f 464f 524d 203d 206f 732e 7061  PDF_FORM = os.pa
-000006d0: 7468 2e6a 6f69 6e28 0a20 2020 206f 732e  th.join(.    os.
-000006e0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-000006f0: 227e 2229 2c20 226f 7574 7075 742e 7064  "~"), "output.pd
-00000700: 6622 0a29 2020 2320 4368 616e 6765 2074  f".)  # Change t
-00000710: 6869 7320 746f 2077 6865 7265 2079 6f75  his to where you
-00000720: 2077 6973 6820 746f 2070 7574 2079 6f75   wish to put you
-00000730: 7220 6669 6c6c 6564 2050 4446 2066 6f72  r filled PDF for
-00000740: 6d0a 0a77 6974 6820 6f70 656e 2850 4154  m..with open(PAT
-00000750: 485f 544f 5f46 494c 4c45 445f 5044 465f  H_TO_FILLED_PDF_
-00000760: 464f 524d 2c20 2277 622b 2229 2061 7320  FORM, "wb+") as 
-00000770: 6f75 7470 7574 3a0a 2020 2020 6f75 7470  output:.    outp
-00000780: 7574 2e77 7269 7465 280a 2020 2020 2020  ut.write(.      
-00000790: 2020 5079 5044 4646 6f72 6d28 5041 5448    PyPDFForm(PATH
-000007a0: 5f54 4f5f 444f 574e 4c4f 4144 4544 5f53  _TO_DOWNLOADED_S
-000007b0: 414d 504c 455f 5044 465f 464f 524d 290a  AMPLE_PDF_FORM).
-000007c0: 2020 2020 2020 2020 2e66 696c 6c28 0a20          .fill(. 
-000007d0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000007e0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-000007f0: 7374 223a 2022 7465 7374 5f31 222c 0a20  st": "test_1",. 
-00000800: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000810: 6368 6563 6b22 3a20 5472 7565 2c0a 2020  check": True,.  
-00000820: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000830: 6573 745f 3222 3a20 2274 6573 745f 3222  est_2": "test_2"
-00000840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000850: 2020 2263 6865 636b 5f32 223a 2046 616c    "check_2": Fal
-00000860: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00000870: 2020 2020 2274 6573 745f 3322 3a20 2274      "test_3": "t
-00000880: 6573 745f 3322 2c0a 2020 2020 2020 2020  est_3",.        
-00000890: 2020 2020 2020 2020 2263 6865 636b 5f33          "check_3
-000008a0: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-000008b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000008c0: 290a 2020 2020 2020 2020 2e72 6561 6428  ).        .read(
-000008d0: 290a 2020 2020 290a 6060 600a 0a41 6674  ).    ).```..Aft
-000008e0: 6572 2072 756e 6e69 6e67 2074 6865 2061  er running the a
-000008f0: 626f 7665 2063 6f64 6520 736e 6970 7065  bove code snippe
-00000900: 7420 796f 7520 6361 6e20 6669 6e64 2060  t you can find `
-00000910: 6f75 7470 7574 2e70 6466 6020 6174 2074  output.pdf` at t
-00000920: 6865 206c 6f63 6174 696f 6e20 796f 7520  he location you 
-00000930: 7370 6563 6966 6965 642c 200a 616e 6420  specified, .and 
-00000940: 6974 2073 686f 756c 6420 6c6f 6f6b 206c  it should look l
-00000950: 696b 6520 5b74 6869 735d 2868 7474 7073  ike [this](https
-00000960: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
-00000970: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
-00000980: 4646 6f72 6d2f 626c 6f62 2f6d 6173 7465  FForm/blob/maste
-00000990: 722f 7064 665f 7361 6d70 6c65 732f 7361  r/pdf_samples/sa
-000009a0: 6d70 6c65 5f66 696c 6c65 642e 7064 6629  mple_filled.pdf)
-000009b0: 2e0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
-000009c0: 696f 6e0a 0a5b 4578 616d 706c 6573 5d28  ion..[Examples](
-000009d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000009e0: 6f6d 2f63 6869 6e61 7061 6e64 616d 616e  om/chinapandaman
-000009f0: 2f50 7950 4446 466f 726d 2f62 6c6f 622f  /PyPDFForm/blob/
-00000a00: 6d61 7374 6572 2f64 6f63 732f 6578 616d  master/docs/exam
-00000a10: 706c 6573 2e6d 6429 0a0a 2323 2048 6f77  ples.md)..## How
-00000a20: 2074 6f20 436f 6e74 7269 6275 7465 0a0a   to Contribute..
-00000a30: 4966 2079 6f75 2077 6973 6820 746f 2069  If you wish to i
-00000a40: 6d70 726f 7665 2074 6869 7320 6c69 6272  mprove this libr
-00000a50: 6172 792c 2074 6865 7265 2069 7320 6f6e  ary, there is on
-00000a60: 6520 7370 6563 6966 6963 2077 6179 2079  e specific way y
-00000a70: 6f75 2063 616e 2063 6f6e 7472 6962 7574  ou can contribut
-00000a80: 6520 0a6f 6e20 746f 7020 6f66 2074 6865  e .on top of the
-00000a90: 2075 7375 616c 206f 7065 6e20 736f 7572   usual open sour
-00000aa0: 6365 2070 726f 6a65 6374 206e 6f72 6d73  ce project norms
-00000ab0: 2073 7563 6820 6173 2069 7373 7565 7320   such as issues 
-00000ac0: 616e 6420 7075 6c6c 2072 6571 7565 7374  and pull request
-00000ad0: 732e 0a0a 4974 2069 7320 6469 6666 6963  s...It is diffic
-00000ae0: 756c 7420 746f 206d 616b 6520 7375 7265  ult to make sure
-00000af0: 2074 6861 7420 7468 6520 6c69 6272 6172   that the librar
-00000b00: 7920 7375 7070 6f72 7473 2061 6c6c 2074  y supports all t
-00000b10: 6865 2050 4446 2066 6f72 6d20 6372 6561  he PDF form crea
-00000b20: 7469 6e67 2074 6f6f 6c73 206f 7574 200a  ting tools out .
-00000b30: 7468 6572 652e 2053 6f20 6966 2079 6f75  there. So if you
-00000b40: 2072 756e 2069 6e74 6f20 6120 6361 7365   run into a case
-00000b50: 2077 6865 7265 2074 6865 206c 6962 7261   where the libra
-00000b60: 7279 2064 6f65 7320 6e6f 7420 776f 726b  ry does not work
-00000b70: 2066 6f72 2063 6572 7461 696e 2050 4446   for certain PDF
-00000b80: 2066 6f72 6d73 2063 7265 6174 6564 2062   forms created b
-00000b90: 7920 0a63 6572 7461 696e 2074 6f6f 6c73  y .certain tools
-00000ba0: 2c20 6665 656c 2066 7265 6520 746f 206f  , feel free to o
-00000bb0: 7065 6e20 616e 2069 7373 7565 2077 6974  pen an issue wit
-00000bc0: 6820 7468 6520 7072 6f62 6c65 6d61 7469  h the problemati
-00000bd0: 6320 5044 4620 666f 726d 2061 7474 6163  c PDF form attac
-00000be0: 6865 642e 2049 2077 696c 6c20 7365 656b  hed. I will seek
-00000bf0: 200a 746f 206d 616b 6520 7468 6520 6c69   .to make the li
-00000c00: 6272 6172 7920 7375 7070 6f72 7420 7468  brary support th
-00000c10: 6520 6174 7461 6368 6564 2050 4446 2066  e attached PDF f
-00000c20: 6f72 6d20 6173 2077 656c 6c20 6173 2074  orm as well as t
-00000c30: 6865 2074 6f6f 6c20 7573 6564 2074 6f20  he tool used to 
-00000c40: 6372 6561 7465 2069 742e 0a              create it..
+00000180: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+00000190: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000001a0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+000001c0: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+000001d0: 4646 6f72 6d2f 626c 6f62 2f6d 6173 7465  FForm/blob/maste
+000001e0: 722f 6c6f 676f 2e70 6e67 223e 3c2f 703e  r/logo.png"></p>
+000001f0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000200: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
+00000210: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000220: 636f 6d2f 6368 696e 6170 616e 6461 6d61  com/chinapandama
+00000230: 6e2f 5079 5044 4646 6f72 6d2f 6163 7469  n/PyPDFForm/acti
+00000240: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000250: 7468 6f6e 2d62 6c61 636b 2d69 736f 7274  thon-black-isort
+00000260: 2e79 6d6c 2f62 6164 6765 2e73 7667 223e  .yml/badge.svg">
+00000270: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6869  //github.com/chi
+00000290: 6e61 7061 6e64 616d 616e 2f50 7950 4446  napandaman/PyPDF
+000002a0: 466f 726d 2f61 6374 696f 6e73 2f77 6f72  Form/actions/wor
+000002b0: 6b66 6c6f 7773 2f70 7974 686f 6e2d 626c  kflows/python-bl
+000002c0: 6163 6b2d 6973 6f72 742e 796d 6c2f 6261  ack-isort.yml/ba
+000002d0: 6467 652e 7376 6722 3e3c 2f61 3e0a 2020  dge.svg"></a>.  
+000002e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+00000300: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+00000310: 4646 6f72 6d2f 6163 7469 6f6e 732f 776f  FForm/actions/wo
+00000320: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
+00000330: 6163 6b61 6765 2e79 6d6c 2f62 6164 6765  ackage.yml/badge
+00000340: 2e73 7667 223e 3c69 6d67 2073 7263 3d22  .svg"><img src="
+00000350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000360: 6f6d 2f63 6869 6e61 7061 6e64 616d 616e  om/chinapandaman
+00000370: 2f50 7950 4446 466f 726d 2f61 6374 696f  /PyPDFForm/actio
+00000380: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+00000390: 686f 6e2d 7061 636b 6167 652e 796d 6c2f  hon-package.yml/
+000003a0: 6261 6467 652e 7376 6722 3e3c 2f61 3e0a  badge.svg"></a>.
+000003b0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000003c0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+000003d0: 6768 2f63 6869 6e61 7061 6e64 616d 616e  gh/chinapandaman
+000003e0: 2f50 7950 4446 466f 726d 223e 3c69 6d67  /PyPDFForm"><img
+000003f0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+00000400: 6465 636f 762e 696f 2f67 682f 6368 696e  decov.io/gh/chin
+00000410: 6170 616e 6461 6d61 6e2f 5079 5044 4646  apandaman/PyPDFF
+00000420: 6f72 6d2f 6272 616e 6368 2f6d 6173 7465  orm/branch/maste
+00000430: 722f 6772 6170 682f 6261 6467 652e 7376  r/graph/badge.sv
+00000440: 673f 746f 6b65 6e3d 4353 524c 4e31 3449  g?token=CSRLN14I
+00000450: 4645 223e 3c2f 613e 0a20 2020 203c 6120  FE"></a>.    <a 
+00000460: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000470: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
+00000480: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
+00000490: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000004a0: 7773 2f70 7974 686f 6e2d 7075 626c 6973  ws/python-publis
+000004b0: 682e 796d 6c2f 6261 6467 652e 7376 6722  h.yml/badge.svg"
+000004c0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000004d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+000004e0: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+000004f0: 4646 6f72 6d2f 6163 7469 6f6e 732f 776f  FForm/actions/wo
+00000500: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
+00000510: 7562 6c69 7368 2e79 6d6c 2f62 6164 6765  ublish.yml/badge
+00000520: 2e73 7667 223e 3c2f 613e 0a3c 2f70 3e0a  .svg"></a>.</p>.
+00000530: 0a23 2320 496e 7472 6f64 7563 7469 6f6e  .## Introduction
+00000540: 0a0a 5079 5044 4646 6f72 6d20 6973 2061  ..PyPDFForm is a
+00000550: 2070 7572 6520 5079 7468 6f6e 206c 6962   pure Python lib
+00000560: 7261 7279 2066 6f72 2050 4446 2066 6f72  rary for PDF for
+00000570: 6d20 7072 6f63 6573 7369 6e67 2e20 0a49  m processing. .I
+00000580: 7420 616c 6c6f 7773 2066 696c 6c69 6e67  t allows filling
+00000590: 2061 2050 4446 2066 6f72 6d20 7072 6f67   a PDF form prog
+000005a0: 7261 6d6d 6174 6963 616c 6c79 2062 7920  rammatically by 
+000005b0: 6372 6561 7469 6e67 200a 6120 5079 7468  creating .a Pyth
+000005c0: 6f6e 2064 6963 7469 6f6e 6172 7920 7769  on dictionary wi
+000005d0: 7468 206b 6579 7320 6d61 7463 6869 6e67  th keys matching
+000005e0: 2069 7473 2061 6e6e 6f74 6174 6564 206e   its annotated n
+000005f0: 616d 6573 200a 666f 7220 656c 656d 656e  ames .for elemen
+00000600: 7473 206c 696b 6520 7465 7874 2066 6965  ts like text fie
+00000610: 6c64 7320 616e 6420 6368 6563 6b62 6f78  lds and checkbox
+00000620: 6573 2e20 4974 2061 6c73 6f20 7375 7070  es. It also supp
+00000630: 6f72 7473 206f 7468 6572 2066 756e 6374  orts other funct
+00000640: 696f 6e61 6c69 7469 6573 2073 7563 6820  ionalities such 
+00000650: 6173 200a 6472 6177 696e 6720 696d 6167  as .drawing imag
+00000660: 6520 616e 6420 6d65 7267 696e 6720 6d75  e and merging mu
+00000670: 6c74 6970 6c65 2050 4446 7320 746f 6765  ltiple PDFs toge
+00000680: 7468 6572 2e0a 0a23 2320 496e 7374 616c  ther...## Instal
+00000690: 6c69 6e67 0a0a 496e 7374 616c 6c20 7573  ling..Install us
+000006a0: 696e 6720 5b70 6970 5d28 6874 7470 733a  ing [pip](https:
+000006b0: 2f2f 7069 702e 7079 7061 2e69 6f2f 656e  //pip.pypa.io/en
+000006c0: 2f73 7461 626c 652f 293a 0a0a 6060 6073  /stable/):..```s
+000006d0: 6865 6c6c 2073 6372 6970 740a 7069 7020  hell script.pip 
+000006e0: 696e 7374 616c 6c20 5079 5044 4646 6f72  install PyPDFFor
+000006f0: 6d0a 6060 600a 0a23 2320 5175 6963 6b20  m.```..## Quick 
+00000700: 4578 616d 706c 650a 0a21 5b5d 2868 7474  Example..![](htt
+00000710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000720: 6368 696e 6170 616e 6461 6d61 6e2f 5079  chinapandaman/Py
+00000730: 5044 4646 6f72 6d2f 626c 6f62 2f6d 6173  PDFForm/blob/mas
+00000740: 7465 722f 6465 6d6f 2e67 6966 290a 0a41  ter/demo.gif)..A
+00000750: 2073 616d 706c 6520 5044 4620 666f 726d   sample PDF form
+00000760: 2063 616e 2062 6520 666f 756e 6420 5b68   can be found [h
+00000770: 6572 655d 2868 7474 7073 3a2f 2f67 6974  ere](https://git
+00000780: 6875 622e 636f 6d2f 6368 696e 6170 616e  hub.com/chinapan
+00000790: 6461 6d61 6e2f 5079 5044 4646 6f72 6d2f  daman/PyPDFForm/
+000007a0: 626c 6f62 2f6d 6173 7465 722f 7064 665f  blob/master/pdf_
+000007b0: 7361 6d70 6c65 732f 7361 6d70 6c65 5f74  samples/sample_t
+000007c0: 656d 706c 6174 652e 7064 6629 2e20 446f  emplate.pdf). Do
+000007d0: 776e 6c6f 6164 2069 7420 616e 6420 7472  wnload it and tr
+000007e0: 793a 0a0a 6060 6070 7974 686f 6e0a 696d  y:..```python.im
+000007f0: 706f 7274 206f 730a 0a66 726f 6d20 5079  port os..from Py
+00000800: 5044 4646 6f72 6d20 696d 706f 7274 2050  PDFForm import P
+00000810: 7950 4446 466f 726d 0a0a 5041 5448 5f54  yPDFForm..PATH_T
+00000820: 4f5f 444f 574e 4c4f 4144 4544 5f53 414d  O_DOWNLOADED_SAM
+00000830: 504c 455f 5044 465f 464f 524d 203d 206f  PLE_PDF_FORM = o
+00000840: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00000850: 206f 732e 7061 7468 2e65 7870 616e 6475   os.path.expandu
+00000860: 7365 7228 227e 2f44 6f77 6e6c 6f61 6473  ser("~/Downloads
+00000870: 2229 2c20 2273 616d 706c 655f 7465 6d70  "), "sample_temp
+00000880: 6c61 7465 2e70 6466 220a 2920 2023 2043  late.pdf".)  # C
+00000890: 6861 6e67 6520 7468 6973 2074 6f20 7768  hange this to wh
+000008a0: 6572 6520 796f 7520 646f 776e 6c6f 6164  ere you download
+000008b0: 6564 2074 6865 2073 616d 706c 6520 5044  ed the sample PD
+000008c0: 4620 666f 726d 0a0a 5041 5448 5f54 4f5f  F form..PATH_TO_
+000008d0: 4649 4c4c 4544 5f50 4446 5f46 4f52 4d20  FILLED_PDF_FORM 
+000008e0: 3d20 6f73 2e70 6174 682e 6a6f 696e 280a  = os.path.join(.
+000008f0: 2020 2020 6f73 2e70 6174 682e 6578 7061      os.path.expa
+00000900: 6e64 7573 6572 2822 7e22 292c 2022 6f75  nduser("~"), "ou
+00000910: 7470 7574 2e70 6466 220a 2920 2023 2043  tput.pdf".)  # C
+00000920: 6861 6e67 6520 7468 6973 2074 6f20 7768  hange this to wh
+00000930: 6572 6520 796f 7520 7769 7368 2074 6f20  ere you wish to 
+00000940: 7075 7420 796f 7572 2066 696c 6c65 6420  put your filled 
+00000950: 5044 4620 666f 726d 0a0a 7769 7468 206f  PDF form..with o
+00000960: 7065 6e28 5041 5448 5f54 4f5f 4649 4c4c  pen(PATH_TO_FILL
+00000970: 4544 5f50 4446 5f46 4f52 4d2c 2022 7762  ED_PDF_FORM, "wb
+00000980: 2b22 2920 6173 206f 7574 7075 743a 0a20  +") as output:. 
+00000990: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
+000009a0: 0a20 2020 2020 2020 2050 7950 4446 466f  .        PyPDFFo
+000009b0: 726d 2850 4154 485f 544f 5f44 4f57 4e4c  rm(PATH_TO_DOWNL
+000009c0: 4f41 4445 445f 5341 4d50 4c45 5f50 4446  OADED_SAMPLE_PDF
+000009d0: 5f46 4f52 4d29 0a20 2020 2020 2020 202e  _FORM).        .
+000009e0: 6669 6c6c 280a 2020 2020 2020 2020 2020  fill(.          
+000009f0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000a00: 2020 2020 2274 6573 7422 3a20 2274 6573      "test": "tes
+00000a10: 745f 3122 2c0a 2020 2020 2020 2020 2020  t_1",.          
+00000a20: 2020 2020 2020 2263 6865 636b 223a 2054        "check": T
+00000a30: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00000a40: 2020 2020 2022 7465 7374 5f32 223a 2022       "test_2": "
+00000a50: 7465 7374 5f32 222c 0a20 2020 2020 2020  test_2",.       
+00000a60: 2020 2020 2020 2020 2022 6368 6563 6b5f           "check_
+00000a70: 3222 3a20 4661 6c73 652c 0a20 2020 2020  2": False,.     
+00000a80: 2020 2020 2020 2020 2020 2022 7465 7374             "test
+00000a90: 5f33 223a 2022 7465 7374 5f33 222c 0a20  _3": "test_3",. 
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000ab0: 6368 6563 6b5f 3322 3a20 5472 7565 2c0a  check_3": True,.
+00000ac0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000ad0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000ae0: 202e 7265 6164 2829 0a20 2020 2029 0a60   .read().    ).`
+00000af0: 6060 0a0a 4166 7465 7220 7275 6e6e 696e  ``..After runnin
+00000b00: 6720 7468 6520 6162 6f76 6520 636f 6465  g the above code
+00000b10: 2073 6e69 7070 6574 2079 6f75 2063 616e   snippet you can
+00000b20: 2066 696e 6420 606f 7574 7075 742e 7064   find `output.pd
+00000b30: 6660 2061 7420 7468 6520 6c6f 6361 7469  f` at the locati
+00000b40: 6f6e 2079 6f75 2073 7065 6369 6669 6564  on you specified
+00000b50: 2c20 0a61 6e64 2069 7420 7368 6f75 6c64  , .and it should
+00000b60: 206c 6f6f 6b20 6c69 6b65 205b 7468 6973   look like [this
+00000b70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000b80: 2e63 6f6d 2f63 6869 6e61 7061 6e64 616d  .com/chinapandam
+00000b90: 616e 2f50 7950 4446 466f 726d 2f62 6c6f  an/PyPDFForm/blo
+00000ba0: 622f 6d61 7374 6572 2f70 6466 5f73 616d  b/master/pdf_sam
+00000bb0: 706c 6573 2f73 616d 706c 655f 6669 6c6c  ples/sample_fill
+00000bc0: 6564 2e70 6466 292e 0a0a 2323 2044 6f63  ed.pdf)...## Doc
+00000bd0: 756d 656e 7461 7469 6f6e 0a0a 5b45 7861  umentation..[Exa
+00000be0: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
+00000bf0: 6974 6875 622e 636f 6d2f 6368 696e 6170  ithub.com/chinap
+00000c00: 616e 6461 6d61 6e2f 5079 5044 4646 6f72  andaman/PyPDFFor
+00000c10: 6d2f 626c 6f62 2f6d 6173 7465 722f 646f  m/blob/master/do
+00000c20: 6373 2f65 7861 6d70 6c65 732e 6d64 290a  cs/examples.md).
+00000c30: 0a23 2320 486f 7720 746f 2043 6f6e 7472  .## How to Contr
+00000c40: 6962 7574 650a 0a49 6620 796f 7520 7769  ibute..If you wi
+00000c50: 7368 2074 6f20 696d 7072 6f76 6520 7468  sh to improve th
+00000c60: 6973 206c 6962 7261 7279 2c20 7468 6572  is library, ther
+00000c70: 6520 6973 206f 6e65 2073 7065 6369 6669  e is one specifi
+00000c80: 6320 7761 7920 796f 7520 6361 6e20 636f  c way you can co
+00000c90: 6e74 7269 6275 7465 200a 6f6e 2074 6f70  ntribute .on top
+00000ca0: 206f 6620 7468 6520 7573 7561 6c20 6f70   of the usual op
+00000cb0: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
+00000cc0: 7420 6e6f 726d 7320 7375 6368 2061 7320  t norms such as 
+00000cd0: 6973 7375 6573 2061 6e64 2070 756c 6c20  issues and pull 
+00000ce0: 7265 7175 6573 7473 2e0a 0a49 7420 6973  requests...It is
+00000cf0: 2064 6966 6669 6375 6c74 2074 6f20 6d61   difficult to ma
+00000d00: 6b65 2073 7572 6520 7468 6174 2074 6865  ke sure that the
+00000d10: 206c 6962 7261 7279 2073 7570 706f 7274   library support
+00000d20: 7320 616c 6c20 7468 6520 5044 4620 666f  s all the PDF fo
+00000d30: 726d 2063 7265 6174 696e 6720 746f 6f6c  rm creating tool
+00000d40: 7320 6f75 7420 0a74 6865 7265 2e20 536f  s out .there. So
+00000d50: 2069 6620 796f 7520 7275 6e20 696e 746f   if you run into
+00000d60: 2061 2063 6173 6520 7768 6572 6520 7468   a case where th
+00000d70: 6520 6c69 6272 6172 7920 646f 6573 206e  e library does n
+00000d80: 6f74 2077 6f72 6b20 666f 7220 6365 7274  ot work for cert
+00000d90: 6169 6e20 5044 4620 666f 726d 7320 6372  ain PDF forms cr
+00000da0: 6561 7465 6420 6279 200a 6365 7274 6169  eated by .certai
+00000db0: 6e20 746f 6f6c 732c 2066 6565 6c20 6672  n tools, feel fr
+00000dc0: 6565 2074 6f20 6f70 656e 2061 6e20 6973  ee to open an is
+00000dd0: 7375 6520 7769 7468 2074 6865 2070 726f  sue with the pro
+00000de0: 626c 656d 6174 6963 2050 4446 2066 6f72  blematic PDF for
+00000df0: 6d20 6174 7461 6368 6564 2e20 4920 7769  m attached. I wi
+00000e00: 6c6c 2073 6565 6b20 0a74 6f20 6d61 6b65  ll seek .to make
+00000e10: 2074 6865 206c 6962 7261 7279 2073 7570   the library sup
+00000e20: 706f 7274 2074 6865 2061 7474 6163 6865  port the attache
+00000e30: 6420 5044 4620 666f 726d 2061 7320 7765  d PDF form as we
+00000e40: 6c6c 2061 7320 7468 6520 746f 6f6c 2075  ll as the tool u
+00000e50: 7365 6420 746f 2063 7265 6174 6520 6974  sed to create it
+00000e60: 2e0a                                     ..
```

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/constants.py` & `PyPDFForm-1.2.5/PyPDFForm/core/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/filler.py` & `PyPDFForm-1.2.5/PyPDFForm/core/filler.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/font.py` & `PyPDFForm-1.2.5/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/image.py` & `PyPDFForm-1.2.5/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/patterns.py` & `PyPDFForm-1.2.5/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/template.py` & `PyPDFForm-1.2.5/PyPDFForm/core/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/utils.py` & `PyPDFForm-1.2.5/PyPDFForm/core/utils.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/core/watermark.py` & `PyPDFForm-1.2.5/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/element.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/template.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/template.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/middleware/text.py` & `PyPDFForm-1.2.5/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm/wrapper.py` & `PyPDFForm-1.2.5/PyPDFForm/wrapper.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.2.5/PyPDFForm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 5079 5044  : 2.1.Name: PyPD
 00000020: 4646 6f72 6d0a 5665 7273 696f 6e3a 2031  FForm.Version: 1
-00000030: 2e32 2e34 0a53 756d 6d61 7279 3a20 5468  .2.4.Summary: Th
+00000030: 2e32 2e35 0a53 756d 6d61 7279 3a20 5468  .2.5.Summary: Th
 00000040: 6520 5079 7468 6f6e 206c 6962 7261 7279  e Python library
 00000050: 2066 6f72 2050 4446 2066 6f72 6d73 2e0a   for PDF forms..
 00000060: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000070: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
 00000080: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
 00000090: 4646 6f72 6d0a 4175 7468 6f72 3a20 4a69  FForm.Author: Ji
 000000a0: 6e67 6520 4c69 0a43 6c61 7373 6966 6965  nge Li.Classifie
@@ -18,180 +18,214 @@
 00000110: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
 00000120: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
 00000130: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
 00000140: 732d 5079 7468 6f6e 3a20 3e3d 332e 370a  s-Python: >=3.7.
 00000150: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000160: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
 00000170: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
-00000180: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
-00000190: 2050 7950 4446 466f 726d 2021 5b63 6f64   PyPDFForm ![cod
-000001a0: 6520 666f 726d 6174 7469 6e67 5d28 6874  e formatting](ht
-000001b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000001c0: 2f63 6869 6e61 7061 6e64 616d 616e 2f50  /chinapandaman/P
-000001d0: 7950 4446 466f 726d 2f61 6374 696f 6e73  yPDFForm/actions
-000001e0: 2f77 6f72 6b66 6c6f 7773 2f70 7974 686f  /workflows/pytho
-000001f0: 6e2d 626c 6163 6b2d 6973 6f72 742e 796d  n-black-isort.ym
-00000200: 6c2f 6261 6467 652e 7376 6729 2021 5b74  l/badge.svg) ![t
-00000210: 6573 7473 5d28 6874 7470 733a 2f2f 6769  ests](https://gi
-00000220: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
-00000230: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
-00000240: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000250: 7773 2f70 7974 686f 6e2d 7061 636b 6167  ws/python-packag
-00000260: 652e 796d 6c2f 6261 6467 652e 7376 6729  e.yml/badge.svg)
-00000270: 205b 215b 636f 6465 636f 765d 2868 7474   [![codecov](htt
-00000280: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000290: 6768 2f63 6869 6e61 7061 6e64 616d 616e  gh/chinapandaman
-000002a0: 2f50 7950 4446 466f 726d 2f62 7261 6e63  /PyPDFForm/branc
-000002b0: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
-000002c0: 6164 6765 2e73 7667 3f74 6f6b 656e 3d43  adge.svg?token=C
-000002d0: 5352 4c4e 3134 4946 4529 5d28 6874 7470  SRLN14IFE)](http
-000002e0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
-000002f0: 682f 6368 696e 6170 616e 6461 6d61 6e2f  h/chinapandaman/
-00000300: 5079 5044 4646 6f72 6d29 2021 5b64 6570  PyPDFForm) ![dep
-00000310: 6c6f 795d 2868 7474 7073 3a2f 2f67 6974  loy](https://git
-00000320: 6875 622e 636f 6d2f 6368 696e 6170 616e  hub.com/chinapan
-00000330: 6461 6d61 6e2f 5079 5044 4646 6f72 6d2f  daman/PyPDFForm/
-00000340: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000350: 732f 7079 7468 6f6e 2d70 7562 6c69 7368  s/python-publish
-00000360: 2e79 6d6c 2f62 6164 6765 2e73 7667 290a  .yml/badge.svg).
-00000370: 0a50 7950 4446 466f 726d 2069 7320 6120  .PyPDFForm is a 
-00000380: 7075 7265 2050 7974 686f 6e20 6c69 6272  pure Python libr
-00000390: 6172 7920 666f 7220 5044 4620 666f 726d  ary for PDF form
-000003a0: 2070 726f 6365 7373 696e 672e 200a 4974   processing. .It
-000003b0: 2061 6c6c 6f77 7320 6669 6c6c 696e 6720   allows filling 
-000003c0: 6120 5044 4620 666f 726d 2070 726f 6772  a PDF form progr
-000003d0: 616d 6d61 7469 6361 6c6c 7920 6279 2063  ammatically by c
-000003e0: 7265 6174 696e 6720 0a61 2050 7974 686f  reating .a Pytho
-000003f0: 6e20 6469 6374 696f 6e61 7279 2077 6974  n dictionary wit
-00000400: 6820 6b65 7973 206d 6174 6368 696e 6720  h keys matching 
-00000410: 6974 7320 616e 6e6f 7461 7465 6420 6e61  its annotated na
-00000420: 6d65 7320 0a66 6f72 2065 6c65 6d65 6e74  mes .for element
-00000430: 7320 6c69 6b65 2074 6578 7420 6669 656c  s like text fiel
-00000440: 6473 2061 6e64 2063 6865 636b 626f 7865  ds and checkboxe
-00000450: 732e 2049 7420 616c 736f 2073 7570 706f  s. It also suppo
-00000460: 7274 7320 6f74 6865 7220 6675 6e63 7469  rts other functi
-00000470: 6f6e 616c 6974 6965 7320 7375 6368 2061  onalities such a
-00000480: 7320 0a64 7261 7769 6e67 2069 6d61 6765  s .drawing image
-00000490: 2061 6e64 206d 6572 6769 6e67 206d 756c   and merging mul
-000004a0: 7469 706c 6520 5044 4673 2074 6f67 6574  tiple PDFs toget
-000004b0: 6865 722e 0a0a 2323 2049 6e73 7461 6c6c  her...## Install
-000004c0: 696e 670a 0a49 6e73 7461 6c6c 2075 7369  ing..Install usi
-000004d0: 6e67 205b 7069 705d 2868 7474 7073 3a2f  ng [pip](https:/
-000004e0: 2f70 6970 2e70 7970 612e 696f 2f65 6e2f  /pip.pypa.io/en/
-000004f0: 7374 6162 6c65 2f29 3a0a 0a60 6060 7368  stable/):..```sh
-00000500: 656c 6c20 7363 7269 7074 0a70 6970 2069  ell script.pip i
-00000510: 6e73 7461 6c6c 2050 7950 4446 466f 726d  nstall PyPDFForm
-00000520: 0a60 6060 0a0a 2323 2051 7569 636b 2045  .```..## Quick E
-00000530: 7861 6d70 6c65 0a0a 4120 7361 6d70 6c65  xample..A sample
-00000540: 2050 4446 2066 6f72 6d20 6361 6e20 6265   PDF form can be
-00000550: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
-00000560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000570: 2f63 6869 6e61 7061 6e64 616d 616e 2f50  /chinapandaman/P
-00000580: 7950 4446 466f 726d 2f62 6c6f 622f 6d61  yPDFForm/blob/ma
-00000590: 7374 6572 2f70 6466 5f73 616d 706c 6573  ster/pdf_samples
-000005a0: 2f73 616d 706c 655f 7465 6d70 6c61 7465  /sample_template
-000005b0: 2e70 6466 292e 2044 6f77 6e6c 6f61 6420  .pdf). Download 
-000005c0: 6974 2061 6e64 2074 7279 3a0a 0a60 6060  it and try:..```
-000005d0: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f73  python.import os
-000005e0: 0a0a 6672 6f6d 2050 7950 4446 466f 726d  ..from PyPDFForm
-000005f0: 2069 6d70 6f72 7420 5079 5044 4646 6f72   import PyPDFFor
-00000600: 6d0a 0a50 4154 485f 544f 5f44 4f57 4e4c  m..PATH_TO_DOWNL
-00000610: 4f41 4445 445f 5341 4d50 4c45 5f50 4446  OADED_SAMPLE_PDF
-00000620: 5f46 4f52 4d20 3d20 6f73 2e70 6174 682e  _FORM = os.path.
-00000630: 6a6f 696e 280a 2020 2020 6f73 2e70 6174  join(.    os.pat
-00000640: 682e 6578 7061 6e64 7573 6572 2822 7e2f  h.expanduser("~/
-00000650: 446f 776e 6c6f 6164 7322 292c 2022 7361  Downloads"), "sa
-00000660: 6d70 6c65 5f74 656d 706c 6174 652e 7064  mple_template.pd
-00000670: 6622 0a29 2020 2320 4368 616e 6765 2074  f".)  # Change t
-00000680: 6869 7320 746f 2077 6865 7265 2079 6f75  his to where you
-00000690: 2064 6f77 6e6c 6f61 6465 6420 7468 6520   downloaded the 
-000006a0: 7361 6d70 6c65 2050 4446 2066 6f72 6d0a  sample PDF form.
-000006b0: 0a50 4154 485f 544f 5f46 494c 4c45 445f  .PATH_TO_FILLED_
-000006c0: 5044 465f 464f 524d 203d 206f 732e 7061  PDF_FORM = os.pa
-000006d0: 7468 2e6a 6f69 6e28 0a20 2020 206f 732e  th.join(.    os.
-000006e0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-000006f0: 227e 2229 2c20 226f 7574 7075 742e 7064  "~"), "output.pd
-00000700: 6622 0a29 2020 2320 4368 616e 6765 2074  f".)  # Change t
-00000710: 6869 7320 746f 2077 6865 7265 2079 6f75  his to where you
-00000720: 2077 6973 6820 746f 2070 7574 2079 6f75   wish to put you
-00000730: 7220 6669 6c6c 6564 2050 4446 2066 6f72  r filled PDF for
-00000740: 6d0a 0a77 6974 6820 6f70 656e 2850 4154  m..with open(PAT
-00000750: 485f 544f 5f46 494c 4c45 445f 5044 465f  H_TO_FILLED_PDF_
-00000760: 464f 524d 2c20 2277 622b 2229 2061 7320  FORM, "wb+") as 
-00000770: 6f75 7470 7574 3a0a 2020 2020 6f75 7470  output:.    outp
-00000780: 7574 2e77 7269 7465 280a 2020 2020 2020  ut.write(.      
-00000790: 2020 5079 5044 4646 6f72 6d28 5041 5448    PyPDFForm(PATH
-000007a0: 5f54 4f5f 444f 574e 4c4f 4144 4544 5f53  _TO_DOWNLOADED_S
-000007b0: 414d 504c 455f 5044 465f 464f 524d 290a  AMPLE_PDF_FORM).
-000007c0: 2020 2020 2020 2020 2e66 696c 6c28 0a20          .fill(. 
-000007d0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000007e0: 2020 2020 2020 2020 2020 2020 2022 7465               "te
-000007f0: 7374 223a 2022 7465 7374 5f31 222c 0a20  st": "test_1",. 
-00000800: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000810: 6368 6563 6b22 3a20 5472 7565 2c0a 2020  check": True,.  
-00000820: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000830: 6573 745f 3222 3a20 2274 6573 745f 3222  est_2": "test_2"
-00000840: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000850: 2020 2263 6865 636b 5f32 223a 2046 616c    "check_2": Fal
-00000860: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00000870: 2020 2020 2274 6573 745f 3322 3a20 2274      "test_3": "t
-00000880: 6573 745f 3322 2c0a 2020 2020 2020 2020  est_3",.        
-00000890: 2020 2020 2020 2020 2263 6865 636b 5f33          "check_3
-000008a0: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-000008b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000008c0: 290a 2020 2020 2020 2020 2e72 6561 6428  ).        .read(
-000008d0: 290a 2020 2020 290a 6060 600a 0a41 6674  ).    ).```..Aft
-000008e0: 6572 2072 756e 6e69 6e67 2074 6865 2061  er running the a
-000008f0: 626f 7665 2063 6f64 6520 736e 6970 7065  bove code snippe
-00000900: 7420 796f 7520 6361 6e20 6669 6e64 2060  t you can find `
-00000910: 6f75 7470 7574 2e70 6466 6020 6174 2074  output.pdf` at t
-00000920: 6865 206c 6f63 6174 696f 6e20 796f 7520  he location you 
-00000930: 7370 6563 6966 6965 642c 200a 616e 6420  specified, .and 
-00000940: 6974 2073 686f 756c 6420 6c6f 6f6b 206c  it should look l
-00000950: 696b 6520 5b74 6869 735d 2868 7474 7073  ike [this](https
-00000960: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
-00000970: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
-00000980: 4646 6f72 6d2f 626c 6f62 2f6d 6173 7465  FForm/blob/maste
-00000990: 722f 7064 665f 7361 6d70 6c65 732f 7361  r/pdf_samples/sa
-000009a0: 6d70 6c65 5f66 696c 6c65 642e 7064 6629  mple_filled.pdf)
-000009b0: 2e0a 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
-000009c0: 696f 6e0a 0a5b 4578 616d 706c 6573 5d28  ion..[Examples](
-000009d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000009e0: 6f6d 2f63 6869 6e61 7061 6e64 616d 616e  om/chinapandaman
-000009f0: 2f50 7950 4446 466f 726d 2f62 6c6f 622f  /PyPDFForm/blob/
-00000a00: 6d61 7374 6572 2f64 6f63 732f 6578 616d  master/docs/exam
-00000a10: 706c 6573 2e6d 6429 0a0a 2323 2048 6f77  ples.md)..## How
-00000a20: 2074 6f20 436f 6e74 7269 6275 7465 0a0a   to Contribute..
-00000a30: 4966 2079 6f75 2077 6973 6820 746f 2069  If you wish to i
-00000a40: 6d70 726f 7665 2074 6869 7320 6c69 6272  mprove this libr
-00000a50: 6172 792c 2074 6865 7265 2069 7320 6f6e  ary, there is on
-00000a60: 6520 7370 6563 6966 6963 2077 6179 2079  e specific way y
-00000a70: 6f75 2063 616e 2063 6f6e 7472 6962 7574  ou can contribut
-00000a80: 6520 0a6f 6e20 746f 7020 6f66 2074 6865  e .on top of the
-00000a90: 2075 7375 616c 206f 7065 6e20 736f 7572   usual open sour
-00000aa0: 6365 2070 726f 6a65 6374 206e 6f72 6d73  ce project norms
-00000ab0: 2073 7563 6820 6173 2069 7373 7565 7320   such as issues 
-00000ac0: 616e 6420 7075 6c6c 2072 6571 7565 7374  and pull request
-00000ad0: 732e 0a0a 4974 2069 7320 6469 6666 6963  s...It is diffic
-00000ae0: 756c 7420 746f 206d 616b 6520 7375 7265  ult to make sure
-00000af0: 2074 6861 7420 7468 6520 6c69 6272 6172   that the librar
-00000b00: 7920 7375 7070 6f72 7473 2061 6c6c 2074  y supports all t
-00000b10: 6865 2050 4446 2066 6f72 6d20 6372 6561  he PDF form crea
-00000b20: 7469 6e67 2074 6f6f 6c73 206f 7574 200a  ting tools out .
-00000b30: 7468 6572 652e 2053 6f20 6966 2079 6f75  there. So if you
-00000b40: 2072 756e 2069 6e74 6f20 6120 6361 7365   run into a case
-00000b50: 2077 6865 7265 2074 6865 206c 6962 7261   where the libra
-00000b60: 7279 2064 6f65 7320 6e6f 7420 776f 726b  ry does not work
-00000b70: 2066 6f72 2063 6572 7461 696e 2050 4446   for certain PDF
-00000b80: 2066 6f72 6d73 2063 7265 6174 6564 2062   forms created b
-00000b90: 7920 0a63 6572 7461 696e 2074 6f6f 6c73  y .certain tools
-00000ba0: 2c20 6665 656c 2066 7265 6520 746f 206f  , feel free to o
-00000bb0: 7065 6e20 616e 2069 7373 7565 2077 6974  pen an issue wit
-00000bc0: 6820 7468 6520 7072 6f62 6c65 6d61 7469  h the problemati
-00000bd0: 6320 5044 4620 666f 726d 2061 7474 6163  c PDF form attac
-00000be0: 6865 642e 2049 2077 696c 6c20 7365 656b  hed. I will seek
-00000bf0: 200a 746f 206d 616b 6520 7468 6520 6c69   .to make the li
-00000c00: 6272 6172 7920 7375 7070 6f72 7420 7468  brary support th
-00000c10: 6520 6174 7461 6368 6564 2050 4446 2066  e attached PDF f
-00000c20: 6f72 6d20 6173 2077 656c 6c20 6173 2074  orm as well as t
-00000c30: 6865 2074 6f6f 6c20 7573 6564 2074 6f20  he tool used to 
-00000c40: 6372 6561 7465 2069 742e 0a              create it..
+00000180: 4669 6c65 3a20 4c49 4345 4e53 450a 0a3c  File: LICENSE..<
+00000190: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000001a0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+000001c0: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+000001d0: 4646 6f72 6d2f 626c 6f62 2f6d 6173 7465  FForm/blob/maste
+000001e0: 722f 6c6f 676f 2e70 6e67 223e 3c2f 703e  r/logo.png"></p>
+000001f0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000200: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
+00000210: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000220: 636f 6d2f 6368 696e 6170 616e 6461 6d61  com/chinapandama
+00000230: 6e2f 5079 5044 4646 6f72 6d2f 6163 7469  n/PyPDFForm/acti
+00000240: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000250: 7468 6f6e 2d62 6c61 636b 2d69 736f 7274  thon-black-isort
+00000260: 2e79 6d6c 2f62 6164 6765 2e73 7667 223e  .yml/badge.svg">
+00000270: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6869  //github.com/chi
+00000290: 6e61 7061 6e64 616d 616e 2f50 7950 4446  napandaman/PyPDF
+000002a0: 466f 726d 2f61 6374 696f 6e73 2f77 6f72  Form/actions/wor
+000002b0: 6b66 6c6f 7773 2f70 7974 686f 6e2d 626c  kflows/python-bl
+000002c0: 6163 6b2d 6973 6f72 742e 796d 6c2f 6261  ack-isort.yml/ba
+000002d0: 6467 652e 7376 6722 3e3c 2f61 3e0a 2020  dge.svg"></a>.  
+000002e0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000002f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+00000300: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+00000310: 4646 6f72 6d2f 6163 7469 6f6e 732f 776f  FForm/actions/wo
+00000320: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
+00000330: 6163 6b61 6765 2e79 6d6c 2f62 6164 6765  ackage.yml/badge
+00000340: 2e73 7667 223e 3c69 6d67 2073 7263 3d22  .svg"><img src="
+00000350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000360: 6f6d 2f63 6869 6e61 7061 6e64 616d 616e  om/chinapandaman
+00000370: 2f50 7950 4446 466f 726d 2f61 6374 696f  /PyPDFForm/actio
+00000380: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+00000390: 686f 6e2d 7061 636b 6167 652e 796d 6c2f  hon-package.yml/
+000003a0: 6261 6467 652e 7376 6722 3e3c 2f61 3e0a  badge.svg"></a>.
+000003b0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000003c0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
+000003d0: 6768 2f63 6869 6e61 7061 6e64 616d 616e  gh/chinapandaman
+000003e0: 2f50 7950 4446 466f 726d 223e 3c69 6d67  /PyPDFForm"><img
+000003f0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
+00000400: 6465 636f 762e 696f 2f67 682f 6368 696e  decov.io/gh/chin
+00000410: 6170 616e 6461 6d61 6e2f 5079 5044 4646  apandaman/PyPDFF
+00000420: 6f72 6d2f 6272 616e 6368 2f6d 6173 7465  orm/branch/maste
+00000430: 722f 6772 6170 682f 6261 6467 652e 7376  r/graph/badge.sv
+00000440: 673f 746f 6b65 6e3d 4353 524c 4e31 3449  g?token=CSRLN14I
+00000450: 4645 223e 3c2f 613e 0a20 2020 203c 6120  FE"></a>.    <a 
+00000460: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000470: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
+00000480: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
+00000490: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+000004a0: 7773 2f70 7974 686f 6e2d 7075 626c 6973  ws/python-publis
+000004b0: 682e 796d 6c2f 6261 6467 652e 7376 6722  h.yml/badge.svg"
+000004c0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000004d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+000004e0: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+000004f0: 4646 6f72 6d2f 6163 7469 6f6e 732f 776f  FForm/actions/wo
+00000500: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
+00000510: 7562 6c69 7368 2e79 6d6c 2f62 6164 6765  ublish.yml/badge
+00000520: 2e73 7667 223e 3c2f 613e 0a3c 2f70 3e0a  .svg"></a>.</p>.
+00000530: 0a23 2320 496e 7472 6f64 7563 7469 6f6e  .## Introduction
+00000540: 0a0a 5079 5044 4646 6f72 6d20 6973 2061  ..PyPDFForm is a
+00000550: 2070 7572 6520 5079 7468 6f6e 206c 6962   pure Python lib
+00000560: 7261 7279 2066 6f72 2050 4446 2066 6f72  rary for PDF for
+00000570: 6d20 7072 6f63 6573 7369 6e67 2e20 0a49  m processing. .I
+00000580: 7420 616c 6c6f 7773 2066 696c 6c69 6e67  t allows filling
+00000590: 2061 2050 4446 2066 6f72 6d20 7072 6f67   a PDF form prog
+000005a0: 7261 6d6d 6174 6963 616c 6c79 2062 7920  rammatically by 
+000005b0: 6372 6561 7469 6e67 200a 6120 5079 7468  creating .a Pyth
+000005c0: 6f6e 2064 6963 7469 6f6e 6172 7920 7769  on dictionary wi
+000005d0: 7468 206b 6579 7320 6d61 7463 6869 6e67  th keys matching
+000005e0: 2069 7473 2061 6e6e 6f74 6174 6564 206e   its annotated n
+000005f0: 616d 6573 200a 666f 7220 656c 656d 656e  ames .for elemen
+00000600: 7473 206c 696b 6520 7465 7874 2066 6965  ts like text fie
+00000610: 6c64 7320 616e 6420 6368 6563 6b62 6f78  lds and checkbox
+00000620: 6573 2e20 4974 2061 6c73 6f20 7375 7070  es. It also supp
+00000630: 6f72 7473 206f 7468 6572 2066 756e 6374  orts other funct
+00000640: 696f 6e61 6c69 7469 6573 2073 7563 6820  ionalities such 
+00000650: 6173 200a 6472 6177 696e 6720 696d 6167  as .drawing imag
+00000660: 6520 616e 6420 6d65 7267 696e 6720 6d75  e and merging mu
+00000670: 6c74 6970 6c65 2050 4446 7320 746f 6765  ltiple PDFs toge
+00000680: 7468 6572 2e0a 0a23 2320 496e 7374 616c  ther...## Instal
+00000690: 6c69 6e67 0a0a 496e 7374 616c 6c20 7573  ling..Install us
+000006a0: 696e 6720 5b70 6970 5d28 6874 7470 733a  ing [pip](https:
+000006b0: 2f2f 7069 702e 7079 7061 2e69 6f2f 656e  //pip.pypa.io/en
+000006c0: 2f73 7461 626c 652f 293a 0a0a 6060 6073  /stable/):..```s
+000006d0: 6865 6c6c 2073 6372 6970 740a 7069 7020  hell script.pip 
+000006e0: 696e 7374 616c 6c20 5079 5044 4646 6f72  install PyPDFFor
+000006f0: 6d0a 6060 600a 0a23 2320 5175 6963 6b20  m.```..## Quick 
+00000700: 4578 616d 706c 650a 0a21 5b5d 2868 7474  Example..![](htt
+00000710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000720: 6368 696e 6170 616e 6461 6d61 6e2f 5079  chinapandaman/Py
+00000730: 5044 4646 6f72 6d2f 626c 6f62 2f6d 6173  PDFForm/blob/mas
+00000740: 7465 722f 6465 6d6f 2e67 6966 290a 0a41  ter/demo.gif)..A
+00000750: 2073 616d 706c 6520 5044 4620 666f 726d   sample PDF form
+00000760: 2063 616e 2062 6520 666f 756e 6420 5b68   can be found [h
+00000770: 6572 655d 2868 7474 7073 3a2f 2f67 6974  ere](https://git
+00000780: 6875 622e 636f 6d2f 6368 696e 6170 616e  hub.com/chinapan
+00000790: 6461 6d61 6e2f 5079 5044 4646 6f72 6d2f  daman/PyPDFForm/
+000007a0: 626c 6f62 2f6d 6173 7465 722f 7064 665f  blob/master/pdf_
+000007b0: 7361 6d70 6c65 732f 7361 6d70 6c65 5f74  samples/sample_t
+000007c0: 656d 706c 6174 652e 7064 6629 2e20 446f  emplate.pdf). Do
+000007d0: 776e 6c6f 6164 2069 7420 616e 6420 7472  wnload it and tr
+000007e0: 793a 0a0a 6060 6070 7974 686f 6e0a 696d  y:..```python.im
+000007f0: 706f 7274 206f 730a 0a66 726f 6d20 5079  port os..from Py
+00000800: 5044 4646 6f72 6d20 696d 706f 7274 2050  PDFForm import P
+00000810: 7950 4446 466f 726d 0a0a 5041 5448 5f54  yPDFForm..PATH_T
+00000820: 4f5f 444f 574e 4c4f 4144 4544 5f53 414d  O_DOWNLOADED_SAM
+00000830: 504c 455f 5044 465f 464f 524d 203d 206f  PLE_PDF_FORM = o
+00000840: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00000850: 206f 732e 7061 7468 2e65 7870 616e 6475   os.path.expandu
+00000860: 7365 7228 227e 2f44 6f77 6e6c 6f61 6473  ser("~/Downloads
+00000870: 2229 2c20 2273 616d 706c 655f 7465 6d70  "), "sample_temp
+00000880: 6c61 7465 2e70 6466 220a 2920 2023 2043  late.pdf".)  # C
+00000890: 6861 6e67 6520 7468 6973 2074 6f20 7768  hange this to wh
+000008a0: 6572 6520 796f 7520 646f 776e 6c6f 6164  ere you download
+000008b0: 6564 2074 6865 2073 616d 706c 6520 5044  ed the sample PD
+000008c0: 4620 666f 726d 0a0a 5041 5448 5f54 4f5f  F form..PATH_TO_
+000008d0: 4649 4c4c 4544 5f50 4446 5f46 4f52 4d20  FILLED_PDF_FORM 
+000008e0: 3d20 6f73 2e70 6174 682e 6a6f 696e 280a  = os.path.join(.
+000008f0: 2020 2020 6f73 2e70 6174 682e 6578 7061      os.path.expa
+00000900: 6e64 7573 6572 2822 7e22 292c 2022 6f75  nduser("~"), "ou
+00000910: 7470 7574 2e70 6466 220a 2920 2023 2043  tput.pdf".)  # C
+00000920: 6861 6e67 6520 7468 6973 2074 6f20 7768  hange this to wh
+00000930: 6572 6520 796f 7520 7769 7368 2074 6f20  ere you wish to 
+00000940: 7075 7420 796f 7572 2066 696c 6c65 6420  put your filled 
+00000950: 5044 4620 666f 726d 0a0a 7769 7468 206f  PDF form..with o
+00000960: 7065 6e28 5041 5448 5f54 4f5f 4649 4c4c  pen(PATH_TO_FILL
+00000970: 4544 5f50 4446 5f46 4f52 4d2c 2022 7762  ED_PDF_FORM, "wb
+00000980: 2b22 2920 6173 206f 7574 7075 743a 0a20  +") as output:. 
+00000990: 2020 206f 7574 7075 742e 7772 6974 6528     output.write(
+000009a0: 0a20 2020 2020 2020 2050 7950 4446 466f  .        PyPDFFo
+000009b0: 726d 2850 4154 485f 544f 5f44 4f57 4e4c  rm(PATH_TO_DOWNL
+000009c0: 4f41 4445 445f 5341 4d50 4c45 5f50 4446  OADED_SAMPLE_PDF
+000009d0: 5f46 4f52 4d29 0a20 2020 2020 2020 202e  _FORM).        .
+000009e0: 6669 6c6c 280a 2020 2020 2020 2020 2020  fill(.          
+000009f0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000a00: 2020 2020 2274 6573 7422 3a20 2274 6573      "test": "tes
+00000a10: 745f 3122 2c0a 2020 2020 2020 2020 2020  t_1",.          
+00000a20: 2020 2020 2020 2263 6865 636b 223a 2054        "check": T
+00000a30: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00000a40: 2020 2020 2022 7465 7374 5f32 223a 2022       "test_2": "
+00000a50: 7465 7374 5f32 222c 0a20 2020 2020 2020  test_2",.       
+00000a60: 2020 2020 2020 2020 2022 6368 6563 6b5f           "check_
+00000a70: 3222 3a20 4661 6c73 652c 0a20 2020 2020  2": False,.     
+00000a80: 2020 2020 2020 2020 2020 2022 7465 7374             "test
+00000a90: 5f33 223a 2022 7465 7374 5f33 222c 0a20  _3": "test_3",. 
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000ab0: 6368 6563 6b5f 3322 3a20 5472 7565 2c0a  check_3": True,.
+00000ac0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000ad0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000ae0: 202e 7265 6164 2829 0a20 2020 2029 0a60   .read().    ).`
+00000af0: 6060 0a0a 4166 7465 7220 7275 6e6e 696e  ``..After runnin
+00000b00: 6720 7468 6520 6162 6f76 6520 636f 6465  g the above code
+00000b10: 2073 6e69 7070 6574 2079 6f75 2063 616e   snippet you can
+00000b20: 2066 696e 6420 606f 7574 7075 742e 7064   find `output.pd
+00000b30: 6660 2061 7420 7468 6520 6c6f 6361 7469  f` at the locati
+00000b40: 6f6e 2079 6f75 2073 7065 6369 6669 6564  on you specified
+00000b50: 2c20 0a61 6e64 2069 7420 7368 6f75 6c64  , .and it should
+00000b60: 206c 6f6f 6b20 6c69 6b65 205b 7468 6973   look like [this
+00000b70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000b80: 2e63 6f6d 2f63 6869 6e61 7061 6e64 616d  .com/chinapandam
+00000b90: 616e 2f50 7950 4446 466f 726d 2f62 6c6f  an/PyPDFForm/blo
+00000ba0: 622f 6d61 7374 6572 2f70 6466 5f73 616d  b/master/pdf_sam
+00000bb0: 706c 6573 2f73 616d 706c 655f 6669 6c6c  ples/sample_fill
+00000bc0: 6564 2e70 6466 292e 0a0a 2323 2044 6f63  ed.pdf)...## Doc
+00000bd0: 756d 656e 7461 7469 6f6e 0a0a 5b45 7861  umentation..[Exa
+00000be0: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
+00000bf0: 6974 6875 622e 636f 6d2f 6368 696e 6170  ithub.com/chinap
+00000c00: 616e 6461 6d61 6e2f 5079 5044 4646 6f72  andaman/PyPDFFor
+00000c10: 6d2f 626c 6f62 2f6d 6173 7465 722f 646f  m/blob/master/do
+00000c20: 6373 2f65 7861 6d70 6c65 732e 6d64 290a  cs/examples.md).
+00000c30: 0a23 2320 486f 7720 746f 2043 6f6e 7472  .## How to Contr
+00000c40: 6962 7574 650a 0a49 6620 796f 7520 7769  ibute..If you wi
+00000c50: 7368 2074 6f20 696d 7072 6f76 6520 7468  sh to improve th
+00000c60: 6973 206c 6962 7261 7279 2c20 7468 6572  is library, ther
+00000c70: 6520 6973 206f 6e65 2073 7065 6369 6669  e is one specifi
+00000c80: 6320 7761 7920 796f 7520 6361 6e20 636f  c way you can co
+00000c90: 6e74 7269 6275 7465 200a 6f6e 2074 6f70  ntribute .on top
+00000ca0: 206f 6620 7468 6520 7573 7561 6c20 6f70   of the usual op
+00000cb0: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
+00000cc0: 7420 6e6f 726d 7320 7375 6368 2061 7320  t norms such as 
+00000cd0: 6973 7375 6573 2061 6e64 2070 756c 6c20  issues and pull 
+00000ce0: 7265 7175 6573 7473 2e0a 0a49 7420 6973  requests...It is
+00000cf0: 2064 6966 6669 6375 6c74 2074 6f20 6d61   difficult to ma
+00000d00: 6b65 2073 7572 6520 7468 6174 2074 6865  ke sure that the
+00000d10: 206c 6962 7261 7279 2073 7570 706f 7274   library support
+00000d20: 7320 616c 6c20 7468 6520 5044 4620 666f  s all the PDF fo
+00000d30: 726d 2063 7265 6174 696e 6720 746f 6f6c  rm creating tool
+00000d40: 7320 6f75 7420 0a74 6865 7265 2e20 536f  s out .there. So
+00000d50: 2069 6620 796f 7520 7275 6e20 696e 746f   if you run into
+00000d60: 2061 2063 6173 6520 7768 6572 6520 7468   a case where th
+00000d70: 6520 6c69 6272 6172 7920 646f 6573 206e  e library does n
+00000d80: 6f74 2077 6f72 6b20 666f 7220 6365 7274  ot work for cert
+00000d90: 6169 6e20 5044 4620 666f 726d 7320 6372  ain PDF forms cr
+00000da0: 6561 7465 6420 6279 200a 6365 7274 6169  eated by .certai
+00000db0: 6e20 746f 6f6c 732c 2066 6565 6c20 6672  n tools, feel fr
+00000dc0: 6565 2074 6f20 6f70 656e 2061 6e20 6973  ee to open an is
+00000dd0: 7375 6520 7769 7468 2074 6865 2070 726f  sue with the pro
+00000de0: 626c 656d 6174 6963 2050 4446 2066 6f72  blematic PDF for
+00000df0: 6d20 6174 7461 6368 6564 2e20 4920 7769  m attached. I wi
+00000e00: 6c6c 2073 6565 6b20 0a74 6f20 6d61 6b65  ll seek .to make
+00000e10: 2074 6865 206c 6962 7261 7279 2073 7570   the library sup
+00000e20: 706f 7274 2074 6865 2061 7474 6163 6865  port the attache
+00000e30: 6420 5044 4620 666f 726d 2061 7320 7765  d PDF form as we
+00000e40: 6c6c 2061 7320 7468 6520 746f 6f6c 2075  ll as the tool u
+00000e50: 7365 6420 746f 2063 7265 6174 6520 6974  sed to create it
+00000e60: 2e0a                                     ..
```

### Comparing `PyPDFForm-1.2.4/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.2.5/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.4/README.md` & `PyPDFForm-1.2.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,172 +1,206 @@
-00000000: 2320 5079 5044 4646 6f72 6d20 215b 636f  # PyPDFForm ![co
-00000010: 6465 2066 6f72 6d61 7474 696e 675d 2868  de formatting](h
-00000020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000030: 6d2f 6368 696e 6170 616e 6461 6d61 6e2f  m/chinapandaman/
-00000040: 5079 5044 4646 6f72 6d2f 6163 7469 6f6e  PyPDFForm/action
-00000050: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
-00000060: 6f6e 2d62 6c61 636b 2d69 736f 7274 2e79  on-black-isort.y
-00000070: 6d6c 2f62 6164 6765 2e73 7667 2920 215b  ml/badge.svg) ![
-00000080: 7465 7374 735d 2868 7474 7073 3a2f 2f67  tests](https://g
-00000090: 6974 6875 622e 636f 6d2f 6368 696e 6170  ithub.com/chinap
-000000a0: 616e 6461 6d61 6e2f 5079 5044 4646 6f72  andaman/PyPDFFor
-000000b0: 6d2f 6163 7469 6f6e 732f 776f 726b 666c  m/actions/workfl
-000000c0: 6f77 732f 7079 7468 6f6e 2d70 6163 6b61  ows/python-packa
-000000d0: 6765 2e79 6d6c 2f62 6164 6765 2e73 7667  ge.yml/badge.svg
-000000e0: 2920 5b21 5b63 6f64 6563 6f76 5d28 6874  ) [![codecov](ht
-000000f0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000100: 2f67 682f 6368 696e 6170 616e 6461 6d61  /gh/chinapandama
-00000110: 6e2f 5079 5044 4646 6f72 6d2f 6272 616e  n/PyPDFForm/bran
-00000120: 6368 2f6d 6173 7465 722f 6772 6170 682f  ch/master/graph/
-00000130: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
-00000140: 4353 524c 4e31 3449 4645 295d 2868 7474  CSRLN14IFE)](htt
-00000150: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-00000160: 6768 2f63 6869 6e61 7061 6e64 616d 616e  gh/chinapandaman
-00000170: 2f50 7950 4446 466f 726d 2920 215b 6465  /PyPDFForm) ![de
-00000180: 706c 6f79 5d28 6874 7470 733a 2f2f 6769  ploy](https://gi
-00000190: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
-000001a0: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
-000001b0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000001c0: 7773 2f70 7974 686f 6e2d 7075 626c 6973  ws/python-publis
-000001d0: 682e 796d 6c2f 6261 6467 652e 7376 6729  h.yml/badge.svg)
-000001e0: 0a0a 5079 5044 4646 6f72 6d20 6973 2061  ..PyPDFForm is a
-000001f0: 2070 7572 6520 5079 7468 6f6e 206c 6962   pure Python lib
-00000200: 7261 7279 2066 6f72 2050 4446 2066 6f72  rary for PDF for
-00000210: 6d20 7072 6f63 6573 7369 6e67 2e20 0a49  m processing. .I
-00000220: 7420 616c 6c6f 7773 2066 696c 6c69 6e67  t allows filling
-00000230: 2061 2050 4446 2066 6f72 6d20 7072 6f67   a PDF form prog
-00000240: 7261 6d6d 6174 6963 616c 6c79 2062 7920  rammatically by 
-00000250: 6372 6561 7469 6e67 200a 6120 5079 7468  creating .a Pyth
-00000260: 6f6e 2064 6963 7469 6f6e 6172 7920 7769  on dictionary wi
-00000270: 7468 206b 6579 7320 6d61 7463 6869 6e67  th keys matching
-00000280: 2069 7473 2061 6e6e 6f74 6174 6564 206e   its annotated n
-00000290: 616d 6573 200a 666f 7220 656c 656d 656e  ames .for elemen
-000002a0: 7473 206c 696b 6520 7465 7874 2066 6965  ts like text fie
-000002b0: 6c64 7320 616e 6420 6368 6563 6b62 6f78  lds and checkbox
-000002c0: 6573 2e20 4974 2061 6c73 6f20 7375 7070  es. It also supp
-000002d0: 6f72 7473 206f 7468 6572 2066 756e 6374  orts other funct
-000002e0: 696f 6e61 6c69 7469 6573 2073 7563 6820  ionalities such 
-000002f0: 6173 200a 6472 6177 696e 6720 696d 6167  as .drawing imag
-00000300: 6520 616e 6420 6d65 7267 696e 6720 6d75  e and merging mu
-00000310: 6c74 6970 6c65 2050 4446 7320 746f 6765  ltiple PDFs toge
-00000320: 7468 6572 2e0a 0a23 2320 496e 7374 616c  ther...## Instal
-00000330: 6c69 6e67 0a0a 496e 7374 616c 6c20 7573  ling..Install us
-00000340: 696e 6720 5b70 6970 5d28 6874 7470 733a  ing [pip](https:
-00000350: 2f2f 7069 702e 7079 7061 2e69 6f2f 656e  //pip.pypa.io/en
-00000360: 2f73 7461 626c 652f 293a 0a0a 6060 6073  /stable/):..```s
-00000370: 6865 6c6c 2073 6372 6970 740a 7069 7020  hell script.pip 
-00000380: 696e 7374 616c 6c20 5079 5044 4646 6f72  install PyPDFFor
-00000390: 6d0a 6060 600a 0a23 2320 5175 6963 6b20  m.```..## Quick 
-000003a0: 4578 616d 706c 650a 0a41 2073 616d 706c  Example..A sampl
-000003b0: 6520 5044 4620 666f 726d 2063 616e 2062  e PDF form can b
-000003c0: 6520 666f 756e 6420 5b68 6572 655d 2868  e found [here](h
-000003d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003e0: 6d2f 6368 696e 6170 616e 6461 6d61 6e2f  m/chinapandaman/
-000003f0: 5079 5044 4646 6f72 6d2f 626c 6f62 2f6d  PyPDFForm/blob/m
-00000400: 6173 7465 722f 7064 665f 7361 6d70 6c65  aster/pdf_sample
-00000410: 732f 7361 6d70 6c65 5f74 656d 706c 6174  s/sample_templat
-00000420: 652e 7064 6629 2e20 446f 776e 6c6f 6164  e.pdf). Download
-00000430: 2069 7420 616e 6420 7472 793a 0a0a 6060   it and try:..``
-00000440: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-00000450: 730a 0a66 726f 6d20 5079 5044 4646 6f72  s..from PyPDFFor
-00000460: 6d20 696d 706f 7274 2050 7950 4446 466f  m import PyPDFFo
-00000470: 726d 0a0a 5041 5448 5f54 4f5f 444f 574e  rm..PATH_TO_DOWN
-00000480: 4c4f 4144 4544 5f53 414d 504c 455f 5044  LOADED_SAMPLE_PD
-00000490: 465f 464f 524d 203d 206f 732e 7061 7468  F_FORM = os.path
-000004a0: 2e6a 6f69 6e28 0a20 2020 206f 732e 7061  .join(.    os.pa
-000004b0: 7468 2e65 7870 616e 6475 7365 7228 227e  th.expanduser("~
-000004c0: 2f44 6f77 6e6c 6f61 6473 2229 2c20 2273  /Downloads"), "s
-000004d0: 616d 706c 655f 7465 6d70 6c61 7465 2e70  ample_template.p
-000004e0: 6466 220a 2920 2023 2043 6861 6e67 6520  df".)  # Change 
-000004f0: 7468 6973 2074 6f20 7768 6572 6520 796f  this to where yo
-00000500: 7520 646f 776e 6c6f 6164 6564 2074 6865  u downloaded the
-00000510: 2073 616d 706c 6520 5044 4620 666f 726d   sample PDF form
-00000520: 0a0a 5041 5448 5f54 4f5f 4649 4c4c 4544  ..PATH_TO_FILLED
-00000530: 5f50 4446 5f46 4f52 4d20 3d20 6f73 2e70  _PDF_FORM = os.p
-00000540: 6174 682e 6a6f 696e 280a 2020 2020 6f73  ath.join(.    os
-00000550: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
-00000560: 2822 7e22 292c 2022 6f75 7470 7574 2e70  ("~"), "output.p
-00000570: 6466 220a 2920 2023 2043 6861 6e67 6520  df".)  # Change 
-00000580: 7468 6973 2074 6f20 7768 6572 6520 796f  this to where yo
-00000590: 7520 7769 7368 2074 6f20 7075 7420 796f  u wish to put yo
-000005a0: 7572 2066 696c 6c65 6420 5044 4620 666f  ur filled PDF fo
-000005b0: 726d 0a0a 7769 7468 206f 7065 6e28 5041  rm..with open(PA
-000005c0: 5448 5f54 4f5f 4649 4c4c 4544 5f50 4446  TH_TO_FILLED_PDF
-000005d0: 5f46 4f52 4d2c 2022 7762 2b22 2920 6173  _FORM, "wb+") as
-000005e0: 206f 7574 7075 743a 0a20 2020 206f 7574   output:.    out
-000005f0: 7075 742e 7772 6974 6528 0a20 2020 2020  put.write(.     
-00000600: 2020 2050 7950 4446 466f 726d 2850 4154     PyPDFForm(PAT
-00000610: 485f 544f 5f44 4f57 4e4c 4f41 4445 445f  H_TO_DOWNLOADED_
-00000620: 5341 4d50 4c45 5f50 4446 5f46 4f52 4d29  SAMPLE_PDF_FORM)
-00000630: 0a20 2020 2020 2020 202e 6669 6c6c 280a  .        .fill(.
-00000640: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000650: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00000660: 6573 7422 3a20 2274 6573 745f 3122 2c0a  est": "test_1",.
-00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2263 6865 636b 223a 2054 7275 652c 0a20  "check": True,. 
-00000690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000006a0: 7465 7374 5f32 223a 2022 7465 7374 5f32  test_2": "test_2
-000006b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000006c0: 2020 2022 6368 6563 6b5f 3222 3a20 4661     "check_2": Fa
-000006d0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-000006e0: 2020 2020 2022 7465 7374 5f33 223a 2022       "test_3": "
-000006f0: 7465 7374 5f33 222c 0a20 2020 2020 2020  test_3",.       
-00000700: 2020 2020 2020 2020 2022 6368 6563 6b5f           "check_
-00000710: 3322 3a20 5472 7565 2c0a 2020 2020 2020  3": True,.      
-00000720: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000730: 2029 0a20 2020 2020 2020 202e 7265 6164   ).        .read
-00000740: 2829 0a20 2020 2029 0a60 6060 0a0a 4166  ().    ).```..Af
-00000750: 7465 7220 7275 6e6e 696e 6720 7468 6520  ter running the 
-00000760: 6162 6f76 6520 636f 6465 2073 6e69 7070  above code snipp
-00000770: 6574 2079 6f75 2063 616e 2066 696e 6420  et you can find 
-00000780: 606f 7574 7075 742e 7064 6660 2061 7420  `output.pdf` at 
-00000790: 7468 6520 6c6f 6361 7469 6f6e 2079 6f75  the location you
-000007a0: 2073 7065 6369 6669 6564 2c20 0a61 6e64   specified, .and
-000007b0: 2069 7420 7368 6f75 6c64 206c 6f6f 6b20   it should look 
-000007c0: 6c69 6b65 205b 7468 6973 5d28 6874 7470  like [this](http
-000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-000007e0: 6869 6e61 7061 6e64 616d 616e 2f50 7950  hinapandaman/PyP
-000007f0: 4446 466f 726d 2f62 6c6f 622f 6d61 7374  DFForm/blob/mast
-00000800: 6572 2f70 6466 5f73 616d 706c 6573 2f73  er/pdf_samples/s
-00000810: 616d 706c 655f 6669 6c6c 6564 2e70 6466  ample_filled.pdf
-00000820: 292e 0a0a 2323 2044 6f63 756d 656e 7461  )...## Documenta
-00000830: 7469 6f6e 0a0a 5b45 7861 6d70 6c65 735d  tion..[Examples]
-00000840: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000850: 636f 6d2f 6368 696e 6170 616e 6461 6d61  com/chinapandama
-00000860: 6e2f 5079 5044 4646 6f72 6d2f 626c 6f62  n/PyPDFForm/blob
-00000870: 2f6d 6173 7465 722f 646f 6373 2f65 7861  /master/docs/exa
-00000880: 6d70 6c65 732e 6d64 290a 0a23 2320 486f  mples.md)..## Ho
-00000890: 7720 746f 2043 6f6e 7472 6962 7574 650a  w to Contribute.
-000008a0: 0a49 6620 796f 7520 7769 7368 2074 6f20  .If you wish to 
-000008b0: 696d 7072 6f76 6520 7468 6973 206c 6962  improve this lib
-000008c0: 7261 7279 2c20 7468 6572 6520 6973 206f  rary, there is o
-000008d0: 6e65 2073 7065 6369 6669 6320 7761 7920  ne specific way 
-000008e0: 796f 7520 6361 6e20 636f 6e74 7269 6275  you can contribu
-000008f0: 7465 200a 6f6e 2074 6f70 206f 6620 7468  te .on top of th
-00000900: 6520 7573 7561 6c20 6f70 656e 2073 6f75  e usual open sou
-00000910: 7263 6520 7072 6f6a 6563 7420 6e6f 726d  rce project norm
-00000920: 7320 7375 6368 2061 7320 6973 7375 6573  s such as issues
-00000930: 2061 6e64 2070 756c 6c20 7265 7175 6573   and pull reques
-00000940: 7473 2e0a 0a49 7420 6973 2064 6966 6669  ts...It is diffi
-00000950: 6375 6c74 2074 6f20 6d61 6b65 2073 7572  cult to make sur
-00000960: 6520 7468 6174 2074 6865 206c 6962 7261  e that the libra
-00000970: 7279 2073 7570 706f 7274 7320 616c 6c20  ry supports all 
-00000980: 7468 6520 5044 4620 666f 726d 2063 7265  the PDF form cre
-00000990: 6174 696e 6720 746f 6f6c 7320 6f75 7420  ating tools out 
-000009a0: 0a74 6865 7265 2e20 536f 2069 6620 796f  .there. So if yo
-000009b0: 7520 7275 6e20 696e 746f 2061 2063 6173  u run into a cas
-000009c0: 6520 7768 6572 6520 7468 6520 6c69 6272  e where the libr
-000009d0: 6172 7920 646f 6573 206e 6f74 2077 6f72  ary does not wor
-000009e0: 6b20 666f 7220 6365 7274 6169 6e20 5044  k for certain PD
-000009f0: 4620 666f 726d 7320 6372 6561 7465 6420  F forms created 
-00000a00: 6279 200a 6365 7274 6169 6e20 746f 6f6c  by .certain tool
-00000a10: 732c 2066 6565 6c20 6672 6565 2074 6f20  s, feel free to 
-00000a20: 6f70 656e 2061 6e20 6973 7375 6520 7769  open an issue wi
-00000a30: 7468 2074 6865 2070 726f 626c 656d 6174  th the problemat
-00000a40: 6963 2050 4446 2066 6f72 6d20 6174 7461  ic PDF form atta
-00000a50: 6368 6564 2e20 4920 7769 6c6c 2073 6565  ched. I will see
-00000a60: 6b20 0a74 6f20 6d61 6b65 2074 6865 206c  k .to make the l
-00000a70: 6962 7261 7279 2073 7570 706f 7274 2074  ibrary support t
-00000a80: 6865 2061 7474 6163 6865 6420 5044 4620  he attached PDF 
-00000a90: 666f 726d 2061 7320 7765 6c6c 2061 7320  form as well as 
-00000aa0: 7468 6520 746f 6f6c 2075 7365 6420 746f  the tool used to
-00000ab0: 2063 7265 6174 6520 6974 2e0a             create it..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000020: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000030: 6869 6e61 7061 6e64 616d 616e 2f50 7950  hinapandaman/PyP
+00000040: 4446 466f 726d 2f62 6c6f 622f 6d61 7374  DFForm/blob/mast
+00000050: 6572 2f6c 6f67 6f2e 706e 6722 3e3c 2f70  er/logo.png"></p
+00000060: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
+00000070: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00000080: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000090: 2e63 6f6d 2f63 6869 6e61 7061 6e64 616d  .com/chinapandam
+000000a0: 616e 2f50 7950 4446 466f 726d 2f61 6374  an/PyPDFForm/act
+000000b0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+000000c0: 7974 686f 6e2d 626c 6163 6b2d 6973 6f72  ython-black-isor
+000000d0: 742e 796d 6c2f 6261 6467 652e 7376 6722  t.yml/badge.svg"
+000000e0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6368  ://github.com/ch
+00000100: 696e 6170 616e 6461 6d61 6e2f 5079 5044  inapandaman/PyPD
+00000110: 4646 6f72 6d2f 6163 7469 6f6e 732f 776f  FForm/actions/wo
+00000120: 726b 666c 6f77 732f 7079 7468 6f6e 2d62  rkflows/python-b
+00000130: 6c61 636b 2d69 736f 7274 2e79 6d6c 2f62  lack-isort.yml/b
+00000140: 6164 6765 2e73 7667 223e 3c2f 613e 0a20  adge.svg"></a>. 
+00000150: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000170: 6869 6e61 7061 6e64 616d 616e 2f50 7950  hinapandaman/PyP
+00000180: 4446 466f 726d 2f61 6374 696f 6e73 2f77  DFForm/actions/w
+00000190: 6f72 6b66 6c6f 7773 2f70 7974 686f 6e2d  orkflows/python-
+000001a0: 7061 636b 6167 652e 796d 6c2f 6261 6467  package.yml/badg
+000001b0: 652e 7376 6722 3e3c 696d 6720 7372 633d  e.svg"><img src=
+000001c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000001d0: 636f 6d2f 6368 696e 6170 616e 6461 6d61  com/chinapandama
+000001e0: 6e2f 5079 5044 4646 6f72 6d2f 6163 7469  n/PyPDFForm/acti
+000001f0: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000200: 7468 6f6e 2d70 6163 6b61 6765 2e79 6d6c  thon-package.yml
+00000210: 2f62 6164 6765 2e73 7667 223e 3c2f 613e  /badge.svg"></a>
+00000220: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000230: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000240: 2f67 682f 6368 696e 6170 616e 6461 6d61  /gh/chinapandama
+00000250: 6e2f 5079 5044 4646 6f72 6d22 3e3c 696d  n/PyPDFForm"><im
+00000260: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+00000270: 6f64 6563 6f76 2e69 6f2f 6768 2f63 6869  odecov.io/gh/chi
+00000280: 6e61 7061 6e64 616d 616e 2f50 7950 4446  napandaman/PyPDF
+00000290: 466f 726d 2f62 7261 6e63 682f 6d61 7374  Form/branch/mast
+000002a0: 6572 2f67 7261 7068 2f62 6164 6765 2e73  er/graph/badge.s
+000002b0: 7667 3f74 6f6b 656e 3d43 5352 4c4e 3134  vg?token=CSRLN14
+000002c0: 4946 4522 3e3c 2f61 3e0a 2020 2020 3c61  IFE"></a>.    <a
+000002d0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000002e0: 6974 6875 622e 636f 6d2f 6368 696e 6170  ithub.com/chinap
+000002f0: 616e 6461 6d61 6e2f 5079 5044 4646 6f72  andaman/PyPDFFor
+00000300: 6d2f 6163 7469 6f6e 732f 776f 726b 666c  m/actions/workfl
+00000310: 6f77 732f 7079 7468 6f6e 2d70 7562 6c69  ows/python-publi
+00000320: 7368 2e79 6d6c 2f62 6164 6765 2e73 7667  sh.yml/badge.svg
+00000330: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000340: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000350: 6869 6e61 7061 6e64 616d 616e 2f50 7950  hinapandaman/PyP
+00000360: 4446 466f 726d 2f61 6374 696f 6e73 2f77  DFForm/actions/w
+00000370: 6f72 6b66 6c6f 7773 2f70 7974 686f 6e2d  orkflows/python-
+00000380: 7075 626c 6973 682e 796d 6c2f 6261 6467  publish.yml/badg
+00000390: 652e 7376 6722 3e3c 2f61 3e0a 3c2f 703e  e.svg"></a>.</p>
+000003a0: 0a0a 2323 2049 6e74 726f 6475 6374 696f  ..## Introductio
+000003b0: 6e0a 0a50 7950 4446 466f 726d 2069 7320  n..PyPDFForm is 
+000003c0: 6120 7075 7265 2050 7974 686f 6e20 6c69  a pure Python li
+000003d0: 6272 6172 7920 666f 7220 5044 4620 666f  brary for PDF fo
+000003e0: 726d 2070 726f 6365 7373 696e 672e 200a  rm processing. .
+000003f0: 4974 2061 6c6c 6f77 7320 6669 6c6c 696e  It allows fillin
+00000400: 6720 6120 5044 4620 666f 726d 2070 726f  g a PDF form pro
+00000410: 6772 616d 6d61 7469 6361 6c6c 7920 6279  grammatically by
+00000420: 2063 7265 6174 696e 6720 0a61 2050 7974   creating .a Pyt
+00000430: 686f 6e20 6469 6374 696f 6e61 7279 2077  hon dictionary w
+00000440: 6974 6820 6b65 7973 206d 6174 6368 696e  ith keys matchin
+00000450: 6720 6974 7320 616e 6e6f 7461 7465 6420  g its annotated 
+00000460: 6e61 6d65 7320 0a66 6f72 2065 6c65 6d65  names .for eleme
+00000470: 6e74 7320 6c69 6b65 2074 6578 7420 6669  nts like text fi
+00000480: 656c 6473 2061 6e64 2063 6865 636b 626f  elds and checkbo
+00000490: 7865 732e 2049 7420 616c 736f 2073 7570  xes. It also sup
+000004a0: 706f 7274 7320 6f74 6865 7220 6675 6e63  ports other func
+000004b0: 7469 6f6e 616c 6974 6965 7320 7375 6368  tionalities such
+000004c0: 2061 7320 0a64 7261 7769 6e67 2069 6d61   as .drawing ima
+000004d0: 6765 2061 6e64 206d 6572 6769 6e67 206d  ge and merging m
+000004e0: 756c 7469 706c 6520 5044 4673 2074 6f67  ultiple PDFs tog
+000004f0: 6574 6865 722e 0a0a 2323 2049 6e73 7461  ether...## Insta
+00000500: 6c6c 696e 670a 0a49 6e73 7461 6c6c 2075  lling..Install u
+00000510: 7369 6e67 205b 7069 705d 2868 7474 7073  sing [pip](https
+00000520: 3a2f 2f70 6970 2e70 7970 612e 696f 2f65  ://pip.pypa.io/e
+00000530: 6e2f 7374 6162 6c65 2f29 3a0a 0a60 6060  n/stable/):..```
+00000540: 7368 656c 6c20 7363 7269 7074 0a70 6970  shell script.pip
+00000550: 2069 6e73 7461 6c6c 2050 7950 4446 466f   install PyPDFFo
+00000560: 726d 0a60 6060 0a0a 2323 2051 7569 636b  rm.```..## Quick
+00000570: 2045 7861 6d70 6c65 0a0a 215b 5d28 6874   Example..![](ht
+00000580: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000590: 2f63 6869 6e61 7061 6e64 616d 616e 2f50  /chinapandaman/P
+000005a0: 7950 4446 466f 726d 2f62 6c6f 622f 6d61  yPDFForm/blob/ma
+000005b0: 7374 6572 2f64 656d 6f2e 6769 6629 0a0a  ster/demo.gif)..
+000005c0: 4120 7361 6d70 6c65 2050 4446 2066 6f72  A sample PDF for
+000005d0: 6d20 6361 6e20 6265 2066 6f75 6e64 205b  m can be found [
+000005e0: 6865 7265 5d28 6874 7470 733a 2f2f 6769  here](https://gi
+000005f0: 7468 7562 2e63 6f6d 2f63 6869 6e61 7061  thub.com/chinapa
+00000600: 6e64 616d 616e 2f50 7950 4446 466f 726d  ndaman/PyPDFForm
+00000610: 2f62 6c6f 622f 6d61 7374 6572 2f70 6466  /blob/master/pdf
+00000620: 5f73 616d 706c 6573 2f73 616d 706c 655f  _samples/sample_
+00000630: 7465 6d70 6c61 7465 2e70 6466 292e 2044  template.pdf). D
+00000640: 6f77 6e6c 6f61 6420 6974 2061 6e64 2074  ownload it and t
+00000650: 7279 3a0a 0a60 6060 7079 7468 6f6e 0a69  ry:..```python.i
+00000660: 6d70 6f72 7420 6f73 0a0a 6672 6f6d 2050  mport os..from P
+00000670: 7950 4446 466f 726d 2069 6d70 6f72 7420  yPDFForm import 
+00000680: 5079 5044 4646 6f72 6d0a 0a50 4154 485f  PyPDFForm..PATH_
+00000690: 544f 5f44 4f57 4e4c 4f41 4445 445f 5341  TO_DOWNLOADED_SA
+000006a0: 4d50 4c45 5f50 4446 5f46 4f52 4d20 3d20  MPLE_PDF_FORM = 
+000006b0: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
+000006c0: 2020 6f73 2e70 6174 682e 6578 7061 6e64    os.path.expand
+000006d0: 7573 6572 2822 7e2f 446f 776e 6c6f 6164  user("~/Download
+000006e0: 7322 292c 2022 7361 6d70 6c65 5f74 656d  s"), "sample_tem
+000006f0: 706c 6174 652e 7064 6622 0a29 2020 2320  plate.pdf".)  # 
+00000700: 4368 616e 6765 2074 6869 7320 746f 2077  Change this to w
+00000710: 6865 7265 2079 6f75 2064 6f77 6e6c 6f61  here you downloa
+00000720: 6465 6420 7468 6520 7361 6d70 6c65 2050  ded the sample P
+00000730: 4446 2066 6f72 6d0a 0a50 4154 485f 544f  DF form..PATH_TO
+00000740: 5f46 494c 4c45 445f 5044 465f 464f 524d  _FILLED_PDF_FORM
+00000750: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00000760: 0a20 2020 206f 732e 7061 7468 2e65 7870  .    os.path.exp
+00000770: 616e 6475 7365 7228 227e 2229 2c20 226f  anduser("~"), "o
+00000780: 7574 7075 742e 7064 6622 0a29 2020 2320  utput.pdf".)  # 
+00000790: 4368 616e 6765 2074 6869 7320 746f 2077  Change this to w
+000007a0: 6865 7265 2079 6f75 2077 6973 6820 746f  here you wish to
+000007b0: 2070 7574 2079 6f75 7220 6669 6c6c 6564   put your filled
+000007c0: 2050 4446 2066 6f72 6d0a 0a77 6974 6820   PDF form..with 
+000007d0: 6f70 656e 2850 4154 485f 544f 5f46 494c  open(PATH_TO_FIL
+000007e0: 4c45 445f 5044 465f 464f 524d 2c20 2277  LED_PDF_FORM, "w
+000007f0: 622b 2229 2061 7320 6f75 7470 7574 3a0a  b+") as output:.
+00000800: 2020 2020 6f75 7470 7574 2e77 7269 7465      output.write
+00000810: 280a 2020 2020 2020 2020 5079 5044 4646  (.        PyPDFF
+00000820: 6f72 6d28 5041 5448 5f54 4f5f 444f 574e  orm(PATH_TO_DOWN
+00000830: 4c4f 4144 4544 5f53 414d 504c 455f 5044  LOADED_SAMPLE_PD
+00000840: 465f 464f 524d 290a 2020 2020 2020 2020  F_FORM).        
+00000850: 2e66 696c 6c28 0a20 2020 2020 2020 2020  .fill(.         
+00000860: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000870: 2020 2020 2022 7465 7374 223a 2022 7465       "test": "te
+00000880: 7374 5f31 222c 0a20 2020 2020 2020 2020  st_1",.         
+00000890: 2020 2020 2020 2022 6368 6563 6b22 3a20         "check": 
+000008a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000008b0: 2020 2020 2020 2274 6573 745f 3222 3a20        "test_2": 
+000008c0: 2274 6573 745f 3222 2c0a 2020 2020 2020  "test_2",.      
+000008d0: 2020 2020 2020 2020 2020 2263 6865 636b            "check
+000008e0: 5f32 223a 2046 616c 7365 2c0a 2020 2020  _2": False,.    
+000008f0: 2020 2020 2020 2020 2020 2020 2274 6573              "tes
+00000900: 745f 3322 3a20 2274 6573 745f 3322 2c0a  t_3": "test_3",.
+00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000920: 2263 6865 636b 5f33 223a 2054 7275 652c  "check_3": True,
+00000930: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000940: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00000950: 2020 2e72 6561 6428 290a 2020 2020 290a    .read().    ).
+00000960: 6060 600a 0a41 6674 6572 2072 756e 6e69  ```..After runni
+00000970: 6e67 2074 6865 2061 626f 7665 2063 6f64  ng the above cod
+00000980: 6520 736e 6970 7065 7420 796f 7520 6361  e snippet you ca
+00000990: 6e20 6669 6e64 2060 6f75 7470 7574 2e70  n find `output.p
+000009a0: 6466 6020 6174 2074 6865 206c 6f63 6174  df` at the locat
+000009b0: 696f 6e20 796f 7520 7370 6563 6966 6965  ion you specifie
+000009c0: 642c 200a 616e 6420 6974 2073 686f 756c  d, .and it shoul
+000009d0: 6420 6c6f 6f6b 206c 696b 6520 5b74 6869  d look like [thi
+000009e0: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+000009f0: 622e 636f 6d2f 6368 696e 6170 616e 6461  b.com/chinapanda
+00000a00: 6d61 6e2f 5079 5044 4646 6f72 6d2f 626c  man/PyPDFForm/bl
+00000a10: 6f62 2f6d 6173 7465 722f 7064 665f 7361  ob/master/pdf_sa
+00000a20: 6d70 6c65 732f 7361 6d70 6c65 5f66 696c  mples/sample_fil
+00000a30: 6c65 642e 7064 6629 2e0a 0a23 2320 446f  led.pdf)...## Do
+00000a40: 6375 6d65 6e74 6174 696f 6e0a 0a5b 4578  cumentation..[Ex
+00000a50: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
+00000a60: 6769 7468 7562 2e63 6f6d 2f63 6869 6e61  github.com/china
+00000a70: 7061 6e64 616d 616e 2f50 7950 4446 466f  pandaman/PyPDFFo
+00000a80: 726d 2f62 6c6f 622f 6d61 7374 6572 2f64  rm/blob/master/d
+00000a90: 6f63 732f 6578 616d 706c 6573 2e6d 6429  ocs/examples.md)
+00000aa0: 0a0a 2323 2048 6f77 2074 6f20 436f 6e74  ..## How to Cont
+00000ab0: 7269 6275 7465 0a0a 4966 2079 6f75 2077  ribute..If you w
+00000ac0: 6973 6820 746f 2069 6d70 726f 7665 2074  ish to improve t
+00000ad0: 6869 7320 6c69 6272 6172 792c 2074 6865  his library, the
+00000ae0: 7265 2069 7320 6f6e 6520 7370 6563 6966  re is one specif
+00000af0: 6963 2077 6179 2079 6f75 2063 616e 2063  ic way you can c
+00000b00: 6f6e 7472 6962 7574 6520 0a6f 6e20 746f  ontribute .on to
+00000b10: 7020 6f66 2074 6865 2075 7375 616c 206f  p of the usual o
+00000b20: 7065 6e20 736f 7572 6365 2070 726f 6a65  pen source proje
+00000b30: 6374 206e 6f72 6d73 2073 7563 6820 6173  ct norms such as
+00000b40: 2069 7373 7565 7320 616e 6420 7075 6c6c   issues and pull
+00000b50: 2072 6571 7565 7374 732e 0a0a 4974 2069   requests...It i
+00000b60: 7320 6469 6666 6963 756c 7420 746f 206d  s difficult to m
+00000b70: 616b 6520 7375 7265 2074 6861 7420 7468  ake sure that th
+00000b80: 6520 6c69 6272 6172 7920 7375 7070 6f72  e library suppor
+00000b90: 7473 2061 6c6c 2074 6865 2050 4446 2066  ts all the PDF f
+00000ba0: 6f72 6d20 6372 6561 7469 6e67 2074 6f6f  orm creating too
+00000bb0: 6c73 206f 7574 200a 7468 6572 652e 2053  ls out .there. S
+00000bc0: 6f20 6966 2079 6f75 2072 756e 2069 6e74  o if you run int
+00000bd0: 6f20 6120 6361 7365 2077 6865 7265 2074  o a case where t
+00000be0: 6865 206c 6962 7261 7279 2064 6f65 7320  he library does 
+00000bf0: 6e6f 7420 776f 726b 2066 6f72 2063 6572  not work for cer
+00000c00: 7461 696e 2050 4446 2066 6f72 6d73 2063  tain PDF forms c
+00000c10: 7265 6174 6564 2062 7920 0a63 6572 7461  reated by .certa
+00000c20: 696e 2074 6f6f 6c73 2c20 6665 656c 2066  in tools, feel f
+00000c30: 7265 6520 746f 206f 7065 6e20 616e 2069  ree to open an i
+00000c40: 7373 7565 2077 6974 6820 7468 6520 7072  ssue with the pr
+00000c50: 6f62 6c65 6d61 7469 6320 5044 4620 666f  oblematic PDF fo
+00000c60: 726d 2061 7474 6163 6865 642e 2049 2077  rm attached. I w
+00000c70: 696c 6c20 7365 656b 200a 746f 206d 616b  ill seek .to mak
+00000c80: 6520 7468 6520 6c69 6272 6172 7920 7375  e the library su
+00000c90: 7070 6f72 7420 7468 6520 6174 7461 6368  pport the attach
+00000ca0: 6564 2050 4446 2066 6f72 6d20 6173 2077  ed PDF form as w
+00000cb0: 656c 6c20 6173 2074 6865 2074 6f6f 6c20  ell as the tool 
+00000cc0: 7573 6564 2074 6f20 6372 6561 7465 2069  used to create i
+00000cd0: 742e 0a                                  t..
```

### Comparing `PyPDFForm-1.2.4/setup.py` & `PyPDFForm-1.2.5/setup.py`

 * *Files identical despite different names*

