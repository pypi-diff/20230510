# Comparing `tmp/Slpapy-0.3.6.tar.gz` & `tmp/Slpapy-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.6.tar", last modified: Wed May 10 02:21:22 2023, max compression
+gzip compressed data, was "Slpapy-0.3.7.tar", last modified: Wed May 10 02:29:55 2023, max compression
```

## Comparing `Slpapy-0.3.6.tar` & `Slpapy-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 02:21:22.351101 Slpapy-0.3.6/
--rw-rw-rw-   0        0        0      159 2023-05-10 02:21:22.350103 Slpapy-0.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 02:21:22.313202 Slpapy-0.3.6/Slpapy/
--rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.6/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.6/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:21:22.348137 Slpapy-0.3.6/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.6/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.6/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.6/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:21:22.322207 Slpapy-0.3.6/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-10 02:21:21.000000 Slpapy-0.3.6/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-10 02:21:22.000000 Slpapy-0.3.6/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:21:21.000000 Slpapy-0.3.6/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-10 02:21:21.000000 Slpapy-0.3.6/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 02:21:21.000000 Slpapy-0.3.6/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 02:21:22.351101 Slpapy-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-05-10 02:20:57.000000 Slpapy-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:29:55.950097 Slpapy-0.3.7/
+-rw-rw-rw-   0        0        0      159 2023-05-10 02:29:55.950097 Slpapy-0.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 02:29:55.914193 Slpapy-0.3.7/Slpapy/
+-rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.7/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.7/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:29:55.948102 Slpapy-0.3.7/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.7/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.7/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.7/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:29:55.922171 Slpapy-0.3.7/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-10 02:29:55.000000 Slpapy-0.3.7/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-05-10 02:29:55.000000 Slpapy-0.3.7/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:29:55.000000 Slpapy-0.3.7/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-10 02:29:55.000000 Slpapy-0.3.7/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 02:29:55.000000 Slpapy-0.3.7/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 02:29:55.951094 Slpapy-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-05-10 02:29:43.000000 Slpapy-0.3.7/setup.py
```

### Comparing `Slpapy-0.3.6/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.7/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.7/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.3.7/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy/processing_analyze.py` & `Slpapy-0.3.7/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.6/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.7/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

