# Comparing `tmp/ms_entropy-0.4.2.tar.gz` & `tmp/ms_entropy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.4.2.tar", last modified: Wed Apr 19 04:58:36 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.0.tar", last modified: Wed May 10 07:44:12 2023, max compression
```

## Comparing `ms_entropy-0.4.2.tar` & `ms_entropy-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.4.2/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       48 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.4.2/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/mimas/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)     4939 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/
--rw-rw-r--   0 yli       (1000) yli       (1000)     5950 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     5153 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     6002 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/
--rw-rw-r--   0 yli       (1000) yli       (1000)    16189 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      107 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/ms_entropy/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20202 2023-04-19 04:56:46.000000 ms_entropy-0.4.2/ms_entropy/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    33392 2023-03-27 19:39:45.000000 ms_entropy-0.4.2/ms_entropy/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     4317 2023-04-19 04:48:23.000000 ms_entropy-0.4.2/ms_entropy/tools.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   958514 2023-03-25 19:23:59.000000 ms_entropy-0.4.2/ms_entropy/tools_cython.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     7974 2023-03-25 18:55:15.000000 ms_entropy-0.4.2/ms_entropy/tools_cython.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)      751 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       44 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1371 2023-04-19 04:51:23.000000 ms_entropy-0.4.2/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.0/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       48 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.0/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/mimas/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/mimas/spectra/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.537449 ms_entropy-0.5.0/manuscript/src/mimas/spectra/fast_entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4939 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.541448 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5950 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5153 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     6002 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.541448 ms_entropy-0.5.0/manuscript/src/mimas/spectra/spectral_entropy_published/
+-rw-rw-r--   0 yli       (1000) yli       (1000)    16189 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.537449 ms_entropy-0.5.0/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.0/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.545448 ms_entropy-0.5.0/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)      730 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      103 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1541 2023-05-10 07:43:00.000000 ms_entropy-0.5.0/setup.py
```

### Comparing `ms_entropy-0.4.2/LICENSE` & `ms_entropy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/README.md` & `ms_entropy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx` & `ms_entropy-0.5.0/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx` & `ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx` & `ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx` & `ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx` & `ms_entropy-0.5.0/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.2/ms_entropy/tools_cython.c` & `ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
-        "name": "ms_entropy.tools_cython",
+        "name": "ms_entropy.tools.fast_entropy",
         "sources": [
-            "ms_entropy/tools_cython.pyx"
+            "ms_entropy/tools/fast_entropy.pyx"
         ]
     },
-    "module_name": "ms_entropy.tools_cython"
+    "module_name": "ms_entropy.tools.fast_entropy"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
@@ -747,16 +747,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__ms_entropy__tools_cython
-#define __PYX_HAVE_API__ms_entropy__tools_cython
+#define __PYX_HAVE__ms_entropy__tools__fast_entropy
+#define __PYX_HAVE_API__ms_entropy__tools__fast_entropy
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
@@ -995,15 +995,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "ms_entropy/tools_cython.pyx",
+  "ms_entropy/tools/fast_entropy.pyx",
   "__init__.pxd",
   "stringsource",
   "type.pxd",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
@@ -1056,26 +1056,26 @@
 #else
     #define __pyx_add_acquisition_count(memview)\
             __pyx_add_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
             __pyx_sub_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
 #endif
 
+/* ForceInitThreads.proto */
+#ifndef __PYX_FORCE_INIT_THREADS
+  #define __PYX_FORCE_INIT_THREADS 0
+#endif
+
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
-/* ForceInitThreads.proto */
-#ifndef __PYX_FORCE_INIT_THREADS
-  #define __PYX_FORCE_INIT_THREADS 0
-#endif
-
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
@@ -1294,49 +1294,49 @@
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 
-/* "ms_entropy/tools_cython.pyx":4
+/* "ms_entropy/tools/fast_entropy.pyx":4
  * cimport numpy as np
  * 
  * ctypedef np.float32_t float32             # <<<<<<<<<<<<<<
  * ctypedef np.int64_t int_64
  * ctypedef np.int8_t int_8
  */
-typedef __pyx_t_5numpy_float32_t __pyx_t_10ms_entropy_12tools_cython_float32;
+typedef __pyx_t_5numpy_float32_t __pyx_t_10ms_entropy_5tools_12fast_entropy_float32;
 
-/* "ms_entropy/tools_cython.pyx":5
+/* "ms_entropy/tools/fast_entropy.pyx":5
  * 
  * ctypedef np.float32_t float32
  * ctypedef np.int64_t int_64             # <<<<<<<<<<<<<<
  * ctypedef np.int8_t int_8
  * ctypedef np.uint32_t uint_32
  */
-typedef __pyx_t_5numpy_int64_t __pyx_t_10ms_entropy_12tools_cython_int_64;
+typedef __pyx_t_5numpy_int64_t __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64;
 
-/* "ms_entropy/tools_cython.pyx":6
+/* "ms_entropy/tools/fast_entropy.pyx":6
  * ctypedef np.float32_t float32
  * ctypedef np.int64_t int_64
  * ctypedef np.int8_t int_8             # <<<<<<<<<<<<<<
  * ctypedef np.uint32_t uint_32
  * from libc.math cimport log2,log,pow
  */
-typedef __pyx_t_5numpy_int8_t __pyx_t_10ms_entropy_12tools_cython_int_8;
+typedef __pyx_t_5numpy_int8_t __pyx_t_10ms_entropy_5tools_12fast_entropy_int_8;
 
-/* "ms_entropy/tools_cython.pyx":7
+/* "ms_entropy/tools/fast_entropy.pyx":7
  * ctypedef np.int64_t int_64
  * ctypedef np.int8_t int_8
  * ctypedef np.uint32_t uint_32             # <<<<<<<<<<<<<<
  * from libc.math cimport log2,log,pow
  * 
  */
-typedef __pyx_t_5numpy_uint32_t __pyx_t_10ms_entropy_12tools_cython_uint_32;
+typedef __pyx_t_5numpy_uint32_t __pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32;
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
@@ -1395,28 +1395,14 @@
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
-struct __pyx_opt_args_10ms_entropy_12tools_cython_centroid_spectrum;
-
-/* "ms_entropy/tools_cython.pyx":76
- * 
- * 
- * cpdef centroid_spectrum(float32[:,::1] spectrum,ms2_ppm=None, ms2_da=None):             # <<<<<<<<<<<<<<
- *     """
- *     Calculate centroid spectrum from a spectrum.
- */
-struct __pyx_opt_args_10ms_entropy_12tools_cython_centroid_spectrum {
-  int __pyx_n;
-  PyObject *ms2_ppm;
-  PyObject *ms2_da;
-};
 
 /* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
@@ -1753,43 +1739,14 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
-/* ObjectGetItem.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
-#else
-#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
-#endif
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1884,14 +1841,43 @@
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
 static CYTHON_UNUSED int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *); /*proto*/
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
+/* ObjectGetItem.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+#else
+#define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
+#endif
+
 /* decode_c_string_utf16.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = 0;
     return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
 }
 static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
     int byteorder = -1;
@@ -2134,34 +2120,31 @@
                 int ndim,
                 __Pyx_TypeInfo *dtype,
                 __Pyx_BufFmt_StackElem stack[],
                 __Pyx_memviewslice *memviewslice,
                 PyObject *original_obj);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32__const__(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32__const__(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_uint_32__const__(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32__const__(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_8__const__(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_int_8__const__(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
-static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32(const char *itemp);
-static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32(const char *itemp, PyObject *obj);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_64(PyObject *, int writable_flag);
+static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(const char *itemp);
+static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(const char *itemp, PyObject *obj);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
@@ -2272,21 +2255,21 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int64(npy_int64 value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int8(npy_int8 value);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
@@ -2341,32 +2324,29 @@
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'libc.math' */
 
-/* Module declarations from 'ms_entropy.tools_cython' */
+/* Module declarations from 'ms_entropy.tools.fast_entropy' */
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static void __pyx_f_10ms_entropy_12tools_cython_entropy_similarity_search_fast(__pyx_t_10ms_entropy_12tools_cython_int_64, __pyx_t_10ms_entropy_12tools_cython_int_64, __pyx_t_10ms_entropy_12tools_cython_float32, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int, __pyx_t_10ms_entropy_12tools_cython_int_64, __pyx_t_10ms_entropy_12tools_cython_int_64, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_apply_weight_to_intensity(__Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static double __pyx_f_10ms_entropy_12tools_cython_spectral_entropy(__Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_centroid_spectrum(__Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_10ms_entropy_12tools_cython_centroid_spectrum *__pyx_optional_args); /*proto*/
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_centroid_spectrum_c(__Pyx_memviewslice, double, double); /*proto*/
-static int __pyx_f_10ms_entropy_12tools_cython_check_centroid_c(__Pyx_memviewslice, double, double); /*proto*/
+static void __pyx_f_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(__pyx_t_10ms_entropy_5tools_12fast_entropy_int_64, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64, __pyx_t_10ms_entropy_5tools_12fast_entropy_float32, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_10ms_entropy_5tools_12fast_entropy_apply_weight_to_intensity(__Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static double __pyx_f_10ms_entropy_5tools_12fast_entropy_spectral_entropy(__Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static PyObject *assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
 static struct __pyx_memoryview_obj *__pyx_memview_slice(struct __pyx_memoryview_obj *, PyObject *); /*proto*/
@@ -2392,34 +2372,32 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_float32 = { "float32", NULL, sizeof(__pyx_t_10ms_entropy_12tools_cython_float32), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_float32__const__ = { "const float32", NULL, sizeof(__pyx_t_10ms_entropy_12tools_cython_float32 const ), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_uint_32__const__ = { "const uint_32", NULL, sizeof(__pyx_t_10ms_entropy_12tools_cython_uint_32 const ), { 0 }, 0, IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_uint_32 const ) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_uint_32 const ), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_int_8__const__ = { "const int_8", NULL, sizeof(__pyx_t_10ms_entropy_12tools_cython_int_8 const ), { 0 }, 0, IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_int_8 const ) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_int_8 const ), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_int_64 = { "int_64", NULL, sizeof(__pyx_t_10ms_entropy_12tools_cython_int_64), { 0 }, 0, IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_int_64) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_10ms_entropy_12tools_cython_int_64), 0 };
-#define __Pyx_MODULE_NAME "ms_entropy.tools_cython"
-extern int __pyx_module_is_main_ms_entropy__tools_cython;
-int __pyx_module_is_main_ms_entropy__tools_cython = 0;
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32 = { "float32", NULL, sizeof(__pyx_t_10ms_entropy_5tools_12fast_entropy_float32), { 0 }, 0, 'R', 0, 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32__const__ = { "const float32", NULL, sizeof(__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 const ), { 0 }, 0, 'R', 0, 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32__const__ = { "const uint_32", NULL, sizeof(__pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32 const ), { 0 }, 0, IS_UNSIGNED(__pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32 const ) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32 const ), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_int_8__const__ = { "const int_8", NULL, sizeof(__pyx_t_10ms_entropy_5tools_12fast_entropy_int_8 const ), { 0 }, 0, IS_UNSIGNED(__pyx_t_10ms_entropy_5tools_12fast_entropy_int_8 const ) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_10ms_entropy_5tools_12fast_entropy_int_8 const ), 0 };
+#define __Pyx_MODULE_NAME "ms_entropy.tools.fast_entropy"
+extern int __pyx_module_is_main_ms_entropy__tools__fast_entropy;
+int __pyx_module_is_main_ms_entropy__tools__fast_entropy = 0;
 
-/* Implementation of 'ms_entropy.tools_cython' */
+/* Implementation of 'ms_entropy.tools.fast_entropy' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ImportError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_enumerate;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
-static const char __pyx_k_C[] = "C";
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_base[] = "base";
@@ -2431,47 +2409,37 @@
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
-static const char __pyx_k_array[] = "array";
 static const char __pyx_k_class[] = "__class__";
-static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_numpy[] = "numpy";
-static const char __pyx_k_order[] = "order";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
-static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
-static const char __pyx_k_ms2_da[] = "ms2_da";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
-static const char __pyx_k_argsort[] = "argsort";
-static const char __pyx_k_asarray[] = "asarray";
-static const char __pyx_k_float32[] = "float32";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
-static const char __pyx_k_ms2_ppm[] = "ms2_ppm";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_spectrum[] = "spectrum";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_intensity[] = "intensity";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
@@ -2524,15 +2492,14 @@
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
-static PyObject *__pyx_n_u_C;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_ImportError;
@@ -2548,33 +2515,28 @@
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
-static PyObject *__pyx_n_s_argsort;
-static PyObject *__pyx_n_s_array;
-static PyObject *__pyx_n_s_asarray;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_dict;
-static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_flags;
-static PyObject *__pyx_n_s_float32;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
@@ -2583,27 +2545,24 @@
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_library_peaks_intensity;
 static PyObject *__pyx_n_s_library_spec_idx_array;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mixed_spectra_entropy;
 static PyObject *__pyx_n_s_mode;
-static PyObject *__pyx_n_s_ms2_da;
-static PyObject *__pyx_n_s_ms2_ppm;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
-static PyObject *__pyx_n_s_order;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_product_mz_idx_max;
 static PyObject *__pyx_n_s_product_mz_idx_min;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
@@ -2620,33 +2579,30 @@
 static PyObject *__pyx_n_s_search_spectra_idx_max;
 static PyObject *__pyx_n_s_search_spectra_idx_min;
 static PyObject *__pyx_n_s_search_type;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
-static PyObject *__pyx_n_s_spectrum;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
-static PyObject *__pyx_n_s_zeros;
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_entropy_similarity_search_fast(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array); /* proto */
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_2apply_weight_to_intensity(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum); /* proto */
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_4spectral_entropy(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum); /* proto */
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_6centroid_spectrum(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum, PyObject *__pyx_v_ms2_ppm, PyObject *__pyx_v_ms2_da); /* proto */
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array); /* proto */
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_2apply_weight_to_intensity(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum); /* proto */
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_4spectral_entropy(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2685,122 +2641,119 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_float_neg_1_;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
-static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
-static PyObject *__pyx_slice_;
+static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_slice__17;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
-/* "ms_entropy/tools_cython.pyx":11
+/* "ms_entropy/tools/fast_entropy.pyx":11
  * 
  * 
  * cpdef void entropy_similarity_search_fast(int_64 product_mz_idx_min, int_64 product_mz_idx_max,             # <<<<<<<<<<<<<<
  *                                     float32 intensity, float32[:] mixed_spectra_entropy,
  *                                     const float32[:] library_peaks_intensity, const uint_32[:] library_spec_idx_array,
  */
 
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static void __pyx_f_10ms_entropy_12tools_cython_entropy_similarity_search_fast(__pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  __pyx_t_10ms_entropy_12tools_cython_uint_32 __pyx_v_library_spec_idx;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_library_peak_intensity;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity_ab;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity_xlog2x;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_idx;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_t_1;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_t_2;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_t_3;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_t_4;
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static void __pyx_f_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(__pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32 __pyx_v_library_spec_idx;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_library_peak_intensity;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity_ab;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity_xlog2x;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_idx;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_t_1;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_t_2;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_t_3;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   size_t __pyx_t_7;
 
-  /* "ms_entropy/tools_cython.pyx":25
+  /* "ms_entropy/tools/fast_entropy.pyx":25
  *     cdef uint_32 library_spec_idx
  *     cdef float32 library_peak_intensity, intensity_ab
  *     cdef float32 intensity_xlog2x = intensity * log2(intensity)             # <<<<<<<<<<<<<<
  * 
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):
  */
   __pyx_v_intensity_xlog2x = (__pyx_v_intensity * log2(__pyx_v_intensity));
 
-  /* "ms_entropy/tools_cython.pyx":27
+  /* "ms_entropy/tools/fast_entropy.pyx":27
  *     cdef float32 intensity_xlog2x = intensity * log2(intensity)
  * 
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):             # <<<<<<<<<<<<<<
  *         library_spec_idx = library_spec_idx_array[idx]
  *         if (search_type == 0) or \
  */
   __pyx_t_1 = __pyx_v_product_mz_idx_max;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = __pyx_v_product_mz_idx_min; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_idx = __pyx_t_3;
 
-    /* "ms_entropy/tools_cython.pyx":28
+    /* "ms_entropy/tools/fast_entropy.pyx":28
  * 
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):
  *         library_spec_idx = library_spec_idx_array[idx]             # <<<<<<<<<<<<<<
  *         if (search_type == 0) or \
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
  */
     __pyx_t_4 = __pyx_v_idx;
-    __pyx_v_library_spec_idx = (*((__pyx_t_10ms_entropy_12tools_cython_uint_32 const  *) ( /* dim=0 */ (__pyx_v_library_spec_idx_array.data + __pyx_t_4 * __pyx_v_library_spec_idx_array.strides[0]) )));
+    __pyx_v_library_spec_idx = (*((__pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32 const  *) ( /* dim=0 */ (__pyx_v_library_spec_idx_array.data + __pyx_t_4 * __pyx_v_library_spec_idx_array.strides[0]) )));
 
-    /* "ms_entropy/tools_cython.pyx":29
+    /* "ms_entropy/tools/fast_entropy.pyx":29
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):
  *         library_spec_idx = library_spec_idx_array[idx]
  *         if (search_type == 0) or \             # <<<<<<<<<<<<<<
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
  *                 (search_type == 2 and search_array[library_spec_idx]):
  */
     __pyx_t_6 = ((__pyx_v_search_type == 0) != 0);
     if (!__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
       goto __pyx_L6_bool_binop_done;
     }
 
-    /* "ms_entropy/tools_cython.pyx":30
+    /* "ms_entropy/tools/fast_entropy.pyx":30
  *         library_spec_idx = library_spec_idx_array[idx]
  *         if (search_type == 0) or \
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \             # <<<<<<<<<<<<<<
  *                 (search_type == 2 and search_array[library_spec_idx]):
  *             # Match this peak
  */
     __pyx_t_6 = ((__pyx_v_search_type == 1) != 0);
@@ -2817,104 +2770,104 @@
     if (!__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_L8_next_or:;
 
-    /* "ms_entropy/tools_cython.pyx":31
+    /* "ms_entropy/tools/fast_entropy.pyx":31
  *         if (search_type == 0) or \
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
  *                 (search_type == 2 and search_array[library_spec_idx]):             # <<<<<<<<<<<<<<
  *             # Match this peak
  *             library_peak_intensity = library_peaks_intensity[idx]
  */
     __pyx_t_6 = ((__pyx_v_search_type == 2) != 0);
     if (__pyx_t_6) {
     } else {
       __pyx_t_5 = __pyx_t_6;
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_7 = __pyx_v_library_spec_idx;
-    __pyx_t_6 = ((*((__pyx_t_10ms_entropy_12tools_cython_int_8 const  *) ( /* dim=0 */ (__pyx_v_search_array.data + __pyx_t_7 * __pyx_v_search_array.strides[0]) ))) != 0);
+    __pyx_t_6 = ((*((__pyx_t_10ms_entropy_5tools_12fast_entropy_int_8 const  *) ( /* dim=0 */ (__pyx_v_search_array.data + __pyx_t_7 * __pyx_v_search_array.strides[0]) ))) != 0);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L6_bool_binop_done:;
 
-    /* "ms_entropy/tools_cython.pyx":29
+    /* "ms_entropy/tools/fast_entropy.pyx":29
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):
  *         library_spec_idx = library_spec_idx_array[idx]
  *         if (search_type == 0) or \             # <<<<<<<<<<<<<<
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
  *                 (search_type == 2 and search_array[library_spec_idx]):
  */
     if (__pyx_t_5) {
 
-      /* "ms_entropy/tools_cython.pyx":33
+      /* "ms_entropy/tools/fast_entropy.pyx":33
  *                 (search_type == 2 and search_array[library_spec_idx]):
  *             # Match this peak
  *             library_peak_intensity = library_peaks_intensity[idx]             # <<<<<<<<<<<<<<
  *             intensity_ab = intensity + library_peak_intensity
  * 
  */
       __pyx_t_4 = __pyx_v_idx;
-      __pyx_v_library_peak_intensity = (*((__pyx_t_10ms_entropy_12tools_cython_float32 const  *) ( /* dim=0 */ (__pyx_v_library_peaks_intensity.data + __pyx_t_4 * __pyx_v_library_peaks_intensity.strides[0]) )));
+      __pyx_v_library_peak_intensity = (*((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 const  *) ( /* dim=0 */ (__pyx_v_library_peaks_intensity.data + __pyx_t_4 * __pyx_v_library_peaks_intensity.strides[0]) )));
 
-      /* "ms_entropy/tools_cython.pyx":34
+      /* "ms_entropy/tools/fast_entropy.pyx":34
  *             # Match this peak
  *             library_peak_intensity = library_peaks_intensity[idx]
  *             intensity_ab = intensity + library_peak_intensity             # <<<<<<<<<<<<<<
  * 
  *             mixed_spectra_entropy[library_spec_idx] += \
  */
       __pyx_v_intensity_ab = (__pyx_v_intensity + __pyx_v_library_peak_intensity);
 
-      /* "ms_entropy/tools_cython.pyx":36
+      /* "ms_entropy/tools/fast_entropy.pyx":36
  *             intensity_ab = intensity + library_peak_intensity
  * 
  *             mixed_spectra_entropy[library_spec_idx] += \             # <<<<<<<<<<<<<<
  *                 intensity_ab * log2(intensity_ab) - \
  *                 intensity_xlog2x - \
  */
       __pyx_t_7 = __pyx_v_library_spec_idx;
-      *((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_mixed_spectra_entropy.data + __pyx_t_7 * __pyx_v_mixed_spectra_entropy.strides[0]) )) += (((__pyx_v_intensity_ab * log2(__pyx_v_intensity_ab)) - __pyx_v_intensity_xlog2x) - (__pyx_v_library_peak_intensity * log2(__pyx_v_library_peak_intensity)));
+      *((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_mixed_spectra_entropy.data + __pyx_t_7 * __pyx_v_mixed_spectra_entropy.strides[0]) )) += (((__pyx_v_intensity_ab * log2(__pyx_v_intensity_ab)) - __pyx_v_intensity_xlog2x) - (__pyx_v_library_peak_intensity * log2(__pyx_v_library_peak_intensity)));
 
-      /* "ms_entropy/tools_cython.pyx":29
+      /* "ms_entropy/tools/fast_entropy.pyx":29
  *     for idx in range(product_mz_idx_min, product_mz_idx_max):
  *         library_spec_idx = library_spec_idx_array[idx]
  *         if (search_type == 0) or \             # <<<<<<<<<<<<<<
  *                 (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
  *                 (search_type == 2 and search_array[library_spec_idx]):
  */
     }
   }
 
-  /* "ms_entropy/tools_cython.pyx":11
+  /* "ms_entropy/tools/fast_entropy.pyx":11
  * 
  * 
  * cpdef void entropy_similarity_search_fast(int_64 product_mz_idx_min, int_64 product_mz_idx_max,             # <<<<<<<<<<<<<<
  *                                     float32 intensity, float32[:] mixed_spectra_entropy,
  *                                     const float32[:] library_peaks_intensity, const uint_32[:] library_spec_idx_array,
  */
 
   /* function exit code */
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10ms_entropy_12tools_cython_entropy_similarity_search_fast[] = "\n    The mixed_spectra_entropy will be modified in this function.\n    search_type is 0: search all spectra.\n    search_type is 1: search spectra in the range [search_spectra_idx_min, search_spectra_idx_max).\n    search_type is 2: search spectra in the array search_array with entry equals 1, the length of search_array should be equal to the self.total_spectra_num\n\n    Note: the intensity here should be half of the original intensity.\n    ";
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_min;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_max;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity;
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast[] = "\n    The mixed_spectra_entropy will be modified in this function.\n    search_type is 0: search all spectra.\n    search_type is 1: search spectra in the range [search_spectra_idx_min, search_spectra_idx_max).\n    search_type is 2: search spectra in the array search_array with entry equals 1, the length of search_array should be equal to the self.total_spectra_num\n\n    Note: the intensity here should be half of the original intensity.\n    ";
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_1entropy_similarity_search_fast(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_min;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_max;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity;
   __Pyx_memviewslice __pyx_v_mixed_spectra_entropy = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_library_peaks_intensity = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_library_spec_idx_array = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_search_type;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_min;
-  __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_max;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_min;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_max;
   __Pyx_memviewslice __pyx_v_search_array = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("entropy_similarity_search_fast (wrapper)", 0);
@@ -3024,81 +2977,81 @@
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
     }
     __pyx_v_product_mz_idx_min = __Pyx_PyInt_As_npy_int64(values[0]); if (unlikely((__pyx_v_product_mz_idx_min == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L3_error)
     __pyx_v_product_mz_idx_max = __Pyx_PyInt_As_npy_int64(values[1]); if (unlikely((__pyx_v_product_mz_idx_max == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L3_error)
     __pyx_v_intensity = __pyx_PyFloat_AsFloat(values[2]); if (unlikely((__pyx_v_intensity == ((npy_float32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L3_error)
-    __pyx_v_mixed_spectra_entropy = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_mixed_spectra_entropy.memview)) __PYX_ERR(0, 12, __pyx_L3_error)
-    __pyx_v_library_peaks_intensity = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32__const__(values[4], 0); if (unlikely(!__pyx_v_library_peaks_intensity.memview)) __PYX_ERR(0, 13, __pyx_L3_error)
-    __pyx_v_library_spec_idx_array = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_uint_32__const__(values[5], 0); if (unlikely(!__pyx_v_library_spec_idx_array.memview)) __PYX_ERR(0, 13, __pyx_L3_error)
+    __pyx_v_mixed_spectra_entropy = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_mixed_spectra_entropy.memview)) __PYX_ERR(0, 12, __pyx_L3_error)
+    __pyx_v_library_peaks_intensity = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32__const__(values[4], 0); if (unlikely(!__pyx_v_library_peaks_intensity.memview)) __PYX_ERR(0, 13, __pyx_L3_error)
+    __pyx_v_library_spec_idx_array = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32__const__(values[5], 0); if (unlikely(!__pyx_v_library_spec_idx_array.memview)) __PYX_ERR(0, 13, __pyx_L3_error)
     __pyx_v_search_type = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_search_type == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 14, __pyx_L3_error)
     __pyx_v_search_spectra_idx_min = __Pyx_PyInt_As_npy_int64(values[7]); if (unlikely((__pyx_v_search_spectra_idx_min == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 14, __pyx_L3_error)
     __pyx_v_search_spectra_idx_max = __Pyx_PyInt_As_npy_int64(values[8]); if (unlikely((__pyx_v_search_spectra_idx_max == ((npy_int64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 14, __pyx_L3_error)
-    __pyx_v_search_array = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_8__const__(values[9], 0); if (unlikely(!__pyx_v_search_array.memview)) __PYX_ERR(0, 14, __pyx_L3_error)
+    __pyx_v_search_array = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_int_8__const__(values[9], 0); if (unlikely(!__pyx_v_search_array.memview)) __PYX_ERR(0, 14, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("entropy_similarity_search_fast", 1, 10, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 11, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("ms_entropy.tools_cython.entropy_similarity_search_fast", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.entropy_similarity_search_fast", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10ms_entropy_12tools_cython_entropy_similarity_search_fast(__pyx_self, __pyx_v_product_mz_idx_min, __pyx_v_product_mz_idx_max, __pyx_v_intensity, __pyx_v_mixed_spectra_entropy, __pyx_v_library_peaks_intensity, __pyx_v_library_spec_idx_array, __pyx_v_search_type, __pyx_v_search_spectra_idx_min, __pyx_v_search_spectra_idx_max, __pyx_v_search_array);
+  __pyx_r = __pyx_pf_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(__pyx_self, __pyx_v_product_mz_idx_min, __pyx_v_product_mz_idx_max, __pyx_v_intensity, __pyx_v_mixed_spectra_entropy, __pyx_v_library_peaks_intensity, __pyx_v_library_spec_idx_array, __pyx_v_search_type, __pyx_v_search_spectra_idx_min, __pyx_v_search_spectra_idx_max, __pyx_v_search_array);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_entropy_similarity_search_fast(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_12tools_cython_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array) {
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_product_mz_idx_max, __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity, __Pyx_memviewslice __pyx_v_mixed_spectra_entropy, __Pyx_memviewslice __pyx_v_library_peaks_intensity, __Pyx_memviewslice __pyx_v_library_spec_idx_array, int __pyx_v_search_type, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_min, __pyx_t_10ms_entropy_5tools_12fast_entropy_int_64 __pyx_v_search_spectra_idx_max, __Pyx_memviewslice __pyx_v_search_array) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("entropy_similarity_search_fast", 0);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_mixed_spectra_entropy.memview)) { __Pyx_RaiseUnboundLocalError("mixed_spectra_entropy"); __PYX_ERR(0, 11, __pyx_L1_error) }
   if (unlikely(!__pyx_v_library_peaks_intensity.memview)) { __Pyx_RaiseUnboundLocalError("library_peaks_intensity"); __PYX_ERR(0, 11, __pyx_L1_error) }
   if (unlikely(!__pyx_v_library_spec_idx_array.memview)) { __Pyx_RaiseUnboundLocalError("library_spec_idx_array"); __PYX_ERR(0, 11, __pyx_L1_error) }
   if (unlikely(!__pyx_v_search_array.memview)) { __Pyx_RaiseUnboundLocalError("search_array"); __PYX_ERR(0, 11, __pyx_L1_error) }
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_10ms_entropy_12tools_cython_entropy_similarity_search_fast(__pyx_v_product_mz_idx_min, __pyx_v_product_mz_idx_max, __pyx_v_intensity, __pyx_v_mixed_spectra_entropy, __pyx_v_library_peaks_intensity, __pyx_v_library_spec_idx_array, __pyx_v_search_type, __pyx_v_search_spectra_idx_min, __pyx_v_search_spectra_idx_max, __pyx_v_search_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast(__pyx_v_product_mz_idx_min, __pyx_v_product_mz_idx_max, __pyx_v_intensity, __pyx_v_mixed_spectra_entropy, __pyx_v_library_peaks_intensity, __pyx_v_library_spec_idx_array, __pyx_v_search_type, __pyx_v_search_spectra_idx_min, __pyx_v_search_spectra_idx_max, __pyx_v_search_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.entropy_similarity_search_fast", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.entropy_similarity_search_fast", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_mixed_spectra_entropy, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_library_peaks_intensity, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_library_spec_idx_array, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_search_array, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ms_entropy/tools_cython.pyx":42
+/* "ms_entropy/tools/fast_entropy.pyx":42
  * 
  * 
  * cpdef apply_weight_to_intensity(float32[:,::1] spectrum):             # <<<<<<<<<<<<<<
  *     """
  *     Apply the weight to the intensity.
  */
 
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_apply_weight_to_intensity(__Pyx_memviewslice __pyx_v_spectrum, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
+static PyObject *__pyx_f_10ms_entropy_5tools_12fast_entropy_apply_weight_to_intensity(__Pyx_memviewslice __pyx_v_spectrum, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_v_entropy;
   double __pyx_v_weight;
   double __pyx_v_intensity_sum;
   __Pyx_memviewslice __pyx_v_spectrum_weighted = { 0, 0, { 0 }, { 0 }, { 0 } };
   Py_ssize_t __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3116,36 +3069,36 @@
   Py_ssize_t __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_weight_to_intensity", 0);
 
-  /* "ms_entropy/tools_cython.pyx":47
+  /* "ms_entropy/tools/fast_entropy.pyx":47
  *     The spectrum is a 2D array like: [[m/z, intensity], [m/z, intensity], ...]
  *     """
  *     cdef double entropy=spectral_entropy(spectrum)             # <<<<<<<<<<<<<<
  *     cdef double weight, intensity_sum
  *     cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)
  */
-  __pyx_v_entropy = __pyx_f_10ms_entropy_12tools_cython_spectral_entropy(__pyx_v_spectrum, 0);
+  __pyx_v_entropy = __pyx_f_10ms_entropy_5tools_12fast_entropy_spectral_entropy(__pyx_v_spectrum, 0);
 
-  /* "ms_entropy/tools_cython.pyx":49
+  /* "ms_entropy/tools/fast_entropy.pyx":49
  *     cdef double entropy=spectral_entropy(spectrum)
  *     cdef double weight, intensity_sum
  *     cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)             # <<<<<<<<<<<<<<
  *     if entropy<3:
  *         weight = 0.25 + 0.25 * entropy
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_spectrum, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_spectrum, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
@@ -3155,1613 +3108,389 @@
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_spectrum_weighted = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "ms_entropy/tools_cython.pyx":50
+  /* "ms_entropy/tools/fast_entropy.pyx":50
  *     cdef double weight, intensity_sum
  *     cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)
  *     if entropy<3:             # <<<<<<<<<<<<<<
  *         weight = 0.25 + 0.25 * entropy
  *         intensity_sum = 0.
  */
   __pyx_t_6 = ((__pyx_v_entropy < 3.0) != 0);
   if (__pyx_t_6) {
 
-    /* "ms_entropy/tools_cython.pyx":51
+    /* "ms_entropy/tools/fast_entropy.pyx":51
  *     cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)
  *     if entropy<3:
  *         weight = 0.25 + 0.25 * entropy             # <<<<<<<<<<<<<<
  *         intensity_sum = 0.
  *         for i in range(spectrum_weighted.shape[0]):
  */
     __pyx_v_weight = (0.25 + (0.25 * __pyx_v_entropy));
 
-    /* "ms_entropy/tools_cython.pyx":52
+    /* "ms_entropy/tools/fast_entropy.pyx":52
  *     if entropy<3:
  *         weight = 0.25 + 0.25 * entropy
  *         intensity_sum = 0.             # <<<<<<<<<<<<<<
  *         for i in range(spectrum_weighted.shape[0]):
  *             spectrum_weighted[i,1] = pow(spectrum_weighted[i,1],weight)
  */
     __pyx_v_intensity_sum = 0.;
 
-    /* "ms_entropy/tools_cython.pyx":53
+    /* "ms_entropy/tools/fast_entropy.pyx":53
  *         weight = 0.25 + 0.25 * entropy
  *         intensity_sum = 0.
  *         for i in range(spectrum_weighted.shape[0]):             # <<<<<<<<<<<<<<
  *             spectrum_weighted[i,1] = pow(spectrum_weighted[i,1],weight)
  *             intensity_sum += spectrum_weighted[i,1]
  */
     __pyx_t_7 = (__pyx_v_spectrum_weighted.shape[0]);
     __pyx_t_8 = __pyx_t_7;
     for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
       __pyx_v_i = __pyx_t_9;
 
-      /* "ms_entropy/tools_cython.pyx":54
+      /* "ms_entropy/tools/fast_entropy.pyx":54
  *         intensity_sum = 0.
  *         for i in range(spectrum_weighted.shape[0]):
  *             spectrum_weighted[i,1] = pow(spectrum_weighted[i,1],weight)             # <<<<<<<<<<<<<<
  *             intensity_sum += spectrum_weighted[i,1]
  * 
  */
       __pyx_t_10 = __pyx_v_i;
       __pyx_t_11 = 1;
       __pyx_t_12 = __pyx_v_i;
       __pyx_t_13 = 1;
-      *((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_12 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_13)) )) = pow((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_10 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_11)) ))), __pyx_v_weight);
+      *((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_12 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_13)) )) = pow((*((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_10 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_11)) ))), __pyx_v_weight);
 
-      /* "ms_entropy/tools_cython.pyx":55
+      /* "ms_entropy/tools/fast_entropy.pyx":55
  *         for i in range(spectrum_weighted.shape[0]):
  *             spectrum_weighted[i,1] = pow(spectrum_weighted[i,1],weight)
  *             intensity_sum += spectrum_weighted[i,1]             # <<<<<<<<<<<<<<
  * 
  *         if intensity_sum>0:
  */
       __pyx_t_11 = __pyx_v_i;
       __pyx_t_10 = 1;
-      __pyx_v_intensity_sum = (__pyx_v_intensity_sum + (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_11 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_10)) ))));
+      __pyx_v_intensity_sum = (__pyx_v_intensity_sum + (*((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_11 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_10)) ))));
     }
 
-    /* "ms_entropy/tools_cython.pyx":57
+    /* "ms_entropy/tools/fast_entropy.pyx":57
  *             intensity_sum += spectrum_weighted[i,1]
  * 
  *         if intensity_sum>0:             # <<<<<<<<<<<<<<
  *             for i in range(spectrum_weighted.shape[0]):
  *                 spectrum_weighted[i,1] /= intensity_sum
  */
     __pyx_t_6 = ((__pyx_v_intensity_sum > 0.0) != 0);
     if (__pyx_t_6) {
 
-      /* "ms_entropy/tools_cython.pyx":58
+      /* "ms_entropy/tools/fast_entropy.pyx":58
  * 
  *         if intensity_sum>0:
  *             for i in range(spectrum_weighted.shape[0]):             # <<<<<<<<<<<<<<
  *                 spectrum_weighted[i,1] /= intensity_sum
  * 
  */
       __pyx_t_7 = (__pyx_v_spectrum_weighted.shape[0]);
       __pyx_t_8 = __pyx_t_7;
       for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
         __pyx_v_i = __pyx_t_9;
 
-        /* "ms_entropy/tools_cython.pyx":59
+        /* "ms_entropy/tools/fast_entropy.pyx":59
  *         if intensity_sum>0:
  *             for i in range(spectrum_weighted.shape[0]):
  *                 spectrum_weighted[i,1] /= intensity_sum             # <<<<<<<<<<<<<<
  * 
  *     return spectrum_weighted
  */
         __pyx_t_10 = __pyx_v_i;
         __pyx_t_11 = 1;
-        *((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_10 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_11)) )) /= __pyx_v_intensity_sum;
+        *((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_spectrum_weighted.data + __pyx_t_10 * __pyx_v_spectrum_weighted.strides[0]) )) + __pyx_t_11)) )) /= __pyx_v_intensity_sum;
       }
 
-      /* "ms_entropy/tools_cython.pyx":57
+      /* "ms_entropy/tools/fast_entropy.pyx":57
  *             intensity_sum += spectrum_weighted[i,1]
  * 
  *         if intensity_sum>0:             # <<<<<<<<<<<<<<
  *             for i in range(spectrum_weighted.shape[0]):
  *                 spectrum_weighted[i,1] /= intensity_sum
  */
     }
 
-    /* "ms_entropy/tools_cython.pyx":50
+    /* "ms_entropy/tools/fast_entropy.pyx":50
  *     cdef double weight, intensity_sum
  *     cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)
  *     if entropy<3:             # <<<<<<<<<<<<<<
  *         weight = 0.25 + 0.25 * entropy
  *         intensity_sum = 0.
  */
   }
 
-  /* "ms_entropy/tools_cython.pyx":61
+  /* "ms_entropy/tools/fast_entropy.pyx":61
  *                 spectrum_weighted[i,1] /= intensity_sum
  * 
  *     return spectrum_weighted             # <<<<<<<<<<<<<<
  * 
  * cpdef double spectral_entropy(float32[:,::1] spectrum) nogil:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_spectrum_weighted, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_spectrum_weighted, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "ms_entropy/tools_cython.pyx":42
+  /* "ms_entropy/tools/fast_entropy.pyx":42
  * 
  * 
  * cpdef apply_weight_to_intensity(float32[:,::1] spectrum):             # <<<<<<<<<<<<<<
  *     """
  *     Apply the weight to the intensity.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum_weighted, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
-static char __pyx_doc_10ms_entropy_12tools_cython_2apply_weight_to_intensity[] = "\n    Apply the weight to the intensity.\n    The spectrum is a 2D array like: [[m/z, intensity], [m/z, intensity], ...]\n    ";
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum) {
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
+static char __pyx_doc_10ms_entropy_5tools_12fast_entropy_2apply_weight_to_intensity[] = "\n    Apply the weight to the intensity.\n    The spectrum is a 2D array like: [[m/z, intensity], [m/z, intensity], ...]\n    ";
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_3apply_weight_to_intensity(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum) {
   __Pyx_memviewslice __pyx_v_spectrum = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("apply_weight_to_intensity (wrapper)", 0);
   assert(__pyx_arg_spectrum); {
-    __pyx_v_spectrum = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(__pyx_arg_spectrum, PyBUF_WRITABLE); if (unlikely(!__pyx_v_spectrum.memview)) __PYX_ERR(0, 42, __pyx_L3_error)
+    __pyx_v_spectrum = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(__pyx_arg_spectrum, PyBUF_WRITABLE); if (unlikely(!__pyx_v_spectrum.memview)) __PYX_ERR(0, 42, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("ms_entropy.tools_cython.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10ms_entropy_12tools_cython_2apply_weight_to_intensity(__pyx_self, __pyx_v_spectrum);
+  __pyx_r = __pyx_pf_10ms_entropy_5tools_12fast_entropy_2apply_weight_to_intensity(__pyx_self, __pyx_v_spectrum);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_2apply_weight_to_intensity(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum) {
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_2apply_weight_to_intensity(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("apply_weight_to_intensity", 0);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_spectrum.memview)) { __Pyx_RaiseUnboundLocalError("spectrum"); __PYX_ERR(0, 42, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_10ms_entropy_12tools_cython_apply_weight_to_intensity(__pyx_v_spectrum, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10ms_entropy_5tools_12fast_entropy_apply_weight_to_intensity(__pyx_v_spectrum, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.apply_weight_to_intensity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ms_entropy/tools_cython.pyx":63
+/* "ms_entropy/tools/fast_entropy.pyx":63
  *     return spectrum_weighted
  * 
  * cpdef double spectral_entropy(float32[:,::1] spectrum) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.
  */
 
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
-static double __pyx_f_10ms_entropy_12tools_cython_spectral_entropy(__Pyx_memviewslice __pyx_v_spectrum, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
+static double __pyx_f_10ms_entropy_5tools_12fast_entropy_spectral_entropy(__Pyx_memviewslice __pyx_v_spectrum, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_v_entropy;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity;
+  __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 __pyx_v_intensity;
   Py_ssize_t __pyx_v_i;
   double __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
 
-  /* "ms_entropy/tools_cython.pyx":67
+  /* "ms_entropy/tools/fast_entropy.pyx":67
  *     Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.
  *     """
  *     cdef double entropy=0.             # <<<<<<<<<<<<<<
  *     cdef float32 intensity
  *     for i in range(spectrum.shape[0]):
  */
   __pyx_v_entropy = 0.;
 
-  /* "ms_entropy/tools_cython.pyx":69
+  /* "ms_entropy/tools/fast_entropy.pyx":69
  *     cdef double entropy=0.
  *     cdef float32 intensity
  *     for i in range(spectrum.shape[0]):             # <<<<<<<<<<<<<<
  *         intensity=spectrum[i,1]
  *         if intensity>0:
  */
   __pyx_t_1 = (__pyx_v_spectrum.shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "ms_entropy/tools_cython.pyx":70
+    /* "ms_entropy/tools/fast_entropy.pyx":70
  *     cdef float32 intensity
  *     for i in range(spectrum.shape[0]):
  *         intensity=spectrum[i,1]             # <<<<<<<<<<<<<<
  *         if intensity>0:
  *             entropy+=-intensity*log(intensity)
  */
     __pyx_t_4 = __pyx_v_i;
     __pyx_t_5 = 1;
-    __pyx_v_intensity = (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_4 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_5)) )));
+    __pyx_v_intensity = (*((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_4 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_5)) )));
 
-    /* "ms_entropy/tools_cython.pyx":71
+    /* "ms_entropy/tools/fast_entropy.pyx":71
  *     for i in range(spectrum.shape[0]):
  *         intensity=spectrum[i,1]
  *         if intensity>0:             # <<<<<<<<<<<<<<
  *             entropy+=-intensity*log(intensity)
  *     return entropy
  */
     __pyx_t_6 = ((__pyx_v_intensity > 0.0) != 0);
     if (__pyx_t_6) {
 
-      /* "ms_entropy/tools_cython.pyx":72
+      /* "ms_entropy/tools/fast_entropy.pyx":72
  *         intensity=spectrum[i,1]
  *         if intensity>0:
  *             entropy+=-intensity*log(intensity)             # <<<<<<<<<<<<<<
  *     return entropy
  * 
  */
       __pyx_v_entropy = (__pyx_v_entropy + ((-__pyx_v_intensity) * log(__pyx_v_intensity)));
 
-      /* "ms_entropy/tools_cython.pyx":71
+      /* "ms_entropy/tools/fast_entropy.pyx":71
  *     for i in range(spectrum.shape[0]):
  *         intensity=spectrum[i,1]
  *         if intensity>0:             # <<<<<<<<<<<<<<
  *             entropy+=-intensity*log(intensity)
  *     return entropy
  */
     }
   }
 
-  /* "ms_entropy/tools_cython.pyx":73
+  /* "ms_entropy/tools/fast_entropy.pyx":73
  *         if intensity>0:
  *             entropy+=-intensity*log(intensity)
  *     return entropy             # <<<<<<<<<<<<<<
  * 
- * 
  */
   __pyx_r = __pyx_v_entropy;
   goto __pyx_L0;
 
-  /* "ms_entropy/tools_cython.pyx":63
+  /* "ms_entropy/tools/fast_entropy.pyx":63
  *     return spectrum_weighted
  * 
  * cpdef double spectral_entropy(float32[:,::1] spectrum) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
-static char __pyx_doc_10ms_entropy_12tools_cython_4spectral_entropy[] = "\n    Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.\n    ";
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum) {
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum); /*proto*/
+static char __pyx_doc_10ms_entropy_5tools_12fast_entropy_4spectral_entropy[] = "\n    Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.\n    ";
+static PyObject *__pyx_pw_10ms_entropy_5tools_12fast_entropy_5spectral_entropy(PyObject *__pyx_self, PyObject *__pyx_arg_spectrum) {
   __Pyx_memviewslice __pyx_v_spectrum = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("spectral_entropy (wrapper)", 0);
   assert(__pyx_arg_spectrum); {
-    __pyx_v_spectrum = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(__pyx_arg_spectrum, PyBUF_WRITABLE); if (unlikely(!__pyx_v_spectrum.memview)) __PYX_ERR(0, 63, __pyx_L3_error)
+    __pyx_v_spectrum = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(__pyx_arg_spectrum, PyBUF_WRITABLE); if (unlikely(!__pyx_v_spectrum.memview)) __PYX_ERR(0, 63, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("ms_entropy.tools_cython.spectral_entropy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.spectral_entropy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10ms_entropy_12tools_cython_4spectral_entropy(__pyx_self, __pyx_v_spectrum);
+  __pyx_r = __pyx_pf_10ms_entropy_5tools_12fast_entropy_4spectral_entropy(__pyx_self, __pyx_v_spectrum);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_4spectral_entropy(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum) {
+static PyObject *__pyx_pf_10ms_entropy_5tools_12fast_entropy_4spectral_entropy(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spectral_entropy", 0);
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(!__pyx_v_spectrum.memview)) { __Pyx_RaiseUnboundLocalError("spectrum"); __PYX_ERR(0, 63, __pyx_L1_error) }
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_10ms_entropy_12tools_cython_spectral_entropy(__pyx_v_spectrum, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_10ms_entropy_5tools_12fast_entropy_spectral_entropy(__pyx_v_spectrum, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.spectral_entropy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("ms_entropy.tools.fast_entropy.spectral_entropy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ms_entropy/tools_cython.pyx":76
- * 
- * 
- * cpdef centroid_spectrum(float32[:,::1] spectrum,ms2_ppm=None, ms2_da=None):             # <<<<<<<<<<<<<<
- *     """
- *     Calculate centroid spectrum from a spectrum.
- */
-
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_7centroid_spectrum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_centroid_spectrum(__Pyx_memviewslice __pyx_v_spectrum, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_10ms_entropy_12tools_cython_centroid_spectrum *__pyx_optional_args) {
-  PyObject *__pyx_v_ms2_ppm = ((PyObject *)Py_None);
-  PyObject *__pyx_v_ms2_da = ((PyObject *)Py_None);
-  int __pyx_v_need_centroid;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  double __pyx_t_3;
-  double __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("centroid_spectrum", 0);
-  if (__pyx_optional_args) {
-    if (__pyx_optional_args->__pyx_n > 0) {
-      __pyx_v_ms2_ppm = __pyx_optional_args->ms2_ppm;
-      if (__pyx_optional_args->__pyx_n > 1) {
-        __pyx_v_ms2_da = __pyx_optional_args->ms2_da;
-      }
-    }
-  }
-  __PYX_INC_MEMVIEW(&__pyx_v_spectrum, 1);
-  __Pyx_INCREF(__pyx_v_ms2_ppm);
-  __Pyx_INCREF(__pyx_v_ms2_da);
-
-  /* "ms_entropy/tools_cython.pyx":88
- *     :param ms2_da: the mass accuracy in Da.
- *     """
- *     if ms2_da is None:             # <<<<<<<<<<<<<<
- *         ms2_da = -1.
- *     else:
- */
-  __pyx_t_1 = (__pyx_v_ms2_da == Py_None);
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
-
-    /* "ms_entropy/tools_cython.pyx":89
- *     """
- *     if ms2_da is None:
- *         ms2_da = -1.             # <<<<<<<<<<<<<<
- *     else:
- *         ms2_ppm = -1.
- */
-    __Pyx_INCREF(__pyx_float_neg_1_);
-    __Pyx_DECREF_SET(__pyx_v_ms2_da, __pyx_float_neg_1_);
-
-    /* "ms_entropy/tools_cython.pyx":88
- *     :param ms2_da: the mass accuracy in Da.
- *     """
- *     if ms2_da is None:             # <<<<<<<<<<<<<<
- *         ms2_da = -1.
- *     else:
- */
-    goto __pyx_L3;
-  }
-
-  /* "ms_entropy/tools_cython.pyx":91
- *         ms2_da = -1.
- *     else:
- *         ms2_ppm = -1.             # <<<<<<<<<<<<<<
- * 
- *     # Check whether the spectrum needs to be centroided or not.
- */
-  /*else*/ {
-    __Pyx_INCREF(__pyx_float_neg_1_);
-    __Pyx_DECREF_SET(__pyx_v_ms2_ppm, __pyx_float_neg_1_);
-  }
-  __pyx_L3:;
-
-  /* "ms_entropy/tools_cython.pyx":94
- * 
- *     # Check whether the spectrum needs to be centroided or not.
- *     cdef int need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)             # <<<<<<<<<<<<<<
- *     while need_centroid:
- *         spectrum = centroid_spectrum_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- */
-  __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_ppm); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_da); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_v_need_centroid = __pyx_f_10ms_entropy_12tools_cython_check_centroid_c(__pyx_v_spectrum, __pyx_t_3, __pyx_t_4);
-
-  /* "ms_entropy/tools_cython.pyx":95
- *     # Check whether the spectrum needs to be centroided or not.
- *     cdef int need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *     while need_centroid:             # <<<<<<<<<<<<<<
- *         spectrum = centroid_spectrum_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *         need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- */
-  while (1) {
-    __pyx_t_2 = (__pyx_v_need_centroid != 0);
-    if (!__pyx_t_2) break;
-
-    /* "ms_entropy/tools_cython.pyx":96
- *     cdef int need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *     while need_centroid:
- *         spectrum = centroid_spectrum_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)             # <<<<<<<<<<<<<<
- *         need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *     return np.asarray(spectrum)
- */
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_ppm); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 96, __pyx_L1_error)
-    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_da); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 96, __pyx_L1_error)
-    __pyx_t_5 = __pyx_f_10ms_entropy_12tools_cython_centroid_spectrum_c(__pyx_v_spectrum, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(__pyx_t_5, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 96, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum, 1);
-    __pyx_v_spectrum = __pyx_t_6;
-    __pyx_t_6.memview = NULL;
-    __pyx_t_6.data = NULL;
-
-    /* "ms_entropy/tools_cython.pyx":97
- *     while need_centroid:
- *         spectrum = centroid_spectrum_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *         need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)             # <<<<<<<<<<<<<<
- *     return np.asarray(spectrum)
- * 
- */
-    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_ppm); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 97, __pyx_L1_error)
-    __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_ms2_da); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 97, __pyx_L1_error)
-    __pyx_v_need_centroid = __pyx_f_10ms_entropy_12tools_cython_check_centroid_c(__pyx_v_spectrum, __pyx_t_3, __pyx_t_4);
-  }
-
-  /* "ms_entropy/tools_cython.pyx":98
- *         spectrum = centroid_spectrum_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *         need_centroid = check_centroid_c(spectrum, ms2_ppm=ms2_ppm, ms2_da=ms2_da)
- *     return np.asarray(spectrum)             # <<<<<<<<<<<<<<
- * 
- * cdef centroid_spectrum_c(float32[:,::1] spec,double ms2_ppm, double ms2_da):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_asarray); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __pyx_memoryview_fromslice(__pyx_v_spectrum, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32, 0);; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_9)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_9);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
-    }
-  }
-  __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
-  goto __pyx_L0;
-
-  /* "ms_entropy/tools_cython.pyx":76
- * 
- * 
- * cpdef centroid_spectrum(float32[:,::1] spectrum,ms2_ppm=None, ms2_da=None):             # <<<<<<<<<<<<<<
- *     """
- *     Calculate centroid spectrum from a spectrum.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.centroid_spectrum", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum, 1);
-  __Pyx_XDECREF(__pyx_v_ms2_ppm);
-  __Pyx_XDECREF(__pyx_v_ms2_da);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* Python wrapper */
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_7centroid_spectrum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10ms_entropy_12tools_cython_6centroid_spectrum[] = "\n    Calculate centroid spectrum from a spectrum.\n    At least one of the ms2_ppm or ms2_da need be not None. If both ms2_da and ms2_ppm is given, ms2_da will be used.\n\n    :param spectrum: The spectrum should be a 2D array with the first dimension being the m/z values and \n                     the second dimension being the intensity values.\n                     The spectrum need to be sorted by m/z.\n                     The spectrum should be in C order.\n    :param ms2_ppm: the mass accuracy in ppm.\n    :param ms2_da: the mass accuracy in Da.\n    ";
-static PyObject *__pyx_pw_10ms_entropy_12tools_cython_7centroid_spectrum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  __Pyx_memviewslice __pyx_v_spectrum = { 0, 0, { 0 }, { 0 }, { 0 } };
-  PyObject *__pyx_v_ms2_ppm = 0;
-  PyObject *__pyx_v_ms2_da = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("centroid_spectrum (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_spectrum,&__pyx_n_s_ms2_ppm,&__pyx_n_s_ms2_da,0};
-    PyObject* values[3] = {0,0,0};
-    values[1] = ((PyObject *)Py_None);
-    values[2] = ((PyObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_spectrum)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ms2_ppm);
-          if (value) { values[1] = value; kw_args--; }
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ms2_da);
-          if (value) { values[2] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "centroid_spectrum") < 0)) __PYX_ERR(0, 76, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_spectrum = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_spectrum.memview)) __PYX_ERR(0, 76, __pyx_L3_error)
-    __pyx_v_ms2_ppm = values[1];
-    __pyx_v_ms2_da = values[2];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("centroid_spectrum", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 76, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("ms_entropy.tools_cython.centroid_spectrum", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10ms_entropy_12tools_cython_6centroid_spectrum(__pyx_self, __pyx_v_spectrum, __pyx_v_ms2_ppm, __pyx_v_ms2_da);
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_10ms_entropy_12tools_cython_6centroid_spectrum(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_spectrum, PyObject *__pyx_v_ms2_ppm, PyObject *__pyx_v_ms2_da) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  struct __pyx_opt_args_10ms_entropy_12tools_cython_centroid_spectrum __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("centroid_spectrum", 0);
-  __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_spectrum.memview)) { __Pyx_RaiseUnboundLocalError("spectrum"); __PYX_ERR(0, 76, __pyx_L1_error) }
-  __pyx_t_2.__pyx_n = 2;
-  __pyx_t_2.ms2_ppm = __pyx_v_ms2_ppm;
-  __pyx_t_2.ms2_da = __pyx_v_ms2_da;
-  __pyx_t_1 = __pyx_f_10ms_entropy_12tools_cython_centroid_spectrum(__pyx_v_spectrum, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.centroid_spectrum", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_spectrum, 1);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "ms_entropy/tools_cython.pyx":100
- *     return np.asarray(spectrum)
- * 
- * cdef centroid_spectrum_c(float32[:,::1] spec,double ms2_ppm, double ms2_da):             # <<<<<<<<<<<<<<
- *     """
- *     Calculate centroid spectrum from a spectrum.
- */
-
-static PyObject *__pyx_f_10ms_entropy_12tools_cython_centroid_spectrum_c(__Pyx_memviewslice __pyx_v_spec, double __pyx_v_ms2_ppm, double __pyx_v_ms2_da) {
-  __Pyx_memviewslice __pyx_v_intensity_order = { 0, 0, { 0 }, { 0 }, { 0 } };
-  __Pyx_memviewslice __pyx_v_spec_new = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_v_spec_new_i;
-  double __pyx_v_mz_delta_allowed;
-  Py_ssize_t __pyx_v_idx;
-  Py_ssize_t __pyx_v_x;
-  Py_ssize_t __pyx_v_i_left;
-  Py_ssize_t __pyx_v_i_right;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_mz_delta_left;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_mz_delta_right;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity_sum;
-  __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_v_intensity_weighted_sum;
-  Py_ssize_t __pyx_v_i_cur;
-  PyObject *__pyx_v_spec_result = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  __Pyx_memviewslice __pyx_t_4 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  PyObject *__pyx_t_5 = NULL;
-  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  PyObject *__pyx_t_7 = NULL;
-  __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  int __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
-  Py_ssize_t __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
-  Py_ssize_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  int __pyx_t_18;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("centroid_spectrum_c", 0);
-
-  /* "ms_entropy/tools_cython.pyx":111
- *     :param ms2_da: the mass accuracy in Da.
- *     """
- *     cdef int_64[:] intensity_order = np.argsort(spec[:, 1])             # <<<<<<<<<<<<<<
- *     cdef float32[:,::1] spec_new=np.zeros((spec.shape[0],2),dtype=np.float32,order='C')
- *     cdef int spec_new_i=0
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argsort); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4.data = __pyx_v_spec.data;
-  __pyx_t_4.memview = __pyx_v_spec.memview;
-  __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
-  __pyx_t_4.shape[0] = __pyx_v_spec.shape[0];
-__pyx_t_4.strides[0] = __pyx_v_spec.strides[0];
-    __pyx_t_4.suboffsets[0] = -1;
-
-{
-    Py_ssize_t __pyx_tmp_idx = 1;
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_spec.strides[1];
-        __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
-}
-
-__pyx_t_2 = __pyx_memoryview_fromslice(__pyx_t_4, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
-  __pyx_t_4.memview = NULL;
-  __pyx_t_4.data = NULL;
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_64(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 111, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_intensity_order = __pyx_t_6;
-  __pyx_t_6.memview = NULL;
-  __pyx_t_6.data = NULL;
-
-  /* "ms_entropy/tools_cython.pyx":112
- *     """
- *     cdef int_64[:] intensity_order = np.argsort(spec[:, 1])
- *     cdef float32[:,::1] spec_new=np.zeros((spec.shape[0],2),dtype=np.float32,order='C')             # <<<<<<<<<<<<<<
- *     cdef int spec_new_i=0
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t((__pyx_v_spec.shape[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __Pyx_INCREF(__pyx_int_2);
-  __Pyx_GIVEREF(__pyx_int_2);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_2);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_order, __pyx_n_u_C) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(__pyx_t_7, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 112, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_v_spec_new = __pyx_t_8;
-  __pyx_t_8.memview = NULL;
-  __pyx_t_8.data = NULL;
-
-  /* "ms_entropy/tools_cython.pyx":113
- *     cdef int_64[:] intensity_order = np.argsort(spec[:, 1])
- *     cdef float32[:,::1] spec_new=np.zeros((spec.shape[0],2),dtype=np.float32,order='C')
- *     cdef int spec_new_i=0             # <<<<<<<<<<<<<<
- * 
- *     cdef double mz_delta_allowed
- */
-  __pyx_v_spec_new_i = 0;
-
-  /* "ms_entropy/tools_cython.pyx":120
- *     cdef float32 mz_delta_left,mz_delta_right,intensity_sum,intensity_weighted_sum
- * 
- *     with nogil:             # <<<<<<<<<<<<<<
- *         for x in range(intensity_order.shape[0]-1, -1, -1):
- *             idx = intensity_order[x]
- */
-  {
-      #ifdef WITH_THREAD
-      PyThreadState *_save;
-      Py_UNBLOCK_THREADS
-      __Pyx_FastGIL_Remember();
-      #endif
-      /*try:*/ {
-
-        /* "ms_entropy/tools_cython.pyx":121
- * 
- *     with nogil:
- *         for x in range(intensity_order.shape[0]-1, -1, -1):             # <<<<<<<<<<<<<<
- *             idx = intensity_order[x]
- *             if ms2_da >= 0:
- */
-        for (__pyx_t_9 = ((__pyx_v_intensity_order.shape[0]) - 1); __pyx_t_9 > -1L; __pyx_t_9-=1) {
-          __pyx_v_x = __pyx_t_9;
-
-          /* "ms_entropy/tools_cython.pyx":122
- *     with nogil:
- *         for x in range(intensity_order.shape[0]-1, -1, -1):
- *             idx = intensity_order[x]             # <<<<<<<<<<<<<<
- *             if ms2_da >= 0:
- *                 mz_delta_allowed = ms2_da
- */
-          __pyx_t_10 = __pyx_v_x;
-          __pyx_v_idx = (*((__pyx_t_10ms_entropy_12tools_cython_int_64 *) ( /* dim=0 */ (__pyx_v_intensity_order.data + __pyx_t_10 * __pyx_v_intensity_order.strides[0]) )));
-
-          /* "ms_entropy/tools_cython.pyx":123
- *         for x in range(intensity_order.shape[0]-1, -1, -1):
- *             idx = intensity_order[x]
- *             if ms2_da >= 0:             # <<<<<<<<<<<<<<
- *                 mz_delta_allowed = ms2_da
- *             else:
- */
-          __pyx_t_11 = ((__pyx_v_ms2_da >= 0.0) != 0);
-          if (__pyx_t_11) {
-
-            /* "ms_entropy/tools_cython.pyx":124
- *             idx = intensity_order[x]
- *             if ms2_da >= 0:
- *                 mz_delta_allowed = ms2_da             # <<<<<<<<<<<<<<
- *             else:
- *                 mz_delta_allowed = ms2_ppm * 1e-6 * spec[idx, 0]
- */
-            __pyx_v_mz_delta_allowed = __pyx_v_ms2_da;
-
-            /* "ms_entropy/tools_cython.pyx":123
- *         for x in range(intensity_order.shape[0]-1, -1, -1):
- *             idx = intensity_order[x]
- *             if ms2_da >= 0:             # <<<<<<<<<<<<<<
- *                 mz_delta_allowed = ms2_da
- *             else:
- */
-            goto __pyx_L8;
-          }
-
-          /* "ms_entropy/tools_cython.pyx":126
- *                 mz_delta_allowed = ms2_da
- *             else:
- *                 mz_delta_allowed = ms2_ppm * 1e-6 * spec[idx, 0]             # <<<<<<<<<<<<<<
- * 
- *             if spec[idx, 1] > 0:
- */
-          /*else*/ {
-            __pyx_t_10 = __pyx_v_idx;
-            __pyx_t_12 = 0;
-            __pyx_v_mz_delta_allowed = ((__pyx_v_ms2_ppm * 1e-6) * (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_10 * __pyx_v_spec.strides[0]) )) + __pyx_t_12)) ))));
-          }
-          __pyx_L8:;
-
-          /* "ms_entropy/tools_cython.pyx":128
- *                 mz_delta_allowed = ms2_ppm * 1e-6 * spec[idx, 0]
- * 
- *             if spec[idx, 1] > 0:             # <<<<<<<<<<<<<<
- *                 # Find left board for current peak
- *                 i_left = idx - 1
- */
-          __pyx_t_12 = __pyx_v_idx;
-          __pyx_t_10 = 1;
-          __pyx_t_11 = (((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_12 * __pyx_v_spec.strides[0]) )) + __pyx_t_10)) ))) > 0.0) != 0);
-          if (__pyx_t_11) {
-
-            /* "ms_entropy/tools_cython.pyx":130
- *             if spec[idx, 1] > 0:
- *                 # Find left board for current peak
- *                 i_left = idx - 1             # <<<<<<<<<<<<<<
- *                 while i_left >= 0:
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]
- */
-            __pyx_v_i_left = (__pyx_v_idx - 1);
-
-            /* "ms_entropy/tools_cython.pyx":131
- *                 # Find left board for current peak
- *                 i_left = idx - 1
- *                 while i_left >= 0:             # <<<<<<<<<<<<<<
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]
- *                     if mz_delta_left <= mz_delta_allowed:
- */
-            while (1) {
-              __pyx_t_11 = ((__pyx_v_i_left >= 0) != 0);
-              if (!__pyx_t_11) break;
-
-              /* "ms_entropy/tools_cython.pyx":132
- *                 i_left = idx - 1
- *                 while i_left >= 0:
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]             # <<<<<<<<<<<<<<
- *                     if mz_delta_left <= mz_delta_allowed:
- *                         i_left -= 1
- */
-              __pyx_t_10 = __pyx_v_idx;
-              __pyx_t_12 = 0;
-              __pyx_t_13 = __pyx_v_i_left;
-              __pyx_t_14 = 0;
-              __pyx_v_mz_delta_left = ((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_10 * __pyx_v_spec.strides[0]) )) + __pyx_t_12)) ))) - (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_13 * __pyx_v_spec.strides[0]) )) + __pyx_t_14)) ))));
-
-              /* "ms_entropy/tools_cython.pyx":133
- *                 while i_left >= 0:
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]
- *                     if mz_delta_left <= mz_delta_allowed:             # <<<<<<<<<<<<<<
- *                         i_left -= 1
- *                     else:
- */
-              __pyx_t_11 = ((__pyx_v_mz_delta_left <= __pyx_v_mz_delta_allowed) != 0);
-              if (__pyx_t_11) {
-
-                /* "ms_entropy/tools_cython.pyx":134
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]
- *                     if mz_delta_left <= mz_delta_allowed:
- *                         i_left -= 1             # <<<<<<<<<<<<<<
- *                     else:
- *                         break
- */
-                __pyx_v_i_left = (__pyx_v_i_left - 1);
-
-                /* "ms_entropy/tools_cython.pyx":133
- *                 while i_left >= 0:
- *                     mz_delta_left = spec[idx, 0] - spec[i_left, 0]
- *                     if mz_delta_left <= mz_delta_allowed:             # <<<<<<<<<<<<<<
- *                         i_left -= 1
- *                     else:
- */
-                goto __pyx_L12;
-              }
-
-              /* "ms_entropy/tools_cython.pyx":136
- *                         i_left -= 1
- *                     else:
- *                         break             # <<<<<<<<<<<<<<
- *                 i_left += 1
- * 
- */
-              /*else*/ {
-                goto __pyx_L11_break;
-              }
-              __pyx_L12:;
-            }
-            __pyx_L11_break:;
-
-            /* "ms_entropy/tools_cython.pyx":137
- *                     else:
- *                         break
- *                 i_left += 1             # <<<<<<<<<<<<<<
- * 
- *                 # Find right board for current peak
- */
-            __pyx_v_i_left = (__pyx_v_i_left + 1);
-
-            /* "ms_entropy/tools_cython.pyx":140
- * 
- *                 # Find right board for current peak
- *                 i_right = idx + 1             # <<<<<<<<<<<<<<
- *                 while i_right < spec.shape[0]:
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]
- */
-            __pyx_v_i_right = (__pyx_v_idx + 1);
-
-            /* "ms_entropy/tools_cython.pyx":141
- *                 # Find right board for current peak
- *                 i_right = idx + 1
- *                 while i_right < spec.shape[0]:             # <<<<<<<<<<<<<<
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]
- *                     if mz_delta_right <= mz_delta_allowed:
- */
-            while (1) {
-              __pyx_t_11 = ((__pyx_v_i_right < (__pyx_v_spec.shape[0])) != 0);
-              if (!__pyx_t_11) break;
-
-              /* "ms_entropy/tools_cython.pyx":142
- *                 i_right = idx + 1
- *                 while i_right < spec.shape[0]:
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]             # <<<<<<<<<<<<<<
- *                     if mz_delta_right <= mz_delta_allowed:
- *                         i_right += 1
- */
-              __pyx_t_14 = __pyx_v_i_right;
-              __pyx_t_13 = 0;
-              __pyx_t_12 = __pyx_v_idx;
-              __pyx_t_10 = 0;
-              __pyx_v_mz_delta_right = ((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_14 * __pyx_v_spec.strides[0]) )) + __pyx_t_13)) ))) - (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_12 * __pyx_v_spec.strides[0]) )) + __pyx_t_10)) ))));
-
-              /* "ms_entropy/tools_cython.pyx":143
- *                 while i_right < spec.shape[0]:
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]
- *                     if mz_delta_right <= mz_delta_allowed:             # <<<<<<<<<<<<<<
- *                         i_right += 1
- *                     else:
- */
-              __pyx_t_11 = ((__pyx_v_mz_delta_right <= __pyx_v_mz_delta_allowed) != 0);
-              if (__pyx_t_11) {
-
-                /* "ms_entropy/tools_cython.pyx":144
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]
- *                     if mz_delta_right <= mz_delta_allowed:
- *                         i_right += 1             # <<<<<<<<<<<<<<
- *                     else:
- *                         break
- */
-                __pyx_v_i_right = (__pyx_v_i_right + 1);
-
-                /* "ms_entropy/tools_cython.pyx":143
- *                 while i_right < spec.shape[0]:
- *                     mz_delta_right = spec[i_right, 0] - spec[idx, 0]
- *                     if mz_delta_right <= mz_delta_allowed:             # <<<<<<<<<<<<<<
- *                         i_right += 1
- *                     else:
- */
-                goto __pyx_L15;
-              }
-
-              /* "ms_entropy/tools_cython.pyx":146
- *                         i_right += 1
- *                     else:
- *                         break             # <<<<<<<<<<<<<<
- * 
- *                 # Merge those peaks
- */
-              /*else*/ {
-                goto __pyx_L14_break;
-              }
-              __pyx_L15:;
-            }
-            __pyx_L14_break:;
-
-            /* "ms_entropy/tools_cython.pyx":149
- * 
- *                 # Merge those peaks
- *                 intensity_sum = 0             # <<<<<<<<<<<<<<
- *                 intensity_weighted_sum = 0
- *                 for i_cur in range(i_left, i_right):
- */
-            __pyx_v_intensity_sum = 0.0;
-
-            /* "ms_entropy/tools_cython.pyx":150
- *                 # Merge those peaks
- *                 intensity_sum = 0
- *                 intensity_weighted_sum = 0             # <<<<<<<<<<<<<<
- *                 for i_cur in range(i_left, i_right):
- *                     intensity_sum += spec[i_cur, 1]
- */
-            __pyx_v_intensity_weighted_sum = 0.0;
-
-            /* "ms_entropy/tools_cython.pyx":151
- *                 intensity_sum = 0
- *                 intensity_weighted_sum = 0
- *                 for i_cur in range(i_left, i_right):             # <<<<<<<<<<<<<<
- *                     intensity_sum += spec[i_cur, 1]
- *                     intensity_weighted_sum += spec[i_cur, 0]*spec[i_cur, 1]
- */
-            __pyx_t_15 = __pyx_v_i_right;
-            __pyx_t_16 = __pyx_t_15;
-            for (__pyx_t_17 = __pyx_v_i_left; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
-              __pyx_v_i_cur = __pyx_t_17;
-
-              /* "ms_entropy/tools_cython.pyx":152
- *                 intensity_weighted_sum = 0
- *                 for i_cur in range(i_left, i_right):
- *                     intensity_sum += spec[i_cur, 1]             # <<<<<<<<<<<<<<
- *                     intensity_weighted_sum += spec[i_cur, 0]*spec[i_cur, 1]
- * 
- */
-              __pyx_t_10 = __pyx_v_i_cur;
-              __pyx_t_12 = 1;
-              __pyx_v_intensity_sum = (__pyx_v_intensity_sum + (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_10 * __pyx_v_spec.strides[0]) )) + __pyx_t_12)) ))));
-
-              /* "ms_entropy/tools_cython.pyx":153
- *                 for i_cur in range(i_left, i_right):
- *                     intensity_sum += spec[i_cur, 1]
- *                     intensity_weighted_sum += spec[i_cur, 0]*spec[i_cur, 1]             # <<<<<<<<<<<<<<
- * 
- *                 spec_new[spec_new_i, 0] = intensity_weighted_sum / intensity_sum
- */
-              __pyx_t_12 = __pyx_v_i_cur;
-              __pyx_t_10 = 0;
-              __pyx_t_13 = __pyx_v_i_cur;
-              __pyx_t_14 = 1;
-              __pyx_v_intensity_weighted_sum = (__pyx_v_intensity_weighted_sum + ((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_12 * __pyx_v_spec.strides[0]) )) + __pyx_t_10)) ))) * (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec.data + __pyx_t_13 * __pyx_v_spec.strides[0]) )) + __pyx_t_14)) )))));
-            }
-
-            /* "ms_entropy/tools_cython.pyx":155
- *                     intensity_weighted_sum += spec[i_cur, 0]*spec[i_cur, 1]
- * 
- *                 spec_new[spec_new_i, 0] = intensity_weighted_sum / intensity_sum             # <<<<<<<<<<<<<<
- *                 spec_new[spec_new_i, 1] = intensity_sum
- *                 spec_new_i += 1
- */
-            __pyx_t_14 = __pyx_v_spec_new_i;
-            __pyx_t_13 = 0;
-            *((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec_new.data + __pyx_t_14 * __pyx_v_spec_new.strides[0]) )) + __pyx_t_13)) )) = (__pyx_v_intensity_weighted_sum / __pyx_v_intensity_sum);
-
-            /* "ms_entropy/tools_cython.pyx":156
- * 
- *                 spec_new[spec_new_i, 0] = intensity_weighted_sum / intensity_sum
- *                 spec_new[spec_new_i, 1] = intensity_sum             # <<<<<<<<<<<<<<
- *                 spec_new_i += 1
- *                 spec[i_left:i_right, 1] = 0
- */
-            __pyx_t_13 = __pyx_v_spec_new_i;
-            __pyx_t_14 = 1;
-            *((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spec_new.data + __pyx_t_13 * __pyx_v_spec_new.strides[0]) )) + __pyx_t_14)) )) = __pyx_v_intensity_sum;
-
-            /* "ms_entropy/tools_cython.pyx":157
- *                 spec_new[spec_new_i, 0] = intensity_weighted_sum / intensity_sum
- *                 spec_new[spec_new_i, 1] = intensity_sum
- *                 spec_new_i += 1             # <<<<<<<<<<<<<<
- *                 spec[i_left:i_right, 1] = 0
- * 
- */
-            __pyx_v_spec_new_i = (__pyx_v_spec_new_i + 1);
-
-            /* "ms_entropy/tools_cython.pyx":158
- *                 spec_new[spec_new_i, 1] = intensity_sum
- *                 spec_new_i += 1
- *                 spec[i_left:i_right, 1] = 0             # <<<<<<<<<<<<<<
- * 
- *     spec_result = spec_new[:spec_new_i,:]
- */
-            __pyx_t_4.data = __pyx_v_spec.data;
-            __pyx_t_4.memview = __pyx_v_spec.memview;
-            __PYX_INC_MEMVIEW(&__pyx_t_4, 0);
-            __pyx_t_18 = -1;
-            if (unlikely(__pyx_memoryview_slice_memviewslice(
-    &__pyx_t_4,
-    __pyx_v_spec.shape[0], __pyx_v_spec.strides[0], __pyx_v_spec.suboffsets[0],
-    0,
-    0,
-    &__pyx_t_18,
-    __pyx_v_i_left,
-    __pyx_v_i_right,
-    0,
-    1,
-    1,
-    0,
-    1) < 0))
-{
-    __PYX_ERR(0, 158, __pyx_L4_error)
-}
-
-{
-    Py_ssize_t __pyx_tmp_idx = 1;
-    Py_ssize_t __pyx_tmp_stride = __pyx_v_spec.strides[1];
-        __pyx_t_4.data += __pyx_tmp_idx * __pyx_tmp_stride;
-}
-
-{
-                __pyx_t_10ms_entropy_12tools_cython_float32 __pyx_temp_scalar = 0.0;
-                {
-                    Py_ssize_t __pyx_temp_extent_0 = __pyx_t_4.shape[0];
-                    Py_ssize_t __pyx_temp_stride_0 = __pyx_t_4.strides[0];
-                    char *__pyx_temp_pointer_0;
-                    Py_ssize_t __pyx_temp_idx_0;
-                    __pyx_temp_pointer_0 = __pyx_t_4.data;
-                    for (__pyx_temp_idx_0 = 0; __pyx_temp_idx_0 < __pyx_temp_extent_0; __pyx_temp_idx_0++) {
-                      *((__pyx_t_10ms_entropy_12tools_cython_float32 *) __pyx_temp_pointer_0) = __pyx_temp_scalar;
-                      __pyx_temp_pointer_0 += __pyx_temp_stride_0;
-                    }
-                }
-            }
-            __PYX_XDEC_MEMVIEW(&__pyx_t_4, 0);
-            __pyx_t_4.memview = NULL;
-            __pyx_t_4.data = NULL;
-
-            /* "ms_entropy/tools_cython.pyx":128
- *                 mz_delta_allowed = ms2_ppm * 1e-6 * spec[idx, 0]
- * 
- *             if spec[idx, 1] > 0:             # <<<<<<<<<<<<<<
- *                 # Find left board for current peak
- *                 i_left = idx - 1
- */
-          }
-        }
-      }
-
-      /* "ms_entropy/tools_cython.pyx":120
- *     cdef float32 mz_delta_left,mz_delta_right,intensity_sum,intensity_weighted_sum
- * 
- *     with nogil:             # <<<<<<<<<<<<<<
- *         for x in range(intensity_order.shape[0]-1, -1, -1):
- *             idx = intensity_order[x]
- */
-      /*finally:*/ {
-        /*normal exit:*/{
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L5;
-        }
-        __pyx_L4_error: {
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L1_error;
-        }
-        __pyx_L5:;
-      }
-  }
-
-  /* "ms_entropy/tools_cython.pyx":160
- *                 spec[i_left:i_right, 1] = 0
- * 
- *     spec_result = spec_new[:spec_new_i,:]             # <<<<<<<<<<<<<<
- *     spec_result=np.array(spec_result)[np.argsort(spec_result[:,0])]
- *     return spec_result
- */
-  __pyx_t_8.data = __pyx_v_spec_new.data;
-  __pyx_t_8.memview = __pyx_v_spec_new.memview;
-  __PYX_INC_MEMVIEW(&__pyx_t_8, 0);
-  __pyx_t_18 = -1;
-  if (unlikely(__pyx_memoryview_slice_memviewslice(
-    &__pyx_t_8,
-    __pyx_v_spec_new.shape[0], __pyx_v_spec_new.strides[0], __pyx_v_spec_new.suboffsets[0],
-    0,
-    0,
-    &__pyx_t_18,
-    0,
-    __pyx_v_spec_new_i,
-    0,
-    0,
-    1,
-    0,
-    1) < 0))
-{
-    __PYX_ERR(0, 160, __pyx_L1_error)
-}
-
-__pyx_t_8.shape[1] = __pyx_v_spec_new.shape[1];
-__pyx_t_8.strides[1] = __pyx_v_spec_new.strides[1];
-    __pyx_t_8.suboffsets[1] = -1;
-
-__pyx_t_7 = __pyx_memoryview_fromslice(__pyx_t_8, 2, (PyObject *(*)(char *)) __pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32, (int (*)(char *, PyObject *)) __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32, 0);; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
-  __pyx_t_8.memview = NULL;
-  __pyx_t_8.data = NULL;
-  __pyx_v_spec_result = __pyx_t_7;
-  __pyx_t_7 = 0;
-
-  /* "ms_entropy/tools_cython.pyx":161
- * 
- *     spec_result = spec_new[:spec_new_i,:]
- *     spec_result=np.array(spec_result)[np.argsort(spec_result[:,0])]             # <<<<<<<<<<<<<<
- *     return spec_result
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
-    }
-  }
-  __pyx_t_7 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_v_spec_result) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_spec_result);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argsort); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_spec_result, __pyx_tuple__2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF_SET(__pyx_v_spec_result, __pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "ms_entropy/tools_cython.pyx":162
- *     spec_result = spec_new[:spec_new_i,:]
- *     spec_result=np.array(spec_result)[np.argsort(spec_result[:,0])]
- *     return spec_result             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_spec_result);
-  __pyx_r = __pyx_v_spec_result;
-  goto __pyx_L0;
-
-  /* "ms_entropy/tools_cython.pyx":100
- *     return np.asarray(spectrum)
- * 
- * cdef centroid_spectrum_c(float32[:,::1] spec,double ms2_ppm, double ms2_da):             # <<<<<<<<<<<<<<
- *     """
- *     Calculate centroid spectrum from a spectrum.
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_4, 1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_6, 1);
-  __Pyx_XDECREF(__pyx_t_7);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_8, 1);
-  __Pyx_AddTraceback("ms_entropy.tools_cython.centroid_spectrum_c", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __PYX_XDEC_MEMVIEW(&__pyx_v_intensity_order, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_v_spec_new, 1);
-  __Pyx_XDECREF(__pyx_v_spec_result);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "ms_entropy/tools_cython.pyx":165
- * 
- * 
- * cdef int check_centroid_c(float32[:,::1] spectrum,double ms2_ppm, double ms2_da):             # <<<<<<<<<<<<<<
- *     """
- *     Check whether the spectrum needs to be centroided or not.
- */
-
-static int __pyx_f_10ms_entropy_12tools_cython_check_centroid_c(__Pyx_memviewslice __pyx_v_spectrum, double __pyx_v_ms2_ppm, double __pyx_v_ms2_da) {
-  int __pyx_v_i;
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  Py_ssize_t __pyx_t_2;
-  Py_ssize_t __pyx_t_3;
-  int __pyx_t_4;
-  Py_ssize_t __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  __Pyx_RefNannySetupContext("check_centroid_c", 0);
-
-  /* "ms_entropy/tools_cython.pyx":179
- *     cdef int i
- * 
- *     if spectrum.shape[0]<=1:             # <<<<<<<<<<<<<<
- *         return 0
- * 
- */
-  __pyx_t_1 = (((__pyx_v_spectrum.shape[0]) <= 1) != 0);
-  if (__pyx_t_1) {
-
-    /* "ms_entropy/tools_cython.pyx":180
- * 
- *     if spectrum.shape[0]<=1:
- *         return 0             # <<<<<<<<<<<<<<
- * 
- *     if ms2_da>0:
- */
-    __pyx_r = 0;
-    goto __pyx_L0;
-
-    /* "ms_entropy/tools_cython.pyx":179
- *     cdef int i
- * 
- *     if spectrum.shape[0]<=1:             # <<<<<<<<<<<<<<
- *         return 0
- * 
- */
-  }
-
-  /* "ms_entropy/tools_cython.pyx":182
- *         return 0
- * 
- *     if ms2_da>0:             # <<<<<<<<<<<<<<
- *         # Use Da accuracy
- *         for i in range(1, spectrum.shape[0]):
- */
-  __pyx_t_1 = ((__pyx_v_ms2_da > 0.0) != 0);
-  if (__pyx_t_1) {
-
-    /* "ms_entropy/tools_cython.pyx":184
- *     if ms2_da>0:
- *         # Use Da accuracy
- *         for i in range(1, spectrum.shape[0]):             # <<<<<<<<<<<<<<
- *             if spectrum[i, 0]-spectrum[i-1, 0] < ms2_da:
- *                 return 1
- */
-    __pyx_t_2 = (__pyx_v_spectrum.shape[0]);
-    __pyx_t_3 = __pyx_t_2;
-    for (__pyx_t_4 = 1; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-      __pyx_v_i = __pyx_t_4;
-
-      /* "ms_entropy/tools_cython.pyx":185
- *         # Use Da accuracy
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < ms2_da:             # <<<<<<<<<<<<<<
- *                 return 1
- *     else:
- */
-      __pyx_t_5 = __pyx_v_i;
-      __pyx_t_6 = 0;
-      __pyx_t_7 = (__pyx_v_i - 1);
-      __pyx_t_8 = 0;
-      __pyx_t_1 = ((((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_5 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_6)) ))) - (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_7 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_8)) )))) < __pyx_v_ms2_da) != 0);
-      if (__pyx_t_1) {
-
-        /* "ms_entropy/tools_cython.pyx":186
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < ms2_da:
- *                 return 1             # <<<<<<<<<<<<<<
- *     else:
- *         # Use ppm accuracy
- */
-        __pyx_r = 1;
-        goto __pyx_L0;
-
-        /* "ms_entropy/tools_cython.pyx":185
- *         # Use Da accuracy
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < ms2_da:             # <<<<<<<<<<<<<<
- *                 return 1
- *     else:
- */
-      }
-    }
-
-    /* "ms_entropy/tools_cython.pyx":182
- *         return 0
- * 
- *     if ms2_da>0:             # <<<<<<<<<<<<<<
- *         # Use Da accuracy
- *         for i in range(1, spectrum.shape[0]):
- */
-    goto __pyx_L4;
-  }
-
-  /* "ms_entropy/tools_cython.pyx":189
- *     else:
- *         # Use ppm accuracy
- *         for i in range(1, spectrum.shape[0]):             # <<<<<<<<<<<<<<
- *             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:
- *                 return 1
- */
-  /*else*/ {
-    __pyx_t_2 = (__pyx_v_spectrum.shape[0]);
-    __pyx_t_3 = __pyx_t_2;
-    for (__pyx_t_4 = 1; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-      __pyx_v_i = __pyx_t_4;
-
-      /* "ms_entropy/tools_cython.pyx":190
- *         # Use ppm accuracy
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:             # <<<<<<<<<<<<<<
- *                 return 1
- *     return 0
- */
-      __pyx_t_8 = __pyx_v_i;
-      __pyx_t_7 = 0;
-      __pyx_t_6 = (__pyx_v_i - 1);
-      __pyx_t_5 = 0;
-      __pyx_t_9 = __pyx_v_i;
-      __pyx_t_10 = 0;
-      __pyx_t_1 = ((((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_8 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_7)) ))) - (*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_6 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_5)) )))) < (((*((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=1 */ ((char *) (((__pyx_t_10ms_entropy_12tools_cython_float32 *) ( /* dim=0 */ (__pyx_v_spectrum.data + __pyx_t_9 * __pyx_v_spectrum.strides[0]) )) + __pyx_t_10)) ))) * __pyx_v_ms2_ppm) * 1e-6)) != 0);
-      if (__pyx_t_1) {
-
-        /* "ms_entropy/tools_cython.pyx":191
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:
- *                 return 1             # <<<<<<<<<<<<<<
- *     return 0
- */
-        __pyx_r = 1;
-        goto __pyx_L0;
-
-        /* "ms_entropy/tools_cython.pyx":190
- *         # Use ppm accuracy
- *         for i in range(1, spectrum.shape[0]):
- *             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:             # <<<<<<<<<<<<<<
- *                 return 1
- *     return 0
- */
-      }
-    }
-  }
-  __pyx_L4:;
-
-  /* "ms_entropy/tools_cython.pyx":192
- *             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:
- *                 return 1
- *     return 0             # <<<<<<<<<<<<<<
- */
-  __pyx_r = 0;
-  goto __pyx_L0;
-
-  /* "ms_entropy/tools_cython.pyx":165
- * 
- * 
- * cdef int check_centroid_c(float32[:,::1] spectrum,double ms2_ppm, double ms2_da):             # <<<<<<<<<<<<<<
- *     """
- *     Check whether the spectrum needs to be centroided or not.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
@@ -5286,15 +4015,15 @@
       /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -5418,15 +4147,15 @@
       /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -5550,15 +4279,15 @@
       /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -5974,15 +4703,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -6006,15 +4735,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -6133,15 +4862,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -6407,15 +5136,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(2, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -6651,15 +5380,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -7385,15 +6114,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -7441,15 +6170,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -9170,15 +7899,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -10218,15 +8947,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(2, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -10580,15 +9309,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -11129,15 +9858,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(2, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -11246,15 +9975,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__16, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -12284,15 +11013,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -12340,15 +11069,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -12697,17 +11426,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice_);
-            __Pyx_GIVEREF(__pyx_slice_);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice_);
+            __Pyx_INCREF(__pyx_slice__17);
+            __Pyx_GIVEREF(__pyx_slice__17);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -12732,15 +11461,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice_); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -12872,17 +11601,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice_);
-        __Pyx_GIVEREF(__pyx_slice_);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice_);
+        __Pyx_INCREF(__pyx_slice__17);
+        __Pyx_GIVEREF(__pyx_slice__17);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -13001,15 +11730,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(2, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -15185,15 +13914,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -15241,15 +13970,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(2, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18518,15 +17247,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__22, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -18934,15 +17663,15 @@
   #endif
   __pyx_array_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_array = {
   PyVarObject_HEAD_INIT(0, 0)
-  "ms_entropy.tools_cython.array", /*tp_name*/
+  "ms_entropy.tools.fast_entropy.array", /*tp_name*/
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_array, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19056,15 +17785,15 @@
   {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
-  "ms_entropy.tools_cython.Enum", /*tp_name*/
+  "ms_entropy.tools.fast_entropy.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19320,15 +18049,15 @@
   #endif
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_memoryview = {
   PyVarObject_HEAD_INIT(0, 0)
-  "ms_entropy.tools_cython.memoryview", /*tp_name*/
+  "ms_entropy.tools.fast_entropy.memoryview", /*tp_name*/
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19461,15 +18190,15 @@
 static struct PyGetSetDef __pyx_getsets__memoryviewslice[] = {
   {(char *)"base", __pyx_getprop___pyx_memoryviewslice_base, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
   PyVarObject_HEAD_INIT(0, 0)
-  "ms_entropy.tools_cython._memoryviewslice", /*tp_name*/
+  "ms_entropy.tools.fast_entropy._memoryviewslice", /*tp_name*/
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -19540,35 +18269,34 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
-  {"entropy_similarity_search_fast", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10ms_entropy_12tools_cython_1entropy_similarity_search_fast, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10ms_entropy_12tools_cython_entropy_similarity_search_fast},
-  {"apply_weight_to_intensity", (PyCFunction)__pyx_pw_10ms_entropy_12tools_cython_3apply_weight_to_intensity, METH_O, __pyx_doc_10ms_entropy_12tools_cython_2apply_weight_to_intensity},
-  {"spectral_entropy", (PyCFunction)__pyx_pw_10ms_entropy_12tools_cython_5spectral_entropy, METH_O, __pyx_doc_10ms_entropy_12tools_cython_4spectral_entropy},
-  {"centroid_spectrum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10ms_entropy_12tools_cython_7centroid_spectrum, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10ms_entropy_12tools_cython_6centroid_spectrum},
+  {"entropy_similarity_search_fast", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10ms_entropy_5tools_12fast_entropy_1entropy_similarity_search_fast, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10ms_entropy_5tools_12fast_entropy_entropy_similarity_search_fast},
+  {"apply_weight_to_intensity", (PyCFunction)__pyx_pw_10ms_entropy_5tools_12fast_entropy_3apply_weight_to_intensity, METH_O, __pyx_doc_10ms_entropy_5tools_12fast_entropy_2apply_weight_to_intensity},
+  {"spectral_entropy", (PyCFunction)__pyx_pw_10ms_entropy_5tools_12fast_entropy_5spectral_entropy, METH_O, __pyx_doc_10ms_entropy_5tools_12fast_entropy_4spectral_entropy},
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_tools_cython(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_fast_entropy(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_tools_cython},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_fast_entropy},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "tools_cython",
+    "fast_entropy",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -19591,15 +18319,14 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
-  {&__pyx_n_u_C, __pyx_k_C, sizeof(__pyx_k_C), 0, 1, 0, 1},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
@@ -19615,33 +18342,28 @@
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
-  {&__pyx_n_s_argsort, __pyx_k_argsort, sizeof(__pyx_k_argsort), 0, 0, 1, 1},
-  {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-  {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
-  {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
@@ -19650,27 +18372,24 @@
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_library_peaks_intensity, __pyx_k_library_peaks_intensity, sizeof(__pyx_k_library_peaks_intensity), 0, 0, 1, 1},
   {&__pyx_n_s_library_spec_idx_array, __pyx_k_library_spec_idx_array, sizeof(__pyx_k_library_spec_idx_array), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mixed_spectra_entropy, __pyx_k_mixed_spectra_entropy, sizeof(__pyx_k_mixed_spectra_entropy), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
-  {&__pyx_n_s_ms2_da, __pyx_k_ms2_da, sizeof(__pyx_k_ms2_da), 0, 0, 1, 1},
-  {&__pyx_n_s_ms2_ppm, __pyx_k_ms2_ppm, sizeof(__pyx_k_ms2_ppm), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
-  {&__pyx_n_s_order, __pyx_k_order, sizeof(__pyx_k_order), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_product_mz_idx_max, __pyx_k_product_mz_idx_max, sizeof(__pyx_k_product_mz_idx_max), 0, 0, 1, 1},
   {&__pyx_n_s_product_mz_idx_min, __pyx_k_product_mz_idx_min, sizeof(__pyx_k_product_mz_idx_min), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
@@ -19687,29 +18406,27 @@
   {&__pyx_n_s_search_spectra_idx_max, __pyx_k_search_spectra_idx_max, sizeof(__pyx_k_search_spectra_idx_max), 0, 0, 1, 1},
   {&__pyx_n_s_search_spectra_idx_min, __pyx_k_search_spectra_idx_min, sizeof(__pyx_k_search_spectra_idx_min), 0, 0, 1, 1},
   {&__pyx_n_s_search_type, __pyx_k_search_type, sizeof(__pyx_k_search_type), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
-  {&__pyx_n_s_spectrum, __pyx_k_spectrum, sizeof(__pyx_k_spectrum), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-  {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 27, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
@@ -19723,311 +18440,306 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "ms_entropy/tools_cython.pyx":161
- * 
- *     spec_result = spec_new[:spec_new_i,:]
- *     spec_result=np.array(spec_result)[np.argsort(spec_result[:,0])]             # <<<<<<<<<<<<<<
- *     return spec_result
- * 
- */
-  __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice_);
-  __Pyx_GIVEREF(__pyx_slice_);
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_slice_, __pyx_int_0); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
   /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "../../../home/yli/Software/anaconda3/envs/py39/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__16 = PyTuple_New(1); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__16, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+
+  /* "View.MemoryView":684
+ *         if item is Ellipsis:
+ *             if not seen_ellipsis:
+ *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
+ *                 seen_ellipsis = True
+ *             else:
+ */
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__17);
+  __Pyx_GIVEREF(__pyx_slice__17);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_neg_1_ = PyFloat_FromDouble(-1.); if (unlikely(!__pyx_float_neg_1_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -20226,19 +18938,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC inittools_cython(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC inittools_cython(void)
+__Pyx_PyMODINIT_FUNC initfast_entropy(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initfast_entropy(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_tools_cython(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_tools_cython(void)
+__Pyx_PyMODINIT_FUNC PyInit_fast_entropy(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_fast_entropy(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -20297,43 +19009,43 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_tools_cython(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_fast_entropy(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   static PyThread_type_lock __pyx_t_2[8];
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'tools_cython' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'fast_entropy' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_tools_cython(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_fast_entropy(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20362,15 +19074,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("tools_cython", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("fast_entropy", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -20380,22 +19092,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_ms_entropy__tools_cython) {
+  if (__pyx_module_is_main_ms_entropy__tools__fast_entropy) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "ms_entropy.tools_cython")) {
-      if (unlikely(PyDict_SetItemString(modules, "ms_entropy.tools_cython", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "ms_entropy.tools.fast_entropy")) {
+      if (unlikely(PyDict_SetItemString(modules, "ms_entropy.tools.fast_entropy", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20408,30 +19120,30 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "ms_entropy/tools_cython.pyx":1
+  /* "ms_entropy/tools/fast_entropy.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ms_entropy/tools_cython.pyx":165
- * 
+  /* "ms_entropy/tools/fast_entropy.pyx":63
+ *     return spectrum_weighted
  * 
- * cdef int check_centroid_c(float32[:,::1] spectrum,double ms2_ppm, double ms2_da):             # <<<<<<<<<<<<<<
+ * cpdef double spectral_entropy(float32[:,::1] spectrum) nogil:             # <<<<<<<<<<<<<<
  *     """
- *     Check whether the spectrum needs to be centroided or not.
+ *     Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
@@ -20450,71 +19162,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
@@ -20590,19 +19302,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init ms_entropy.tools_cython", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init ms_entropy.tools.fast_entropy", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init ms_entropy.tools_cython");
+    PyErr_SetString(PyExc_ImportError, "init ms_entropy.tools.fast_entropy");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -21244,130 +19956,14 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -21881,14 +20477,130 @@
     if (likely(PyString_Check(n)))
 #endif
         return __Pyx_PyObject_GetAttrStr(o, n);
 #endif
     return PyObject_GetAttr(o, n);
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+    PyObject *runerr = NULL;
+    Py_ssize_t key_value;
+    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
+    if (unlikely(!(m && m->sq_item))) {
+        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
+        return NULL;
+    }
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
+    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(m && m->mp_subscript)) {
+        return m->mp_subscript(obj, key);
+    }
+    return __Pyx_PyObject_GetIndex(obj, key);
+}
+#endif
+
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
@@ -23651,163 +22363,140 @@
     retval = -1;
 no_fail:
     __Pyx_RefNannyFinishContext();
     return retval;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(PyObject *obj, int writable_flag) {
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
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_float32, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, stack,
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
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_float32__const__(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32__const__(PyObject *obj, int writable_flag) {
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
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_float32__const__, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32__const__, stack,
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
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_uint_32__const__(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32__const__(PyObject *obj, int writable_flag) {
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
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_uint_32__const__, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_uint_32__const__, stack,
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
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_8__const__(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_int_8__const__(PyObject *obj, int writable_flag) {
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
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_int_8__const__, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_int_8__const__, stack,
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
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_12tools_cython_float32(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
                                                  (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_float32, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
 /* MemviewDtypeToObject */
-  static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_10ms_entropy_12tools_cython_float32(const char *itemp) {
-    return (PyObject *) PyFloat_FromDouble(*(__pyx_t_10ms_entropy_12tools_cython_float32 *) itemp);
+  static CYTHON_INLINE PyObject *__pyx_memview_get_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(const char *itemp) {
+    return (PyObject *) PyFloat_FromDouble(*(__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) itemp);
 }
-static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_10ms_entropy_12tools_cython_float32(const char *itemp, PyObject *obj) {
-    __pyx_t_10ms_entropy_12tools_cython_float32 value = __pyx_PyFloat_AsFloat(obj);
+static CYTHON_INLINE int __pyx_memview_set_nn___pyx_t_10ms_entropy_5tools_12fast_entropy_float32(const char *itemp, PyObject *obj) {
+    __pyx_t_10ms_entropy_5tools_12fast_entropy_float32 value = __pyx_PyFloat_AsFloat(obj);
     if ((value == ((npy_float32)-1)) && PyErr_Occurred())
         return 0;
-    *(__pyx_t_10ms_entropy_12tools_cython_float32 *) itemp = value;
+    *(__pyx_t_10ms_entropy_5tools_12fast_entropy_float32 *) itemp = value;
     return 1;
 }
 
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_10ms_entropy_12tools_cython_int_64(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_nn___pyx_t_10ms_entropy_12tools_cython_int_64, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
 /* Declarations */
   #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -24643,52 +23332,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(npy_int8),
                                      little, !is_unsigned);
     }
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
@@ -24878,14 +23529,52 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
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
+/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
```

### Comparing `ms_entropy-0.4.2/ms_entropy/tools_cython.pyx` & `ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -3,80 +3,14 @@
 
 ctypedef np.float32_t float32
 ctypedef np.int64_t int_64
 ctypedef np.int8_t int_8
 ctypedef np.uint32_t uint_32
 from libc.math cimport log2,log,pow
 
-
-cpdef void entropy_similarity_search_fast(int_64 product_mz_idx_min, int_64 product_mz_idx_max,
-                                    float32 intensity, float32[:] mixed_spectra_entropy,
-                                    const float32[:] library_peaks_intensity, const uint_32[:] library_spec_idx_array,
-                                    int search_type, int_64 search_spectra_idx_min, int_64 search_spectra_idx_max, const int_8[:] search_array) nogil:
-    """
-    The mixed_spectra_entropy will be modified in this function.
-    search_type is 0: search all spectra.
-    search_type is 1: search spectra in the range [search_spectra_idx_min, search_spectra_idx_max).
-    search_type is 2: search spectra in the array search_array with entry equals 1, the length of search_array should be equal to the self.total_spectra_num
-
-    Note: the intensity here should be half of the original intensity.
-    """
-    cdef uint_32 library_spec_idx
-    cdef float32 library_peak_intensity, intensity_ab
-    cdef float32 intensity_xlog2x = intensity * log2(intensity)
-
-    for idx in range(product_mz_idx_min, product_mz_idx_max):
-        library_spec_idx = library_spec_idx_array[idx]
-        if (search_type == 0) or \
-                (search_type == 1 and search_spectra_idx_min <= library_spec_idx and library_spec_idx < search_spectra_idx_max) or \
-                (search_type == 2 and search_array[library_spec_idx]):
-            # Match this peak
-            library_peak_intensity = library_peaks_intensity[idx]
-            intensity_ab = intensity + library_peak_intensity
-
-            mixed_spectra_entropy[library_spec_idx] += \
-                intensity_ab * log2(intensity_ab) - \
-                intensity_xlog2x - \
-                library_peak_intensity * log2(library_peak_intensity)
-
-
-cpdef apply_weight_to_intensity(float32[:,::1] spectrum):
-    """
-    Apply the weight to the intensity.
-    The spectrum is a 2D array like: [[m/z, intensity], [m/z, intensity], ...]
-    """
-    cdef double entropy=spectral_entropy(spectrum)
-    cdef double weight, intensity_sum
-    cdef float32[:,::1] spectrum_weighted = np.copy(spectrum)
-    if entropy<3:
-        weight = 0.25 + 0.25 * entropy
-        intensity_sum = 0.
-        for i in range(spectrum_weighted.shape[0]):
-            spectrum_weighted[i,1] = pow(spectrum_weighted[i,1],weight)
-            intensity_sum += spectrum_weighted[i,1]
-
-        if intensity_sum>0:
-            for i in range(spectrum_weighted.shape[0]):
-                spectrum_weighted[i,1] /= intensity_sum
-            
-    return spectrum_weighted
-
-cpdef double spectral_entropy(float32[:,::1] spectrum) nogil:
-    """
-    Compute the spectral entropy of a spectrum. The intensity need to be pre-normalized, the function will not do it.
-    """
-    cdef double entropy=0.
-    cdef float32 intensity
-    for i in range(spectrum.shape[0]):
-        intensity=spectrum[i,1]
-        if intensity>0:
-            entropy+=-intensity*log(intensity)
-    return entropy
-
-
 cpdef centroid_spectrum(float32[:,::1] spectrum,ms2_ppm=None, ms2_da=None):
     """
     Calculate centroid spectrum from a spectrum.
     At least one of the ms2_ppm or ms2_da need be not None. If both ms2_da and ms2_ppm is given, ms2_da will be used.
 
     :param spectrum: The spectrum should be a 2D array with the first dimension being the m/z values and 
                      the second dimension being the intensity values.
```

### Comparing `ms_entropy-0.4.2/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.5.0/ms_entropy.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./ms_entropy/__init__.py
-./ms_entropy/flash_entropy_search.py
-./ms_entropy/flash_entropy_search_core.py
-./ms_entropy/tools.py
 manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
 manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
 manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
 manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
 manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
-ms_entropy/tools_cython.c
-ms_entropy/tools_cython.pyx
 ms_entropy.egg-info/PKG-INFO
 ms_entropy.egg-info/SOURCES.txt
 ms_entropy.egg-info/dependency_links.txt
 ms_entropy.egg-info/requires.txt
-ms_entropy.egg-info/top_level.txt
+ms_entropy.egg-info/top_level.txt
+ms_entropy/tools/fast_entropy.c
+ms_entropy/tools/fast_entropy.pyx
+ms_entropy/tools/fast_spectrum.c
+ms_entropy/tools/fast_spectrum.pyx
```

