# Comparing `tmp/daqp-0.4.0.tar.gz` & `tmp/daqp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daqp-0.4.0.tar", last modified: Thu Apr  6 14:38:36 2023, max compression
+gzip compressed data, was "daqp-0.4.1.tar", last modified: Fri Apr  7 15:49:37 2023, max compression
```

## Comparing `daqp-0.4.0.tar` & `daqp-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:38:36.020512 daqp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-06 14:38:35.000000 daqp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-06 14:38:36.016512 daqp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-06 14:29:56.000000 daqp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:38:36.012512 daqp-0.4.0/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:38:36.016512 daqp-0.4.0/csrc/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/api.c
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/auxiliary.c
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/bnb.c
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/daqp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/daqp_prox.c
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/factorization.c
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-04-06 14:29:56.000000 daqp-0.4.0/csrc/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (123)   808116 2023-04-06 14:38:35.000000 daqp-0.4.0/daqp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:38:36.016512 daqp-0.4.0/daqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-06 14:38:36.000000 daqp-0.4.0/daqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-06 14:38:36.000000 daqp-0.4.0/daqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:38:36.000000 daqp-0.4.0/daqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:38:35.000000 daqp-0.4.0/daqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 14:38:36.000000 daqp-0.4.0/daqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-06 14:29:56.000000 daqp-0.4.0/daqp.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-06 14:29:56.000000 daqp-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 14:38:36.020512 daqp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-06 14:29:56.000000 daqp-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 15:49:36.000000 daqp-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 15:40:58.000000 daqp-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 15:49:37.131278 daqp-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 15:40:58.000000 daqp-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.127278 daqp-0.4.1/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/auxiliary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/bnb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/daqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/daqp_prox.h
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/factorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/csrc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/auxiliary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/bnb.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/daqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/daqp_prox.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/factorization.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)   835898 2023-04-07 15:49:36.000000 daqp-0.4.1/daqp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/daqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:49:36.000000 daqp-0.4.1/daqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-07 15:40:58.000000 daqp-0.4.1/daqp.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 15:40:58.000000 daqp-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:49:37.131278 daqp-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-07 15:40:58.000000 daqp-0.4.1/setup.py
```

### Comparing `daqp-0.4.0/LICENSE` & `daqp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/PKG-INFO` & `daqp-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daqp
-Version: 0.4.0
+Version: 0.4.1
 Summary: DAQP: A dual active-set QP solver
 Home-page: http://github.com/darnstrom/daqp
 Author: Daniel Arnström
 Author-email: daniel.arnstrom@liu.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daqp-0.4.0/README.md` & `daqp-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/api.c` & `daqp-0.4.1/csrc/src/api.c`

 * *Files 5% similar despite different names*

```diff
@@ -30,73 +30,74 @@
     daqp_extract_result(res,work);
     // Add time to result
 #ifdef PROFILING
     res->solve_time = get_time(&timer);
 #else
     res->solve_time = 0; 
 #endif
-    res->setup_time = 0; 
 }
 
 // Setup and solve problem
 void daqp_quadprog(DAQPResult *res, DAQPProblem* qp, DAQPSettings *settings){
     int setup_flag;
-    c_float setup_time=0;
 
     DAQPWorkspace work;
-    work.settings = NULL;
-    setup_flag = setup_daqp(qp,&work,&setup_time);
-    if(settings!=NULL) 
-        *(work.settings) = *settings; 
+    work.settings = settings;
+    setup_flag = setup_daqp(qp,&work,&(res->setup_time));
+    res->exitflag = setup_flag;
 
-    if(setup_flag >= 0)
+    if(setup_flag >= 0){
         daqp_solve(res,&work);
-    else
-        res->exitflag = setup_flag;
-
-    // Add setup time to result 
-    res->setup_time = setup_time; 
-    // Free memory
-    free_daqp_workspace(&work);
-    free_daqp_ldp(&work);
+        // Free memory
+        if(settings != NULL) work.settings = NULL;
+        free_daqp_workspace(&work);
+        free_daqp_ldp(&work);
+    }
 }
 
 // Setup workspace and transform QP to LDP
 int setup_daqp(DAQPProblem* qp, DAQPWorkspace *work, c_float* setup_time){
     int errorflag;
+    int own_settings=1;
 #ifdef PROFILING
     DAQPtimer timer;
     if(setup_time != NULL){
         *setup_time = 0; // in case setup fails 
         tic(&timer);
     }
 #endif
     // Check if QP is well-posed
     //validate_QP(qp);
 
-
-    //
+    // Count number of soft constraints
+    // (to account for it in allocation)
     int ns = 0;
     for(int i = 0; i < qp->m ; i++)
         if(qp->sense[i] & SOFT) ns++;
     // Setup workspace
-    allocate_daqp_settings(work);
+    if(work->settings == NULL)
+        allocate_daqp_settings(work);
+    else
+        own_settings = 0;
     allocate_daqp_workspace(work,qp->n,ns);
     errorflag = setup_daqp_ldp(work,qp);
     if(errorflag < 0){
+        if(own_settings==0) work->settings = NULL;
         free_daqp_workspace(work);
         return errorflag;
     }
     errorflag = setup_daqp_bnb(work,qp->bin_ids,qp->nb, ns);
     if(errorflag < 0){
+        if(own_settings==0) work->settings = NULL;
         free_daqp_workspace(work);
         return errorflag;
     }
     errorflag = activate_constraints(work);
     if(errorflag < 0){
+        if(own_settings==0) work->settings = NULL;
         free_daqp_workspace(work);
         return errorflag;
     }
 #ifdef PROFILING
     if(setup_time != NULL){
         toc(&timer);
         *setup_time = get_time(&timer);
```

### Comparing `daqp-0.4.0/csrc/src/auxiliary.c` & `daqp-0.4.1/csrc/src/auxiliary.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/bnb.c` & `daqp-0.4.1/csrc/src/bnb.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/daqp.c` & `daqp-0.4.1/csrc/src/daqp.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/daqp_prox.c` & `daqp-0.4.1/csrc/src/daqp_prox.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/factorization.c` & `daqp-0.4.1/csrc/src/factorization.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/csrc/src/utils.c` & `daqp-0.4.1/csrc/src/utils.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.0/daqp.c` & `daqp-0.4.1/daqp.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "csrc/include/api.h",
+            "csrc/include/constants.h",
             "csrc/include/types.h"
         ],
         "extra_compile_args": [
-            "-O3"
+            "-O3",
+            "-DPROFILING"
         ],
         "include_dirs": [
             "csrc/include"
         ],
         "library_dirs": [
             "."
         ],
@@ -772,14 +774,15 @@
 #endif
 
 #define __PYX_HAVE__daqp
 #define __PYX_HAVE_API__daqp
 /* Early includes */
 #include "types.h"
 #include "api.h"
+#include "constants.h"
 #include "pythread.h"
 #include <string.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include "pystate.h"
 #ifdef _OPENMP
 #include <omp.h>
@@ -1301,14 +1304,40 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* MemviewSliceInit.proto */
+#define __Pyx_BUF_MAX_NDIMS %(BUF_MAX_NDIMS)d
+#define __Pyx_MEMVIEW_DIRECT   1
+#define __Pyx_MEMVIEW_PTR      2
+#define __Pyx_MEMVIEW_FULL     4
+#define __Pyx_MEMVIEW_CONTIG   8
+#define __Pyx_MEMVIEW_STRIDED  16
+#define __Pyx_MEMVIEW_FOLLOW   32
+#define __Pyx_IS_C_CONTIG 1
+#define __Pyx_IS_F_CONTIG 2
+static int __Pyx_init_memviewslice(
+                struct __pyx_memoryview_obj *memview,
+                int ndim,
+                __Pyx_memviewslice *memviewslice,
+                int memview_is_new_reference);
+static CYTHON_INLINE int __pyx_add_acquisition_count_locked(
+    __pyx_atomic_int *acquisition_count, PyThread_type_lock lock);
+static CYTHON_INLINE int __pyx_sub_acquisition_count_locked(
+    __pyx_atomic_int *acquisition_count, PyThread_type_lock lock);
+#define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
+#define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
+#define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
+#define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
+static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
+static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
@@ -1414,40 +1443,14 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* MemviewSliceInit.proto */
-#define __Pyx_BUF_MAX_NDIMS %(BUF_MAX_NDIMS)d
-#define __Pyx_MEMVIEW_DIRECT   1
-#define __Pyx_MEMVIEW_PTR      2
-#define __Pyx_MEMVIEW_FULL     4
-#define __Pyx_MEMVIEW_CONTIG   8
-#define __Pyx_MEMVIEW_STRIDED  16
-#define __Pyx_MEMVIEW_FOLLOW   32
-#define __Pyx_IS_C_CONTIG 1
-#define __Pyx_IS_F_CONTIG 2
-static int __Pyx_init_memviewslice(
-                struct __pyx_memoryview_obj *memview,
-                int ndim,
-                __Pyx_memviewslice *memviewslice,
-                int memview_is_new_reference);
-static CYTHON_INLINE int __pyx_add_acquisition_count_locked(
-    __pyx_atomic_int *acquisition_count, PyThread_type_lock lock);
-static CYTHON_INLINE int __pyx_sub_acquisition_count_locked(
-    __pyx_atomic_int *acquisition_count, PyThread_type_lock lock);
-#define __pyx_get_slice_count_pointer(memview) (memview->acquisition_count_aligned_p)
-#define __pyx_get_slice_count(memview) (*__pyx_get_slice_count_pointer(memview))
-#define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
-#define __PYX_XDEC_MEMVIEW(slice, have_gil) __Pyx_XDEC_MEMVIEW(slice, have_gil, __LINE__)
-static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
-static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *, int, int);
-
 /* RaiseTooManyValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
 
 /* IterFinish.proto */
@@ -1823,48 +1826,48 @@
                 int ndim,
                 __Pyx_TypeInfo *dtype,
                 __Pyx_BufFmt_StackElem stack[],
                 __Pyx_memviewslice *memviewslice,
                 PyObject *original_obj);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_double(PyObject *, int writable_flag);
-
-/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *, int writable_flag);
 
-/* MemviewDtypeToObject.proto */
-static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
-static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
-
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_double(PyObject *, int writable_flag);
+
+/* MemviewDtypeToObject.proto */
+static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
+static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
+
+/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
 
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
+/* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
@@ -1962,26 +1965,28 @@
 static const char __pyx_k_lam[] = "lam";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_res[] = "res";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_daqp[] = "daqp";
 static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_fill[] = "fill";
 static const char __pyx_k_info[] = "info";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_class[] = "__class__";
+static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_nodes[] = "nodes";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_sense[] = "sense";
 static const char __pyx_k_shape[] = "shape";
@@ -2001,32 +2006,46 @@
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_asarray[] = "asarray";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_problem[] = "problem";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_daqp_pyx[] = "daqp.pyx";
+static const char __pyx_k_dual_tol[] = "dual_tol";
+static const char __pyx_k_eps_prox[] = "eps_prox";
+static const char __pyx_k_eta_prox[] = "eta_prox";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
+static const char __pyx_k_rho_soft[] = "rho_soft";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_settings[] = "settings";
+static const char __pyx_k_zero_tol[] = "zero_tol";
 static const char __pyx_k_TypeError[] = "TypeError";
+static const char __pyx_k_cycle_tol[] = "cycle_tol";
 static const char __pyx_k_enumerate[] = "enumerate";
+static const char __pyx_k_pivot_tol[] = "pivot_tol";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_abs_subopt[] = "abs_subopt";
+static const char __pyx_k_fval_bound[] = "fval_bound";
+static const char __pyx_k_iter_limit[] = "iter_limit";
 static const char __pyx_k_iterations[] = "iterations";
+static const char __pyx_k_primal_tol[] = "primal_tol";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_rel_subopt[] = "rel_subopt";
 static const char __pyx_k_setup_time[] = "setup_time";
 static const char __pyx_k_solve_time[] = "solve_time";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_bin_ids_cand[] = "bin_ids_cand";
+static const char __pyx_k_progress_tol[] = "progress_tol";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
@@ -2080,46 +2099,55 @@
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
+static PyObject *__pyx_n_s_abs_subopt;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_asarray;
 static PyObject *__pyx_n_s_ascontiguousarray;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bin_ids_cand;
 static PyObject *__pyx_n_s_blower;
 static PyObject *__pyx_n_s_bupper;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
+static PyObject *__pyx_n_s_cycle_tol;
 static PyObject *__pyx_n_s_daqp;
 static PyObject *__pyx_kp_s_daqp_pyx;
 static PyObject *__pyx_n_s_dict;
+static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
+static PyObject *__pyx_n_s_dual_tol;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
+static PyObject *__pyx_n_s_eps_prox;
 static PyObject *__pyx_n_s_error;
+static PyObject *__pyx_n_s_eta_prox;
 static PyObject *__pyx_n_s_f;
+static PyObject *__pyx_n_s_fill;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
+static PyObject *__pyx_n_s_fval_bound;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_info;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
+static PyObject *__pyx_n_s_iter_limit;
 static PyObject *__pyx_n_s_iterations;
 static PyObject *__pyx_n_s_lam;
 static PyObject *__pyx_n_s_m;
 static PyObject *__pyx_n_s_mA;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
@@ -2133,31 +2161,37 @@
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_nodes;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
+static PyObject *__pyx_n_s_pivot_tol;
+static PyObject *__pyx_n_s_primal_tol;
 static PyObject *__pyx_n_s_problem;
+static PyObject *__pyx_n_s_progress_tol;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_n_s_rel_subopt;
 static PyObject *__pyx_n_s_res;
+static PyObject *__pyx_n_s_rho_soft;
 static PyObject *__pyx_n_s_sense;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_settings;
 static PyObject *__pyx_n_s_setup_time;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_solve;
 static PyObject *__pyx_n_s_solve_time;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
@@ -2169,16 +2203,17 @@
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_x;
+static PyObject *__pyx_n_s_zero_tol;
 static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_4daqp_solve(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_H, __Pyx_memviewslice __pyx_v_f, __Pyx_memviewslice __pyx_v_A, __Pyx_memviewslice __pyx_v_bupper, __Pyx_memviewslice __pyx_v_blower, __Pyx_memviewslice __pyx_v_sense); /* proto */
+static PyObject *__pyx_pf_4daqp_solve(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_H, __Pyx_memviewslice __pyx_v_f, __Pyx_memviewslice __pyx_v_A, __Pyx_memviewslice __pyx_v_bupper, __Pyx_memviewslice __pyx_v_blower, __Pyx_memviewslice __pyx_v_sense, PyObject *__pyx_v_primal_tol, PyObject *__pyx_v_dual_tol, PyObject *__pyx_v_zero_tol, PyObject *__pyx_v_pivot_tol, PyObject *__pyx_v_progress_tol, PyObject *__pyx_v_cycle_tol, PyObject *__pyx_v_iter_limit, PyObject *__pyx_v_fval_bound, PyObject *__pyx_v_eps_prox, PyObject *__pyx_v_eta_prox, PyObject *__pyx_v_rho_soft, PyObject *__pyx_v_rel_subopt, PyObject *__pyx_v_abs_subopt); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2223,75 +2258,141 @@
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__15;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_k_;
+static PyObject *__pyx_k__2;
+static PyObject *__pyx_k__3;
+static PyObject *__pyx_k__4;
+static PyObject *__pyx_k__5;
+static PyObject *__pyx_k__6;
+static PyObject *__pyx_k__7;
+static PyObject *__pyx_k__8;
+static PyObject *__pyx_k__9;
+static PyObject *__pyx_k__10;
+static PyObject *__pyx_k__11;
+static PyObject *__pyx_k__12;
+static __Pyx_memviewslice __pyx_k__13;
+static __Pyx_memviewslice __pyx_k__14;
+static PyObject *__pyx_slice__29;
+static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_tuple__32;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__34;
+static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__38;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__40;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_codeobj__35;
+static PyObject *__pyx_codeobj__42;
 /* Late includes */
 
 /* "daqp.pyx":4
  * cimport daqp
  * 
- * def solve(double[:, :] H, double[:] f, double[:, :] A, double[:] bupper, double[:] blower, int[:] sense):             # <<<<<<<<<<<<<<
- *     cdef int n,m,ms,nb
- *     cdef int* bin_ids_cand
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4daqp_1solve(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_4daqp_1solve = {"solve", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4daqp_1solve, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_4daqp_1solve(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_H = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_f = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_A = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bupper = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_blower = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sense = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_primal_tol = 0;
+  PyObject *__pyx_v_dual_tol = 0;
+  PyObject *__pyx_v_zero_tol = 0;
+  PyObject *__pyx_v_pivot_tol = 0;
+  PyObject *__pyx_v_progress_tol = 0;
+  PyObject *__pyx_v_cycle_tol = 0;
+  PyObject *__pyx_v_iter_limit = 0;
+  PyObject *__pyx_v_fval_bound = 0;
+  PyObject *__pyx_v_eps_prox = 0;
+  PyObject *__pyx_v_eta_prox = 0;
+  PyObject *__pyx_v_rho_soft = 0;
+  PyObject *__pyx_v_rel_subopt = 0;
+  PyObject *__pyx_v_abs_subopt = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("solve (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H,&__pyx_n_s_f,&__pyx_n_s_A,&__pyx_n_s_bupper,&__pyx_n_s_blower,&__pyx_n_s_sense,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_H,&__pyx_n_s_f,&__pyx_n_s_A,&__pyx_n_s_bupper,&__pyx_n_s_blower,&__pyx_n_s_sense,&__pyx_n_s_primal_tol,&__pyx_n_s_dual_tol,&__pyx_n_s_zero_tol,&__pyx_n_s_pivot_tol,&__pyx_n_s_progress_tol,&__pyx_n_s_cycle_tol,&__pyx_n_s_iter_limit,&__pyx_n_s_fval_bound,&__pyx_n_s_eps_prox,&__pyx_n_s_eta_prox,&__pyx_n_s_rho_soft,&__pyx_n_s_rel_subopt,&__pyx_n_s_abs_subopt,0};
+    PyObject* values[19] = {0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0};
+    values[6] = __pyx_k_;
+    values[7] = __pyx_k__2;
+    values[8] = __pyx_k__3;
+    values[9] = __pyx_k__4;
+    values[10] = __pyx_k__5;
+    values[11] = __pyx_k__6;
+    values[12] = __pyx_k__7;
+    values[13] = __pyx_k__8;
+    values[14] = ((PyObject *)__pyx_int_0);
+    values[15] = __pyx_k__9;
+    values[16] = __pyx_k__10;
+    values[17] = __pyx_k__11;
+    values[18] = __pyx_k__12;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case 19: values[18] = PyTuple_GET_ITEM(__pyx_args, 18);
+        CYTHON_FALLTHROUGH;
+        case 18: values[17] = PyTuple_GET_ITEM(__pyx_args, 17);
+        CYTHON_FALLTHROUGH;
+        case 17: values[16] = PyTuple_GET_ITEM(__pyx_args, 16);
+        CYTHON_FALLTHROUGH;
+        case 16: values[15] = PyTuple_GET_ITEM(__pyx_args, 15);
+        CYTHON_FALLTHROUGH;
+        case 15: values[14] = PyTuple_GET_ITEM(__pyx_args, 14);
+        CYTHON_FALLTHROUGH;
+        case 14: values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
+        CYTHON_FALLTHROUGH;
+        case 13: values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
+        CYTHON_FALLTHROUGH;
+        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        CYTHON_FALLTHROUGH;
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -2308,684 +2409,1038 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_H)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, 1); __PYX_ERR(0, 4, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("solve", 0, 4, 19, 1); __PYX_ERR(0, 4, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_A)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, 2); __PYX_ERR(0, 4, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("solve", 0, 4, 19, 2); __PYX_ERR(0, 4, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bupper)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, 3); __PYX_ERR(0, 4, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("solve", 0, 4, 19, 3); __PYX_ERR(0, 4, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
-        if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_blower)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, 4); __PYX_ERR(0, 4, __pyx_L3_error)
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_blower);
+          if (value) { values[4] = value; kw_args--; }
         }
         CYTHON_FALLTHROUGH;
         case  5:
-        if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sense)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, 5); __PYX_ERR(0, 4, __pyx_L3_error)
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sense);
+          if (value) { values[5] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_primal_tol);
+          if (value) { values[6] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dual_tol);
+          if (value) { values[7] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_zero_tol);
+          if (value) { values[8] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  9:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pivot_tol);
+          if (value) { values[9] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_progress_tol);
+          if (value) { values[10] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 11:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cycle_tol);
+          if (value) { values[11] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 12:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_iter_limit);
+          if (value) { values[12] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 13:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_fval_bound);
+          if (value) { values[13] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 14:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_eps_prox);
+          if (value) { values[14] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 15:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_eta_prox);
+          if (value) { values[15] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 16:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rho_soft);
+          if (value) { values[16] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 17:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rel_subopt);
+          if (value) { values[17] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case 18:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_abs_subopt);
+          if (value) { values[18] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "solve") < 0)) __PYX_ERR(0, 4, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-      values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
-      values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case 19: values[18] = PyTuple_GET_ITEM(__pyx_args, 18);
+        CYTHON_FALLTHROUGH;
+        case 18: values[17] = PyTuple_GET_ITEM(__pyx_args, 17);
+        CYTHON_FALLTHROUGH;
+        case 17: values[16] = PyTuple_GET_ITEM(__pyx_args, 16);
+        CYTHON_FALLTHROUGH;
+        case 16: values[15] = PyTuple_GET_ITEM(__pyx_args, 15);
+        CYTHON_FALLTHROUGH;
+        case 15: values[14] = PyTuple_GET_ITEM(__pyx_args, 14);
+        CYTHON_FALLTHROUGH;
+        case 14: values[13] = PyTuple_GET_ITEM(__pyx_args, 13);
+        CYTHON_FALLTHROUGH;
+        case 13: values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
+        CYTHON_FALLTHROUGH;
+        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        CYTHON_FALLTHROUGH;
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
     }
     __pyx_v_H = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_H.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
     __pyx_v_f = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_f.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
     __pyx_v_A = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_A.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
-    __pyx_v_bupper = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_bupper.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
-    __pyx_v_blower = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_blower.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
-    __pyx_v_sense = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sense.memview)) __PYX_ERR(0, 4, __pyx_L3_error)
+    __pyx_v_bupper = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_bupper.memview)) __PYX_ERR(0, 5, __pyx_L3_error)
+    if (values[4]) {
+      __pyx_v_blower = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_blower.memview)) __PYX_ERR(0, 5, __pyx_L3_error)
+    } else {
+      __pyx_v_blower = __pyx_k__13;
+      __PYX_INC_MEMVIEW(&__pyx_v_blower, 1);
+    }
+    if (values[5]) {
+      __pyx_v_sense = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_sense.memview)) __PYX_ERR(0, 5, __pyx_L3_error)
+    } else {
+      __pyx_v_sense = __pyx_k__14;
+      __PYX_INC_MEMVIEW(&__pyx_v_sense, 1);
+    }
+    __pyx_v_primal_tol = values[6];
+    __pyx_v_dual_tol = values[7];
+    __pyx_v_zero_tol = values[8];
+    __pyx_v_pivot_tol = values[9];
+    __pyx_v_progress_tol = values[10];
+    __pyx_v_cycle_tol = values[11];
+    __pyx_v_iter_limit = values[12];
+    __pyx_v_fval_bound = values[13];
+    __pyx_v_eps_prox = values[14];
+    __pyx_v_eta_prox = values[15];
+    __pyx_v_rho_soft = values[16];
+    __pyx_v_rel_subopt = values[17];
+    __pyx_v_abs_subopt = values[18];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("solve", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 4, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("solve", 0, 4, 19, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 4, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("daqp.solve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4daqp_solve(__pyx_self, __pyx_v_H, __pyx_v_f, __pyx_v_A, __pyx_v_bupper, __pyx_v_blower, __pyx_v_sense);
+  __pyx_r = __pyx_pf_4daqp_solve(__pyx_self, __pyx_v_H, __pyx_v_f, __pyx_v_A, __pyx_v_bupper, __pyx_v_blower, __pyx_v_sense, __pyx_v_primal_tol, __pyx_v_dual_tol, __pyx_v_zero_tol, __pyx_v_pivot_tol, __pyx_v_progress_tol, __pyx_v_cycle_tol, __pyx_v_iter_limit, __pyx_v_fval_bound, __pyx_v_eps_prox, __pyx_v_eta_prox, __pyx_v_rho_soft, __pyx_v_rel_subopt, __pyx_v_abs_subopt);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4daqp_solve(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_H, __Pyx_memviewslice __pyx_v_f, __Pyx_memviewslice __pyx_v_A, __Pyx_memviewslice __pyx_v_bupper, __Pyx_memviewslice __pyx_v_blower, __Pyx_memviewslice __pyx_v_sense) {
+static PyObject *__pyx_pf_4daqp_solve(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_H, __Pyx_memviewslice __pyx_v_f, __Pyx_memviewslice __pyx_v_A, __Pyx_memviewslice __pyx_v_bupper, __Pyx_memviewslice __pyx_v_blower, __Pyx_memviewslice __pyx_v_sense, PyObject *__pyx_v_primal_tol, PyObject *__pyx_v_dual_tol, PyObject *__pyx_v_zero_tol, PyObject *__pyx_v_pivot_tol, PyObject *__pyx_v_progress_tol, PyObject *__pyx_v_cycle_tol, PyObject *__pyx_v_iter_limit, PyObject *__pyx_v_fval_bound, PyObject *__pyx_v_eps_prox, PyObject *__pyx_v_eta_prox, PyObject *__pyx_v_rho_soft, PyObject *__pyx_v_rel_subopt, PyObject *__pyx_v_abs_subopt) {
   int __pyx_v_n;
   int __pyx_v_m;
   PyObject *__pyx_v_mA = NULL;
   DAQPProblem __pyx_v_problem;
+  DAQPSettings __pyx_v_settings;
   __Pyx_memviewslice __pyx_v_x = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_lam = { 0, 0, { 0 }, { 0 }, { 0 } };
   DAQPResult __pyx_v_res;
   PyObject *__pyx_v_info = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   __Pyx_memviewslice __pyx_t_5 = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *(*__pyx_t_6)(PyObject *);
   int __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  int __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
+  int __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_12 = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
+  int __pyx_t_15;
   Py_ssize_t __pyx_t_16;
-  DAQPProblem __pyx_t_17;
-  __Pyx_memviewslice __pyx_t_18 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  DAQPResult __pyx_t_19;
-  PyObject *__pyx_t_20 = NULL;
+  Py_ssize_t __pyx_t_17;
+  Py_ssize_t __pyx_t_18;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  Py_ssize_t __pyx_t_21;
+  DAQPProblem __pyx_t_22;
+  double __pyx_t_23;
+  double __pyx_t_24;
+  double __pyx_t_25;
+  double __pyx_t_26;
+  double __pyx_t_27;
+  double __pyx_t_28;
+  double __pyx_t_29;
+  double __pyx_t_30;
+  double __pyx_t_31;
+  double __pyx_t_32;
+  double __pyx_t_33;
+  DAQPSettings __pyx_t_34;
+  __Pyx_memviewslice __pyx_t_35 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  DAQPResult __pyx_t_36;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("solve", 0);
 
-  /* "daqp.pyx":7
+  /* "daqp.pyx":14
  *     cdef int n,m,ms,nb
  *     cdef int* bin_ids_cand
  *     A = np.ascontiguousarray(A)             # <<<<<<<<<<<<<<
  *     mA, n = np.shape(A)
  *     m = np.size(bupper)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_A, 1);
   __pyx_v_A = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "daqp.pyx":8
+  /* "daqp.pyx":15
  *     cdef int* bin_ids_cand
  *     A = np.ascontiguousarray(A)
  *     mA, n = np.shape(A)             # <<<<<<<<<<<<<<
  *     m = np.size(bupper)
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
+ * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 8, __pyx_L1_error)
+      __PYX_ERR(0, 15, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 8, __pyx_L1_error)
+    __PYX_ERR(0, 15, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_mA = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_n = __pyx_t_7;
 
-  /* "daqp.pyx":9
+  /* "daqp.pyx":16
  *     A = np.ascontiguousarray(A)
  *     mA, n = np.shape(A)
  *     m = np.size(bupper)             # <<<<<<<<<<<<<<
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
+ * 
+ *     if blower is None:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_bupper, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_bupper, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_m = __pyx_t_7;
 
-  /* "daqp.pyx":10
- *     mA, n = np.shape(A)
+  /* "daqp.pyx":18
  *     m = np.size(bupper)
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],             # <<<<<<<<<<<<<<
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
- *     #cdef DAQPSettings settings
+ * 
+ *     if blower is None:             # <<<<<<<<<<<<<<
+ *         blower = np.fill(m, -DAQP_INF)
+ *     if sense is None:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_mA); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = 0;
-  __pyx_t_9 = 0;
-  __pyx_t_10 = -1;
-  if (__pyx_t_8 < 0) {
-    __pyx_t_8 += __pyx_v_H.shape[0];
-    if (unlikely(__pyx_t_8 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_8 >= __pyx_v_H.shape[0])) __pyx_t_10 = 0;
-  if (__pyx_t_9 < 0) {
-    __pyx_t_9 += __pyx_v_H.shape[1];
-    if (unlikely(__pyx_t_9 < 0)) __pyx_t_10 = 1;
-  } else if (unlikely(__pyx_t_9 >= __pyx_v_H.shape[1])) __pyx_t_10 = 1;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 10, __pyx_L1_error)
-  }
-  __pyx_t_11 = 0;
-  __pyx_t_10 = -1;
-  if (__pyx_t_11 < 0) {
-    __pyx_t_11 += __pyx_v_f.shape[0];
-    if (unlikely(__pyx_t_11 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_11 >= __pyx_v_f.shape[0])) __pyx_t_10 = 0;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 10, __pyx_L1_error)
-  }
+  __pyx_t_8 = ((((PyObject *) __pyx_v_blower.memview) == Py_None) != 0);
+  if (__pyx_t_8) {
+
+    /* "daqp.pyx":19
+ * 
+ *     if blower is None:
+ *         blower = np.fill(m, -DAQP_INF)             # <<<<<<<<<<<<<<
+ *     if sense is None:
+ *         sense = np.zeros(m, dtype=int)
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fill); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = PyFloat_FromDouble((-DAQP_INF)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_9 = NULL;
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_7 = 1;
+      }
+    }
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_t_4};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    } else
+    #endif
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_t_4};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    } else
+    #endif
+    {
+      __pyx_t_10 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      if (__pyx_t_9) {
+        __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9); __pyx_t_9 = NULL;
+      }
+      __Pyx_GIVEREF(__pyx_t_2);
+      PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_7, __pyx_t_2);
+      __Pyx_GIVEREF(__pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_7, __pyx_t_4);
+      __pyx_t_2 = 0;
+      __pyx_t_4 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_XDEC_MEMVIEW(&__pyx_v_blower, 1);
+    __pyx_v_blower = __pyx_t_11;
+    __pyx_t_11.memview = NULL;
+    __pyx_t_11.data = NULL;
 
-  /* "daqp.pyx":11
+    /* "daqp.pyx":18
  *     m = np.size(bupper)
+ * 
+ *     if blower is None:             # <<<<<<<<<<<<<<
+ *         blower = np.fill(m, -DAQP_INF)
+ *     if sense is None:
+ */
+  }
+
+  /* "daqp.pyx":20
+ *     if blower is None:
+ *         blower = np.fill(m, -DAQP_INF)
+ *     if sense is None:             # <<<<<<<<<<<<<<
+ *         sense = np.zeros(m, dtype=int)
+ * 
+ */
+  __pyx_t_8 = ((((PyObject *) __pyx_v_sense.memview) == Py_None) != 0);
+  if (__pyx_t_8) {
+
+    /* "daqp.pyx":21
+ *         blower = np.fill(m, -DAQP_INF)
+ *     if sense is None:
+ *         sense = np.zeros(m, dtype=int)             # <<<<<<<<<<<<<<
+ * 
  *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]             # <<<<<<<<<<<<<<
- *     #cdef DAQPSettings settings
- *     #settings.iter_limit = 10000
  */
-  __pyx_t_12 = 0;
-  __pyx_t_13 = 0;
-  __pyx_t_10 = -1;
-  if (__pyx_t_12 < 0) {
-    __pyx_t_12 += __pyx_v_A.shape[0];
-    if (unlikely(__pyx_t_12 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_12 >= __pyx_v_A.shape[0])) __pyx_t_10 = 0;
-  if (__pyx_t_13 < 0) {
-    __pyx_t_13 += __pyx_v_A.shape[1];
-    if (unlikely(__pyx_t_13 < 0)) __pyx_t_10 = 1;
-  } else if (unlikely(__pyx_t_13 >= __pyx_v_A.shape[1])) __pyx_t_10 = 1;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 11, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
+    __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyInt_Type))) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __PYX_XDEC_MEMVIEW(&__pyx_v_sense, 1);
+    __pyx_v_sense = __pyx_t_12;
+    __pyx_t_12.memview = NULL;
+    __pyx_t_12.data = NULL;
+
+    /* "daqp.pyx":20
+ *     if blower is None:
+ *         blower = np.fill(m, -DAQP_INF)
+ *     if sense is None:             # <<<<<<<<<<<<<<
+ *         sense = np.zeros(m, dtype=int)
+ * 
+ */
   }
+
+  /* "daqp.pyx":23
+ *         sense = np.zeros(m, dtype=int)
+ * 
+ *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],             # <<<<<<<<<<<<<<
+ *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
+ * 
+ */
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_4, __pyx_v_mA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_13 = 0;
   __pyx_t_14 = 0;
-  __pyx_t_10 = -1;
+  __pyx_t_15 = -1;
+  if (__pyx_t_13 < 0) {
+    __pyx_t_13 += __pyx_v_H.shape[0];
+    if (unlikely(__pyx_t_13 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_13 >= __pyx_v_H.shape[0])) __pyx_t_15 = 0;
   if (__pyx_t_14 < 0) {
-    __pyx_t_14 += __pyx_v_bupper.shape[0];
-    if (unlikely(__pyx_t_14 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_14 >= __pyx_v_bupper.shape[0])) __pyx_t_10 = 0;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 11, __pyx_L1_error)
-  }
-  __pyx_t_15 = 0;
-  __pyx_t_10 = -1;
-  if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_v_blower.shape[0];
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_15 >= __pyx_v_blower.shape[0])) __pyx_t_10 = 0;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 11, __pyx_L1_error)
+    __pyx_t_14 += __pyx_v_H.shape[1];
+    if (unlikely(__pyx_t_14 < 0)) __pyx_t_15 = 1;
+  } else if (unlikely(__pyx_t_14 >= __pyx_v_H.shape[1])) __pyx_t_15 = 1;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 23, __pyx_L1_error)
   }
   __pyx_t_16 = 0;
-  __pyx_t_10 = -1;
+  __pyx_t_15 = -1;
   if (__pyx_t_16 < 0) {
-    __pyx_t_16 += __pyx_v_sense.shape[0];
-    if (unlikely(__pyx_t_16 < 0)) __pyx_t_10 = 0;
-  } else if (unlikely(__pyx_t_16 >= __pyx_v_sense.shape[0])) __pyx_t_10 = 0;
-  if (unlikely(__pyx_t_10 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_10);
-    __PYX_ERR(0, 11, __pyx_L1_error)
+    __pyx_t_16 += __pyx_v_f.shape[0];
+    if (unlikely(__pyx_t_16 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_16 >= __pyx_v_f.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 23, __pyx_L1_error)
   }
 
-  /* "daqp.pyx":10
- *     mA, n = np.shape(A)
- *     m = np.size(bupper)
+  /* "daqp.pyx":24
+ * 
+ *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
+ *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]             # <<<<<<<<<<<<<<
+ * 
+ *     # Setup settings
+ */
+  __pyx_t_17 = 0;
+  __pyx_t_18 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_17 < 0) {
+    __pyx_t_17 += __pyx_v_A.shape[0];
+    if (unlikely(__pyx_t_17 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_17 >= __pyx_v_A.shape[0])) __pyx_t_15 = 0;
+  if (__pyx_t_18 < 0) {
+    __pyx_t_18 += __pyx_v_A.shape[1];
+    if (unlikely(__pyx_t_18 < 0)) __pyx_t_15 = 1;
+  } else if (unlikely(__pyx_t_18 >= __pyx_v_A.shape[1])) __pyx_t_15 = 1;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+  __pyx_t_19 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_19 < 0) {
+    __pyx_t_19 += __pyx_v_bupper.shape[0];
+    if (unlikely(__pyx_t_19 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_19 >= __pyx_v_bupper.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+  __pyx_t_20 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_20 < 0) {
+    __pyx_t_20 += __pyx_v_blower.shape[0];
+    if (unlikely(__pyx_t_20 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_20 >= __pyx_v_blower.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+  __pyx_t_21 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_21 < 0) {
+    __pyx_t_21 += __pyx_v_sense.shape[0];
+    if (unlikely(__pyx_t_21 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_21 >= __pyx_v_sense.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+
+  /* "daqp.pyx":23
+ *         sense = np.zeros(m, dtype=int)
+ * 
  *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],             # <<<<<<<<<<<<<<
  *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
- *     #cdef DAQPSettings settings
+ * 
  */
-  __pyx_t_17.n = __pyx_v_n;
-  __pyx_t_17.m = __pyx_v_m;
-  __pyx_t_17.ms = __pyx_t_7;
-  __pyx_t_17.H = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_H.data + __pyx_t_8 * __pyx_v_H.strides[0]) ) + __pyx_t_9 * __pyx_v_H.strides[1]) ))));
-  __pyx_t_17.f = (&(*((double *) ( /* dim=0 */ (__pyx_v_f.data + __pyx_t_11 * __pyx_v_f.strides[0]) ))));
-  __pyx_t_17.A = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_A.data + __pyx_t_12 * __pyx_v_A.strides[0]) ) + __pyx_t_13 * __pyx_v_A.strides[1]) ))));
-  __pyx_t_17.bupper = (&(*((double *) ( /* dim=0 */ (__pyx_v_bupper.data + __pyx_t_14 * __pyx_v_bupper.strides[0]) ))));
-  __pyx_t_17.blower = (&(*((double *) ( /* dim=0 */ (__pyx_v_blower.data + __pyx_t_15 * __pyx_v_blower.strides[0]) ))));
-  __pyx_t_17.sense = (&(*((int *) ( /* dim=0 */ (__pyx_v_sense.data + __pyx_t_16 * __pyx_v_sense.strides[0]) ))));
-  __pyx_t_17.bin_ids = NULL;
-  __pyx_t_17.nb = 0;
-  __pyx_v_problem = __pyx_t_17;
+  __pyx_t_22.n = __pyx_v_n;
+  __pyx_t_22.m = __pyx_v_m;
+  __pyx_t_22.ms = __pyx_t_7;
+  __pyx_t_22.H = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_H.data + __pyx_t_13 * __pyx_v_H.strides[0]) ) + __pyx_t_14 * __pyx_v_H.strides[1]) ))));
+  __pyx_t_22.f = (&(*((double *) ( /* dim=0 */ (__pyx_v_f.data + __pyx_t_16 * __pyx_v_f.strides[0]) ))));
+  __pyx_t_22.A = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_A.data + __pyx_t_17 * __pyx_v_A.strides[0]) ) + __pyx_t_18 * __pyx_v_A.strides[1]) ))));
+  __pyx_t_22.bupper = (&(*((double *) ( /* dim=0 */ (__pyx_v_bupper.data + __pyx_t_19 * __pyx_v_bupper.strides[0]) ))));
+  __pyx_t_22.blower = (&(*((double *) ( /* dim=0 */ (__pyx_v_blower.data + __pyx_t_20 * __pyx_v_blower.strides[0]) ))));
+  __pyx_t_22.sense = (&(*((int *) ( /* dim=0 */ (__pyx_v_sense.data + __pyx_t_21 * __pyx_v_sense.strides[0]) ))));
+  __pyx_t_22.bin_ids = NULL;
+  __pyx_t_22.nb = 0;
+  __pyx_v_problem = __pyx_t_22;
+
+  /* "daqp.pyx":27
+ * 
+ *     # Setup settings
+ *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,             # <<<<<<<<<<<<<<
+ *             progress_tol, cycle_tol, iter_limit, fval_bound,
+ *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
+ */
+  __pyx_t_23 = __pyx_PyFloat_AsDouble(__pyx_v_primal_tol); if (unlikely((__pyx_t_23 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_24 = __pyx_PyFloat_AsDouble(__pyx_v_dual_tol); if (unlikely((__pyx_t_24 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_25 = __pyx_PyFloat_AsDouble(__pyx_v_zero_tol); if (unlikely((__pyx_t_25 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_26 = __pyx_PyFloat_AsDouble(__pyx_v_pivot_tol); if (unlikely((__pyx_t_26 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+
+  /* "daqp.pyx":28
+ *     # Setup settings
+ *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,
+ *             progress_tol, cycle_tol, iter_limit, fval_bound,             # <<<<<<<<<<<<<<
+ *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
+ * 
+ */
+  __pyx_t_27 = __pyx_PyFloat_AsDouble(__pyx_v_progress_tol); if (unlikely((__pyx_t_27 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_cycle_tol); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_v_iter_limit); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_28 = __pyx_PyFloat_AsDouble(__pyx_v_fval_bound); if (unlikely((__pyx_t_28 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+
+  /* "daqp.pyx":29
+ *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,
+ *             progress_tol, cycle_tol, iter_limit, fval_bound,
+ *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]             # <<<<<<<<<<<<<<
+ * 
+ *     # Setup output
+ */
+  __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_v_eps_prox); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_30 = __pyx_PyFloat_AsDouble(__pyx_v_eta_prox); if (unlikely((__pyx_t_30 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_31 = __pyx_PyFloat_AsDouble(__pyx_v_rho_soft); if (unlikely((__pyx_t_31 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_32 = __pyx_PyFloat_AsDouble(__pyx_v_rel_subopt); if (unlikely((__pyx_t_32 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_33 = __pyx_PyFloat_AsDouble(__pyx_v_abs_subopt); if (unlikely((__pyx_t_33 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+
+  /* "daqp.pyx":27
+ * 
+ *     # Setup settings
+ *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,             # <<<<<<<<<<<<<<
+ *             progress_tol, cycle_tol, iter_limit, fval_bound,
+ *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
+ */
+  __pyx_t_34.primal_tol = __pyx_t_23;
+  __pyx_t_34.dual_tol = __pyx_t_24;
+  __pyx_t_34.zero_tol = __pyx_t_25;
+  __pyx_t_34.pivot_tol = __pyx_t_26;
+  __pyx_t_34.progress_tol = __pyx_t_27;
+  __pyx_t_34.cycle_tol = __pyx_t_7;
+  __pyx_t_34.iter_limit = __pyx_t_15;
+  __pyx_t_34.fval_bound = __pyx_t_28;
+  __pyx_t_34.eps_prox = __pyx_t_29;
+  __pyx_t_34.eta_prox = __pyx_t_30;
+  __pyx_t_34.rho_soft = __pyx_t_31;
+  __pyx_t_34.rel_subopt = __pyx_t_32;
+  __pyx_t_34.abs_subopt = __pyx_t_33;
+  __pyx_v_settings = __pyx_t_34;
 
-  /* "daqp.pyx":17
- *     #    daqp_default_settings(&settings)
+  /* "daqp.pyx":32
  * 
+ *     # Setup output
  *     cdef double[::1] x = np.zeros(n)             # <<<<<<<<<<<<<<
  *     cdef double[::1] lam = np.zeros(m)
  *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_10);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_x = __pyx_t_18;
-  __pyx_t_18.memview = NULL;
-  __pyx_t_18.data = NULL;
+  __pyx_v_x = __pyx_t_35;
+  __pyx_t_35.memview = NULL;
+  __pyx_t_35.data = NULL;
 
-  /* "daqp.pyx":18
- * 
+  /* "daqp.pyx":33
+ *     # Setup output
  *     cdef double[::1] x = np.zeros(n)
  *     cdef double[::1] lam = np.zeros(m)             # <<<<<<<<<<<<<<
  *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_18 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_18.memview)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_lam = __pyx_t_18;
-  __pyx_t_18.memview = NULL;
-  __pyx_t_18.data = NULL;
+  __pyx_v_lam = __pyx_t_35;
+  __pyx_t_35.memview = NULL;
+  __pyx_t_35.data = NULL;
 
-  /* "daqp.pyx":19
+  /* "daqp.pyx":34
  *     cdef double[::1] x = np.zeros(n)
  *     cdef double[::1] lam = np.zeros(m)
  *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]             # <<<<<<<<<<<<<<
  * 
- *     with nogil:
+ *     # Solve
  */
-  __pyx_t_16 = 0;
-  __pyx_t_7 = -1;
-  if (__pyx_t_16 < 0) {
-    __pyx_t_16 += __pyx_v_x.shape[0];
-    if (unlikely(__pyx_t_16 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_16 >= __pyx_v_x.shape[0])) __pyx_t_7 = 0;
-  if (unlikely(__pyx_t_7 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 19, __pyx_L1_error)
-  }
-  __pyx_t_15 = 0;
-  __pyx_t_7 = -1;
-  if (__pyx_t_15 < 0) {
-    __pyx_t_15 += __pyx_v_lam.shape[0];
-    if (unlikely(__pyx_t_15 < 0)) __pyx_t_7 = 0;
-  } else if (unlikely(__pyx_t_15 >= __pyx_v_lam.shape[0])) __pyx_t_7 = 0;
-  if (unlikely(__pyx_t_7 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_7);
-    __PYX_ERR(0, 19, __pyx_L1_error)
-  }
-  __pyx_t_19.x = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_x.data) + __pyx_t_16)) ))));
-  __pyx_t_19.lam = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_15)) ))));
-  __pyx_t_19.fval = 0.0;
-  __pyx_t_19.soft_slack = 0.0;
-  __pyx_t_19.exitflag = 0;
-  __pyx_t_19.iter = 0;
-  __pyx_t_19.nodes = 0;
-  __pyx_t_19.solve_time = 0.0;
-  __pyx_t_19.setup_time = 0.0;
-  __pyx_v_res = __pyx_t_19;
+  __pyx_t_21 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_21 < 0) {
+    __pyx_t_21 += __pyx_v_x.shape[0];
+    if (unlikely(__pyx_t_21 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_21 >= __pyx_v_x.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 34, __pyx_L1_error)
+  }
+  __pyx_t_20 = 0;
+  __pyx_t_15 = -1;
+  if (__pyx_t_20 < 0) {
+    __pyx_t_20 += __pyx_v_lam.shape[0];
+    if (unlikely(__pyx_t_20 < 0)) __pyx_t_15 = 0;
+  } else if (unlikely(__pyx_t_20 >= __pyx_v_lam.shape[0])) __pyx_t_15 = 0;
+  if (unlikely(__pyx_t_15 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_15);
+    __PYX_ERR(0, 34, __pyx_L1_error)
+  }
+  __pyx_t_36.x = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_x.data) + __pyx_t_21)) ))));
+  __pyx_t_36.lam = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_20)) ))));
+  __pyx_t_36.fval = 0.0;
+  __pyx_t_36.soft_slack = 0.0;
+  __pyx_t_36.exitflag = 0;
+  __pyx_t_36.iter = 0;
+  __pyx_t_36.nodes = 0;
+  __pyx_t_36.solve_time = 0.0;
+  __pyx_t_36.setup_time = 0.0;
+  __pyx_v_res = __pyx_t_36;
 
-  /* "daqp.pyx":21
- *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
+  /* "daqp.pyx":37
  * 
+ *     # Solve
  *     with nogil:             # <<<<<<<<<<<<<<
- *         daqp_quadprog(&res, &problem, NULL)
+ *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "daqp.pyx":22
- * 
+        /* "daqp.pyx":38
+ *     # Solve
  *     with nogil:
- *         daqp_quadprog(&res, &problem, NULL)             # <<<<<<<<<<<<<<
+ *         daqp_quadprog(&res, &problem, &settings)             # <<<<<<<<<<<<<<
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,
  */
-        (void)(daqp_quadprog((&__pyx_v_res), (&__pyx_v_problem), NULL));
+        (void)(daqp_quadprog((&__pyx_v_res), (&__pyx_v_problem), (&__pyx_v_settings)));
       }
 
-      /* "daqp.pyx":21
- *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
+      /* "daqp.pyx":37
  * 
+ *     # Solve
  *     with nogil:             # <<<<<<<<<<<<<<
- *         daqp_quadprog(&res, &problem, NULL)
+ *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
-          goto __pyx_L7;
+          goto __pyx_L9;
         }
-        __pyx_L7:;
+        __pyx_L9:;
       }
   }
 
-  /* "daqp.pyx":23
+  /* "daqp.pyx":39
  *     with nogil:
- *         daqp_quadprog(&res, &problem, NULL)
+ *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,             # <<<<<<<<<<<<<<
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_res.solve_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_solve_time, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.solve_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_solve_time, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":24
- *         daqp_quadprog(&res, &problem, NULL)
+  /* "daqp.pyx":40
+ *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,             # <<<<<<<<<<<<<<
  *             'iterations': res.iter,
  *             'nodes': res.nodes,
  */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_res.setup_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_setup_time, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.setup_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_setup_time, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":25
+  /* "daqp.pyx":41
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,             # <<<<<<<<<<<<<<
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_res.iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_iterations, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.iter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_iterations, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":26
+  /* "daqp.pyx":42
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,
  *             'nodes': res.nodes,             # <<<<<<<<<<<<<<
  *             'lam': np.asarray(lam)}
  *     return np.asarray(x), res.fval, res.exitflag, info
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_res.nodes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_nodes, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.nodes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_nodes, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":27
+  /* "daqp.pyx":43
  *             'iterations': res.iter,
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}             # <<<<<<<<<<<<<<
  *     return np.asarray(x), res.fval, res.exitflag, info
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_lam, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_20 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_20 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_20)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_20);
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_lam, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_20) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_20, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_20); __pyx_t_20 = 0;
+  __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_lam, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_lam, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_info = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_v_info = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "daqp.pyx":28
+  /* "daqp.pyx":44
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}
  *     return np.asarray(x), res.fval, res.exitflag, info             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_x, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_x, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_10 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_10)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.fval); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_res.exitflag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_res.fval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.exitflag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_10 = PyTuple_New(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_4);
   __Pyx_INCREF(__pyx_v_info);
   __Pyx_GIVEREF(__pyx_v_info);
-  PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_v_info);
-  __pyx_t_2 = 0;
-  __pyx_t_4 = 0;
+  PyTuple_SET_ITEM(__pyx_t_10, 3, __pyx_v_info);
   __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
+  __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_10;
+  __pyx_t_10 = 0;
   goto __pyx_L0;
 
   /* "daqp.pyx":4
  * cimport daqp
  * 
- * def solve(double[:, :] H, double[:] f, double[:, :] A, double[:] bupper, double[:] blower, int[:] sense):             # <<<<<<<<<<<<<<
- *     cdef int n,m,ms,nb
- *     cdef int* bin_ids_cand
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_18, 1);
-  __Pyx_XDECREF(__pyx_t_20);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_35, 1);
   __Pyx_AddTraceback("daqp.solve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mA);
   __PYX_XDEC_MEMVIEW(&__pyx_v_x, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_lam, 1);
   __Pyx_XDECREF(__pyx_v_info);
@@ -3199,15 +3654,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -3231,15 +3686,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -3358,15 +3813,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -3632,15 +4087,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -3876,15 +4331,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -4610,15 +5065,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -4666,15 +5121,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -6395,15 +6850,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -7443,15 +7898,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -7805,15 +8260,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -8354,15 +8809,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -8471,15 +8926,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__12, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__26, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -9509,15 +9964,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -9565,15 +10020,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -9922,17 +10377,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__15);
-            __Pyx_GIVEREF(__pyx_slice__15);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__15);
+            __Pyx_INCREF(__pyx_slice__29);
+            __Pyx_GIVEREF(__pyx_slice__29);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__29);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -9957,15 +10412,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__15); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__29); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -10097,17 +10552,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__15);
-        __Pyx_GIVEREF(__pyx_slice__15);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__15);
+        __Pyx_INCREF(__pyx_slice__29);
+        __Pyx_GIVEREF(__pyx_slice__29);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__29);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -10226,15 +10681,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -12410,15 +12865,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -12466,15 +12921,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -15743,15 +16198,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__19, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__33, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -16835,46 +17290,55 @@
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
+  {&__pyx_n_s_abs_subopt, __pyx_k_abs_subopt, sizeof(__pyx_k_abs_subopt), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
   {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bin_ids_cand, __pyx_k_bin_ids_cand, sizeof(__pyx_k_bin_ids_cand), 0, 0, 1, 1},
   {&__pyx_n_s_blower, __pyx_k_blower, sizeof(__pyx_k_blower), 0, 0, 1, 1},
   {&__pyx_n_s_bupper, __pyx_k_bupper, sizeof(__pyx_k_bupper), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
+  {&__pyx_n_s_cycle_tol, __pyx_k_cycle_tol, sizeof(__pyx_k_cycle_tol), 0, 0, 1, 1},
   {&__pyx_n_s_daqp, __pyx_k_daqp, sizeof(__pyx_k_daqp), 0, 0, 1, 1},
   {&__pyx_kp_s_daqp_pyx, __pyx_k_daqp_pyx, sizeof(__pyx_k_daqp_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
+  {&__pyx_n_s_dual_tol, __pyx_k_dual_tol, sizeof(__pyx_k_dual_tol), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
+  {&__pyx_n_s_eps_prox, __pyx_k_eps_prox, sizeof(__pyx_k_eps_prox), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
+  {&__pyx_n_s_eta_prox, __pyx_k_eta_prox, sizeof(__pyx_k_eta_prox), 0, 0, 1, 1},
   {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
+  {&__pyx_n_s_fill, __pyx_k_fill, sizeof(__pyx_k_fill), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
+  {&__pyx_n_s_fval_bound, __pyx_k_fval_bound, sizeof(__pyx_k_fval_bound), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_info, __pyx_k_info, sizeof(__pyx_k_info), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
+  {&__pyx_n_s_iter_limit, __pyx_k_iter_limit, sizeof(__pyx_k_iter_limit), 0, 0, 1, 1},
   {&__pyx_n_s_iterations, __pyx_k_iterations, sizeof(__pyx_k_iterations), 0, 0, 1, 1},
   {&__pyx_n_s_lam, __pyx_k_lam, sizeof(__pyx_k_lam), 0, 0, 1, 1},
   {&__pyx_n_s_m, __pyx_k_m, sizeof(__pyx_k_m), 0, 0, 1, 1},
   {&__pyx_n_s_mA, __pyx_k_mA, sizeof(__pyx_k_mA), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
@@ -16888,31 +17352,37 @@
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_nodes, __pyx_k_nodes, sizeof(__pyx_k_nodes), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+  {&__pyx_n_s_pivot_tol, __pyx_k_pivot_tol, sizeof(__pyx_k_pivot_tol), 0, 0, 1, 1},
+  {&__pyx_n_s_primal_tol, __pyx_k_primal_tol, sizeof(__pyx_k_primal_tol), 0, 0, 1, 1},
   {&__pyx_n_s_problem, __pyx_k_problem, sizeof(__pyx_k_problem), 0, 0, 1, 1},
+  {&__pyx_n_s_progress_tol, __pyx_k_progress_tol, sizeof(__pyx_k_progress_tol), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_n_s_rel_subopt, __pyx_k_rel_subopt, sizeof(__pyx_k_rel_subopt), 0, 0, 1, 1},
   {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
+  {&__pyx_n_s_rho_soft, __pyx_k_rho_soft, sizeof(__pyx_k_rho_soft), 0, 0, 1, 1},
   {&__pyx_n_s_sense, __pyx_k_sense, sizeof(__pyx_k_sense), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_settings, __pyx_k_settings, sizeof(__pyx_k_settings), 0, 0, 1, 1},
   {&__pyx_n_s_setup_time, __pyx_k_setup_time, sizeof(__pyx_k_setup_time), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_solve, __pyx_k_solve, sizeof(__pyx_k_solve), 0, 0, 1, 1},
   {&__pyx_n_s_solve_time, __pyx_k_solve_time, sizeof(__pyx_k_solve_time), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
@@ -16924,14 +17394,15 @@
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
+  {&__pyx_n_s_zero_tol, __pyx_k_zero_tol, sizeof(__pyx_k_zero_tol), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
@@ -16952,278 +17423,278 @@
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__12 = PyTuple_New(1); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
+  __pyx_tuple__26 = PyTuple_New(1); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__12, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  PyTuple_SET_ITEM(__pyx_tuple__26, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__15 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__15);
-  __Pyx_GIVEREF(__pyx_slice__15);
+  __pyx_slice__29 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__29)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__29);
+  __Pyx_GIVEREF(__pyx_slice__29);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "daqp.pyx":4
  * cimport daqp
  * 
- * def solve(double[:, :] H, double[:] f, double[:, :] A, double[:] bupper, double[:] blower, int[:] sense):             # <<<<<<<<<<<<<<
- *     cdef int n,m,ms,nb
- *     cdef int* bin_ids_cand
- */
-  __pyx_tuple__20 = PyTuple_Pack(17, __pyx_n_s_H, __pyx_n_s_f, __pyx_n_s_A, __pyx_n_s_bupper, __pyx_n_s_blower, __pyx_n_s_sense, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_ms, __pyx_n_s_nb, __pyx_n_s_bin_ids_cand, __pyx_n_s_mA, __pyx_n_s_problem, __pyx_n_s_x, __pyx_n_s_lam, __pyx_n_s_res, __pyx_n_s_info); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(6, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_daqp_pyx, __pyx_n_s_solve, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 4, __pyx_L1_error)
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
+ */
+  __pyx_tuple__34 = PyTuple_Pack(31, __pyx_n_s_H, __pyx_n_s_f, __pyx_n_s_A, __pyx_n_s_bupper, __pyx_n_s_blower, __pyx_n_s_sense, __pyx_n_s_primal_tol, __pyx_n_s_dual_tol, __pyx_n_s_zero_tol, __pyx_n_s_pivot_tol, __pyx_n_s_progress_tol, __pyx_n_s_cycle_tol, __pyx_n_s_iter_limit, __pyx_n_s_fval_bound, __pyx_n_s_eps_prox, __pyx_n_s_eta_prox, __pyx_n_s_rho_soft, __pyx_n_s_rel_subopt, __pyx_n_s_abs_subopt, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_ms, __pyx_n_s_nb, __pyx_n_s_bin_ids_cand, __pyx_n_s_mA, __pyx_n_s_problem, __pyx_n_s_settings, __pyx_n_s_x, __pyx_n_s_lam, __pyx_n_s_res, __pyx_n_s_info); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(19, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_daqp_pyx, __pyx_n_s_solve, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 4, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -17457,15 +17928,17 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_daqp(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
-  static PyThread_type_lock __pyx_t_2[8];
+  __Pyx_memviewslice __pyx_t_2 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_3 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  static PyThread_type_lock __pyx_t_4[8];
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -17573,20 +18046,136 @@
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+  /* "daqp.pyx":5
+ * 
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,             # <<<<<<<<<<<<<<
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
+ *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,
+ */
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(Py_None, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_k__13 = __pyx_t_2;
+  __pyx_t_2.memview = NULL;
+  __pyx_t_2.data = NULL;
+  __pyx_t_3 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(Py_None, PyBUF_WRITABLE); if (unlikely(!__pyx_t_3.memview)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_k__14 = __pyx_t_3;
+  __pyx_t_3.memview = NULL;
+  __pyx_t_3.data = NULL;
+
+  /* "daqp.pyx":6
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,             # <<<<<<<<<<<<<<
+ *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,
+ *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
+ */
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_PRIM_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k_ = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_DUAL_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__2 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_ZERO_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__3 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "daqp.pyx":7
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
+ *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,             # <<<<<<<<<<<<<<
+ *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
+ *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,
+ */
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_PIVOT_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__4 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_PROG_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__5 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "daqp.pyx":8
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
+ *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,
+ *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,             # <<<<<<<<<<<<<<
+ *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,
+ *         rel_subopt = DEFAULT_REL_SUBOPT, abs_subopt = DEFAULT_ABS_SUBOPT):
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_int(DEFAULT_CYCLE_TOL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__6 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(DEFAULT_ITER_LIMIT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__7 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DAQP_INF); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__8 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "daqp.pyx":9
+ *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,
+ *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
+ *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,             # <<<<<<<<<<<<<<
+ *         rel_subopt = DEFAULT_REL_SUBOPT, abs_subopt = DEFAULT_ABS_SUBOPT):
+ *     # Setup problem
+ */
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_ETA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__9 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_RHO_SOFT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__10 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "daqp.pyx":10
+ *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
+ *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,
+ *         rel_subopt = DEFAULT_REL_SUBOPT, abs_subopt = DEFAULT_ABS_SUBOPT):             # <<<<<<<<<<<<<<
+ *     # Setup problem
+ *     cdef int n,m,ms,nb
+ */
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_REL_SUBOPT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__11 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyFloat_FromDouble(DEFAULT_ABS_SUBOPT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_k__12 = __pyx_t_1;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
+
   /* "daqp.pyx":4
  * cimport daqp
  * 
- * def solve(double[:, :] H, double[:] f, double[:, :] A, double[:] bupper, double[:] blower, int[:] sense):             # <<<<<<<<<<<<<<
- *     cdef int n,m,ms,nb
- *     cdef int* bin_ids_cand
+ * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
+ *         double[:] bupper, double[:] blower=None, int[:] sense =None,
+ *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4daqp_1solve, NULL, __pyx_n_s_daqp); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_solve, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "daqp.pyx":1
@@ -17615,71 +18204,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
@@ -17694,23 +18283,23 @@
   /* "View.MemoryView":318
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
-  __pyx_t_2[0] = PyThread_allocate_lock();
-  __pyx_t_2[1] = PyThread_allocate_lock();
-  __pyx_t_2[2] = PyThread_allocate_lock();
-  __pyx_t_2[3] = PyThread_allocate_lock();
-  __pyx_t_2[4] = PyThread_allocate_lock();
-  __pyx_t_2[5] = PyThread_allocate_lock();
-  __pyx_t_2[6] = PyThread_allocate_lock();
-  __pyx_t_2[7] = PyThread_allocate_lock();
-  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_2, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
+  __pyx_t_4[0] = PyThread_allocate_lock();
+  __pyx_t_4[1] = PyThread_allocate_lock();
+  __pyx_t_4[2] = PyThread_allocate_lock();
+  __pyx_t_4[3] = PyThread_allocate_lock();
+  __pyx_t_4[4] = PyThread_allocate_lock();
+  __pyx_t_4[5] = PyThread_allocate_lock();
+  __pyx_t_4[6] = PyThread_allocate_lock();
+  __pyx_t_4[7] = PyThread_allocate_lock();
+  memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_4, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
   /* "View.MemoryView":551
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
@@ -17753,14 +18342,16 @@
  */
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_2, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_3, 1);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init daqp", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init daqp");
@@ -17932,14 +18523,146 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* MemviewSliceInit */
+static int
+__Pyx_init_memviewslice(struct __pyx_memoryview_obj *memview,
+                        int ndim,
+                        __Pyx_memviewslice *memviewslice,
+                        int memview_is_new_reference)
+{
+    __Pyx_RefNannyDeclarations
+    int i, retval=-1;
+    Py_buffer *buf = &memview->view;
+    __Pyx_RefNannySetupContext("init_memviewslice", 0);
+    if (unlikely(memviewslice->memview || memviewslice->data)) {
+        PyErr_SetString(PyExc_ValueError,
+            "memviewslice is already initialized!");
+        goto fail;
+    }
+    if (buf->strides) {
+        for (i = 0; i < ndim; i++) {
+            memviewslice->strides[i] = buf->strides[i];
+        }
+    } else {
+        Py_ssize_t stride = buf->itemsize;
+        for (i = ndim - 1; i >= 0; i--) {
+            memviewslice->strides[i] = stride;
+            stride *= buf->shape[i];
+        }
+    }
+    for (i = 0; i < ndim; i++) {
+        memviewslice->shape[i]   = buf->shape[i];
+        if (buf->suboffsets) {
+            memviewslice->suboffsets[i] = buf->suboffsets[i];
+        } else {
+            memviewslice->suboffsets[i] = -1;
+        }
+    }
+    memviewslice->memview = memview;
+    memviewslice->data = (char *)buf->buf;
+    if (__pyx_add_acquisition_count(memview) == 0 && !memview_is_new_reference) {
+        Py_INCREF(memview);
+    }
+    retval = 0;
+    goto no_fail;
+fail:
+    memviewslice->memview = 0;
+    memviewslice->data = 0;
+    retval = -1;
+no_fail:
+    __Pyx_RefNannyFinishContext();
+    return retval;
+}
+#ifndef Py_NO_RETURN
+#define Py_NO_RETURN
+#endif
+static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
+    va_list vargs;
+    char msg[200];
+#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
+    va_start(vargs, fmt);
+#else
+    va_start(vargs);
+#endif
+    vsnprintf(msg, 200, fmt, vargs);
+    va_end(vargs);
+    Py_FatalError(msg);
+}
+static CYTHON_INLINE int
+__pyx_add_acquisition_count_locked(__pyx_atomic_int *acquisition_count,
+                                   PyThread_type_lock lock)
+{
+    int result;
+    PyThread_acquire_lock(lock, 1);
+    result = (*acquisition_count)++;
+    PyThread_release_lock(lock);
+    return result;
+}
+static CYTHON_INLINE int
+__pyx_sub_acquisition_count_locked(__pyx_atomic_int *acquisition_count,
+                                   PyThread_type_lock lock)
+{
+    int result;
+    PyThread_acquire_lock(lock, 1);
+    result = (*acquisition_count)--;
+    PyThread_release_lock(lock);
+    return result;
+}
+static CYTHON_INLINE void
+__Pyx_INC_MEMVIEW(__Pyx_memviewslice *memslice, int have_gil, int lineno)
+{
+    int first_time;
+    struct __pyx_memoryview_obj *memview = memslice->memview;
+    if (unlikely(!memview || (PyObject *) memview == Py_None))
+        return;
+    if (unlikely(__pyx_get_slice_count(memview) < 0))
+        __pyx_fatalerror("Acquisition count is %d (line %d)",
+                         __pyx_get_slice_count(memview), lineno);
+    first_time = __pyx_add_acquisition_count(memview) == 0;
+    if (unlikely(first_time)) {
+        if (have_gil) {
+            Py_INCREF((PyObject *) memview);
+        } else {
+            PyGILState_STATE _gilstate = PyGILState_Ensure();
+            Py_INCREF((PyObject *) memview);
+            PyGILState_Release(_gilstate);
+        }
+    }
+}
+static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *memslice,
+                                             int have_gil, int lineno) {
+    int last_time;
+    struct __pyx_memoryview_obj *memview = memslice->memview;
+    if (unlikely(!memview || (PyObject *) memview == Py_None)) {
+        memslice->memview = NULL;
+        return;
+    }
+    if (unlikely(__pyx_get_slice_count(memview) <= 0))
+        __pyx_fatalerror("Acquisition count is %d (line %d)",
+                         __pyx_get_slice_count(memview), lineno);
+    last_time = __pyx_sub_acquisition_count(memview) == 1;
+    memslice->data = NULL;
+    if (unlikely(last_time)) {
+        if (have_gil) {
+            Py_CLEAR(memslice->memview);
+        } else {
+            PyGILState_STATE _gilstate = PyGILState_Ensure();
+            Py_CLEAR(memslice->memview);
+            PyGILState_Release(_gilstate);
+        }
+    } else {
+        memslice->memview = NULL;
+    }
+}
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
@@ -18272,146 +18995,14 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* MemviewSliceInit */
-static int
-__Pyx_init_memviewslice(struct __pyx_memoryview_obj *memview,
-                        int ndim,
-                        __Pyx_memviewslice *memviewslice,
-                        int memview_is_new_reference)
-{
-    __Pyx_RefNannyDeclarations
-    int i, retval=-1;
-    Py_buffer *buf = &memview->view;
-    __Pyx_RefNannySetupContext("init_memviewslice", 0);
-    if (unlikely(memviewslice->memview || memviewslice->data)) {
-        PyErr_SetString(PyExc_ValueError,
-            "memviewslice is already initialized!");
-        goto fail;
-    }
-    if (buf->strides) {
-        for (i = 0; i < ndim; i++) {
-            memviewslice->strides[i] = buf->strides[i];
-        }
-    } else {
-        Py_ssize_t stride = buf->itemsize;
-        for (i = ndim - 1; i >= 0; i--) {
-            memviewslice->strides[i] = stride;
-            stride *= buf->shape[i];
-        }
-    }
-    for (i = 0; i < ndim; i++) {
-        memviewslice->shape[i]   = buf->shape[i];
-        if (buf->suboffsets) {
-            memviewslice->suboffsets[i] = buf->suboffsets[i];
-        } else {
-            memviewslice->suboffsets[i] = -1;
-        }
-    }
-    memviewslice->memview = memview;
-    memviewslice->data = (char *)buf->buf;
-    if (__pyx_add_acquisition_count(memview) == 0 && !memview_is_new_reference) {
-        Py_INCREF(memview);
-    }
-    retval = 0;
-    goto no_fail;
-fail:
-    memviewslice->memview = 0;
-    memviewslice->data = 0;
-    retval = -1;
-no_fail:
-    __Pyx_RefNannyFinishContext();
-    return retval;
-}
-#ifndef Py_NO_RETURN
-#define Py_NO_RETURN
-#endif
-static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
-    va_list vargs;
-    char msg[200];
-#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
-    va_start(vargs, fmt);
-#else
-    va_start(vargs);
-#endif
-    vsnprintf(msg, 200, fmt, vargs);
-    va_end(vargs);
-    Py_FatalError(msg);
-}
-static CYTHON_INLINE int
-__pyx_add_acquisition_count_locked(__pyx_atomic_int *acquisition_count,
-                                   PyThread_type_lock lock)
-{
-    int result;
-    PyThread_acquire_lock(lock, 1);
-    result = (*acquisition_count)++;
-    PyThread_release_lock(lock);
-    return result;
-}
-static CYTHON_INLINE int
-__pyx_sub_acquisition_count_locked(__pyx_atomic_int *acquisition_count,
-                                   PyThread_type_lock lock)
-{
-    int result;
-    PyThread_acquire_lock(lock, 1);
-    result = (*acquisition_count)--;
-    PyThread_release_lock(lock);
-    return result;
-}
-static CYTHON_INLINE void
-__Pyx_INC_MEMVIEW(__Pyx_memviewslice *memslice, int have_gil, int lineno)
-{
-    int first_time;
-    struct __pyx_memoryview_obj *memview = memslice->memview;
-    if (unlikely(!memview || (PyObject *) memview == Py_None))
-        return;
-    if (unlikely(__pyx_get_slice_count(memview) < 0))
-        __pyx_fatalerror("Acquisition count is %d (line %d)",
-                         __pyx_get_slice_count(memview), lineno);
-    first_time = __pyx_add_acquisition_count(memview) == 0;
-    if (unlikely(first_time)) {
-        if (have_gil) {
-            Py_INCREF((PyObject *) memview);
-        } else {
-            PyGILState_STATE _gilstate = PyGILState_Ensure();
-            Py_INCREF((PyObject *) memview);
-            PyGILState_Release(_gilstate);
-        }
-    }
-}
-static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *memslice,
-                                             int have_gil, int lineno) {
-    int last_time;
-    struct __pyx_memoryview_obj *memview = memslice->memview;
-    if (unlikely(!memview || (PyObject *) memview == Py_None)) {
-        memslice->memview = NULL;
-        return;
-    }
-    if (unlikely(__pyx_get_slice_count(memview) <= 0))
-        __pyx_fatalerror("Acquisition count is %d (line %d)",
-                         __pyx_get_slice_count(memview), lineno);
-    last_time = __pyx_sub_acquisition_count(memview) == 1;
-    memslice->data = NULL;
-    if (unlikely(last_time)) {
-        if (have_gil) {
-            Py_CLEAR(memslice->memview);
-        } else {
-            PyGILState_STATE _gilstate = PyGILState_Ensure();
-            Py_CLEAR(memslice->memview);
-            PyGILState_Release(_gilstate);
-        }
-    } else {
-        memslice->memview = NULL;
-    }
-}
-
 /* RaiseTooManyValuesToUnpack */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
     PyErr_Format(PyExc_ValueError,
                  "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
 }
 
 /* RaiseNeedMoreValuesToUnpack */
@@ -20800,72 +21391,72 @@
     retval = -1;
 no_fail:
     __Pyx_RefNannyFinishContext();
     return retval;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_double(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_double(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 2,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
                                                  &__Pyx_TypeInfo_double, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_double(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
                                                  PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_double, stack,
+                                                 &__Pyx_TypeInfo_int, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_int(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_double(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_int, stack,
+                                                 PyBUF_RECORDS_RO | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_double, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
@@ -20992,14 +21583,52 @@
     __Pyx_XDECREF(shape_tuple);
     __Pyx_XDECREF(temp_int);
     __Pyx_XDECREF(array_obj);
     __Pyx_RefNannyFinishContext();
     return new_mvs;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -21188,52 +21817,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
```

### Comparing `daqp-0.4.0/daqp.egg-info/PKG-INFO` & `daqp-0.4.1/daqp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daqp
-Version: 0.4.0
+Version: 0.4.1
 Summary: DAQP: A dual active-set QP solver
 Home-page: http://github.com/darnstrom/daqp
 Author: Daniel Arnström
 Author-email: daniel.arnstrom@liu.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daqp-0.4.0/setup.py` & `daqp-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,29 +31,27 @@
             'csrc/src/bnb.c', 
             'csrc/src/daqp.c', 
             'csrc/src/daqp_prox.c', 
             'csrc/src/factorization.c', 
             'csrc/src/utils.c', 
             ],
         library_dirs=['.'],
-        extra_compile_args=["-O3"],
+        extra_compile_args=["-O3", "-DPROFILING"],
         include_dirs=['csrc/include'])
 
 setup(name='daqp',
-        version='0.4.0',
+        version='0.4.1',
         description='DAQP: A dual active-set QP solver',
         url='http://github.com/darnstrom/daqp',
         author='Daniel Arnström',
         author_email='daniel.arnstrom@liu.se',
         license='MIT',
         long_description=open('README.md','r').read(),
         long_description_content_type='text/markdown',
         ext_modules=cythonize(cython_ext),
         cmdclass={'build_ext': build_ext},
-        package_data = {'':["daqp.pyx","daqp.pxd"]},
-        include_package_data = True,
         zip_safe=False)
 
 # Cleanup C-source
 if src_path and os.path.exists(src_path):
     rmtree(csrc_dir)
     os.remove(pathlib.Path('./LICENSE'))
```

