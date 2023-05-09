# Comparing `tmp/unisci-1.4.6.tar.gz` & `tmp/unisci-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.4.6.tar", last modified: Tue May  2 02:45:02 2023, max compression
+gzip compressed data, was "unisci-1.4.7.tar", last modified: Tue May  9 23:32:57 2023, max compression
```

## Comparing `unisci-1.4.6.tar` & `unisci-1.4.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:45:02.401394 unisci-1.4.6/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.6/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.6/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:45:02.401087 unisci-1.4.6/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.6/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-02 02:45:02.401503 unisci-1.4.6/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-02 02:43:58.000000 unisci-1.4.6/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:45:02.397016 unisci-1.4.6/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-02 02:43:54.000000 unisci-1.4.6/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.6/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.6/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.6/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:45:02.399329 unisci-1.4.6/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.6/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.6/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.6/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1842 2023-04-30 22:59:28.000000 unisci-1.4.6/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:45:02.400696 unisci-1.4.6/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.6/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.6/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.6/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    39591 2023-05-02 02:42:15.000000 unisci-1.4.6/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:45:02.398495 unisci-1.4.6/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:45:02.000000 unisci-1.4.6/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-02 02:45:02.000000 unisci-1.4.6/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-02 02:45:02.000000 unisci-1.4.6/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-02 02:45:02.000000 unisci-1.4.6/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-02 02:45:02.000000 unisci-1.4.6/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.908730 unisci-1.4.7/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.7/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.7/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-09 23:32:57.908362 unisci-1.4.7/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.7/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-09 23:32:57.908831 unisci-1.4.7/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-09 23:31:21.000000 unisci-1.4.7/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.904358 unisci-1.4.7/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-09 23:30:45.000000 unisci-1.4.7/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.7/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.7/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.7/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.906651 unisci-1.4.7/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.7/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.7/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.7/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1881 2023-05-09 23:31:16.000000 unisci-1.4.7/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.907923 unisci-1.4.7/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.7/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-05-03 23:47:40.000000 unisci-1.4.7/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.7/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    39591 2023-05-03 23:43:10.000000 unisci-1.4.7/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-09 23:32:57.905851 unisci-1.4.7/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-09 23:32:57.000000 unisci-1.4.7/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.4.6/LICENSE` & `unisci-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/PKG-INFO` & `unisci-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.6
+Version: 1.4.7
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.6/README.md` & `unisci-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/setup.py` & `unisci-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.4.6',
+    version='1.4.7',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.4.6/unisci/_conversion_factors.py` & `unisci-1.4.7/unisci/_conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/_error.py` & `unisci-1.4.7/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/formulas/_validation.py` & `unisci-1.4.7/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/formulas/chemistry.py` & `unisci-1.4.7/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/metric.py` & `unisci-1.4.7/unisci/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     'z': 1e-21,
     'a': 1e-18,
     'f': 1e-15,
     'p': 1e-12,
     'n': 1e-9,
     'µ': 1e-6,
     'mc': 1e-6,     # for those who cannot use the µ symbol
+    'u': 1e-6,      # alternate option
     'm': 1e-3,
     'c': 1e-2,
     'd': 1e-1,
     'da': 1e1,
     'h': 1e2,
     'k': 1e3,
     'M': 1e6,
```

### Comparing `unisci-1.4.6/unisci/periodic/periodic-table-lookup.json` & `unisci-1.4.7/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/periodic/periodic-table-numbers.json` & `unisci-1.4.7/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/periodic/periodic-table-symbols.json` & `unisci-1.4.7/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci/types.py` & `unisci-1.4.7/unisci/types.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.6/unisci.egg-info/PKG-INFO` & `unisci-1.4.7/unisci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.6
+Version: 1.4.7
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.6/unisci.egg-info/SOURCES.txt` & `unisci-1.4.7/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

