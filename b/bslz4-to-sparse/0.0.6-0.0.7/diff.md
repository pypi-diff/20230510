# Comparing `tmp/bslz4_to_sparse-0.0.6.tar.gz` & `tmp/bslz4_to_sparse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bslz4_to_sparse-0.0.6.tar", last modified: Sat May  6 11:59:19 2023, max compression
+gzip compressed data, was "bslz4_to_sparse-0.0.7.tar", last modified: Wed May 10 08:00:27 2023, max compression
```

## Comparing `bslz4_to_sparse-0.0.6.tar` & `bslz4_to_sparse-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.399632 bslz4_to_sparse-0.0.6/
--rw-r--r--   0 wright    (2427) id11      (1611)     1067 2023-03-06 21:46:52.000000 bslz4_to_sparse-0.0.6/LICENSE
--rw-r--r--   0 wright    (2427) id11      (1611)      142 2023-03-13 13:21:39.000000 bslz4_to_sparse-0.0.6/MANIFEST.in
--rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-06 11:59:19.397646 bslz4_to_sparse-0.0.6/PKG-INFO
--rw-r--r--   0 wright    (2427) id11      (1611)      226 2023-03-07 11:25:12.000000 bslz4_to_sparse-0.0.6/README.md
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.257643 bslz4_to_sparse-0.0.6/bitshuffle/
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.324650 bslz4_to_sparse-0.0.6/bitshuffle/src/
--rw-r--r--   0 wright    (2427) id11      (1611)    65340 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.c
--rw-r--r--   0 wright    (2427) id11      (1611)     4533 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.h
--rw-r--r--   0 wright    (2427) id11      (1611)     2233 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_internals.h
--rw-r--r--   0 wright    (2427) id11      (1611)     2483 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.c
--rw-r--r--   0 wright    (2427) id11      (1611)     2616 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.h
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.349668 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/
--rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/PKG-INFO
--rw-r--r--   0 wright    (2427) id11      (1611)      737 2023-05-06 11:59:19.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/SOURCES.txt
--rw-r--r--   0 wright    (2427) id11      (1611)        1 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/dependency_links.txt
--rw-r--r--   0 wright    (2427) id11      (1611)       11 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/requires.txt
--rw-r--r--   0 wright    (2427) id11      (1611)       16 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/top_level.txt
--rw-r--r--   0 wright    (2427) id11      (1611)    28422 2023-04-21 14:28:51.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparsemodule.c
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.261647 bslz4_to_sparse-0.0.6/lz4/
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.362660 bslz4_to_sparse-0.0.6/lz4/lib/
--rw-r--r--   0 wright    (2427) id11      (1611)   114204 2023-03-12 06:07:55.000000 bslz4_to_sparse-0.0.6/lz4/lib/lz4.c
--rw-r--r--   0 wright    (2427) id11      (1611)    44421 2023-03-12 06:07:57.000000 bslz4_to_sparse-0.0.6/lz4/lib/lz4.h
--rw-r--r--   0 wright    (2427) id11      (1611)      118 2023-03-07 07:34:45.000000 bslz4_to_sparse-0.0.6/pyproject.toml
--rw-r--r--   0 wright    (2427) id11      (1611)       38 2023-05-06 11:59:19.400632 bslz4_to_sparse-0.0.6/setup.cfg
--rw-r--r--   0 wright    (2427) id11      (1611)     2780 2023-05-06 11:57:53.000000 bslz4_to_sparse-0.0.6/setup.py
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.385629 bslz4_to_sparse-0.0.6/src/
--rw-r--r--   0 wright    (2427) id11      (1611)     3390 2023-05-06 11:58:03.000000 bslz4_to_sparse-0.0.6/src/__init__.py
--rw-r--r--   0 wright    (2427) id11      (1611)     3842 2023-03-17 14:19:19.000000 bslz4_to_sparse-0.0.6/src/bshuf.c
--rw-r--r--   0 wright    (2427) id11      (1611)     1337 2023-03-17 13:49:45.000000 bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.c
--rw-r--r--   0 wright    (2427) id11      (1611)     1548 2023-03-17 13:49:47.000000 bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.pyf
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.391650 bslz4_to_sparse-0.0.6/test/
--rw-r--r--   0 wright    (2427) id11      (1611)     4249 2023-03-27 14:17:12.000000 bslz4_to_sparse-0.0.6/test/test1.py
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.676675 bslz4_to_sparse-0.0.7/
+-rw-r--r--   0 wright    (2427) id11      (1611)     1067 2023-03-06 21:46:52.000000 bslz4_to_sparse-0.0.7/LICENSE
+-rw-r--r--   0 wright    (2427) id11      (1611)      162 2023-05-10 07:59:45.000000 bslz4_to_sparse-0.0.7/MANIFEST.in
+-rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-10 08:00:27.675667 bslz4_to_sparse-0.0.7/PKG-INFO
+-rw-r--r--   0 wright    (2427) id11      (1611)      226 2023-03-07 11:25:12.000000 bslz4_to_sparse-0.0.7/README.md
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.355752 bslz4_to_sparse-0.0.7/bitshuffle/
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.497708 bslz4_to_sparse-0.0.7/bitshuffle/src/
+-rw-r--r--   0 wright    (2427) id11      (1611)    65340 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_core.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     4533 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_core.h
+-rw-r--r--   0 wright    (2427) id11      (1611)     2233 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_internals.h
+-rw-r--r--   0 wright    (2427) id11      (1611)     2483 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.7/bitshuffle/src/iochain.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     2616 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.7/bitshuffle/src/iochain.h
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.560685 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/
+-rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-10 08:00:26.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/PKG-INFO
+-rw-r--r--   0 wright    (2427) id11      (1611)      737 2023-05-10 08:00:27.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/SOURCES.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)        1 2023-05-10 08:00:26.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/dependency_links.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)       11 2023-05-10 08:00:26.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/requires.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)       16 2023-05-10 08:00:26.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/top_level.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)    28422 2023-04-21 14:28:51.000000 bslz4_to_sparse-0.0.7/bslz4_to_sparsemodule.c
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.359682 bslz4_to_sparse-0.0.7/lz4/
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.590668 bslz4_to_sparse-0.0.7/lz4/lib/
+-rw-r--r--   0 wright    (2427) id11      (1611)   114204 2023-03-12 06:07:55.000000 bslz4_to_sparse-0.0.7/lz4/lib/lz4.c
+-rw-r--r--   0 wright    (2427) id11      (1611)    44421 2023-03-12 06:07:57.000000 bslz4_to_sparse-0.0.7/lz4/lib/lz4.h
+-rw-r--r--   0 wright    (2427) id11      (1611)      118 2023-03-07 07:34:45.000000 bslz4_to_sparse-0.0.7/pyproject.toml
+-rw-r--r--   0 wright    (2427) id11      (1611)       38 2023-05-10 08:00:27.676707 bslz4_to_sparse-0.0.7/setup.cfg
+-rw-r--r--   0 wright    (2427) id11      (1611)     2737 2023-05-10 08:00:03.000000 bslz4_to_sparse-0.0.7/setup.py
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.646715 bslz4_to_sparse-0.0.7/src/
+-rw-r--r--   0 wright    (2427) id11      (1611)     3390 2023-05-10 08:00:01.000000 bslz4_to_sparse-0.0.7/src/__init__.py
+-rw-r--r--   0 wright    (2427) id11      (1611)     3842 2023-03-17 14:19:19.000000 bslz4_to_sparse-0.0.7/src/bshuf.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     1337 2023-03-17 13:49:45.000000 bslz4_to_sparse-0.0.7/src/bslz4_to_sparse.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     1548 2023-03-17 13:49:47.000000 bslz4_to_sparse-0.0.7/src/bslz4_to_sparse.pyf
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-10 08:00:27.661665 bslz4_to_sparse-0.0.7/test/
+-rw-r--r--   0 wright    (2427) id11      (1611)     4249 2023-03-27 14:17:12.000000 bslz4_to_sparse-0.0.7/test/test1.py
```

### Comparing `bslz4_to_sparse-0.0.6/LICENSE` & `bslz4_to_sparse-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.c` & `bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_core.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.h` & `bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_core.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_internals.h` & `bslz4_to_sparse-0.0.7/bitshuffle/src/bitshuffle_internals.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.c` & `bslz4_to_sparse-0.0.7/bitshuffle/src/iochain.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.h` & `bslz4_to_sparse-0.0.7/bitshuffle/src/iochain.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/SOURCES.txt` & `bslz4_to_sparse-0.0.7/bslz4_to_sparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/bslz4_to_sparsemodule.c` & `bslz4_to_sparse-0.0.7/bslz4_to_sparsemodule.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/lz4/lib/lz4.c` & `bslz4_to_sparse-0.0.7/lz4/lib/lz4.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/lz4/lib/lz4.h` & `bslz4_to_sparse-0.0.7/lz4/lib/lz4.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/setup.py` & `bslz4_to_sparse-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             if line.find('avx2')>=0:
                 flags.append('-mavx2')
                 break
 
 ext = Extension( "bslz4_to_sparse",
                  sources = ["src/bslz4_to_sparse.pyf",
                             "src/bslz4_to_sparse.c",
-                            "src/bshuf.c",
                             "lz4/lib/lz4.c",
                             "bitshuffle/src/bitshuffle_core.c",
                             "bitshuffle/src/iochain.c",  ],
                  include_dirs  = [ numpy.get_include(),
                                    numpy.f2py.get_include(), ],
                  extra_compile_args = flags + [ '-O3',
                                     '-DF2PY_REPORT_ON_ARRAY_COPY=1',
@@ -63,12 +62,12 @@
        ext_package = 'bslz4_to_sparse',
        ext_modules = [ext, ],
        cmdclass = { 'build_ext' : build_ext_subclass },
        install_requires = ["numpy", "h5py"],
        author = 'Jon Wright',
        author_email = 'wright@esrf.fr',
        url = "http://github.com/jonwright/bslz4_to_sparse",
-       version = '0.0.6',
+       version = '0.0.7',
        license = 'MIT',
        long_description = readme,
        long_description_content_type='text/markdown',
 )
```

### Comparing `bslz4_to_sparse-0.0.6/src/__init__.py` & `bslz4_to_sparse-0.0.7/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import numpy as np
 import ctypes
 from .bslz4_to_sparse import bslz4_uint32_t, bslz4_uint16_t, bslz4_uint8_t
 
-version = '0.0.6'
+version = '0.0.7'
 
 # We cast away the 'read-only' nature of python bytes.
 # Not needed for the latest numpy.
 buffer_from_memory = ctypes.pythonapi.PyMemoryView_FromMemory
 buffer_from_memory.restype = ctypes.py_object
 buffer_from_memory.argtypes = (ctypes.c_void_p, ctypes.c_int, ctypes.c_int)
```

### Comparing `bslz4_to_sparse-0.0.6/src/bshuf.c` & `bslz4_to_sparse-0.0.7/src/bshuf.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.c` & `bslz4_to_sparse-0.0.7/src/bslz4_to_sparse.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.pyf` & `bslz4_to_sparse-0.0.7/src/bslz4_to_sparse.pyf`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.6/test/test1.py` & `bslz4_to_sparse-0.0.7/test/test1.py`

 * *Files identical despite different names*

