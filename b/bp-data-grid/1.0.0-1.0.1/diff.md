# Comparing `tmp/bp_data_grid-1.0.0.tar.gz` & `tmp/bp_data_grid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-1.0.0.tar", last modified: Wed May  3 12:57:20 2023, max compression
+gzip compressed data, was "bp_data_grid-1.0.1.tar", last modified: Wed May 10 09:27:06 2023, max compression
```

## Comparing `bp_data_grid-1.0.0.tar` & `bp_data_grid-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.711582 bp_data_grid-1.0.0/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-1.0.0/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-1.0.0/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-03 12:57:20.711248 bp_data_grid-1.0.0/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2805 2023-05-03 12:51:36.000000 bp_data_grid-1.0.0/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.697098 bp_data_grid-1.0.0/bp_data_grid.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-03 12:57:20.000000 bp_data_grid-1.0.0/bp_data_grid.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-05-03 12:57:20.000000 bp_data_grid-1.0.0/bp_data_grid.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-03 12:57:20.000000 bp_data_grid-1.0.0/bp_data_grid.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-03 12:57:20.000000 bp_data_grid-1.0.0/bp_data_grid.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-05-03 12:57:20.000000 bp_data_grid-1.0.0/bp_data_grid.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.698314 bp_data_grid-1.0.0/data_grid/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-24 06:27:21.000000 bp_data_grid-1.0.0/data_grid/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.692584 bp_data_grid-1.0.0/data_grid/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.699730 bp_data_grid-1.0.0/data_grid/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:57:20.710128 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1506424 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/index-de62a779.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/index.es-d000f1b8-b218389b.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      555 2023-04-24 08:58:17.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-24 08:57:11.000000 bp_data_grid-1.0.0/data_grid/frontend/dist/vite.svg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-1.0.0/data_grid/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-03 12:57:20.711729 bp_data_grid-1.0.0/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      767 2023-05-03 12:56:59.000000 bp_data_grid-1.0.0/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.313239 bp_data_grid-1.0.1/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-1.0.1/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-1.0.1/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-10 09:27:06.312937 bp_data_grid-1.0.1/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2805 2023-05-03 12:51:36.000000 bp_data_grid-1.0.1/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.305243 bp_data_grid-1.0.1/bp_data_grid.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-10 09:27:06.000000 bp_data_grid-1.0.1/bp_data_grid.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-05-10 09:27:06.000000 bp_data_grid-1.0.1/bp_data_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-10 09:27:06.000000 bp_data_grid-1.0.1/bp_data_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-10 09:27:06.000000 bp_data_grid-1.0.1/bp_data_grid.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-05-10 09:27:06.000000 bp_data_grid-1.0.1/bp_data_grid.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.306174 bp_data_grid-1.0.1/data_grid/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-24 06:27:21.000000 bp_data_grid-1.0.1/data_grid/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.300290 bp_data_grid-1.0.1/data_grid/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.307108 bp_data_grid-1.0.1/data_grid/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 09:27:06.312325 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-05-10 09:25:25.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-10 09:25:25.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1506424 2023-05-10 09:25:25.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/index-de62a779.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   150073 2023-05-10 09:25:25.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/index.es-d000f1b8-b218389b.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-05-10 09:25:25.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      555 2023-05-10 09:25:43.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-10 09:25:24.000000 bp_data_grid-1.0.1/data_grid/frontend/dist/vite.svg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-1.0.1/data_grid/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-10 09:27:06.313340 bp_data_grid-1.0.1/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      767 2023-05-10 09:27:01.000000 bp_data_grid-1.0.1/setup.py
```

### Comparing `bp_data_grid-1.0.0/LICENSE` & `bp_data_grid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/PKG-INFO` & `bp_data_grid-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp_data_grid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.0/README.md` & `bp_data_grid-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/bp_data_grid.egg-info/PKG-INFO` & `bp_data_grid-1.0.1/bp_data_grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bp-data-grid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Show data in data grid
 Home-page: UNKNOWN
 Author: Bluepinapple
 Author-email: vivek.sthul@bluepinapple.com
 License: UNKNOWN
 Description: # Data Grid
```

### Comparing `bp_data_grid-1.0.0/bp_data_grid.egg-info/SOURCES.txt` & `bp_data_grid-1.0.1/bp_data_grid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/__init__.py` & `bp_data_grid-1.0.1/data_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js` & `bp_data_grid-1.0.1/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/assets/index-de62a779.js` & `bp_data_grid-1.0.1/data_grid/frontend/dist/assets/index-de62a779.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/assets/index.es-d000f1b8-b218389b.js` & `bp_data_grid-1.0.1/data_grid/frontend/dist/assets/index.es-d000f1b8-b218389b.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js` & `bp_data_grid-1.0.1/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/index.html` & `bp_data_grid-1.0.1/data_grid/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/frontend/dist/vite.svg` & `bp_data_grid-1.0.1/data_grid/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/data_grid/register.py` & `bp_data_grid-1.0.1/data_grid/register.py`

 * *Files identical despite different names*

### Comparing `bp_data_grid-1.0.0/setup.py` & `bp_data_grid-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp_data_grid",
-    version="1.0.0",
+    version="1.0.1",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Show data in data grid",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

