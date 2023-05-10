# Comparing `tmp/satanua-0.0.1.tar.gz` & `tmp/satanua-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satanua-0.0.1.tar", last modified: Wed May 10 17:15:59 2023, max compression
+gzip compressed data, was "satanua-0.0.2.tar", last modified: Wed May 10 17:22:47 2023, max compression
```

## Comparing `satanua-0.0.1.tar` & `satanua-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:15:59.865356 satanua-0.0.1/
--rw-rw-rw-   0        0        0     1065 2023-05-10 15:41:23.000000 satanua-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2020 2023-05-10 17:15:59.866377 satanua-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1492 2023-05-10 17:14:38.000000 satanua-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-10 15:42:37.000000 satanua-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      667 2023-05-10 17:15:59.868371 satanua-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 17:15:59.802165 satanua-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 17:15:59.841919 satanua-0.0.1/src/satanua/
--rw-rw-rw-   0        0        0      295 2023-05-10 17:02:01.000000 satanua-0.0.1/src/satanua/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-05-10 16:26:50.000000 satanua-0.0.1/src/satanua/connection_pin.py
--rw-rw-rw-   0        0        0      524 2023-05-10 16:09:10.000000 satanua-0.0.1/src/satanua/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-10 16:07:02.000000 satanua-0.0.1/src/satanua/enums.py
--rw-rw-rw-   0        0        0     1959 2023-05-10 16:23:44.000000 satanua-0.0.1/src/satanua/gate.py
--rw-rw-rw-   0        0        0     9371 2023-05-10 16:58:33.000000 satanua-0.0.1/src/satanua/gate_block.py
--rw-rw-rw-   0        0        0     1512 2023-05-10 16:27:09.000000 satanua-0.0.1/src/satanua/id_tracker.py
--rw-rw-rw-   0        0        0     1480 2023-05-10 16:25:20.000000 satanua-0.0.1/src/satanua/switch.py
--rw-rw-rw-   0        0        0      963 2023-05-10 16:59:53.000000 satanua-0.0.1/src/satanua/test.py
--rw-rw-rw-   0        0        0      496 2023-05-10 16:22:35.000000 satanua-0.0.1/src/satanua/wire.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:15:59.863839 satanua-0.0.1/src/satanua.egg-info/
--rw-rw-rw-   0        0        0     2020 2023-05-10 17:15:59.000000 satanua-0.0.1/src/satanua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-10 17:15:59.000000 satanua-0.0.1/src/satanua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:15:59.000000 satanua-0.0.1/src/satanua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 17:15:59.000000 satanua-0.0.1/src/satanua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 17:22:47.029750 satanua-0.0.2/
+-rw-rw-rw-   0        0        0     1065 2023-05-10 15:41:23.000000 satanua-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2019 2023-05-10 17:22:47.029750 satanua-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-05-10 17:19:59.000000 satanua-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-10 15:42:37.000000 satanua-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      667 2023-05-10 17:22:47.031749 satanua-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 17:22:46.939994 satanua-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 17:22:47.011717 satanua-0.0.2/src/satanua/
+-rw-rw-rw-   0        0        0      302 2023-05-10 17:22:07.000000 satanua-0.0.2/src/satanua/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-05-10 17:22:07.000000 satanua-0.0.2/src/satanua/connection_pin.py
+-rw-rw-rw-   0        0        0      524 2023-05-10 16:09:10.000000 satanua-0.0.2/src/satanua/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-10 16:07:02.000000 satanua-0.0.2/src/satanua/enums.py
+-rw-rw-rw-   0        0        0     1961 2023-05-10 17:22:09.000000 satanua-0.0.2/src/satanua/gate.py
+-rw-rw-rw-   0        0        0     9375 2023-05-10 17:22:09.000000 satanua-0.0.2/src/satanua/gate_block.py
+-rw-rw-rw-   0        0        0     1513 2023-05-10 17:22:10.000000 satanua-0.0.2/src/satanua/id_tracker.py
+-rw-rw-rw-   0        0        0     1482 2023-05-10 17:22:11.000000 satanua-0.0.2/src/satanua/switch.py
+-rw-rw-rw-   0        0        0      968 2023-05-10 17:22:12.000000 satanua-0.0.2/src/satanua/test.py
+-rw-rw-rw-   0        0        0      497 2023-05-10 17:22:14.000000 satanua-0.0.2/src/satanua/wire.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:22:47.028738 satanua-0.0.2/src/satanua.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-05-10 17:22:46.000000 satanua-0.0.2/src/satanua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-05-10 17:22:46.000000 satanua-0.0.2/src/satanua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:22:46.000000 satanua-0.0.2/src/satanua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 17:22:46.000000 satanua-0.0.2/src/satanua.egg-info/top_level.txt
```

### Comparing `satanua-0.0.1/LICENSE` & `satanua-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satanua-0.0.1/PKG-INFO` & `satanua-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satanua
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for converting logic formulas to .atanua files
 Home-page: https://github.com/YLashko/satanua/
 Author: Wym
 Author-email: dewreator2@gmail.com
 Project-URL: Bug Tracker, https://github.com/YLashko/satanua/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,15 @@
     coordinates = [0, 0]
 )
 decoder.build()
 ```
 `formulas`+`modes` in this example is the equivalent of
 
 ```math
-\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\
-OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
+\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\ OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
 
 ```
 
 
 You can then export the whole scene to .atanua using 
 ```python
 from satanua import render_all
```

### Comparing `satanua-0.0.1/README.md` & `satanua-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     coordinates = [0, 0]
 )
 decoder.build()
 ```
 `formulas`+`modes` in this example is the equivalent of
 
 ```math
-\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\
-OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
+\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\ OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
 
 ```
 
 
 You can then export the whole scene to .atanua using 
 ```python
 from satanua import render_all
```

### Comparing `satanua-0.0.1/setup.cfg` & `satanua-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6174 616e 7561 0d0a 7665 7273   = satanua..vers
-00000020: 696f 6e20 3d20 302e 302e 310d 0a61 7574  ion = 0.0.1..aut
+00000020: 696f 6e20 3d20 302e 302e 320d 0a61 7574  ion = 0.0.2..aut
 00000030: 686f 7220 3d20 5779 6d0d 0a61 7574 686f  hor = Wym..autho
 00000040: 725f 656d 6169 6c20 3d20 6465 7772 6561  r_email = dewrea
 00000050: 746f 7232 4067 6d61 696c 2e63 6f6d 0d0a  tor2@gmail.com..
 00000060: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000070: 6c69 6272 6172 7920 666f 7220 636f 6e76  library for conv
 00000080: 6572 7469 6e67 206c 6f67 6963 2066 6f72  erting logic for
 00000090: 6d75 6c61 7320 746f 202e 6174 616e 7561  mulas to .atanua
```

### Comparing `satanua-0.0.1/src/satanua/connection_pin.py` & `satanua-0.0.2/src/satanua/connection_pin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from constants import GRID_SIZE, SCENE_SIZE
-from wire import Wire
+from .constants import GRID_SIZE, SCENE_SIZE
+from .wire import Wire
 
 def _id(gate_a, gate_b):
     return f"{gate_a.id} {gate_b.id}"
 
 def rotate_and_mirror(x, y, rotate, mirror_x, mirror_y):
     for _ in range(rotate):
         x, y = SCENE_SIZE - y, x
```

### Comparing `satanua-0.0.1/src/satanua/constants.py` & `satanua-0.0.2/src/satanua/constants.py`

 * *Files identical despite different names*

### Comparing `satanua-0.0.1/src/satanua/gate.py` & `satanua-0.0.2/src/satanua/gate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from wire import Wire
-from constants import *
+from .wire import Wire
+from .constants import *
 
 def _id(gate_a, gate_b):
     return f"{gate_a.id} {gate_b.id}"
 
 def rotate_and_mirror(x, y, rotate, mirror_x, mirror_y):
     for _ in range(rotate):
         x, y = SCENE_SIZE - y, x
```

### Comparing `satanua-0.0.1/src/satanua/gate_block.py` & `satanua-0.0.2/src/satanua/gate_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from constants import *
-from gate import Gate
-from connection_pin import ConnectionPin
-from switch import Switch
+from .constants import *
+from .gate import Gate
+from .connection_pin import ConnectionPin
+from .switch import Switch
 
 def count_inputs(svf):
     return sum([sum([int(num != None) for num in row]) for row in svf])
 
 class GateBlock:
     def __init__(self, gates_type, coordinates, obj_stack, wire_stack, size=8, input_gates = None):
         self.size = size
```

### Comparing `satanua-0.0.1/src/satanua/id_tracker.py` & `satanua-0.0.2/src/satanua/id_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from constants import SCENE_SIZE
+from .constants import SCENE_SIZE
 
 
 def _id(gate_a, gate_b):
     return f"{gate_a.id} {gate_b.id}"
 
 def render_all(os, ws, rotate=0, mirror_x=False, mirror_y=False):
     return '<?xml version="1.0" ?>\n<Atanua Version="Atanua/Win32 1.3.141220 (debug) - Wym" ChipCount="5" WireCount="3" key="267" scale="16">\n' + \
```

### Comparing `satanua-0.0.1/src/satanua/switch.py` & `satanua-0.0.2/src/satanua/switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from constants import GRID_SIZE, SCENE_SIZE
-from wire import Wire
+from .constants import GRID_SIZE, SCENE_SIZE
+from .wire import Wire
 
 def _id(gate_a, gate_b):
     return f"{gate_a.id} {gate_b.id}"
 
 def rotate_and_mirror(x, y, rotate, mirror_x, mirror_y):
     for _ in range(rotate):
         x, y = SCENE_SIZE - y, x
```

### Comparing `satanua-0.0.1/src/satanua/test.py` & `satanua-0.0.2/src/satanua/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from gate import Gate
-from connection_pin import ConnectionPin
-from gate_block import GateBlock, SingleVarScheme, MultiVarScheme, Decoder
-from wire import Wire
-from id_tracker import WireStack, ObjStack, render_all
+from .gate import Gate
+from .connection_pin import ConnectionPin
+from .gate_block import GateBlock, SingleVarScheme, MultiVarScheme, Decoder
+from .wire import Wire
+from .id_tracker import WireStack, ObjStack, render_all
 
 
 class App:
     def __init__(self) -> None:
         self.ws = WireStack()
         self.os = ObjStack()
```

### Comparing `satanua-0.0.1/src/satanua.egg-info/PKG-INFO` & `satanua-0.0.2/src/satanua.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satanua
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for converting logic formulas to .atanua files
 Home-page: https://github.com/YLashko/satanua/
 Author: Wym
 Author-email: dewreator2@gmail.com
 Project-URL: Bug Tracker, https://github.com/YLashko/satanua/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,15 @@
     coordinates = [0, 0]
 )
 decoder.build()
 ```
 `formulas`+`modes` in this example is the equivalent of
 
 ```math
-\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\
-OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
+\displaylines{OutVal_1 = \overline{A}B\overline{C}+AC+A\overline{B}C \\ OutVal_2 = (\overline{A})*(A+\overline{B}+\overline{C})*(\overline{A}+\overline{B}+C)}
 
 ```
 
 
 You can then export the whole scene to .atanua using 
 ```python
 from satanua import render_all
```

