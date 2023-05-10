# Comparing `tmp/datana-0.3.1.0.tar.gz` & `tmp/datana-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datana-0.3.1.0.tar", last modified: Fri Feb 24 11:52:25 2023, max compression
+gzip compressed data, was "datana-0.3.1.2.tar", last modified: Wed May 10 13:01:17 2023, max compression
```

## Comparing `datana-0.3.1.0.tar` & `datana-0.3.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 11:52:25.490229 datana-0.3.1.0/
--rw-rw-rw-   0        0        0      379 2023-02-24 11:52:25.489230 datana-0.3.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-24 11:52:25.471383 datana-0.3.1.0/datana/
--rw-rw-rw-   0        0        0       25 2022-09-09 06:43:52.000000 datana-0.3.1.0/datana/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-02-24 08:51:40.000000 datana-0.3.1.0/datana/atom.py
--rw-rw-rw-   0        0        0     1137 2022-12-07 08:28:44.000000 datana-0.3.1.0/datana/dos.py
--rw-rw-rw-   0        0        0     6035 2023-02-22 09:01:20.000000 datana-0.3.1.0/datana/dynamic.py
--rw-rw-rw-   0        0        0     5411 2022-09-14 03:18:58.000000 datana-0.3.1.0/datana/figure.py
--rw-rw-rw-   0        0        0     1887 2023-02-24 08:53:44.000000 datana-0.3.1.0/datana/plotting.py
--rw-rw-rw-   0        0        0     4801 2022-09-14 06:41:22.000000 datana-0.3.1.0/datana/spectrum.py
--rw-rw-rw-   0        0        0    20815 2023-02-24 08:52:44.000000 datana-0.3.1.0/datana/structure.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:52:25.489230 datana-0.3.1.0/datana.egg-info/
--rw-rw-rw-   0        0        0      379 2023-02-24 11:52:23.000000 datana-0.3.1.0/datana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-02-24 11:52:23.000000 datana-0.3.1.0/datana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 11:52:23.000000 datana-0.3.1.0/datana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-24 11:52:23.000000 datana-0.3.1.0/datana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-24 11:52:25.490229 datana-0.3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-02-24 11:46:12.000000 datana-0.3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.858216 datana-0.3.1.2/
+-rw-rw-rw-   0        0        0      379 2023-05-10 13:01:17.857219 datana-0.3.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.825609 datana-0.3.1.2/datana/
+-rw-rw-rw-   0        0        0       25 2022-09-09 06:43:52.000000 datana-0.3.1.2/datana/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-02-24 08:51:40.000000 datana-0.3.1.2/datana/atom.py
+-rw-rw-rw-   0        0        0     1137 2022-12-07 08:28:44.000000 datana-0.3.1.2/datana/dos.py
+-rw-rw-rw-   0        0        0     6042 2023-05-09 06:10:24.000000 datana-0.3.1.2/datana/dynamic.py
+-rw-rw-rw-   0        0        0     5411 2022-09-14 03:18:58.000000 datana-0.3.1.2/datana/figure.py
+-rw-rw-rw-   0        0        0     1887 2023-02-24 08:53:44.000000 datana-0.3.1.2/datana/plotting.py
+-rw-rw-rw-   0        0        0     4801 2022-09-14 06:41:22.000000 datana-0.3.1.2/datana/spectrum.py
+-rw-rw-rw-   0        0        0    21857 2023-05-09 06:10:00.000000 datana-0.3.1.2/datana/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:17.856250 datana-0.3.1.2/datana.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-10 13:01:16.000000 datana-0.3.1.2/datana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 13:01:15.000000 datana-0.3.1.2/datana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:01:17.858216 datana-0.3.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-05-10 13:00:07.000000 datana-0.3.1.2/setup.py
```

### Comparing `datana-0.3.1.0/datana/atom.py` & `datana-0.3.1.2/datana/atom.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.0/datana/dos.py` & `datana-0.3.1.2/datana/dos.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.0/datana/dynamic.py` & `datana-0.3.1.2/datana/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import copy
-from structure import Structure
+from datana.structure import Structure
 
 class Dynamic:
     def __init__(self):
         self._temperature = []
         self._energy = []
         self._structures = []
```

### Comparing `datana-0.3.1.0/datana/figure.py` & `datana-0.3.1.2/datana/figure.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.0/datana/plotting.py` & `datana-0.3.1.2/datana/plotting.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.0/datana/spectrum.py` & `datana-0.3.1.2/datana/spectrum.py`

 * *Files identical despite different names*

### Comparing `datana-0.3.1.0/datana/structure.py` & `datana-0.3.1.2/datana/structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from functools import reduce
 import copy
-from atom import Atom
+from datana.atom import Atom
+import random
 
 class Structure:
     def __init__(self, a = 1.0, b = 1.0, c = 1.0, alpha = np.pi/2, beta = np.pi/2, gamma = np.pi/2):
         self._lattice = np.array([[a, 0.0, 0.0], [0.0, b, 0.0], [0.0, 0.0, c]])
         self._atom = []
         self._species = []
         self._coords_direct = []
@@ -167,14 +168,34 @@
         del coords_copy
         self.update_cartesian()
         force_copy = copy.deepcopy(self._forces)
         for i in range(a*b*c):
             self._forces = np.concatenate((self._forces, force_copy))
         del force_copy
         self._isFix *= a*b*c
+
+    def replacement(self, initial_num = -1, replace_element = 'H'):
+        self._species[initial_num] = replace_element
+        self._atom[initial_num] = Atom(replace_element)
+    
+    def random_replacement(self, initial_element, replace_element, replace_num = -1):
+        initial_element_num = 0
+        replace_ele_list = []
+        for i, j in enumerate(self._atom):
+            if j._type == initial_element:
+                initial_element_num += 1
+                replace_ele_list.append(i)
+        if replace_num < 0 or replace_num > initial_element_num: replace_number = initial_element_num
+        replace_list = random.sample(replace_ele_list, replace_num)
+        structures_from_random_replacement = Structures()
+        for i in replace_list:
+            structure_temp = copy.deepcopy(self)
+            structure_temp.replacement(i, replace_element)
+            structures_from_random_replacement.add(copy.deepcopy(structure_temp))
+        return structures_from_random_replacement
     
     def to_POSCAR(self, file_name = 'POSCAR', mode = 'Direct'):
         isFix = False
         
         with open(file_name, 'w') as f:
             f.write('POSCAR_created_by_datana\n')
             f.write('1.0000000000\n')
```

### Comparing `datana-0.3.1.0/setup.py` & `datana-0.3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name = 'datana',
-	version = '0.3.1.0',
+	version = '0.3.1.2',
 	author = 'MasterLegend',
 	description = 'datana pakage',
 	long_description = 'Datana is a package for data processing in the field of chemistry. It can be used to process both computational and experimental data.',
 	long_description_content_type = 'text/markdown',
 	url = 'https://github.com/MasterLegend/datana',
 	py_modules = ['datana.spectrum', 'datana.figure', 'datana.atom', 'datana.structure', 'datana.dynamic', 'datana.dos', 'datana.plotting'],
 )
```

