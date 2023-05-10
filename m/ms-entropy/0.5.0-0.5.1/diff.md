# Comparing `tmp/ms_entropy-0.5.0.tar.gz` & `tmp/ms_entropy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.0.tar", last modified: Wed May 10 07:44:12 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.1.tar", last modified: Wed May 10 07:52:48 2023, max compression
```

## Comparing `ms_entropy-0.5.0.tar` & `ms_entropy-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.0/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       48 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.0/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/mimas/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.533449 ms_entropy-0.5.0/manuscript/src/mimas/spectra/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.537449 ms_entropy-0.5.0/manuscript/src/mimas/spectra/fast_entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)     4939 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.541448 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/
--rw-rw-r--   0 yli       (1000) yli       (1000)     5950 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     5153 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     6002 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.541448 ms_entropy-0.5.0/manuscript/src/mimas/spectra/spectral_entropy_published/
--rw-rw-r--   0 yli       (1000) yli       (1000)    16189 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.537449 ms_entropy-0.5.0/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.0/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:44:12.545448 ms_entropy-0.5.0/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)      730 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      103 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-10 07:44:12.000000 ms_entropy-0.5.0/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.0/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-10 07:44:12.549448 ms_entropy-0.5.0/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1541 2023-05-10 07:43:00.000000 ms_entropy-0.5.0/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.1/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.1/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.1/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.683582 ms_entropy-0.5.1/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.1/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       52 2023-05-10 07:39:35.000000 ms_entropy-0.5.1/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20245 2023-05-10 07:39:35.000000 ms_entropy-0.5.1/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.1/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.1/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       40 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1974 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4249 2023-05-10 07:39:40.000000 ms_entropy-0.5.1/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.1/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.1/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.1/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.1/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.1/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.1/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-10 07:52:48.687582 ms_entropy-0.5.1/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      422 2023-05-10 07:52:48.000000 ms_entropy-0.5.1/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)      896 2023-05-10 07:52:48.000000 ms_entropy-0.5.1/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-10 07:52:48.000000 ms_entropy-0.5.1/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      103 2023-05-10 07:52:48.000000 ms_entropy-0.5.1/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-10 07:52:48.000000 ms_entropy-0.5.1/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.1/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-10 07:52:48.691582 ms_entropy-0.5.1/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1541 2023-05-10 07:52:45.000000 ms_entropy-0.5.1/setup.py
```

### Comparing `ms_entropy-0.5.0/LICENSE` & `ms_entropy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.0/README.md` & `ms_entropy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.0/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx` & `ms_entropy-0.5.1/ms_entropy/tools/fast_spectrum.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# cython: infer_types=True
-
 import numpy as np
 cimport numpy as np
-from libc.math cimport log2,log,pow
 
 ctypedef np.float32_t float32
 ctypedef np.int64_t int_64
-
-
-
+ctypedef np.int8_t int_8
+ctypedef np.uint32_t uint_32
+from libc.math cimport log2,log,pow
 
 cpdef centroid_spectrum(float32[:,::1] spectrum,ms2_ppm=None, ms2_da=None):
     """
     Calculate centroid spectrum from a spectrum.
     At least one of the ms2_ppm or ms2_da need be not None. If both ms2_da and ms2_ppm is given, ms2_da will be used.
 
     :param spectrum: The spectrum should be a 2D array with the first dimension being the m/z values and 
@@ -95,68 +92,35 @@
                 spec[i_left:i_right, 1] = 0
 
     spec_result = spec_new[:spec_new_i,:]
     spec_result=np.array(spec_result)[np.argsort(spec_result[:,0])]
     return spec_result
 
 
-
-cdef int check_centroid_c(float32[:,::1] spectrum,double ms2_ppm, double ms2_da) nogil:
+cdef int check_centroid_c(float32[:,::1] spectrum,double ms2_ppm, double ms2_da):
     """
     Check whether the spectrum needs to be centroided or not.
     At least one of the ms2_ppm or ms2_da need be not None. If both ms2_da and ms2_ppm is given, ms2_da will be used.
     
     :param spectrum: the spectrum should be a 2D array with the first dimension being the m/z values and 
                      the second dimension being the intensity values.
                      The spectrum need to be sorted by m/z.
                      The spectrum should be in C order.
     :param ms2_ppm: the mass accuracy in ppm.
     :param ms2_da: the mass accuracy in Da.
     """
+    cdef int i
+    
     if spectrum.shape[0]<=1:
         return 0
 
     if ms2_da>0:
         # Use Da accuracy
         for i in range(1, spectrum.shape[0]):
             if spectrum[i, 0]-spectrum[i-1, 0] < ms2_da:
                 return 1
     else:
         # Use ppm accuracy
         for i in range(1, spectrum.shape[0]):
             if spectrum[i, 0]-spectrum[i-1, 0] < spectrum[i, 0]*ms2_ppm*1e-6:
                 return 1
     return 0
-
-
-#################################### TO Check ###############################################
-################################
-# Sort spectra
-cdef void sort_spectrum_by_mz_in_place_c(float32[:,:] spec) nogil:
-    cdef long n = spec.shape[0]
-    cdef long new_n = 0
-    cdef long i
-
-    while n > 1:
-        new_n = 0
-        for i in range(1, n):
-            if spec[i - 1][0] > spec[i][0]:
-                spec[i - 1][0], spec[i][0] = spec[i][0], spec[i - 1][0]
-                spec[i - 1][1], spec[i][1] = spec[i][1], spec[i - 1][1]
-                new_n = i
-        n = new_n
-
-
-cdef void sort_spectrum_by_intensity_in_place_c(float32[:,:] spec) nogil:
-    cdef long n = spec.shape[0]
-    cdef long new_n = 0
-    cdef long i
-
-    while n > 1:
-        new_n = 0
-        for i in range(1, n):
-            if spec[i - 1][1] > spec[i][1]:
-                spec[i - 1][0], spec[i][0] = spec[i][0], spec[i - 1][0]
-                spec[i - 1][1], spec[i][1] = spec[i][1], spec[i - 1][1]
-                new_n = i
-        n = new_n
-################################
```

### Comparing `ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.5.1/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.0/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.5.1/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.0/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.5.1/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.0/setup.py` & `ms_entropy-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.0',
+    version='0.5.1',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=['ms_entropy'],
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
```

