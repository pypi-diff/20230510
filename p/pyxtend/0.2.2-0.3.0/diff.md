# Comparing `tmp/pyxtend-0.2.2.tar.gz` & `tmp/pyxtend-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtend-0.2.2.tar", last modified: Wed May 10 03:45:54 2023, max compression
+gzip compressed data, was "pyxtend-0.3.0.tar", last modified: Wed May 10 04:00:27 2023, max compression
```

## Comparing `pyxtend-0.2.2.tar` & `pyxtend-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.406304 pyxtend-0.2.2/
--rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1261 2023-05-10 03:45:54.406304 pyxtend-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-10 01:25:20.000000 pyxtend-0.2.2/README.md
--rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      640 2023-05-10 03:45:54.408300 pyxtend-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.379305 pyxtend-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.392305 pyxtend-0.2.2/src/pyxtend/
--rw-rw-rw-   0        0        0       62 2023-05-10 03:32:58.000000 pyxtend-0.2.2/src/pyxtend/__init__.py
--rw-rw-rw-   0        0        0     1720 2023-05-10 03:29:48.000000 pyxtend-0.2.2/src/pyxtend/struct.py
--rw-rw-rw-   0        0        0      270 2023-05-10 03:14:44.000000 pyxtend-0.2.2/src/pyxtend/vprint.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:45:54.405300 pyxtend-0.2.2/src/pyxtend.egg-info/
--rw-rw-rw-   0        0        0     1261 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 03:45:54.000000 pyxtend-0.2.2/src/pyxtend.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 04:00:26.993981 pyxtend-0.3.0/
+-rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1261 2023-05-10 04:00:26.994981 pyxtend-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-10 01:25:20.000000 pyxtend-0.3.0/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      640 2023-05-10 04:00:26.996981 pyxtend-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 04:00:26.962983 pyxtend-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 04:00:26.975982 pyxtend-0.3.0/src/pyxtend/
+-rw-rw-rw-   0        0        0       62 2023-05-10 03:32:58.000000 pyxtend-0.3.0/src/pyxtend/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-05-10 03:54:49.000000 pyxtend-0.3.0/src/pyxtend/struct.py
+-rw-rw-rw-   0        0        0      270 2023-05-10 03:14:44.000000 pyxtend-0.3.0/src/pyxtend/vprint.py
+drwxrwxrwx   0        0        0        0 2023-05-10 04:00:26.992979 pyxtend-0.3.0/src/pyxtend.egg-info/
+-rw-rw-rw-   0        0        0     1261 2023-05-10 04:00:26.000000 pyxtend-0.3.0/src/pyxtend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-10 04:00:26.000000 pyxtend-0.3.0/src/pyxtend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 04:00:26.000000 pyxtend-0.3.0/src/pyxtend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 04:00:26.000000 pyxtend-0.3.0/src/pyxtend.egg-info/top_level.txt
```

### Comparing `pyxtend-0.2.2/LICENSE` & `pyxtend-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxtend-0.2.2/PKG-INFO` & `pyxtend-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtend
-Version: 0.2.2
+Version: 0.3.0
 Summary: Some functions for Python
 Home-page: https://github.com/jss367/pyxtend
 Author: Julius
 Author-email: julius.simonelli@gmail.com
 Project-URL: Bug Tracker, https://github.com/jss367/pyxtend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtend-0.2.2/README.md` & `pyxtend-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyxtend-0.2.2/setup.cfg` & `pyxtend-0.3.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7978 7465 6e64 0d0a 7665 7273   = pyxtend..vers
-00000020: 696f 6e20 3d20 302e 322e 320d 0a61 7574  ion = 0.2.2..aut
+00000020: 696f 6e20 3d20 302e 332e 300d 0a61 7574  ion = 0.3.0..aut
 00000030: 686f 7220 3d20 4a75 6c69 7573 0d0a 6175  hor = Julius..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206a 756c  thor_email = jul
 00000050: 6975 732e 7369 6d6f 6e65 6c6c 6940 676d  ius.simonelli@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 2053 6f6d 6520 6675 6e63  tion = Some func
 00000080: 7469 6f6e 7320 666f 7220 5079 7468 6f6e  tions for Python
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `pyxtend-0.2.2/src/pyxtend/struct.py` & `pyxtend-0.3.0/src/pyxtend/struct.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from collections.abc import Iterable
 from typing import Any, Union
 
-import numpy as np
-from shapely.geometry.base import BaseGeometry
-
 
 def struct(obj: Any, level: int = 0, limit: int = 3) -> Union[str, dict]:
     """
     Returns the general structure of a given Python object.
 
     Args:
         obj: The Python object to analyze.
@@ -21,20 +18,23 @@
 
     if isinstance(obj, (int, float, bool)):
         return obj_type_name
     elif isinstance(obj, str):
         return "str"
     elif obj_type_name in ["Tensor", "EagerTensor"]:
         return {obj_type_name: [f"{obj.dtype}, shape={tuple(getattr(obj, 'shape', ()))}"]}
-    elif isinstance(obj, np.ndarray):
+    elif obj_type_name == "ndarray":
         inner_structure = "empty" if obj.size == 0 else struct(obj.item(0), level + 1)
-        return {f"{type(obj).__name__}": [f"{obj.dtype}, shape={obj.shape}"]}
-    elif isinstance(obj, BaseGeometry):
-        coords = np.array(obj.exterior.coords)
-        return {f"{type(obj).__name__}": [f"float64, shape={coords.shape}"]}
+        shape = tuple(obj.shape)
+        dtype = obj.dtype.name
+        return {f"{type(obj).__name__}": [f"{dtype}, shape={shape}"]}
+    elif obj_type_name == "Polygon":
+        coords = list(getattr(obj, "exterior", {}).coords) if hasattr(obj, "exterior") else []
+        shape = (len(coords), len(coords[0]) if coords else 0)
+        return {f"{type(obj).__name__}": [f"float64, shape={shape}"]}
     elif isinstance(obj, Iterable) and not isinstance(obj, (str, bytes)):
         if level < limit:
             inner_structure = [struct(x, level + 1) for x in obj]
             if len(obj) > 3:
                 inner_structure = inner_structure[:3] + [f"...{len(obj)} total"]
             return {type(obj).__name__: inner_structure}
         else:
```

### Comparing `pyxtend-0.2.2/src/pyxtend.egg-info/PKG-INFO` & `pyxtend-0.3.0/src/pyxtend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtend
-Version: 0.2.2
+Version: 0.3.0
 Summary: Some functions for Python
 Home-page: https://github.com/jss367/pyxtend
 Author: Julius
 Author-email: julius.simonelli@gmail.com
 Project-URL: Bug Tracker, https://github.com/jss367/pyxtend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

