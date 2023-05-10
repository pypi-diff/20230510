# Comparing `tmp/tetgen-0.6.2.tar.gz` & `tmp/tetgen-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetgen-0.6.2.tar", last modified: Fri Jan 13 04:32:23 2023, max compression
+gzip compressed data, was "tetgen-0.6.3.tar", last modified: Wed May 10 19:05:11 2023, max compression
```

## Comparing `tetgen-0.6.2.tar` & `tetgen-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:32:23.549594 tetgen-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34790 2023-01-13 04:32:09.000000 tetgen-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-13 04:32:09.000000 tetgen-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-01-13 04:32:23.549594 tetgen-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-13 04:32:09.000000 tetgen-0.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-13 04:32:09.000000 tetgen-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 04:32:23.549594 tetgen-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-13 04:32:09.000000 tetgen-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:32:23.545595 tetgen-0.6.2/tetgen/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:32:23.541594 tetgen-0.6.2/tetgen/cython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:32:23.549594 tetgen-0.6.2/tetgen/cython/tetgen/
--rw-r--r--   0 runner    (1001) docker     (123)  1085606 2023-01-13 04:32:22.000000 tetgen-0.6.2/tetgen/cython/tetgen/_tetgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   193035 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/cython/tetgen/predicates.cxx
--rw-r--r--   0 runner    (1001) docker     (123)  1286513 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/cython/tetgen/tetgen.cxx
--rw-r--r--   0 runner    (1001) docker     (123)   145931 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/cython/tetgen/tetgen.h
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/cython/tetgen/tetgen_wrap.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/cython/tetgen/tetgen_wrap.h
--rw-r--r--   0 runner    (1001) docker     (123)    26718 2023-01-13 04:32:09.000000 tetgen-0.6.2/tetgen/pytetgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:32:23.545595 tetgen-0.6.2/tetgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-01-13 04:32:23.000000 tetgen-0.6.2/tetgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-13 04:32:23.000000 tetgen-0.6.2/tetgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 04:32:23.000000 tetgen-0.6.2/tetgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-13 04:32:23.000000 tetgen-0.6.2/tetgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-13 04:32:23.000000 tetgen-0.6.2/tetgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.616332 tetgen-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34790 2023-05-10 19:04:53.000000 tetgen-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 19:04:53.000000 tetgen-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-10 19:05:11.616332 tetgen-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 19:04:53.000000 tetgen-0.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-10 19:04:53.000000 tetgen-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:05:11.616332 tetgen-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-10 19:04:53.000000 tetgen-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.612332 tetgen-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 19:04:53.000000 tetgen-0.6.3/tests/test_tetgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.612332 tetgen-0.6.3/tetgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.612332 tetgen-0.6.3/tetgen/cython/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.616332 tetgen-0.6.3/tetgen/cython/tetgen/
+-rw-r--r--   0 runner    (1001) docker     (123)  1087260 2023-05-10 19:05:10.000000 tetgen-0.6.3/tetgen/cython/tetgen/_tetgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   193035 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/cython/tetgen/predicates.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)  1286513 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/cython/tetgen/tetgen.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)   145931 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/cython/tetgen/tetgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/cython/tetgen/tetgen_wrap.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/cython/tetgen/tetgen_wrap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28122 2023-05-10 19:04:53.000000 tetgen-0.6.3/tetgen/pytetgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:05:11.612332 tetgen-0.6.3/tetgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-10 19:05:11.000000 tetgen-0.6.3/tetgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-10 19:05:11.000000 tetgen-0.6.3/tetgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:05:11.000000 tetgen-0.6.3/tetgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 19:05:11.000000 tetgen-0.6.3/tetgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 19:05:11.000000 tetgen-0.6.3/tetgen.egg-info/top_level.txt
```

### Comparing `tetgen-0.6.2/LICENSE` & `tetgen-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/PKG-INFO` & `tetgen-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tetgen
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python interface to tetgen
 Home-page: https://github.com/pyvista/tetgen
-Author: Alex Kaszynski
-Author-email: akascap@gmail.com
+Author: PyVista Developers
+Author-email: info@pyvista.org
 Keywords: TetGen
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `tetgen-0.6.2/README.rst` & `tetgen-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/pyproject.toml` & `tetgen-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/setup.py` & `tetgen-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 setup(
     name="tetgen",
     packages=["tetgen"],
     version=__version__,
     description="Python interface to tetgen",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
-    author="Alex Kaszynski",
-    author_email="akascap@gmail.com",
+    author="PyVista Developers",
+    author_email="info@pyvista.org",
     url="https://github.com/pyvista/tetgen",
     classifiers=[
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `tetgen-0.6.2/tetgen/cython/tetgen/_tetgen.cpp` & `tetgen-0.6.3/tetgen/cython/tetgen/_tetgen.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "TETLIBRARY",
                 null
             ]
         ],
         "depends": [
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "tetgen/cython/tetgen/tetgen.h",
             "tetgen/cython/tetgen/tetgen_wrap.h"
         ],
         "extra_compile_args": [
             "-std=gnu++11",
             "-O3",
             "-w"
         ],
         "include_dirs": [
             "tetgen/cython/tetgen",
-            "/tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "tetgen._tetgen",
         "sources": [
             "tetgen/cython/tetgen/_tetgen.pyx",
             "tetgen/cython/tetgen/tetgen.cxx",
             "tetgen/cython/tetgen/predicates.cxx",
@@ -45,16 +45,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -239,15 +239,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -278,15 +278,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1151,195 +1151,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1372,42 +1372,42 @@
 struct __pyx_obj_6tetgen_7_tetgen_PyBehavior;
 struct __pyx_obj_6tetgen_7_tetgen_PyTetgenio;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2088,20 +2088,28 @@
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -7025,15 +7033,15 @@
   __Pyx_XDECREF(__pyx_v_plc);
   __Pyx_XDECREF(__pyx_v_order);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7042,29 +7050,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7075,15 +7083,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7092,29 +7100,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7125,15 +7133,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7142,29 +7150,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7175,15 +7183,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7192,29 +7200,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7225,15 +7233,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7242,29 +7250,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7275,212 +7283,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7496,15 +7504,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7512,53 +7520,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -7566,30 +7574,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7604,15 +7612,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7628,15 +7636,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7644,53 +7652,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -7698,30 +7706,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7736,15 +7744,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7760,15 +7768,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7776,53 +7784,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -7830,30 +7838,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7868,176 +7876,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22448,26 +22456,26 @@
  * 
  *         # Set behavior
  */
   __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Settings_error_Order_should_be_1); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "../../../../../tmp/build-env-7u8rgru7/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-lx4702v8/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 951, __pyx_L1_error)
@@ -22919,52 +22927,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -23700,28 +23723,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -25534,44 +25557,62 @@
     return -1;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `tetgen-0.6.2/tetgen/cython/tetgen/predicates.cxx` & `tetgen-0.6.3/tetgen/cython/tetgen/predicates.cxx`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/tetgen/cython/tetgen/tetgen.cxx` & `tetgen-0.6.3/tetgen/cython/tetgen/tetgen.cxx`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/tetgen/cython/tetgen/tetgen.h` & `tetgen-0.6.3/tetgen/cython/tetgen/tetgen.h`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/tetgen/cython/tetgen/tetgen_wrap.cxx` & `tetgen-0.6.3/tetgen/cython/tetgen/tetgen_wrap.cxx`

 * *Files identical despite different names*

### Comparing `tetgen-0.6.2/tetgen/pytetgen.py` & `tetgen-0.6.3/tetgen/pytetgen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,84 @@
-"""Python module to interface with wrapped TetGen C++ code
-"""
+"""Python module to interface with wrapped TetGen C++ code."""
 import ctypes
 import logging
 
 import numpy as np
 import pyvista as pv
-from pyvista._vtk import VTK9
 from tetgen import _tetgen
 
 LOG = logging.getLogger(__name__)
 LOG.setLevel("CRITICAL")
 
 
 invalid_input = TypeError(
-    "Invalid input.  Must be either a pyvista.PolyData\n" + "object or vertex and face arrays"
+    "Invalid input. Must be either a pyvista.PolyData object or vertex and face arrays."
 )
 
 
 class TetGen:
     """Input, clean, and tetrahedralize surface meshes using TetGen.
 
     Parameters
     ----------
-    args : str, :class:`pyvista.PolyData` or (``np.ndarray``, ``np.ndarray``)
+    args : str | pyvista.PolyData | numpy.ndarray
         Either a pyvista surface mesh or a ``n x 3`` vertex array and ``n x 3`` face
         array.
 
     Examples
     --------
-    Tetrahedralize a sphere using pyvista
+    Tetrahedralize a sphere using pyvista.
 
     >>> import pyvista
     >>> import tetgen
     >>> sphere = pyvista.Sphere(theta_resolution=10, phi_resolution=10)
     >>> tgen = tetgen.TetGen(sphere)
     >>> nodes, elem = tgen.tetrahedralize()
     >>> tgen.grid.plot(show_edges=True)
 
-    Tetrahedralize a cube using numpy arrays
+    Tetrahedralize a cube using numpy arrays.
 
     >>> import numpy as np
     >>> import tetgen
-    >>> v = np.array([[0, 0, 0], [1, 0, 0],
-                      [1, 1, 0], [0, 1, 0],
-                      [0, 0, 1], [1, 0, 1],
-                      [1, 1, 1], [0, 1, 1],])
-    >>> f = np.vstack([[0, 1, 2], [2, 3, 0],
-                       [0, 1, 5], [5, 4, 0],
-                       [1, 2, 6], [6, 5, 1],
-                       [2, 3, 7], [7, 6, 2],
-                       [3, 0, 4], [4, 7, 3],
-                       [4, 5, 6], [6, 7, 4]])
+    >>> v = np.array(
+    ...     [
+    ...         [0, 0, 0],
+    ...         [1, 0, 0],
+    ...         [1, 1, 0],
+    ...         [0, 1, 0],
+    ...         [0, 0, 1],
+    ...         [1, 0, 1],
+    ...         [1, 1, 1],
+    ...         [0, 1, 1],
+    ...     ]
+    ... )
+    >>> f = np.vstack(
+    ...     [
+    ...         [0, 1, 2],
+    ...         [2, 3, 0],
+    ...         [0, 1, 5],
+    ...         [5, 4, 0],
+    ...         [1, 2, 6],
+    ...         [6, 5, 1],
+    ...         [2, 3, 7],
+    ...         [7, 6, 2],
+    ...         [3, 0, 4],
+    ...         [4, 7, 3],
+    ...         [4, 5, 6],
+    ...         [6, 7, 4],
+    ...     ]
+    ... )
     >>> tgen = tetgen.TetGen(v, f)
     >>> nodes, elems = tgen.tetrahedralize()
     """
 
     _updated = None
 
     def __init__(self, *args):
-        """initializes MeshFix using a mesh"""
+        """Initialize MeshFix using a mesh or arrays."""
         self.v = None
         self.f = None
         self.node = None
         self.elem = None
         self._grid = None
 
         def parse_mesh(mesh):
@@ -82,15 +98,15 @@
         elif isinstance(args[0], str):
             mesh = pv.read(args[0])
             parse_mesh(mesh)
         else:
             raise invalid_input
 
     def _load_arrays(self, v, f):
-        """Loads triangular mesh from vertex and face arrays
+        """Load triangular mesh from vertex and face arrays.
 
         Face arrays/lists are v and f.  Both vertex and face arrays
         should be 2D arrays with each vertex containing XYZ data and
         each face containing three points.
         """
         # Check inputs
         if not isinstance(v, np.ndarray):
@@ -111,22 +127,34 @@
 
         # Store to self
         self.v = v
         self.f = f
 
     def make_manifold(self, verbose=False):
         """Reconstruct a manifold clean surface from input mesh.
+
         Updates mesh in-place.
 
-        Requires pymeshfix
+        Requires `pymeshfix <https://pypi.org/project/pymeshfix/>`_.
 
         Parameters
         ----------
-        verbose : bool, optional
-            Controls output printing.  Default False.
+        verbose : bool, default: False
+            Enable verbose output.
+
+        Examples
+        --------
+        Create a mesh and ensure it's manfold.
+
+        >>> import pyvista
+        >>> import tetgen
+        >>> sphere = pyvista.Sphere(theta_resolution=10, phi_resolution=10)
+        >>> tgen = tetgen.TetGen(sphere)
+        >>> tgen.make_manifold()
+
         """
         try:
             import pymeshfix
         except ImportError:
             raise ImportError("pymeshfix not installed.  Please run:\n" "pip install pymeshfix")
 
         # Run meshfix
@@ -134,23 +162,60 @@
         meshfix.repair(verbose)
 
         # overwrite this object with cleaned mesh
         self.v = meshfix.v
         self.f = meshfix.f
 
     def plot(self, **kwargs):
-        """Displays input mesh
+        """Display the input mesh.
+
+        See :func:`pyvista.plot` for available arguments.
+
+        Examples
+        --------
+        Plot the input mesh.
+
+        >>> import pyvista
+        >>> import tetgen
+        >>> sphere = pyvista.Sphere(theta_resolution=10, phi_resolution=10)
+        >>> tgen = tetgen.TetGen(sphere)
+        >>> tgen.plot()
 
-        See help(:func:`pyvista.plot`) for available arguments.
         """
         self.mesh.plot(**kwargs)
 
     @property
     def mesh(self):
-        """Return the surface mesh"""
+        """Return the surface mesh.
+
+        Returns
+        -------
+        pyvista.PolyData
+            Input surface mesh.
+
+        Examples
+        --------
+        Generate a :class:`tetgen.TetGen` and return a :class:`pyvista.PolyData`.
+
+        >>> import pyvista
+        >>> import tetgen
+        >>> sphere = pyvista.Sphere(theta_resolution=10, phi_resolution=10)
+        >>> tgen = tetgen.TetGen(sphere)
+        >>> tgen.mesh
+        PolyData (0x7fa3c97138e0)
+          N Cells:    160
+          N Points:   82
+          N Strips:   0
+          X Bounds:   -4.924e-01, 4.924e-01
+          Y Bounds:   -4.683e-01, 4.683e-01
+          Z Bounds:   -5.000e-01, 5.000e-01
+          N Arrays:   0
+
+
+        """
         triangles = np.empty((self.f.shape[0], 4), dtype="int")
         triangles[:, -3:] = self.f
         triangles[:, 0] = 3
         return pv.PolyData(self.v, triangles, deep=False)
 
     def tetrahedralize(
         self,
@@ -233,16 +298,16 @@
         metric_scale=1.0,
         smooth_alpha=0.3,
         coarsen_percent=1.0,
         elem_growth_ratio=0.0,
         refine_progress_ratio=0.333,
         switches=None,
     ):
-        """Generates tetrahedrals interior to the surface mesh
-        described by the vertex and face arrays already loaded.
+        """Generate tetrahedrals interior to the surface mesh.
+
         Returns nodes and elements belonging to the all tetrahedral
         mesh.
 
         The tetrahedral generator uses the C++ library TetGen and can
         be configured by either using a string of ``switches`` or by
         changing the underlying behavior using optional inputs.
 
@@ -254,85 +319,91 @@
         Parameters
         ----------
         quality : bool, optional
             Enables/disables mesh improvement.  Enabled by default.
             Disable this to speed up mesh generation while sacrificing
             quality.  Default True.
 
-        minratio : double, optional.
+        minratio : double, default: 2.0
             Maximum allowable radius-edge ratio.  Must be greater than
             1.0 the closer to 1.0, the higher the quality of the mesh.
             Be sure to raise ``steinerleft`` to allow for the addition of
             points to improve the quality of the mesh.  Avoid overly
             restrictive requirements, otherwise, meshing will appear
-            to hang.  Default 2.0
+            to hang.
 
             Testing has showed that 1.1 is a reasonable input for a
             high quality mesh.
 
-        mindihedral : double, optional
+        mindihedral : double, default: 0.0
             Minimum allowable dihedral angle.  The larger this number,
             the higher the quality of the resulting mesh.  Be sure to
             raise ``steinerleft`` to allow for the addition of points to
             improve the quality of the mesh.  Avoid overly restrictive
             requirements, otherwise, meshing will appear to hang.
-            Default 0.0
 
             Testing has shown that 10 is a reasonable input
 
-        verbose : int, optional
+        verbose : int, default: 0
             Controls the underlying TetGen library to output text to
             console.  Users using iPython will not see this output.
             Setting to 1 enables some information about the mesh
             generation while setting verbose to 2 enables more debug
-            output.  Default 0, or no output.
+            output.  Default is no output
 
-        nobisect : bool, optional
+        nobisect : bool, default: False
             Controls if Steiner points are added to the input surface
             mesh.  When enabled, the surface mesh will be modified.
-            Default False.
 
             Testing has shown that if your input surface mesh is
             already well shaped, disabling this setting will improve
             meshing speed and mesh quality.
 
-        steinerleft : int, optional
+        steinerleft : int, default: 100000
             Steiner points are points added to the original surface
             mesh to create a valid tetrahedral mesh.  Settings this to
             -1 will allow tetgen to create an unlimited number of
             steiner points, but the program will likely hang if this
             is used in combination with narrow quality requirements.
-            Default 100000.
 
             The first type of Steiner points are used in creating an
             initial tetrahedralization of PLC. These Steiner points
             are mandatory in order to create a valid
             tetrahedralization
 
             The second type of Steiner points are used in creating
             quality tetra- hedral meshes of PLCs. These Steiner points
             are optional, while they may be necessary in order to
             improve the mesh quality or to conform the size of mesh
             elements.
 
-        order : int optional
+        order : int, default: 2
             Controls whether TetGen creates linear tetrahedrals or
             quadradic tetrahedrals.  Set order to 2 to output
-            quadradic tetrahedrals.  Default 2.
+            quadradic tetrahedrals.
+
+        Returns
+        -------
+        nodes : numpy.ndarray
+            Array of nodes representing the tetrahedral mesh.
+
+        elems : numpy.ndarray
+            Array of elements representing the tetrahedral mesh.
 
         Examples
         --------
         The following switches "pq1.1/10Y" would be:
 
-        >>> node, elem = tgen.tetrahedralize(nobisect=True, quality=True,
-                                             minratio=1.1, mindihedral=10)
+        >>> nodes, elems = tgen.tetrahedralize(
+        ...     nobisect=True, quality=True, minratio=1.1, mindihedral=10
+        ... )
 
         Using the switches option:
 
-        >>> node, elem = tgen.tetrahedralize(switches="pq1.1/10Y")
+        >>> nodes, elems = tgen.tetrahedralize(switches="pq1.1/10Y")
 
         Notes
         -----
         There are many other options and the TetGen documentation
         contains descriptions only for the switches of the original
         C++ program.  This is the relationship between tetgen switches
         and python optional inputs:
@@ -494,15 +565,14 @@
         +---------------------------+---------------+---------+
         | elem_growth_ratio         | ``'-r#'``     | 0.0.    |
         +---------------------------+---------------+---------+
         | refine_progress_ratio     | ``'-r/#'``    | 0.333.  |
         +---------------------------+---------------+---------+
 
         """
-
         # format switches
         if switches is None:
             switches_str = b""
         else:
             switches_str = bytes(switches, "utf-8")
 
         # check verbose switch
@@ -617,15 +687,15 @@
         )
         self._updated = True
 
         return self.node, self.elem
 
     @property
     def grid(self):
-        """Returns a :class:`pyvista.UnstructuredGrid`"""
+        """Return a :class:`pyvista.UnstructuredGrid`."""
         if self.node is None:
             raise RuntimeError("Run Tetrahedralize first")
 
         if self._grid is not None and not self._updated:
             return self._grid
 
         buf = np.empty((self.elem.shape[0], 1), pv.ID_TYPE)
@@ -636,44 +706,44 @@
         elif self.elem.shape[1] == 10:  # quadradic
             buf[:] = 10
             cell_type[:] = 24
         else:
             raise Exception("Invalid element array shape %s" % str(self.elem.shape))
 
         cells = np.hstack((buf, self.elem))
-        if VTK9:
-            self._grid = pv.UnstructuredGrid(cells, cell_type, self.node)
-        else:
-            offset = np.cumsum(buf + 1) - (buf[0] + 1)
-            self._grid = pv.UnstructuredGrid(offset, cells, cell_type, self.node)
+        self._grid = pv.UnstructuredGrid(cells, cell_type, self.node)
 
         self._updated = False
         return self._grid
 
     def write(self, filename, binary=False):
-        """Writes an unstructured grid to disk.
+        """Write an unstructured grid to disk.
 
         Parameters
         ----------
         filename : str
             Filename of grid to be written.  The file extension will
             select the type of writer to use.
 
             - ``".vtk"`` will use the vtk legacy writer
             - ``".vtu"`` will select the VTK XML writer
-            - ``".cdb"`` will write an ANSYS APDL archive file
 
-        binary : bool, optional
-            Writes as a binary file by default.  Set to False to write
-            ASCII.  Ignored when output is a cdb.
+        binary : bool, default: False
+            Writes as a binary file by default.  Set to ``False`` to write
+            ASCII.
 
         Examples
         --------
-        >>> tgen.write('grid.vtk', binary=True)
+        Write to a VTK file.
+
+        >>> tgen.write("grid.vtk", binary=True)
 
         Notes
         -----
         Binary files write much faster than ASCII, but binary files
         written on one system may not be readable on other systems.
         Binary can be used only with the legacy writer.
+
+        You can use utilities like `meshio <https://github.com/nschloe/meshio>`_
+        to convert to other formats in order to import into FEA software.
         """
         self.grid.save(filename, binary)
```

### Comparing `tetgen-0.6.2/tetgen.egg-info/PKG-INFO` & `tetgen-0.6.3/tetgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tetgen
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python interface to tetgen
 Home-page: https://github.com/pyvista/tetgen
-Author: Alex Kaszynski
-Author-email: akascap@gmail.com
+Author: PyVista Developers
+Author-email: info@pyvista.org
 Keywords: TetGen
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

