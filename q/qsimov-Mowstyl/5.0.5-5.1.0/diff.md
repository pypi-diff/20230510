# Comparing `tmp/qsimov-Mowstyl-5.0.5.tar.gz` & `tmp/qsimov-Mowstyl-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsimov-Mowstyl-5.0.5.tar", last modified: Sun Jun 19 18:22:53 2022, max compression
+gzip compressed data, was "qsimov-Mowstyl-5.1.0.tar", last modified: Wed May 10 20:28:10 2023, max compression
```

## Comparing `qsimov-Mowstyl-5.0.5.tar` & `qsimov-Mowstyl-5.1.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.116357 qsimov-Mowstyl-5.0.5/
--rw-rw-rw-   0        0        0     1111 2020-08-24 08:47:52.000000 qsimov-Mowstyl-5.0.5/LICENSE
--rw-rw-rw-   0        0        0      855 2022-06-19 18:22:53.116357 qsimov-Mowstyl-5.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3060 2022-04-06 19:39:51.000000 qsimov-Mowstyl-5.0.5/README.md
--rw-rw-rw-   0        0        0      110 2021-07-23 13:21:51.000000 qsimov-Mowstyl-5.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.091359 qsimov-Mowstyl-5.0.5/qsimov/
--rw-rw-rw-   0        0        0      455 2022-04-19 11:09:10.000000 qsimov-Mowstyl-5.0.5/qsimov/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.095358 qsimov-Mowstyl-5.0.5/qsimov/connectors/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:13:55.000000 qsimov-Mowstyl-5.0.5/qsimov/connectors/__init__.py
--rw-rw-rw-   0        0        0      897 2022-05-24 09:37:52.000000 qsimov-Mowstyl-5.0.5/qsimov/connectors/drewom.py
--rw-rw-rw-   0        0        0      226 2021-02-27 01:28:39.000000 qsimov-Mowstyl-5.0.5/qsimov/connectors/forestapi.py
--rw-rw-rw-   0        0        0    13971 2022-05-24 22:15:38.000000 qsimov-Mowstyl-5.0.5/qsimov/connectors/parser.py
--rw-rw-rw-   0        0        0     8107 2022-05-21 19:50:42.000000 qsimov-Mowstyl-5.0.5/qsimov/connectors/qsimovapi.py
--rw-rw-rw-   0        0        0     3616 2022-04-19 11:09:36.000000 qsimov-Mowstyl-5.0.5/qsimov/qsimov.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.098359 qsimov-Mowstyl-5.0.5/qsimov/samples/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:14:03.000000 qsimov-Mowstyl-5.0.5/qsimov/samples/__init__.py
--rw-rw-rw-   0        0        0     2631 2022-05-21 18:59:40.000000 qsimov-Mowstyl-5.0.5/qsimov/samples/djcircuit.py
--rw-rw-rw-   0        0        0      736 2022-05-24 22:21:45.000000 qsimov-Mowstyl-5.0.5/qsimov/samples/fourier.py
--rw-rw-rw-   0        0        0     3986 2021-11-05 11:42:46.000000 qsimov-Mowstyl-5.0.5/qsimov/samples/state_gate.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.109359 qsimov-Mowstyl-5.0.5/qsimov/structures/
--rw-rw-rw-   0        0        0        0 2021-11-07 14:14:09.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/__init__.py
--rw-rw-rw-   0        0        0    12917 2021-11-08 00:37:00.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/funmatrix.py
--rw-rw-rw-   0        0        0      126 2022-02-10 11:19:15.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qbase.py
--rw-rw-rw-   0        0        0     5260 2022-05-21 18:58:15.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qcircuit.py
--rw-rw-rw-   0        0        0      527 2022-05-22 18:40:22.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qdesign.py
--rw-rw-rw-   0        0        0     4255 2022-05-21 18:10:45.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qgate.py
--rw-rw-rw-   0        0        0    13622 2022-05-22 18:04:38.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qregistry.py
--rw-rw-rw-   0        0        0     6292 2022-05-22 18:16:19.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qstructure.py
--rw-rw-rw-   0        0        0    17690 2022-06-19 18:22:37.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/qsystem.py
--rw-rw-rw-   0        0        0     4842 2022-05-24 17:47:37.000000 qsimov-Mowstyl-5.0.5/qsimov/structures/simple_gate.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.111361 qsimov-Mowstyl-5.0.5/qsimov/utils/
--rw-rw-rw-   0        0        0        0 2022-02-10 11:50:33.000000 qsimov-Mowstyl-5.0.5/qsimov/utils/__init__.py
--rw-rw-rw-   0        0        0     5577 2022-02-10 15:44:35.000000 qsimov-Mowstyl-5.0.5/qsimov/utils/bloch.py
-drwxrwxrwx   0        0        0        0 2022-06-19 18:22:53.115358 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/
--rw-rw-rw-   0        0        0      855 2022-06-19 18:22:52.000000 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2022-06-19 18:22:53.000000 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-19 18:22:52.000000 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-06-19 18:22:52.000000 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-06-19 18:22:52.000000 qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-19 18:22:53.116357 qsimov-Mowstyl-5.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1403 2022-06-19 18:09:31.000000 qsimov-Mowstyl-5.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.102136 qsimov-Mowstyl-5.1.0/
+-rw-rw-rw-   0        0        0     1111 2020-08-24 08:47:52.000000 qsimov-Mowstyl-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0      855 2023-05-10 20:28:10.102136 qsimov-Mowstyl-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3786 2023-02-17 14:46:14.000000 qsimov-Mowstyl-5.1.0/README.md
+-rw-rw-rw-   0        0        0      110 2021-07-23 13:21:51.000000 qsimov-Mowstyl-5.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.077136 qsimov-Mowstyl-5.1.0/qsimov/
+-rw-rw-rw-   0        0        0      455 2023-04-22 14:30:17.000000 qsimov-Mowstyl-5.1.0/qsimov/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.080136 qsimov-Mowstyl-5.1.0/qsimov/connectors/
+-rw-rw-rw-   0        0        0        0 2021-11-07 14:13:55.000000 qsimov-Mowstyl-5.1.0/qsimov/connectors/__init__.py
+-rw-rw-rw-   0        0        0      897 2022-05-24 09:37:52.000000 qsimov-Mowstyl-5.1.0/qsimov/connectors/drewom.py
+-rw-rw-rw-   0        0        0      226 2021-02-27 01:28:39.000000 qsimov-Mowstyl-5.1.0/qsimov/connectors/forestapi.py
+-rw-rw-rw-   0        0        0    11402 2023-02-09 15:30:43.000000 qsimov-Mowstyl-5.1.0/qsimov/connectors/parser.py
+-rw-rw-rw-   0        0        0     8107 2022-05-21 19:50:42.000000 qsimov-Mowstyl-5.1.0/qsimov/connectors/qsimovapi.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.082136 qsimov-Mowstyl-5.1.0/qsimov/cores/
+-rw-rw-rw-   0        0        0        0 2021-11-07 14:13:55.000000 qsimov-Mowstyl-5.1.0/qsimov/cores/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-22 14:33:19.000000 qsimov-Mowstyl-5.1.0/qsimov/cores/bdoki.py
+-rw-rw-rw-   0        0        0     3616 2022-04-19 11:09:36.000000 qsimov-Mowstyl-5.1.0/qsimov/qsimov.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.085138 qsimov-Mowstyl-5.1.0/qsimov/samples/
+-rw-rw-rw-   0        0        0        0 2021-11-07 14:14:03.000000 qsimov-Mowstyl-5.1.0/qsimov/samples/__init__.py
+-rw-rw-rw-   0        0        0     2631 2022-05-21 18:59:40.000000 qsimov-Mowstyl-5.1.0/qsimov/samples/djcircuit.py
+-rw-rw-rw-   0        0        0      736 2022-05-24 22:21:45.000000 qsimov-Mowstyl-5.1.0/qsimov/samples/fourier.py
+-rw-rw-rw-   0        0        0     3986 2021-11-05 11:42:46.000000 qsimov-Mowstyl-5.1.0/qsimov/samples/state_gate.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.095137 qsimov-Mowstyl-5.1.0/qsimov/structures/
+-rw-rw-rw-   0        0        0        0 2021-11-07 14:14:09.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/__init__.py
+-rw-rw-rw-   0        0        0    12917 2021-11-08 00:37:00.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/funmatrix.py
+-rw-rw-rw-   0        0        0      126 2022-02-10 11:19:15.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qbase.py
+-rw-rw-rw-   0        0        0     7264 2023-05-10 19:59:59.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qcircuit.py
+-rw-rw-rw-   0        0        0      527 2022-05-22 18:40:22.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qdesign.py
+-rw-rw-rw-   0        0        0     6420 2023-05-10 20:01:20.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qgate.py
+-rw-rw-rw-   0        0        0    15880 2023-05-10 19:57:04.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qregistry.py
+-rw-rw-rw-   0        0        0     6829 2023-05-10 19:24:28.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qstructure.py
+-rw-rw-rw-   0        0        0    18742 2023-05-10 20:08:40.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/qsystem.py
+-rw-rw-rw-   0        0        0     5160 2023-05-10 20:27:49.000000 qsimov-Mowstyl-5.1.0/qsimov/structures/simple_gate.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.097136 qsimov-Mowstyl-5.1.0/qsimov/utils/
+-rw-rw-rw-   0        0        0        0 2022-02-10 11:50:33.000000 qsimov-Mowstyl-5.1.0/qsimov/utils/__init__.py
+-rw-rw-rw-   0        0        0     5577 2022-02-10 15:44:35.000000 qsimov-Mowstyl-5.1.0/qsimov/utils/bloch.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:10.101136 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/
+-rw-rw-rw-   0        0        0      855 2023-05-10 20:28:10.000000 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      917 2023-05-10 20:28:10.000000 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 20:28:10.000000 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-10 20:28:10.000000 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 20:28:10.000000 qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 20:28:10.102136 qsimov-Mowstyl-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-05-10 19:21:49.000000 qsimov-Mowstyl-5.1.0/setup.py
```

### Comparing `qsimov-Mowstyl-5.0.5/LICENSE` & `qsimov-Mowstyl-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/PKG-INFO` & `qsimov-Mowstyl-5.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsimov-Mowstyl
-Version: 5.0.5
+Version: 5.1.0
 Summary: QSimov Quantum computer simulator
 Home-page: https://github.com/Mowstyl/QSimov
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: quantum
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qsimov-Mowstyl-5.0.5/README.md` & `qsimov-Mowstyl-5.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # QSimov
 
-This is the quantum framework QSimov, written in Python.
+QSimov is a quantum computing toolkit developed in Python, initially as an End Degree Project at UCLM. It allows the user to work both at a low level using quantum gates and registers and at a higher level using the design tools. It has been created in such a way that it allows an almost immediate translation from the circuit diagram to the code necessary to execute it.
+From the moment of its creation, QSimov has been focused on being able to be used in learning and not on big computers and datacenters. For this reason, the simplicity of use and the low hardware requirements have always been what have guided its development. It is capable of running up to 29 entangled qubits on a laptop with 16 GB of RAM and several thousand non-entangled qubits under the same conditions.
 
 ## Getting Started
 
 By following this instructions you will have a working binary.
 
 ### Prerequisites
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/connectors/drewom.py` & `qsimov-Mowstyl-5.1.0/qsimov/connectors/drewom.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/connectors/qsimovapi.py` & `qsimov-Mowstyl-5.1.0/qsimov/connectors/qsimovapi.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/qsimov.py` & `qsimov-Mowstyl-5.1.0/qsimov/qsimov.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/samples/djcircuit.py` & `qsimov-Mowstyl-5.1.0/qsimov/samples/djcircuit.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/samples/fourier.py` & `qsimov-Mowstyl-5.1.0/qsimov/samples/fourier.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/samples/state_gate.py` & `qsimov-Mowstyl-5.1.0/qsimov/samples/state_gate.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/funmatrix.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/funmatrix.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/qdesign.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/qdesign.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/qregistry.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/qregistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,56 +3,74 @@
 Data Structures:
     QRegistry: Quantum Registry, base of all quantum related operations
 
 Functions:
     superposition: join two registries into one by calculating tensor product.
 """
 import numpy as np
+import sympy as sp
 
+from sympy.functions.elementary.complexes import arg
 from qsimov.structures.funmatrix import Funmatrix
 from qsimov.structures.simple_gate import SimpleGate
 from qsimov.structures.qstructure import QStructure, _get_op_data, \
                                          _get_qubit_set, _get_key_with_defaults
 from qsimov.connectors.qsimovapi import apply_design
 
 
 class QRegistry(QStructure):
     """Quantum Registry, base of all quantum related operations."""
 
-    def __init__(self, num_qubits, doki=None, verbose=False):
+    def __init__(self, num_qubits, data=None, doki=None, verbose=False):
         """Initialize QRegistry to state 0.
 
         num_qubits -> number of QuBits in the registry.
         """
         if doki is None:
             import doki
         self.doki = doki
-        if num_qubits is not None:
-            if num_qubits > 0:
-                self.reg = self.doki.registry_new(num_qubits, verbose)
-                self.qubit_map = {i: i for i in range(num_qubits)}
-                self.classic_vals = {}
-                self.num_qubits = num_qubits
-                self.num_bits = 0
-                self.size = 2**num_qubits
+        if data is None:
+            if num_qubits is not None:
+                if num_qubits > 0:
+                    self.reg = self.doki.registry_new(num_qubits, verbose)
+                    self.qubit_map = {i: i for i in range(num_qubits)}
+                    self.classic_vals = {}
+                    self.num_qubits = num_qubits
+                    self.num_bits = 0
+                    self.size = 2**num_qubits
+                else:
+                    raise ValueError("num_qubits must be greater than 0")
             else:
-                raise ValueError("num_qubits must be greater than 0")
+                self.reg = None
+                self.num_qubits = 0
+                self.num_bits = 0
+                self.size = 0
+                self.qubit_map = {}
+                self.classic_vals = {}
         else:
-            self.reg = None
-            self.num_qubits = 0
-            self.num_bits = 0
-            self.size = 0
-            self.qubit_map = {}
-            self.classic_vals = {}
+            self.reg = self.doki.registry_new_data(data["num_qubits"], data["reg"], verbose)
+            self.num_qubits = data["num_qubits"]
+            self.num_bits = data["num_bits"]
+            self.size = data["size"]
+            self.qubit_map = data["qubit_map"]
+            self.classic_vals = data["classic_vals"]
         self.verbose = verbose
 
     def __del__(self):
         """Clean after deletion."""
         self.free()
 
+    def get_data(self):
+        return {"reg": self.get_state(),
+                "num_qubits": self.num_qubits,
+                "num_bits": self.num_bits,
+                "size": self.size,
+                "qubit_map": self.qubit_map,
+                "classic_vals": self.classic_vals}
+
     def get_classic(self, id):
         """Return classic bit value (if qubit has been measured)."""
         if id in self.classic_vals:
             return self.classic_vals[id]
         return None
 
     def free(self):
@@ -122,28 +140,43 @@
                                 else final_mess[id]
                                 for id in range(num_total)
                                 if id not in new_reg.qubit_map}
 
         return (new_reg, final_mess)
 
     def apply_gate(self, gate, targets=None, controls=None, anticontrols=None,
-                   num_threads=-1):
+                   num_threads=-1, target=None, control=None, anticontrol=None):
         """Add specified gate to this QGate.
 
         Positional arguments:
             gate: string with the name of the gate to apply, or a QGate
         Keyworded arguments:
             targets: id or list of ids of the qubits the gate will target
             controls: id or set of ids of the qubit that will act as controls
             anticontrols: id or set of ids of the qubit that will act as
                          anticontrols
             num_threads: number of threads to use
         Return:
             A new QRegistry
         """
+        if target is not None:
+            print("[WARNING] target keyworded argument is deprecated. Please use targets instead")
+            if targets is not None:
+                raise ValueError("target argument can't be set alongside targets")
+            targets = target
+        if control is not None:
+            print("[WARNING] control keyworded argument is deprecated. Please use controls instead")
+            if controls is not None:
+                raise ValueError("control argument can't be set alongside controls")
+            controls = control
+        if anticontrol is not None:
+            print("[WARNING] anticontrol keyworded argument is deprecated. Please use anticontrols instead")
+            if anticontrols is not None:
+                raise ValueError("anticontrol argument can't be set alongside anticontrols")
+            anticontrols = anticontrol
         if not np.allclose(num_threads % 1, 0):
             raise ValueError("num_threads must be an integer")
         num_threads = int(num_threads)
         num_qubits = self.num_qubits + self.num_bits
         op_data = _get_op_data(num_qubits, 0, gate, targets, None, None,
                                controls, anticontrols, None, None)
         gate = op_data["gate"]
@@ -162,15 +195,18 @@
         controls -= classic_controls
         controls -= classic_anticontrols
         new_reg = None
         if type(gate) == SimpleGate:
             aux_targets = [self.qubit_map[id] for id in targets]
             aux_controls = {self.qubit_map[id] for id in controls}
             aux_anticontrols = {self.qubit_map[id] for id in anticontrols}
-            doki_reg = self.doki.registry_apply(self.reg, gate.gate,
+            auxg = gate.gate
+            if hasattr(self.doki, "BRegistry"):
+                auxg = gate.matrix
+            doki_reg = self.doki.registry_apply(self.reg, auxg,
                                                 aux_targets, aux_controls,
                                                 aux_anticontrols,
                                                 num_threads, self.verbose)
             new_reg = QRegistry(None, doki=self.doki)
             new_reg.reg = doki_reg
             new_reg.num_qubits = self.num_qubits
             new_reg.num_bits = self.num_bits
@@ -240,26 +276,38 @@
                     entropy += p * np.log(p)
                 elif type(base) == int or type(base) == float:
                     entropy += p * np.log(p)/np.log(base)
         return -entropy
 
     def get_bloch_coords(self, key=None):
         """Get the polar coordinates of ONE qubit in the bloch sphere."""
+        if hasattr(self.doki, "BRegistry"):
+            start, stop, step = _get_key_with_defaults(key, self.num_qubits,
+                                                       0, self.num_qubits, 1)
+            ids = [id for id in range(start, stop, step)]
+            coords = [(sp.acos(self.reg.r[id].v[2, 0]),
+                       sp.atan2(self.reg.r[id].v[1, 0], self.reg.r[id].v[0, 0]))
+                      if self.reg.r[id].v[0, 0] != 0
+                      else (sp.acos(self.reg.r[id].v[2, 0]), 0)
+                      for id in ids]
+            return coords
         if self.num_qubits != 1:
             raise NotImplementedError("Bloch sphere is only supported for " +
                                       "1 qubit registries")
         if key is not None and key >= self.get_num_qubits():
             raise ValueError(f"Qubit {key} is not in this registry")
         if key is not None and key in self.classic_vals:
             raise ValueError("That is a classical bit, not a qubit")
         state = self.get_state(canonical=True)
         cos_t2 = state[0].real
         sin_t2 = abs(state[1])
-        phi = np.angle(state[1])
-        theta = np.arctan2(sin_t2, cos_t2) * 2
+        phi = arg(state[1])
+        if phi == sp.nan:
+            phi = 0
+        theta = sp.atan2(sin_t2, cos_t2) * 2
         if theta < 0:
             theta += 2 * np.pi
         if phi < 0:
             phi += 2 * np.pi
         return (theta, phi)
 
     def bra(self):
@@ -280,20 +328,14 @@
         if id in self.classic_vals:
             return self.classic_vals[id]
         for i in range(self.get_num_qubits(), id):
             if i in self.classic_vals:
                 id -= 1
         return self.doki.registry_prob(self.reg, id, num_threads, self.verbose)
 
-    def bloch(self, key=None):
-        """Return matplotlib bloch sphere."""
-        theta, phi = self.get_bloch_coords(key=key)
-        from qsimov.utils.bloch import draw_bloch_sphere
-        return draw_bloch_sphere(theta, phi)
-
 
 def superposition(a, b, num_threads=-1, verbose=False):
     """Join two registries into one by calculating tensor product."""
     if not np.allclose(num_threads % 1, 0):
         raise ValueError("num_threads must be an integer")
     num_threads = int(num_threads)
     doki_reg = None
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/qstructure.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/qstructure.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Iterable
 from qsimov.structures.qbase import QBase
 from qsimov.structures.simple_gate import SimpleGate
 
 
 class QStructure(QBase):
     @abstractmethod
-    def __init__(self, num_qubits, doki=None, verbose=False):
+    def __init__(self, num_qubits, data=None, doki=None, verbose=False):
         pass
 
     @abstractmethod
     def apply_gate(self, gate, targets=None, controls=None, anticontrols=None,
                    num_threads=-1):
         pass
 
@@ -28,14 +28,18 @@
         pass
 
     @abstractmethod
     def get_state(self, key=None, canonical=False):
         pass
 
     @abstractmethod
+    def get_data(self):
+        pass
+
+    @abstractmethod
     def get_classic(self, id):
         pass
 
     @abstractmethod
     def clone(self, num_threads=-1):
         pass
 
@@ -43,17 +47,26 @@
     def free(self):
         pass
 
     @abstractmethod
     def get_bloch_coords(self, key=None):
         pass
 
-    @abstractmethod
     def bloch(self, key=None):
-        pass
+        """Return matplotlib bloch sphere."""
+        all_coords = self.get_bloch_coords(key=key)
+        if type(all_coords) != list:
+            all_coords = [all_coords]
+        from qsimov.utils.bloch import draw_bloch_sphere
+        figs = [draw_bloch_sphere(float(coords[0]), float(coords[1])) if coords is not None
+                else None
+                for coords in all_coords]
+        if key is not None and type(key) != slice:
+            figs = figs[0]
+        return figs
 
 
 def _get_op_data(num_qubits, num_bits, gate, targets, c_targets, outputs,
                  controls, anticontrols, c_controls, c_anticontrols,
                  empty=False):
     """Do basic error checking for arguments and return them."""
     targets = _get_qubit_set(num_qubits, targets, True, "targets")
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/qsystem.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/qsystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,46 @@
                                         _get_op_data, _get_key_with_defaults
 from qsimov.structures.qregistry import QRegistry, superposition
 
 
 class QSystem(QStructure):
     """Quantum System, preferred over QRegistry (can save a lot of space)."""
 
-    def __init__(self, num_qubits, doki=None, verbose=False):
+    def __init__(self, num_qubits, data=None, doki=None, verbose=False):
         """Initialize QSystem to state 0.
 
         num_qubits -> number of QuBits in the system.
         """
         if doki is None:
             import doki
         self.doki = doki
-        if num_qubits is None:
-            self.regs = None
-            self.qubitMap = None
-            self.num_qubits = 0
+        if data is None:
+            if num_qubits is None:
+                self.regs = None
+                self.qubitMap = None
+                self.num_qubits = 0
+            else:
+                self.regs = [[QRegistry(1, doki=self.doki), [id]]
+                             for id in range(num_qubits)]
+                self.qubitMap = {id: id for id in range(num_qubits)}
+                self.num_qubits = num_qubits
         else:
-            self.regs = [[QRegistry(1, doki=self.doki), [id]]
-                         for id in range(num_qubits)]
-            self.qubitMap = {id: id for id in range(num_qubits)}
-            self.num_qubits = num_qubits
+            self.regs = [[QRegistry(None, data=data["regs"][i][0], doki=self.doki),
+                          data["regs"][i][1]]
+                         for i in range(len(data["regs"]))]
+            self.qubitMap = data["qubit_map"]
+            self.num_qubits = data["num_qubits"]
         self.verbose = verbose
 
+    def get_data(self):
+        return {"regs": [[self.regs[i][0].get_data(), self.regs[i][1]]
+                         for i in range(len(self.regs))],
+                "qubit_map": self.qubitMap,
+                "num_qubits": self.num_qubits}
+
     def free(self, deep=False):
         """Release memory held by the QSystem."""
         if self.regs is not None:
             if deep:
                 for reg, _ in self.regs:
                     if isinstance(reg, QRegistry):
                         reg.free()
@@ -236,29 +249,44 @@
         return self.as_qregistry().get_state(key=key, canonical=canonical)
 
     def get_classic(self, id):
         """Return classic bit value."""
         return None
 
     def apply_gate(self, gate, targets=None, controls=None, anticontrols=None,
-                   num_threads=-1, deep=False):
+                   num_threads=-1, deep=False, target=None, control=None, anticontrol=None):
         """Apply specified gate to specified qubit with specified controls.
 
         Positional arguments:
             gate: string with the name of the gate to apply, or a QGate
         Keyworded arguments:
             targets: id of the least significant qubit the gate will target
             controls: id or list of ids of the qubit that will act as
                      controls
             anticontrols: id or list of ids of the qubit that will act as
                          anticontrols
             num_threads: number of threads to use
             optimize: only for QGates. Whether to use optimized lines or
                       user defined lines
         """
+        if target is not None:
+            print("[WARNING] target keyworded argument is deprecated. Please use targets instead")
+            if targets is not None:
+                raise ValueError("target argument can't be set alongside targets")
+            targets = target
+        if control is not None:
+            print("[WARNING] control keyworded argument is deprecated. Please use controls instead")
+            if controls is not None:
+                raise ValueError("control argument can't be set alongside controls")
+            controls = control
+        if anticontrol is not None:
+            print("[WARNING] anticontrol keyworded argument is deprecated. Please use anticontrols instead")
+            if anticontrols is not None:
+                raise ValueError("anticontrol argument can't be set alongside anticontrols")
+            anticontrols = anticontrol
         if not np.allclose(num_threads % 1, 0):
             raise ValueError("num_threads must be an integer")
         num_threads = int(num_threads)
         num_qubits = self.get_num_qubits()
         op_data = _get_op_data(num_qubits, 0, gate, targets, None, None,
                                controls, anticontrols, None, None)
         gate = op_data["gate"]
@@ -367,27 +395,14 @@
                 coords[i] = reg.get_bloch_coords(new_id)
             except Exception:
                 pass
         if key is not None and type(key) != slice:
             coords = coords[0]
         return coords
 
-    def bloch(self, key=None):
-        """Return matplotlib bloch sphere."""
-        all_coords = self.get_bloch_coords(key=key)
-        if type(all_coords) != list:
-            all_coords = [all_coords]
-        from qsimov.utils.bloch import draw_bloch_sphere
-        figs = [draw_bloch_sphere(coords[0], coords[1]) if coords is not None
-                else None
-                for coords in all_coords]
-        if key is not None and type(key) != slice:
-            figs = figs[0]
-        return figs
-
 
 def join_systems(most, least, deep=False):
     """Return a system that contains both a and b systems."""
     res = QSystem(None, doki=most.doki)
     res.regs = []
     res.qubitMap = {}
     exception = None
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/structures/simple_gate.py` & `qsimov-Mowstyl-5.1.0/qsimov/structures/simple_gate.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,44 +5,47 @@
 
 Functions:
     add_gate: adds a gate to the list of available gates.
 """
 import doki
 import numpy as np
 import qsimov.connectors.parser as prs
-from qsimov.structures.qbase import QBase
+import sympy as sp
 
 from collections.abc import Iterable
+from qsimov.structures.qbase import QBase
+from sympy.matrices import Matrix
+from sympy.codegen.cfunctions import log2
+from sympy.physics.quantum.dagger import Dagger
 
 
 class SimpleGate(QBase):
     """Quantum gate with its associated matrix."""
 
     def __init__(self, gate_string):
         """Load a gate that is in the list of gates."""
         name, args, invert, self_invert = prs.get_gate_data(gate_string)
-        aux_matrix = _get_gate_matrix(name, args, invert, self_invert)
-        self.matrix = np.array(aux_matrix, dtype=complex)
+        self.matrix = _get_gate_matrix(name, args, self_invert)
         if self.matrix.shape[0] != self.matrix.shape[1]:
             raise ValueError("Not a square matrix")
-        self.num_qubits = int(np.log2(self.matrix.shape[0]))
+        self.num_qubits = int(log2(self.matrix.shape[0]))
         if 2**self.num_qubits != self.matrix.shape[0]:
             raise ValueError("Shape must be 2^n x 2^n. n = number of qubits")
-        if self_invert:
+        inverse = self.matrix
+        if not self_invert:
             inverse = self.matrix
-        else:
-            inverse = self.matrix.conj().T
-        identity = np.dot(self.matrix, inverse)
-        identity = np.exp(-1j * np.angle(identity[0, 0])) * identity
-        if not np.allclose(identity,
-                           np.eye(2**self.num_qubits, dtype=complex)):
-            raise ValueError("Failed testing inverse")
+            if isinstance(self.matrix, Matrix):
+                inverse = Dagger(self.matrix)
+            else:
+                inverse = self.matrix.conj().T
+        _check_inverse(gate_string, self.matrix, inverse)
         if invert:
             self.matrix = inverse
-        self.gate = doki.gate_new(self.num_qubits, self.matrix.tolist(), False)
+        aux = np.array(self.matrix).astype(complex)
+        self.gate = doki.gate_new(self.num_qubits, aux.tolist(), False)
         self._str = name
         if args is not None:
             if prs._gate_data[name][2]:  # has_invert_arg
                 args = args[:-1]
             self._str += "(" + ",".join([str(arg) for arg in args]) + ")"
         if invert and not self_invert:
             self._str += "-1"
@@ -77,51 +80,63 @@
         if gate_str[-2:] == "-1":
             gate_str = gate_str[:-2]
         else:
             gate_str += "-1"
         return SimpleGate(gate_str)
 
 
-def _get_gate_matrix(name, args, invert, self_invert):
+def _check_inverse(name, matrix, inverse):
+    got = None
+    if isinstance(matrix, Matrix):
+        got = np.array(matrix @ inverse).astype(complex)
+        '''
+        if not ex.equals(got) and not ex.equals(sp.N(got)):
+            print("Expected:", ex)
+            print("Got:", got)
+            print("Got:", sp.simplify(got))
+            print(ex.equals(got))
+            print([[ex[i, j].equals(got[i, j]) for j in range(ex.shape[1])] for i in range(ex.shape[0])])
+            print(sp.N(got))
+            print(ex.equals(sp.N(got)))
+            raise ValueError("Failed testing inverse of " + name)
+        '''
+    else:
+        got = np.dot(matrix, inverse)
+    ex = np.eye(matrix.shape[0], dtype=complex)
+    if not np.allclose(got, ex):
+        raise ValueError("Failed testing inverse of " + name)
+
+
+def _get_gate_matrix(name, args, self_invert):
     """Get gate matrix from parser's get_gate_data info."""
     gate_function = prs._gate_func[name]
-    aux_matrix = None
+    matrix = None
     if type(args) != str and isinstance(args, Iterable):
-        aux_matrix = gate_function(*args)
+        matrix = gate_function(*args)
     elif args is not None:
-        aux_matrix = gate_function(args)
+        matrix = gate_function(args)
     else:
-        aux_matrix = gate_function()
-    if not isinstance(aux_matrix, list):
-        # numpy array to list
-        if (callable(getattr(aux_matrix, "tolist", None))):
-            aux_matrix = aux_matrix.tolist()
-        # scipy sparse matrix to numpy array
-        elif (callable(getattr(aux_matrix, "toarray", None))):
-            aux_matrix = aux_matrix.toarray()
-            # numpy array to list
-            if (callable(getattr(aux_matrix, "tolist", None))):
-                aux_matrix = aux_matrix.tolist()
-        elif isinstance(aux_matrix, Iterable) and \
-                all(isinstance(row, Iterable) for row in aux_matrix):
-            aux_matrix = [[elem for elem in row] for row in aux_matrix]
-    return aux_matrix
+        matrix = gate_function()
+
+    return Matrix(matrix)
 
 
-def add_gate(name, funct, min_args, max_args, has_invert_arg=False,
+def add_gate(name, funct, min_args, max_args, has_invert_arg=None,
              is_own_inverse=False, aliases=[], overwrite=False):
     """Add specified gate to the list of available gates."""
+    if has_invert_arg is not None:
+        print("[WARNING] has_invert_arg keyworded argument has been deprecated, and will be removed. Currently it does nothing.")
     if name in prs._gate_func and not overwrite:
         raise ValueError(name + " gate has already been defined. " +
                          "Set overwrite=True if you want to overwrite it.")
     aliases.append(name)
     aliases = {alias.lower() for alias in aliases}
     for alias in aliases:
         if alias in prs._gate_alias and prs._gate_alias[alias] != name:
             raise ValueError("Alias " + alias + " for gate " + name +
                              " is in use by gate " + prs._gate_alias[alias] +
                              ". Either remove this alias or modify the older" +
                              " gate.")
     prs._gate_func[name] = funct
-    prs._gate_data[name] = (min_args, max_args, has_invert_arg, is_own_inverse)
+    prs._gate_data[name] = (min_args, max_args, is_own_inverse)
     for alias in aliases:
         prs._gate_alias[alias.lower()] = name
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov/utils/bloch.py` & `qsimov-Mowstyl-5.1.0/qsimov/utils/bloch.py`

 * *Files identical despite different names*

### Comparing `qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/PKG-INFO` & `qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsimov-Mowstyl
-Version: 5.0.5
+Version: 5.1.0
 Summary: QSimov Quantum computer simulator
 Home-page: https://github.com/Mowstyl/QSimov
 Author: Hernán Indíbil de la Cruz Calvo
 Author-email: HernanIndibil.LaCruz@alu.uclm.es
 License: MIT
 Keywords: quantum
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qsimov-Mowstyl-5.0.5/qsimov_Mowstyl.egg-info/SOURCES.txt` & `qsimov-Mowstyl-5.1.0/qsimov_Mowstyl.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 qsimov/__init__.py
 qsimov/qsimov.py
 qsimov/connectors/__init__.py
 qsimov/connectors/drewom.py
 qsimov/connectors/forestapi.py
 qsimov/connectors/parser.py
 qsimov/connectors/qsimovapi.py
+qsimov/cores/__init__.py
+qsimov/cores/bdoki.py
 qsimov/samples/__init__.py
 qsimov/samples/djcircuit.py
 qsimov/samples/fourier.py
 qsimov/samples/state_gate.py
 qsimov/structures/__init__.py
 qsimov/structures/funmatrix.py
 qsimov/structures/qbase.py
```

### Comparing `qsimov-Mowstyl-5.0.5/setup.py` & `qsimov-Mowstyl-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 def main():
     """Code to be executed on install."""
     setup(
         name="qsimov-Mowstyl",
-        version="5.0.5",
+        version="5.1.0",
         author="Hernán Indíbil de la Cruz Calvo",
         author_email="HernanIndibil.LaCruz@alu.uclm.es",
         license="MIT",
         packages=find_packages(include=['qsimov', 'qsimov.*']),
         url="https://github.com/Mowstyl/QSimov",
         description="QSimov Quantum computer simulator",
         long_description="QSimov is a quantum computer simulator based on " +
@@ -26,14 +26,14 @@
             'Topic :: Scientific/Engineering :: Mathematics',
             'Topic :: Software Development :: Libraries :: Python Modules',
         ],
         keywords="quantum",
         install_requires=[
             "numpy>=1.21",
             "matplotlib>=3.5.1",
-            "doki-Mowstyl>=1.3.2"
+            "doki-Mowstyl>=1.4.0"
         ]
     )
 
 
 if __name__ == "__main__":
     main()
```

