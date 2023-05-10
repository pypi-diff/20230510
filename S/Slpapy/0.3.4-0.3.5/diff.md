# Comparing `tmp/Slpapy-0.3.4.tar.gz` & `tmp/Slpapy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.4.tar", last modified: Wed May 10 01:43:42 2023, max compression
+gzip compressed data, was "Slpapy-0.3.5.tar", last modified: Wed May 10 02:09:24 2023, max compression
```

## Comparing `Slpapy-0.3.4.tar` & `Slpapy-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:43:42.789896 Slpapy-0.3.4/
--rw-rw-rw-   0        0        0      159 2023-05-10 01:43:42.788899 Slpapy-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 01:43:42.761970 Slpapy-0.3.4/Slpapy/
--rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.4/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.4/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:43:42.787901 Slpapy-0.3.4/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.4/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.3.4/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.4/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.4/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.4/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.4/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.4/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.4/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.4/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.4/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.4/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.4/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.4/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.3.4/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.4/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:43:42.768952 Slpapy-0.3.4/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-10 01:43:42.000000 Slpapy-0.3.4/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-10 01:43:42.000000 Slpapy-0.3.4/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:43:42.000000 Slpapy-0.3.4/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-10 01:43:42.000000 Slpapy-0.3.4/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 01:43:42.000000 Slpapy-0.3.4/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:43:42.789896 Slpapy-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-05-10 01:43:36.000000 Slpapy-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:24.960825 Slpapy-0.3.5/
+-rw-rw-rw-   0        0        0      159 2023-05-10 02:09:24.959828 Slpapy-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:24.922943 Slpapy-0.3.5/Slpapy/
+-rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.5/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.5/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:24.957833 Slpapy-0.3.5/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.5/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.5/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.5/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.5/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.5/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.5/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.5/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.5/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.5/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.5/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.5/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.5/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43458 2023-05-09 09:26:02.000000 Slpapy-0.3.5/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.3.5/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.5/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:24.932900 Slpapy-0.3.5/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-10 02:09:24.000000 Slpapy-0.3.5/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-10 02:09:24.000000 Slpapy-0.3.5/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:09:24.000000 Slpapy-0.3.5/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-10 02:09:24.000000 Slpapy-0.3.5/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 02:09:24.000000 Slpapy-0.3.5/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 02:09:24.960825 Slpapy-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-05-10 02:09:17.000000 Slpapy-0.3.5/setup.py
```

### Comparing `Slpapy-0.3.4/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.5/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.5/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/Spatial_map.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/beats.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/logging.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.3.5/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy/processing_analyze.py` & `Slpapy-0.3.5/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.4/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.5/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

