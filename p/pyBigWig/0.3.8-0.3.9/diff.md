# Comparing `tmp/pyBigWig-0.3.8.tar.gz` & `tmp/pyBigWig-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyBigWig-0.3.8.tar", last modified: Wed Dec 13 14:53:02 2017, max compression
+gzip compressed data, was "dist/pyBigWig-0.3.9.tar", last modified: Mon Dec 18 08:50:31 2017, max compression
```

## Comparing `pyBigWig-0.3.8.tar` & `pyBigWig-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/
-drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/libBigWig/
--rw-r-----   0 ryan      (1038) bioinfo    (532)     1078 2015-11-16 14:07:25.000000 pyBigWig-0.3.8/libBigWig/LICENSE
--rw-r-----   0 ryan      (1038) bioinfo    (532)    12559 2017-09-21 07:02:17.000000 pyBigWig-0.3.8/libBigWig/README.md
--rw-r-----   0 ryan      (1038) bioinfo    (532)    29467 2017-11-03 11:03:01.000000 pyBigWig-0.3.8/libBigWig/bigWig.h
--rw-r-----   0 ryan      (1038) bioinfo    (532)     4431 2017-11-03 11:03:01.000000 pyBigWig-0.3.8/libBigWig/bigWigIO.h
--rw-r-----   0 ryan      (1038) bioinfo    (532)     2910 2017-03-29 14:40:37.000000 pyBigWig-0.3.8/libBigWig/bwCommon.h
--rw-r-----   0 ryan      (1038) bioinfo    (532)    13543 2017-11-03 11:03:01.000000 pyBigWig-0.3.8/libBigWig/bwRead.c
--rw-r-----   0 ryan      (1038) bioinfo    (532)    13625 2017-09-21 07:02:17.000000 pyBigWig-0.3.8/libBigWig/bwStats.c
--rw-r-----   0 ryan      (1038) bioinfo    (532)    26278 2017-09-21 07:02:17.000000 pyBigWig-0.3.8/libBigWig/bwValues.c
--rw-r-----   0 ryan      (1038) bioinfo    (532)     3836 2017-03-29 14:40:37.000000 pyBigWig-0.3.8/libBigWig/bwValues.h
--rw-r-----   0 ryan      (1038) bioinfo    (532)    46766 2017-09-21 07:02:17.000000 pyBigWig-0.3.8/libBigWig/bwWrite.c
--rw-r-----   0 ryan      (1038) bioinfo    (532)    10474 2017-11-03 11:03:01.000000 pyBigWig-0.3.8/libBigWig/io.c
-drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/pyBigWig.egg-info/
--rw-r-----   0 ryan      (1038) bioinfo    (532)      381 2017-12-13 14:52:55.000000 pyBigWig-0.3.8/pyBigWig.egg-info/SOURCES.txt
-drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/pyBigWigTest/
--rw-r-----   0 ryan      (1038) bioinfo    (532)        0 2015-11-26 21:53:35.000000 pyBigWig-0.3.8/pyBigWigTest/__init__.py
--rw-r-----   0 ryan      (1038) bioinfo    (532)    27148 2017-11-03 12:41:09.000000 pyBigWig-0.3.8/pyBigWigTest/test.bigBed
--rw-r-----   0 ryan      (1038) bioinfo    (532)    12966 2015-11-26 21:53:35.000000 pyBigWig-0.3.8/pyBigWigTest/test.bw
--rw-r-----   0 ryan      (1038) bioinfo    (532)    10687 2017-11-03 12:41:09.000000 pyBigWig-0.3.8/pyBigWigTest/test.py
--rw-r-----   0 ryan      (1038) bioinfo    (532)     1078 2015-10-09 11:11:26.000000 pyBigWig-0.3.8/LICENSE.txt
--rw-r-----   0 ryan      (1038) bioinfo    (532)      118 2016-11-22 08:18:05.000000 pyBigWig-0.3.8/MANIFEST.in
--rw-r-----   0 ryan      (1038) bioinfo    (532)    18572 2017-09-21 07:02:17.000000 pyBigWig-0.3.8/README.md
--rw-r-----   0 ryan      (1038) bioinfo    (532)    51776 2017-12-13 14:41:18.000000 pyBigWig-0.3.8/pyBigWig.c
--rw-r-----   0 ryan      (1038) bioinfo    (532)    18434 2017-12-13 14:44:35.000000 pyBigWig-0.3.8/pyBigWig.h
--rw-r-----   0 ryan      (1038) bioinfo    (532)       79 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/setup.cfg
--rwxr-x---   0 ryan      (1038) bioinfo    (532)     3541 2017-12-13 14:43:58.000000 pyBigWig-0.3.8/setup.py
--rw-r-----   0 ryan      (1038) bioinfo    (532)      416 2017-12-13 14:52:56.000000 pyBigWig-0.3.8/PKG-INFO
+drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/
+drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/libBigWig/
+-rw-r-----   0 ryan      (1038) bioinfo    (532)     1078 2015-11-16 14:07:25.000000 pyBigWig-0.3.9/libBigWig/LICENSE
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    12559 2017-09-21 07:02:17.000000 pyBigWig-0.3.9/libBigWig/README.md
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    29467 2017-11-03 11:03:01.000000 pyBigWig-0.3.9/libBigWig/bigWig.h
+-rw-r-----   0 ryan      (1038) bioinfo    (532)     4431 2017-11-03 11:03:01.000000 pyBigWig-0.3.9/libBigWig/bigWigIO.h
+-rw-r-----   0 ryan      (1038) bioinfo    (532)     2910 2017-03-29 14:40:37.000000 pyBigWig-0.3.9/libBigWig/bwCommon.h
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    13543 2017-11-03 11:03:01.000000 pyBigWig-0.3.9/libBigWig/bwRead.c
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    13625 2017-09-21 07:02:17.000000 pyBigWig-0.3.9/libBigWig/bwStats.c
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    26278 2017-09-21 07:02:17.000000 pyBigWig-0.3.9/libBigWig/bwValues.c
+-rw-r-----   0 ryan      (1038) bioinfo    (532)     3836 2017-03-29 14:40:37.000000 pyBigWig-0.3.9/libBigWig/bwValues.h
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    46766 2017-09-21 07:02:17.000000 pyBigWig-0.3.9/libBigWig/bwWrite.c
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    10474 2017-11-03 11:03:01.000000 pyBigWig-0.3.9/libBigWig/io.c
+drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/pyBigWig.egg-info/
+-rw-r-----   0 ryan      (1038) bioinfo    (532)      381 2017-12-18 08:50:20.000000 pyBigWig-0.3.9/pyBigWig.egg-info/SOURCES.txt
+drwxr-x---   0 ryan      (1038) bioinfo    (532)        0 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/pyBigWigTest/
+-rw-r-----   0 ryan      (1038) bioinfo    (532)        0 2015-11-26 21:53:35.000000 pyBigWig-0.3.9/pyBigWigTest/__init__.py
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    27148 2017-11-03 12:41:09.000000 pyBigWig-0.3.9/pyBigWigTest/test.bigBed
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    12966 2015-11-26 21:53:35.000000 pyBigWig-0.3.9/pyBigWigTest/test.bw
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    10687 2017-11-03 12:41:09.000000 pyBigWig-0.3.9/pyBigWigTest/test.py
+-rw-r-----   0 ryan      (1038) bioinfo    (532)     1078 2015-10-09 11:11:26.000000 pyBigWig-0.3.9/LICENSE.txt
+-rw-r-----   0 ryan      (1038) bioinfo    (532)      118 2016-11-22 08:18:05.000000 pyBigWig-0.3.9/MANIFEST.in
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    18572 2017-09-21 07:02:17.000000 pyBigWig-0.3.9/README.md
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    51780 2017-12-18 08:03:25.000000 pyBigWig-0.3.9/pyBigWig.c
+-rw-r-----   0 ryan      (1038) bioinfo    (532)    18434 2017-12-18 08:35:44.000000 pyBigWig-0.3.9/pyBigWig.h
+-rw-r-----   0 ryan      (1038) bioinfo    (532)       79 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/setup.cfg
+-rwxr-x---   0 ryan      (1038) bioinfo    (532)     3541 2017-12-18 08:35:56.000000 pyBigWig-0.3.9/setup.py
+-rw-r-----   0 ryan      (1038) bioinfo    (532)      416 2017-12-18 08:50:22.000000 pyBigWig-0.3.9/PKG-INFO
```

### Comparing `pyBigWig-0.3.8/libBigWig/LICENSE` & `pyBigWig-0.3.9/libBigWig/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/README.md` & `pyBigWig-0.3.9/libBigWig/README.md`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bigWig.h` & `pyBigWig-0.3.9/libBigWig/bigWig.h`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bigWigIO.h` & `pyBigWig-0.3.9/libBigWig/bigWigIO.h`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwCommon.h` & `pyBigWig-0.3.9/libBigWig/bwCommon.h`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwRead.c` & `pyBigWig-0.3.9/libBigWig/bwRead.c`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwStats.c` & `pyBigWig-0.3.9/libBigWig/bwStats.c`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwValues.c` & `pyBigWig-0.3.9/libBigWig/bwValues.c`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwValues.h` & `pyBigWig-0.3.9/libBigWig/bwValues.h`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/bwWrite.c` & `pyBigWig-0.3.9/libBigWig/bwWrite.c`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/libBigWig/io.c` & `pyBigWig-0.3.9/libBigWig/io.c`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/pyBigWigTest/test.bigBed` & `pyBigWig-0.3.9/pyBigWigTest/test.bigBed`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/pyBigWigTest/test.bw` & `pyBigWig-0.3.9/pyBigWigTest/test.bw`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/pyBigWigTest/test.py` & `pyBigWig-0.3.9/pyBigWigTest/test.py`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/LICENSE.txt` & `pyBigWig-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/README.md` & `pyBigWig-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyBigWig-0.3.8/pyBigWig.c` & `pyBigWig-0.3.9/pyBigWig.c`

 * *Files 0% similar despite different names*

```diff
@@ -924,22 +924,22 @@
 
         for(i=0; i<sz; i++) {
 #ifdef WITHNUMPY
             if(PyArray_Check(chroms)) {
                 foo = PyArray_GETPTR1((PyArrayObject*)chroms, i);
                 tmp = PyArray_GETITEM((PyArrayObject*)chroms, foo);
                 tid = bwGetTid(bw, PyString_AsString(tmp));
+                Py_DECREF(tmp);
             } else {
 #endif
                 tmp = PyList_GetItem(chroms, i);
                 tid = bwGetTid(bw, PyString_AsString(tmp));
 #ifdef WITHNUMPY
             }
 #endif
-            Py_DECREF(tmp);
             if(tid != (uint32_t) self->lastTid) return 0;
         }
 
 #ifdef WITHNUMPY
         if(PyArray_Check(starts)) {
             ustart = getNumpyU32((PyArrayObject*)starts, 0);
         } else {
```

### Comparing `pyBigWig-0.3.8/pyBigWig.h` & `pyBigWig-0.3.9/pyBigWig.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include <Python.h>
 #include <structmember.h>
 #include "bigWig.h"
 
-#define pyBigWigVersion "0.3.8"
+#define pyBigWigVersion "0.3.9"
 
 typedef struct {
     PyObject_HEAD
     bigWigFile_t *bw;
     int32_t lastTid; //The TID of the last written entry (or -1)
     uint32_t lastSpan; //The span of the last written entry (if applicable)
     uint32_t lastStep; //The step of the last written entry (if applicable)
```

### Comparing `pyBigWig-0.3.8/setup.py` & `pyBigWig-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,20 +54,20 @@
                     sources = srcs,
                     libraries = libs,
                     library_dirs = additional_libs, 
                     define_macros = defines,
                     include_dirs = include_dirs)
 
 setup(name = 'pyBigWig',
-       version = '0.3.8',
+       version = '0.3.9',
        description = 'A package for accessing bigWig files using libBigWig',
        author = "Devon P. Ryan",
        author_email = "ryan@ie-freiburg.mpg.de",
        url = "https://github.com/dpryan79/pyBigWig",
-       download_url = "https://github.com/dpryan79/pyBigWig/tarball/0.3.8",
+       download_url = "https://github.com/dpryan79/pyBigWig/tarball/0.3.9",
        keywords = ["bioinformatics", "bigWig", "bigBed"],
        classifier = ["Development Status :: 5 - Production/Stable",
                      "Intended Audience :: Developers",
                      "License :: OSI Approved",
                      "Programming Language :: C",
                      "Programming Language :: Python",
                      "Programming Language :: Python :: 2",
```

