# Comparing `tmp/unisci-1.4.7.tar.gz` & `tmp/unisci-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.4.7.tar", last modified: Tue May  9 23:32:57 2023, max compression
+gzip compressed data, was "unisci-1.4.8.tar", last modified: Wed May 10 02:12:07 2023, max compression
```

## Comparing `unisci-1.4.7.tar` & `unisci-1.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.908730 unisci-1.4.7/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.7/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.7/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-09 23:32:57.908362 unisci-1.4.7/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.7/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-09 23:32:57.908831 unisci-1.4.7/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-09 23:31:21.000000 unisci-1.4.7/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.904358 unisci-1.4.7/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-09 23:30:45.000000 unisci-1.4.7/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.7/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.7/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.7/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.906651 unisci-1.4.7/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.7/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.7/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.7/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.4.7/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.907923 unisci-1.4.7/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.7/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.4.7/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.7/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    39591 2023-05-03 23:43:10.000000 unisci-1.4.7/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.905851 unisci-1.4.7/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:12:07.295144 unisci-1.4.8/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.8/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.8/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-10 02:12:07.294822 unisci-1.4.8/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.8/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-10 02:12:07.295232 unisci-1.4.8/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-10 02:10:52.000000 unisci-1.4.8/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:12:07.289792 unisci-1.4.8/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-10 02:11:01.000000 unisci-1.4.8/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.8/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.8/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.8/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:12:07.292603 unisci-1.4.8/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.8/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.8/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.8/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.4.8/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:12:07.294391 unisci-1.4.8/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.8/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.4.8/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.8/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    39590 2023-05-10 02:08:28.000000 unisci-1.4.8/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-10 02:12:07.291304 unisci-1.4.8/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-10 02:12:07.000000 unisci-1.4.8/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-10 02:12:07.000000 unisci-1.4.8/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-10 02:12:07.000000 unisci-1.4.8/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-10 02:12:07.000000 unisci-1.4.8/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-10 02:12:07.000000 unisci-1.4.8/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.4.7/LICENSE` & `unisci-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/PKG-INFO` & `unisci-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.7
+Version: 1.4.8
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.7/README.md` & `unisci-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/setup.py` & `unisci-1.4.8/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.4.7',
+    version='1.4.8',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.4.7/unisci/_conversion_factors.py` & `unisci-1.4.8/unisci/_conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/_error.py` & `unisci-1.4.8/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/formulas/_validation.py` & `unisci-1.4.8/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/formulas/chemistry.py` & `unisci-1.4.8/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/metric.py` & `unisci-1.4.8/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/periodic/periodic-table-lookup.json` & `unisci-1.4.8/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/periodic/periodic-table-numbers.json` & `unisci-1.4.8/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/periodic/periodic-table-symbols.json` & `unisci-1.4.8/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.7/unisci/types.py` & `unisci-1.4.8/unisci/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1008,15 +1008,15 @@
         return Quantity(self.information["atomic_mass"], {"g": 1, "mol": -1})
     
     @property
     def state(self) -> str:
         """
         Returns the state of the element at room temperature.
         """
-        return self.information["state"]
+        return self.information["phase"]
     
     @property 
     def density(self) -> Quantity:
         """
         Returns the density of the element at room temperature. in g/L if gas, otherwise in g/mL
         """
         if self.state == "Gas":
@@ -1097,15 +1097,15 @@
         Returns a dictionary containing the noble gas and the configuration. 
         Example: {'gas': Element(element_symbol="He"), 'configuration': {'2s': 2, '2p': 4}}
         """
         config_split = self.noble_gas_config_str.split()
         configs = {}
 
         # gets the gas
-        noble_symbol = config_split[0][1:-1:0]   # remove []
+        noble_symbol = config_split[0][1:-1]   # remove []
         noble_gas = Element(element_symbol=noble_symbol)
 
         # gets reset of configurations
         list_configs  = config_split[1::]
         for config in list_configs:
             configs[config[:2:]] = int(config[2::])
 
@@ -1125,15 +1125,15 @@
         """
         return self.information["electronegativity_pauling"]
     
     def get_ionization_energy(self, level: int = 1) -> Quantity:
         """
         Arguments: the level, defaults to first level.
 
-        Raises: an ArgumentError for levels too large, or not integers
+        Raises: an ArgumentError for levels too large, or not integers.
 
         Returns: the level-th ionization energy of the element.
         """
         
         if not isinstance(level, int):
             raise ArgumentError("Level must be an integer.")
```

### Comparing `unisci-1.4.7/unisci.egg-info/PKG-INFO` & `unisci-1.4.8/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.7
+Version: 1.4.8
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.7/unisci.egg-info/SOURCES.txt` & `unisci-1.4.8/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

