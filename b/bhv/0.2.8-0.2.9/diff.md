# Comparing `tmp/bhv-0.2.8.tar.gz` & `tmp/bhv-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.8.tar", last modified: Mon May  8 19:42:57 2023, max compression
+gzip compressed data, was "bhv-0.2.9.tar", last modified: Wed May 10 11:55:51 2023, max compression
```

## Comparing `bhv-0.2.8.tar` & `bhv-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.8/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-08 19:42:57.625020 bhv-0.2.8/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.8/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.8/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12173 2023-05-08 14:41:53.000000 bhv-0.2.8/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2119 2023-05-05 13:49:14.000000 bhv-0.2.8/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11275 2023-05-08 19:42:15.000000 bhv-0.2.8/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.8/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.8/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.8/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.2.8/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.8/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.2.8/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)        7 2023-05-05 10:13:11.000000 bhv-0.2.8/bhv/test.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3359 2023-05-08 19:17:04.000000 bhv-0.2.8/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.8/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-08 19:42:57.625020 bhv-0.2.8/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      356 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-08 19:42:57.000000 bhv-0.2.8/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-08 19:42:57.625020 bhv-0.2.8/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-08 19:33:57.000000 bhv-0.2.8/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.051033 bhv-0.2.9/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.9/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-10 11:55:51.051033 bhv-0.2.9/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.9/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.047700 bhv-0.2.9/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.9/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12173 2023-05-08 14:41:53.000000 bhv-0.2.9/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.2.9/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.2.9/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.9/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.9/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.9/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.2.9/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.9/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    24158 2023-05-05 11:23:02.000000 bhv-0.2.9/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3503 2023-05-10 11:50:50.000000 bhv-0.2.9/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.9/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-10 11:55:51.047700 bhv-0.2.9/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-10 11:55:51.000000 bhv-0.2.9/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-10 11:55:51.051033 bhv-0.2.9/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-10 11:54:44.000000 bhv-0.2.9/setup.py
```

### Comparing `bhv-0.2.8/LICENSE` & `bhv-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/PKG-INFO` & `bhv-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.8
+Version: 0.2.9
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.8/README.md` & `bhv-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/abstract.py` & `bhv-0.2.9/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/embedding.py` & `bhv-0.2.9/bhv/embedding.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
     ar[:on] = True
     return ar
 
 def filln(xs, n):
     ar = torch.empty(len(xs)*n, dtype=torch.bool)
     for i, x in enumerate(xs):
         ar[i*n:(i + 1)*n] = binarize_3(x, n)
-    return ar
+    return ar
```

### Comparing `bhv-0.2.8/bhv/np.py` & `bhv-0.2.9/bhv/np.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .abstract import *
 import numpy as np
-from sys import byteorder
+from sys import byteorder, version_info
 
 
 class NumPyBoolPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
     rng = np.random.default_rng()
 
     def __init__(self, array: np.ndarray):
@@ -165,16 +165,22 @@
 
     def __or__(self, other: 'NumPyPacked8BHV') -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_or(self.data, other.data))
 
     def __invert__(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.bitwise_not(self.data))
 
-    def active(self) -> int:
-        return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
+    if version_info[2] >= 10:
+        def active(self) -> int:
+            return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
+    else:
+        lookup = np.array([bin(i).count("1") for i in range(256)])
+
+        def active(self) -> int:
+            return self.lookup[self.data].sum()
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data))
 
     def repack64(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(self.data.view(dtype=np.uint64))
 
@@ -268,16 +274,20 @@
 
     def __or__(self, other: 'NumPyPacked64BHV') -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.bitwise_or(self.data, other.data))
 
     def __invert__(self) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(np.bitwise_not(self.data))
 
-    def active(self) -> int:
-        return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
+    if version_info[2] >= 10:
+        def active(self) -> int:
+            return int.from_bytes(self.data.tobytes(), byteorder).bit_count()
+    else:
+        def active(self) -> int:
+            return self.repack8().active()
 
     def unpack(self) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.unpackbits(self.data.view(np.uint8)))
 
     def repack8(self) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(self.data.view(dtype=np.uint8))
```

### Comparing `bhv-0.2.8/bhv/poibin.py` & `bhv-0.2.9/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/positions.py` & `bhv-0.2.9/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/pytorch.py` & `bhv-0.2.9/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/shared.py` & `bhv-0.2.9/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/slice.py` & `bhv-0.2.9/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/symbolic.py` & `bhv-0.2.9/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv/vanilla.py` & `bhv-0.2.9/bhv/vanilla.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .abstract import *
 import random
-from sys import byteorder
+from sys import byteorder, version_info
 
 
 class VanillaPermutation(MemoizedPermutation):
     _permutations: 'dict[int | tuple[int, ...], Self]' = {}
 
     def __init__(self, indices):
         self.data = indices
@@ -70,16 +70,20 @@
 
     def __or__(self, other: 'VanillaBHV') -> 'VanillaBHV':
         return self.from_int(self.to_int() | other.to_int())
 
     def __invert__(self) -> 'VanillaBHV':
         return self.from_int(~self.to_int())
 
-    def active(self) -> int:
-        return self.to_int().bit_count()
+    if version_info[2] >= 10:
+        def active(self) -> int:
+            return self.to_int().bit_count()
+    else:
+        def active(self) -> int:
+            return bin(self.to_int()).count("1")
 
     def to_int(self) -> int:
         return int.from_bytes(self.data, byteorder, signed=True)
 
     @classmethod
     def from_int(cls, i: int):
         return VanillaBHV(i.to_bytes(DIMENSION//8, byteorder, signed=True))
```

### Comparing `bhv-0.2.8/bhv/visualization.py` & `bhv-0.2.9/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.8/bhv.egg-info/PKG-INFO` & `bhv-0.2.9/bhv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.8
+Version: 0.2.9
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.8/setup.py` & `bhv-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.8'
+VERSION = '0.2.9'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

