# Comparing `tmp/pyxtend-0.2.0.tar.gz` & `tmp/pyxtend-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtend-0.2.0.tar", last modified: Wed May 10 01:18:27 2023, max compression
+gzip compressed data, was "pyxtend-0.2.2.tar", last modified: Wed May 10 03:45:54 2023, max compression
```

## Comparing `pyxtend-0.2.0.tar` & `pyxtend-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.222142 pyxtend-0.2.0/
--rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      562 2023-05-10 01:18:27.222142 pyxtend-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       61 2022-01-06 02:29:45.000000 pyxtend-0.2.0/README.md
--rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      640 2023-05-10 01:18:27.224176 pyxtend-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.196150 pyxtend-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.206144 pyxtend-0.2.0/src/pyxtend/
--rw-rw-rw-   0        0        0       32 2022-01-02 19:51:01.000000 pyxtend-0.2.0/src/pyxtend/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-05-10 01:12:35.000000 pyxtend-0.2.0/src/pyxtend/pyxtend.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.220174 pyxtend-0.2.0/src/pyxtend.egg-info/
--rw-rw-rw-   0        0        0      562 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.406304 pyxtend-0.2.2/
+-rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1261 2023-05-10 03:45:54.406304 pyxtend-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-10 01:25:20.000000 pyxtend-0.2.2/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      640 2023-05-10 03:45:54.408300 pyxtend-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.379305 pyxtend-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.392305 pyxtend-0.2.2/src/pyxtend/
+-rw-rw-rw-   0        0        0       62 2023-05-10 03:32:58.000000 pyxtend-0.2.2/src/pyxtend/__init__.py
+-rw-rw-rw-   0        0        0     1720 2023-05-10 03:29:48.000000 pyxtend-0.2.2/src/pyxtend/struct.py
+-rw-rw-rw-   0        0        0      270 2023-05-10 03:14:44.000000 pyxtend-0.2.2/src/pyxtend/vprint.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.405300 pyxtend-0.2.2/src/pyxtend.egg-info/
+-rw-rw-rw-   0        0        0     1261 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/top_level.txt
```

### Comparing `pyxtend-0.2.0/LICENSE` & `pyxtend-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxtend-0.2.0/setup.cfg` & `pyxtend-0.2.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7978 7465 6e64 0d0a 7665 7273   = pyxtend..vers
-00000020: 696f 6e20 3d20 302e 322e 300d 0a61 7574  ion = 0.2.0..aut
+00000020: 696f 6e20 3d20 302e 322e 320d 0a61 7574  ion = 0.2.2..aut
 00000030: 686f 7220 3d20 4a75 6c69 7573 0d0a 6175  hor = Julius..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206a 756c  thor_email = jul
 00000050: 6975 732e 7369 6d6f 6e65 6c6c 6940 676d  ius.simonelli@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 2053 6f6d 6520 6675 6e63  tion = Some func
 00000080: 7469 6f6e 7320 666f 7220 5079 7468 6f6e  tions for Python
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `pyxtend-0.2.0/src/pyxtend/pyxtend.py` & `pyxtend-0.2.2/src/pyxtend/struct.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import contextlib
 from collections.abc import Iterable
-from typing import Any, Iterable, Union
+from typing import Any, Union
 
 import numpy as np
-import tensorflow as tf
-import torch
 from shapely.geometry.base import BaseGeometry
 
 
 def struct(obj: Any, level: int = 0, limit: int = 3) -> Union[str, dict]:
     """
     Returns the general structure of a given Python object.
 
@@ -16,44 +13,31 @@
         obj: The Python object to analyze.
         level: The current depth of recursion (default: 0).
         limit: The maximum number of elements to display for each type (default: 3).
 
     Returns:
         The structure of the input object as a dictionary or string.
     """
+    obj_type_name = type(obj).__name__
+
     if isinstance(obj, (int, float, bool)):
-        return type(obj).__name__
+        return obj_type_name
     elif isinstance(obj, str):
         return "str"
-    elif isinstance(obj, torch.Tensor):
-        return {f"{type(obj).__name__}": [f"{obj.dtype}, shape={tuple(obj.shape)}"]}
-    elif isinstance(obj, tf.Tensor):
-        return {f"{type(obj).__name__}": [f"{obj.dtype.name}, shape={tuple(obj.shape)}"]}
+    elif obj_type_name in ["Tensor", "EagerTensor"]:
+        return {obj_type_name: [f"{obj.dtype}, shape={tuple(getattr(obj, 'shape', ()))}"]}
     elif isinstance(obj, np.ndarray):
-        if obj.size == 0:  # Check if the array is empty
-            inner_structure = "empty"
-        else:
-            inner_structure = struct(obj.item(0), level + 1)
+        inner_structure = "empty" if obj.size == 0 else struct(obj.item(0), level + 1)
         return {f"{type(obj).__name__}": [f"{obj.dtype}, shape={obj.shape}"]}
     elif isinstance(obj, BaseGeometry):
         coords = np.array(obj.exterior.coords)
         return {f"{type(obj).__name__}": [f"float64, shape={coords.shape}"]}
     elif isinstance(obj, Iterable) and not isinstance(obj, (str, bytes)):
         if level < limit:
             inner_structure = [struct(x, level + 1) for x in obj]
             if len(obj) > 3:
                 inner_structure = inner_structure[:3] + [f"...{len(obj)} total"]
             return {type(obj).__name__: inner_structure}
         else:
             return {type(obj).__name__: "..."}
     else:
-        return "unsupported"  # type(obj).__name__ or {type(obj).__name__: 'unsupported'}
-
-
-def vprint(*text: str) -> None:
-    """
-    Print the text if verbose=True in outer context.
-    Print nothing if verbose=False or is undefined.
-    """
-    with contextlib.suppress(NameError):
-        if verbose:
-            print(*text)
+        return "unsupported"
```

