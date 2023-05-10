# Comparing `tmp/PythonCoordinates-0.5.7.tar.gz` & `tmp/PythonCoordinates-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonCoordinates-0.5.7.tar", last modified: Wed May 10 17:03:15 2023, max compression
+gzip compressed data, was "PythonCoordinates-0.5.8.tar", last modified: Wed May 10 17:03:43 2023, max compression
```

## Comparing `PythonCoordinates-0.5.7.tar` & `PythonCoordinates-0.5.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.293110 PythonCoordinates-0.5.7/
--rw-rw-rw-   0        0        0     3548 2023-05-10 17:03:15.293110 PythonCoordinates-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     2054 2023-05-10 12:00:22.000000 PythonCoordinates-0.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 17:03:15.293110 PythonCoordinates-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-05-10 14:13:43.000000 PythonCoordinates-0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.276766 PythonCoordinates-0.5.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.280324 PythonCoordinates-0.5.7/src/PythonCoordinates/
--rw-rw-rw-   0        0        0      111 2023-03-24 02:30:00.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.286087 PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/
--rw-rw-rw-   0        0        0     1186 2023-05-10 00:58:48.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/GpsTime.py
--rw-rw-rw-   0        0        0     3690 2023-03-25 01:35:23.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/Physics.py
--rw-rw-rw-   0        0        0       46 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/__init__.py
--rw-rw-rw-   0        0        0    10691 2023-05-10 17:01:45.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/measurement_resolution.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.288339 PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/
--rw-rw-rw-   0        0        0       80 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/__init__.py
--rw-rw-rw-   0        0        0    10323 2023-05-03 20:47:17.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/coordinate_representations.py
--rw-rw-rw-   0        0        0    39302 2023-03-29 01:45:29.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/geospatial_coordinates.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.290324 PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/
--rw-rw-rw-   0        0        0     2383 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/MatrixRotations.py
--rw-rw-rw-   0        0        0       31 2023-03-24 02:30:00.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/__init__.py
--rw-rw-rw-   0        0        0     1665 2023-03-29 01:45:41.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/test_MatrixRotations.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.292607 PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/
--rw-rw-rw-   0        0        0      896 2023-03-25 01:35:23.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/Measurable.py
--rw-rw-rw-   0        0        0       61 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/__init__.py
--rw-rw-rw-   0        0        0    63391 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/physical_quantities.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:03:15.283595 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-05-10 17:03:15.000000 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-10 17:03:15.000000 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:03:15.000000 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 17:03:15.000000 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-10 17:03:15.000000 PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.823463 PythonCoordinates-0.5.8/
+-rw-rw-rw-   0        0        0     3548 2023-05-10 17:03:43.822466 PythonCoordinates-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2054 2023-05-10 12:00:22.000000 PythonCoordinates-0.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 17:03:43.823463 PythonCoordinates-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-05-10 17:03:39.000000 PythonCoordinates-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.802758 PythonCoordinates-0.5.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.805482 PythonCoordinates-0.5.8/src/PythonCoordinates/
+-rw-rw-rw-   0        0        0      111 2023-03-24 02:30:00.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.818479 PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/
+-rw-rw-rw-   0        0        0     1186 2023-05-10 00:58:48.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/GpsTime.py
+-rw-rw-rw-   0        0        0     3690 2023-03-25 01:35:23.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/Physics.py
+-rw-rw-rw-   0        0        0       46 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/__init__.py
+-rw-rw-rw-   0        0        0    10691 2023-05-10 17:01:45.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/measurement_resolution.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.819476 PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/
+-rw-rw-rw-   0        0        0       80 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/__init__.py
+-rw-rw-rw-   0        0        0    10323 2023-05-03 20:47:17.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/coordinate_representations.py
+-rw-rw-rw-   0        0        0    39302 2023-03-29 01:45:29.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/geospatial_coordinates.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.821469 PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/
+-rw-rw-rw-   0        0        0     2383 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/MatrixRotations.py
+-rw-rw-rw-   0        0        0       31 2023-03-24 02:30:00.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/__init__.py
+-rw-rw-rw-   0        0        0     1665 2023-03-29 01:45:41.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/test_MatrixRotations.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.822466 PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/
+-rw-rw-rw-   0        0        0      896 2023-03-25 01:35:23.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/Measurable.py
+-rw-rw-rw-   0        0        0       61 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/__init__.py
+-rw-rw-rw-   0        0        0    63391 2023-02-17 18:40:46.000000 PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/physical_quantities.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:03:43.815668 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-05-10 17:03:43.000000 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-05-10 17:03:43.000000 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:03:43.000000 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 17:03:43.000000 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-10 17:03:43.000000 PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/top_level.txt
```

### Comparing `PythonCoordinates-0.5.7/PKG-INFO` & `PythonCoordinates-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCoordinates
-Version: 0.5.7
+Version: 0.5.8
 Summary: A collection of classes for representing the physical measurable quantities and the methods to locate them
 Home-page: https://gitlab.com/frankmobley/physical_quantities_coordinates
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 Description-Content-Type: text/markdown
 
 # ![Image](./_d29623d8-088c-480c-8d70-0b831a2c23a6.jpg "PythonCoordinates") PythonCoordinates
```

### Comparing `PythonCoordinates-0.5.7/README.md` & `PythonCoordinates-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/setup.py` & `PythonCoordinates-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
     with open('HISTORY.md') as history_file:
         HISTORY = history_file.read()
 
 setup(
     name='PythonCoordinates',
-    version='0.5.7',
+    version='0.5.8',
     packages=find_packages('src', exclude=['test*.py']),
     url='https://gitlab.com/frankmobley/physical_quantities_coordinates',
     license='',
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
     description='A collection of classes for representing the physical '
                 'measurable quantities and the methods to '
```

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/GpsTime.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/GpsTime.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/Physics.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/Physics.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/conversions/measurement_resolution.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/conversions/measurement_resolution.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/coordinate_representations.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/coordinate_representations.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/coordinates/geospatial_coordinates.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/coordinates/geospatial_coordinates.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/MatrixRotations.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/MatrixRotations.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/linear_algebra/test_MatrixRotations.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/linear_algebra/test_MatrixRotations.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/Measurable.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/Measurable.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates/measurables/physical_quantities.py` & `PythonCoordinates-0.5.8/src/PythonCoordinates/measurables/physical_quantities.py`

 * *Files identical despite different names*

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/PKG-INFO` & `PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCoordinates
-Version: 0.5.7
+Version: 0.5.8
 Summary: A collection of classes for representing the physical measurable quantities and the methods to locate them
 Home-page: https://gitlab.com/frankmobley/physical_quantities_coordinates
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 Description-Content-Type: text/markdown
 
 # ![Image](./_d29623d8-088c-480c-8d70-0b831a2c23a6.jpg "PythonCoordinates") PythonCoordinates
```

### Comparing `PythonCoordinates-0.5.7/src/PythonCoordinates.egg-info/SOURCES.txt` & `PythonCoordinates-0.5.8/src/PythonCoordinates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

