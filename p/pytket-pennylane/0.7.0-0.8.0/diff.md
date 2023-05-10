# Comparing `tmp/pytket_pennylane-0.7.0-py3-none-any.whl.zip` & `tmp/pytket_pennylane-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6659 bytes, number of entries: 9
--rw-r--r--  2.0 unx      168 b- defN 23-Jan-18 11:47 pytket/extensions/pennylane/__init__.py
--rw-r--r--  2.0 unx       72 b- defN 23-Jan-18 11:47 pytket/extensions/pennylane/_metadata.py
--rw-r--r--  2.0 unx     3007 b- defN 23-Jan-18 11:47 pytket/extensions/pennylane/pennylane_convert.py
--rw-r--r--  2.0 unx     6052 b- defN 23-Jan-18 11:47 pytket/extensions/pennylane/pytket_device.py
--rw-r--r--  2.0 unx     3846 b- defN 23-Jan-18 11:47 pytket_pennylane-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 11:47 pytket_pennylane-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 23-Jan-18 11:47 pytket_pennylane-0.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 11:47 pytket_pennylane-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      833 b- defN 23-Jan-18 11:47 pytket_pennylane-0.7.0.dist-info/RECORD
-9 files, 14160 bytes uncompressed, 5185 bytes compressed:  63.4%
+Zip file size: 10829 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      168 b- defN 23-May-10 14:28 pytket/extensions/pennylane/__init__.py
+-rw-r--r--  2.0 unx       72 b- defN 23-May-10 14:28 pytket/extensions/pennylane/_metadata.py
+-rw-r--r--  2.0 unx     3007 b- defN 23-May-10 14:28 pytket/extensions/pennylane/pennylane_convert.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-10 14:28 pytket/extensions/pennylane/pytket_device.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3868 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      931 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/RECORD
+10 files, 25637 bytes uncompressed, 9199 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: pytket/extensions/pennylane/pennylane_convert.py
 Comment: 
 
 Filename: pytket/extensions/pennylane/pytket_device.py
 Comment: 
 
-Filename: pytket_pennylane-0.7.0.dist-info/METADATA
+Filename: pytket_pennylane-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_pennylane-0.7.0.dist-info/WHEEL
+Filename: pytket_pennylane-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_pennylane-0.7.0.dist-info/entry_points.txt
+Filename: pytket_pennylane-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_pennylane-0.7.0.dist-info/top_level.txt
+Filename: pytket_pennylane-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytket_pennylane-0.7.0.dist-info/RECORD
+Filename: pytket_pennylane-0.8.0.dist-info/top_level.txt
+Comment: 
+
+Filename: pytket_pennylane-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/pennylane/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.7.0"
+__extension_version__ = "0.8.0"
 __extension_name__ = "pytket-pennylane"
```

## Comparing `pytket_pennylane-0.7.0.dist-info/METADATA` & `pytket_pennylane-0.8.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-pennylane
-Version: 0.7.0
+Version: 0.8.0
 Summary: Pytket extension and Pennylane plugin.
 Author: KN
 Author-email: seyon.sivarajah@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-pennylane/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-pennylane
 Project-URL: Tracker, https://github.com/CQCL/pytket-pennylane/issues
@@ -17,16 +17,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: pytket (~=1.11)
-Requires-Dist: pennylane (~=0.28.0)
+License-File: LICENSE
+Requires-Dist: pytket (~=1.15)
+Requires-Dist: pennylane (~=0.30.0)
 Requires-Dist: pytket-qiskit (~=0.32.0)
 
 # pytket-pennylane
 [Pytket](https://cqcl.github.io/pytket) extension and [PennyLane](https://github.com/PennyLaneAI/pennylane) plugin which allows pytket backends and compilation to be used as a PennyLane device.
 
 
 Pytket is a quantum SDK python package which provides state of the art compilation for quantum
```

## Comparing `pytket_pennylane-0.7.0.dist-info/RECORD` & `pytket_pennylane-0.8.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 pytket/extensions/pennylane/__init__.py,sha256=4cIexBGR7m8_2U2KXWkJT4zTtfc9bPLt62MksSAvWME,168
-pytket/extensions/pennylane/_metadata.py,sha256=OT5PRynaDP92hNCOJ02xfnpIHCPVhhS0ZPTXGdkrL4I,72
+pytket/extensions/pennylane/_metadata.py,sha256=Xr8uC51LDvEFVXfaEH-pm6Dz1VqnXmNzSNUWqKPT6OU,72
 pytket/extensions/pennylane/pennylane_convert.py,sha256=3wwmtxMGiWdJ0VzDgQeIelD4lLDfd0mZmwOP0IUybXw,3007
 pytket/extensions/pennylane/pytket_device.py,sha256=ie8DhpxYKRKswj0Mq7Eos0MqfqzrRmedBjligxy6l-g,6052
-pytket_pennylane-0.7.0.dist-info/METADATA,sha256=vuBGkgeLj7FMok879kc_krOPFqGZm8nui-UqnmGyYJs,3846
-pytket_pennylane-0.7.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pytket_pennylane-0.7.0.dist-info/entry_points.txt,sha256=QMxmLaiyW0CkB11ix3y_UssMos9bA3y6PmfwVLFvZM8,83
-pytket_pennylane-0.7.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_pennylane-0.7.0.dist-info/RECORD,,
+pytket_pennylane-0.8.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_pennylane-0.8.0.dist-info/METADATA,sha256=oS0ou9FcSF-O7CxcKWWqbXvUdk8FvN2imIxRhr72p30,3868
+pytket_pennylane-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_pennylane-0.8.0.dist-info/entry_points.txt,sha256=QMxmLaiyW0CkB11ix3y_UssMos9bA3y6PmfwVLFvZM8,83
+pytket_pennylane-0.8.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_pennylane-0.8.0.dist-info/RECORD,,
```

