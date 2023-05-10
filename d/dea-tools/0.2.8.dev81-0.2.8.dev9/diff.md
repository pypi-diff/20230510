# Comparing `tmp/dea-tools-0.2.8.dev81.tar.gz` & `tmp/dea-tools-0.2.8.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dea-tools-0.2.8.dev81.tar", last modified: Wed May 10 00:35:25 2023, max compression
+gzip compressed data, was "dea-tools-0.2.8.dev9.tar", last modified: Tue Aug 30 06:49:00 2022, max compression
```

## Comparing `dea-tools-0.2.8.dev81.tar` & `dea-tools-0.2.8.dev9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:35:25.954835 dea-tools-0.2.8.dev81/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-10 00:35:25.954835 dea-tools-0.2.8.dev81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:35:25.950834 dea-tools-0.2.8.dev81/dea_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:35:25.954835 dea-tools-0.2.8.dev81/dea_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32250 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    29019 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/miningrehab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/bom.py
--rw-r--r--   0 runner    (1001) docker     (123)    62213 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    59379 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    51764 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    39758 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/landcover.py
--rw-r--r--   0 runner    (1001) docker     (123)    37726 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/pyfes_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/dea_tools/waterbodies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:35:25.950834 dea-tools-0.2.8.dev81/dea_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-10 00:35:24.000000 dea-tools-0.2.8.dev81/dea_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-10 00:35:25.000000 dea-tools-0.2.8.dev81/dea_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:35:24.000000 dea-tools-0.2.8.dev81/dea_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-10 00:35:24.000000 dea-tools-0.2.8.dev81/dea_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 00:35:24.000000 dea-tools-0.2.8.dev81/dea_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:35:25.954835 dea-tools-0.2.8.dev81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-10 00:33:13.000000 dea-tools-0.2.8.dev81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3957 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31477 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11607 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19962 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31368 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/miningrehab.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11170 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19500 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11754 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/bom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62134 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11149 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/climate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40083 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34879 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39611 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/landcover.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42577 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/pyfes_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28904 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40832 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26733 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4542 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/dea_tools/waterbodies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/dea_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-08-30 06:49:00.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-30 06:48:59.000000 dea-tools-0.2.8.dev9/dea_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-30 06:49:00.839710 dea-tools-0.2.8.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-08-30 06:47:03.000000 dea-tools-0.2.8.dev9/setup.py
```

### Comparing `dea-tools-0.2.8.dev81/LICENSE` & `dea-tools-0.2.8.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev81/PKG-INFO` & `dea-tools-0.2.8.dev9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev81
+Version: 0.2.8.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
-Author-email: earth.observation@ga.gov.au
+Author-email: dea@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/x-rst
 Provides-Extra: jupyter
-Provides-Extra: dask_gateway
-Provides-Extra: otps
+Provides-Extra: boto
 License-File: LICENSE
 
 
 dea-tools
 =========
 
 Python functions and algorithms developed to assist in analysing Digital Earth Australia (DEA) data (e.g. loading data, plotting, spatial analysis, machine learning). This includes the following modules:
@@ -39,45 +38,31 @@
 
 -  ``dea_tools.spatial``: Spatial analysis tools (e.g. rasterising, vectorising, contour extraction, image processing)
 -  ``dea_tools.temporal``: Temporal analysis tools (e.g. phenology, temporal statistics, multi-dimensional regression)
 
 **Classification and segmentation**
 
 -  ``dea_tools.classification.py``: Machine learning classification (e.g. training and applying machine learning models on satellite data)
--  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segmentation with RSGISLIB)
+-  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segementation with RSGISLIB)
 
 **Parallel processing**
 
 -  ``dea_tools.dask``: Parallel processing with Dask (e.g. creating Dask clusters for scalable analysis)
 
 **Domain-specific analysis**
 
 -  ``dea_tools.land_cover``: Functions for plotting Digital Earth Australia Land Cover data.
 -  ``dea_tools.coastal``: Coastal and intertidal analysis tools (e.g. tidal tagging, coastal change timeseries)
--  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. gauge data, discharge data)
+-  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. guage data, discharge data)
 -  ``dea_tools.climate``: Retrieving and manipulating gridded climate data (e.g. ERA5)
 -  ``dea_tools.waterbodies``: Loading and processing DEA Waterbodies data (e.g. finding and loading waterbody timeseries data)
 
 Installation
 ------------
 
-With conda
-~~~~~~~~~~
-
-.. code-block:: bash
-
-    wget -O conda-environment.yml https://raw.githubusercontent.com/opendatacube/datacube-core/develop/conda-environment.yml
-
-    mamba env create -f conda-environment.yml
-    conda activate cubeenv
-
-
-Install dea-tools
-~~~~~~~~~~~~~~~~~
-
 Install the package from the source on any system with ``pip``:
 
 .. code-block:: bash
 
     pip install dea-tools
 
 To work with this module on the DEA Sandbox or National Computational Infrastructure environments without installing it, you can add the ``Tools`` directory to the system path from within the ``dea-notebooks`` repository:
@@ -125,7 +110,8 @@
 
 .. code-block:: bash
 
         cd Tools
         rm dea_tools/__version__.py  # if necessary
         pip install . --use-feature=in-tree-build
         python -m build
+
```

### Comparing `dea-tools-0.2.8.dev81/README.rst` & `dea-tools-0.2.8.dev9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,45 +16,31 @@
 
 -  ``dea_tools.spatial``: Spatial analysis tools (e.g. rasterising, vectorising, contour extraction, image processing)
 -  ``dea_tools.temporal``: Temporal analysis tools (e.g. phenology, temporal statistics, multi-dimensional regression)
 
 **Classification and segmentation**
 
 -  ``dea_tools.classification.py``: Machine learning classification (e.g. training and applying machine learning models on satellite data)
--  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segmentation with RSGISLIB)
+-  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segementation with RSGISLIB)
 
 **Parallel processing**
 
 -  ``dea_tools.dask``: Parallel processing with Dask (e.g. creating Dask clusters for scalable analysis)
 
 **Domain-specific analysis**
 
 -  ``dea_tools.land_cover``: Functions for plotting Digital Earth Australia Land Cover data.
 -  ``dea_tools.coastal``: Coastal and intertidal analysis tools (e.g. tidal tagging, coastal change timeseries)
--  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. gauge data, discharge data)
+-  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. guage data, discharge data)
 -  ``dea_tools.climate``: Retrieving and manipulating gridded climate data (e.g. ERA5)
 -  ``dea_tools.waterbodies``: Loading and processing DEA Waterbodies data (e.g. finding and loading waterbody timeseries data)
 
 Installation
 ------------
 
-With conda
-~~~~~~~~~~
-
-.. code-block:: bash
-
-    wget -O conda-environment.yml https://raw.githubusercontent.com/opendatacube/datacube-core/develop/conda-environment.yml
-
-    mamba env create -f conda-environment.yml
-    conda activate cubeenv
-
-
-Install dea-tools
-~~~~~~~~~~~~~~~~~
-
 Install the package from the source on any system with ``pip``:
 
 .. code-block:: bash
 
     pip install dea-tools
 
 To work with this module on the DEA Sandbox or National Computational Infrastructure environments without installing it, you can add the ``Tools`` directory to the system path from within the ``dea-notebooks`` repository:
@@ -102,7 +88,8 @@
 
 .. code-block:: bash
 
         cd Tools
         rm dea_tools/__version__.py  # if necessary
         pip install . --use-feature=in-tree-build
         python -m build
+
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/animations.py` & `dea-tools-0.2.8.dev9/dea_tools/app/animations.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,65 +44,47 @@
 
 from datacube.utils import masking
 from datacube.utils.geometry import Geometry
 from datacube.utils.masking import mask_invalid_data
 import dea_tools.app.widgetconstructors as deawidgets
 from dea_tools.dask import create_local_dask_cluster
 from dea_tools.spatial import reverse_geocode
+from dea_tools.datahandling import pan_sharpen_brovey
 
 import warnings
+
 warnings.filterwarnings("ignore")
 
 # WMS params and satellite style bands
 sat_params = {
     "Landsat": {
-        "products": [
-            "ga_ls5t_ard_3",
-            "ga_ls7e_ard_3",
-            "ga_ls8c_ard_3",
-            "ga_ls9c_ard_3",
-        ],
+        "products": ["ga_ls5t_ard_3", "ga_ls7e_ard_3", "ga_ls8c_ard_3"],
         "styles": {
             "True colour": ("true_colour", ["nbart_red", "nbart_green", "nbart_blue"]),
             "False colour": (
                 "false_colour",
                 ["nbart_swir_1", "nbart_nir", "nbart_green"],
             ),
         },
     },
     "Sentinel-2": {
         "products": [
-            "ga_s2am_ard_3",
-            "ga_s2bm_ard_3",
+            "s2a_ard_granule",
+            "s2b_ard_granule",
+            "s2a_nrt_granule",
+            "s2b_nrt_granule",
         ],
         "styles": {
             "True colour": ("simple_rgb", ["nbart_red", "nbart_green", "nbart_blue"]),
             "False colour": (
                 "infrared_green",
                 ["nbart_swir_2", "nbart_nir_1", "nbart_green"],
             ),
         },
     },
-    "Sentinel-2 and Landsat": {
-        "products": [
-            "ga_s2am_ard_3",
-            "ga_s2bm_ard_3",
-            "ga_ls5t_ard_3",
-            "ga_ls7e_ard_3",
-            "ga_ls8c_ard_3",
-            "ga_ls9c_ard_3",
-        ],
-        "styles": {
-            "True colour": ("simple_rgb", ["nbart_red", "nbart_green", "nbart_blue"]),
-            "False colour": (
-                "infrared_green",
-                ["nbart_common_swir_1", "nbart_common_nir", "nbart_green"],
-            ),
-        },
-    },
 }
 
 
 def make_box_layout():
     return Layout(
         #         border='solid 1px black',
         margin="0px 10px 10px 0px",
@@ -129,15 +111,15 @@
 
     # Clear data load params to trigger data re-load
     self.timeseries_ds = None
     self.load_params = None
     self.query_params = None
 
     if update_basemap:
-
+        
         # Clear all layers and add basemap
         self.map_layers.clear_layers()
         self.map_layers.add_layer(self.basemap)
 
 
 def extract_data(self):
 
@@ -176,16 +158,15 @@
 
         self.load_params = {
             "measurements": sat_params[self.dealayer]["styles"][self.style][1],
             "resolution": (-self.resolution, self.resolution),
             "output_crs": crs,
             "group_by": "solar_day",
             "dask_chunks": {"time": 1, "x": 2048, "y": 2048},
-            "resampling": {"*": "bilinear", "oa_fmask": "nearest", "fmask": "nearest"},
-            "skip_broken_datasets": True,
+            "resampling": {"*": "cubic", "oa_fmask": "nearest", "fmask": "nearest"},
         }
 
         # Load data
         from dea_tools.datahandling import load_ard
 
         timeseries_ds = load_ard(
             dc=dc,
@@ -209,15 +190,15 @@
         timeseries_ds.load()
 
     # Else if no data is returned, return None
     else:
         timeseries_ds = None
 
     # Close down the dask client
-    #     client.shutdown()
+#     client.shutdown()
     client.close()
 
     return timeseries_ds
 
 
 def plot_data(self, fname):
 
@@ -338,15 +319,14 @@
             year=end_date.year - 3, month=end_date.month, day=end_date.day
         )
         self.start_date = start_date.strftime("%Y-%m-%d")
         self.end_date = end_date.strftime("%Y-%m-%d")
         self.dealayer_list = [
             ("Landsat", "Landsat"),
             ("Sentinel-2", "Sentinel-2"),
-            ("Sentinel-2 and Landsat", "Sentinel-2 and Landsat")
         ]
         self.dealayer = self.dealayer_list[0][1]
 
         # Styles
         self.styles_list = ["True colour", "False colour"]
         self.style = self.styles_list[0]
 
@@ -541,21 +521,21 @@
             step=1,
             description="",
             layout={"width": "85%"},
         )
 
         checkbox_rolling_median = deawidgets.create_checkbox(
             self.rolling_median,
-            "Apply rolling median to produce smooth, cloud-free animations",
+            "Apply rolling median to produce<br>smooth, cloud-free animations",
             layout={"width": "85%"},
         )
         text_rolling_median_window = widgets.IntText(
             value=20,
             step=1,
-            description="Rolling window (timesteps)",
+            description="</br>Rolling window (timesteps)",
             layout={
                 "width": "85%",
                 "margin": "0px",
                 "padding": "0px",
                 "display": "none",
             },
         )
@@ -786,57 +766,53 @@
         # Clear data load params to trigger data re-load
         update_map_layers(self)
 
     # Update basemap
     def update_basemap(self, change):
         self.basemap = change.new
         update_map_layers(self, update_basemap=True)
-
+        
     # Change layers shown on the map
     def update_dealayer(self, change):
         self.dealayer = change.new
 
-        if change.new == "Landsat":
+        if change.new == "ga_ls_ard_3":
             self.text_resolution.value = 30
 
-        elif change.new == "Sentinel-2":
+        else:
             self.text_resolution.value = 10
-        
-        elif change.new == "Sentinel-2 and Landsat":
-            self.text_resolution.value = 30
-            
-        # Clear data load params to trigger data re-load
-        update_map_layers(self)
 
     # Set imagery style
     def update_styles(self, change):
         self.style = change.new
 
         # Clear data load params to trigger data re-load
         update_map_layers(self)
-
+        
     # Update good data slider
     def update_floatslider_max_cloud_cover(self, change):
         self.max_cloud_cover = change.new
 
         # Clear data load params to trigger data re-load
         update_map_layers(self)
-
+    
     # Set output file format
     def update_output(self, change):
         self.output_format = change.new
 
     # Update colour stretch
     def update_slider_percentile(self, change):
         self.vmin, self.vmax = change.new
 
     # Update power transform
     def update_slider_power(self, change):
         self.power = change.new
 
+
+
     # Enable unsharp masking and show/hide custom params
     def update_checkbox_unsharp_mask(self, change):
         self.unsharp_mask = change.new
 
         # Show unsharp masking params in menu if activated
         if change.new:
             self.text_unsharp_mask_radius.layout.display = "block"
@@ -896,15 +872,15 @@
 
         # Clear data load params to trigger data re-load
         update_map_layers(self)
 
     # Set output file format
     def update_dropdown_resampling(self, change):
         self.resample_freq = change.new
-
+        
         # Clear data load params to trigger data re-load
         update_map_layers(self)
 
     def run_app(self, change):
 
         # Clear progress bar and output areas before running
         self.status_info.clear_output()
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/changefilmstrips.py` & `dea-tools-0.2.8.dev9/dea_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/crophealth.py` & `dea-tools-0.2.8.dev9/dea_tools/app/crophealth.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # Dates are converted to strings as required by loading function below
     end_date = dt.date.today()
     start_date = end_date - dt.timedelta(days=365)
 
     time = (start_date.strftime("%Y-%m-%d"), end_date.strftime("%Y-%m-%d"))
 
     # Construct the data cube query
-    products = ["ga_s2am_ard_3", "ga_s2bm_ard_3"]
+    products = ["s2a_ard_granule", "s2b_ard_granule"]
     
     query = {
         'x': longitude,
         'y': latitude,
         'time': time,
         'measurements': [
             'nbart_red',
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/deacoastlines.py` & `dea-tools-0.2.8.dev9/dea_tools/app/deacoastlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 from io import BytesIO
 import ipywidgets as widgets
 
 import dea_tools.app.widgetconstructors as deawidgets
 from dea_tools.coastal import get_coastlines, transect_distances
 
 
-WMS_ADDRESS = "https://geoserver.dea.ga.gov.au/geoserver/wms"
-
-
 def make_box_layout():
     return Layout(
         #          border='solid 1px black',
         margin='0px 10px 10px 0px',
         padding='5px 5px 5px 5px',
         width='100%',
         height='100%',
@@ -148,15 +145,15 @@
         #########################################
 
         # Create drawing tools
         desired_drawtools = ['polyline']
         draw_control = deawidgets.create_drawcontrol(desired_drawtools)
 
         # Load DEACoastLines WMS
-        deacl_url = WMS_ADDRESS
+        deacl_url = 'https://geoserver.dea.ga.gov.au/geoserver/wms'
         deacl_layer = 'dea:DEACoastlines'
         deacoastlines = WMSLayer(
             url=deacl_url,
             layers=deacl_layer,
             format='image/png',
             transparent=True,
             attribution='DEA Coastlines © 2020 Geoscience Australia')
@@ -362,15 +359,15 @@
 
     # Update product
     def update_deaoverlay(self, change):
 
         self.product = change.new
 
         # Load DEACoastLines WMS
-        deacl_url = WMS_ADDRESS
+        deacl_url = "https://geoserver.dea.ga.gov.au/geoserver/wms"
         deacl_layer = "dea:DEACoastlines"
         deacoastlines = WMSLayer(
             url=deacl_url,
             layers=deacl_layer,
             format="image/png",
             transparent=True,
             attribution="DEA Coastlines © 2020 Geoscience Australia")
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/imageexport.py` & `dea-tools-0.2.8.dev9/dea_tools/app/imageexport.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,307 +43,333 @@
 from skimage.filters import unsharp_mask
 
 from datacube.utils import masking
 from datacube.utils.geometry import Geometry
 import dea_tools.app.widgetconstructors as deawidgets
 from dea_tools.dask import create_local_dask_cluster
 from dea_tools.spatial import reverse_geocode
-from dea_tools.datahandling import xr_pansharpen
+from dea_tools.datahandling import pan_sharpen_brovey
 
 
 # WMS params and satellite style bands
 sat_params = {
-    "ga_ls_ard_3": {
-        "products": [
-            "ga_ls5t_ard_3",
-            "ga_ls7e_ard_3",
-            "ga_ls8c_ard_3",
-            "ga_ls9c_ard_3",
-        ],
-        "styles": {
-            "True colour": ("true_colour", ["nbart_red", "nbart_green", "nbart_blue"]),
-            "False colour": (
-                "false_colour",
-                ["nbart_swir_1", "nbart_nir", "nbart_green"],
-            ),
-        },
+    'ga_ls_ard_3': {
+        'products': ['ga_ls5t_ard_3', 'ga_ls7e_ard_3', 'ga_ls8c_ard_3'],
+        'styles': {
+            'True colour':
+                ('true_colour', ['nbart_red', 'nbart_green', 'nbart_blue']),
+            'False colour':
+                ('false_colour', ['nbart_swir_1', 'nbart_nir', 'nbart_green'])
+        }
     },
-    "ga_s2m_ard_3": {
-        "products": ["ga_s2am_ard_3", "ga_s2bm_ard_3"],
-        "styles": {
-            "True colour": ("simple_rgb", ["nbart_red", "nbart_green", "nbart_blue"]),
-            "False colour": (
-                "infrared_green",
-                ["nbart_swir_2", "nbart_nir_1", "nbart_green"],
-            ),
-        },
+    's2_ard_granule_nbar_t': {
+        'products': ['s2a_ard_granule', 's2b_ard_granule'],
+        'styles': {
+            'True colour':
+                ('simple_rgb', ['nbart_red', 'nbart_green', 'nbart_blue']),
+            'False colour': ('infrared_green',
+                             ['nbart_swir_2', 'nbart_nir_1', 'nbart_green'])
+        }
     },
+    's2_nrt_granule_nbar_t': {
+        'products': ['s2a_nrt_granule', 's2b_nrt_granule'],
+        'styles': {
+            'True colour':
+                ('simple_rgb', ['nbart_red', 'nbart_green', 'nbart_blue']),
+            'False colour': ('infrared_green',
+                             ['nbart_swir_2', 'nbart_nir_1', 'nbart_green'])
+        }
+    }
 }
 
 
 def make_box_layout():
     return Layout(
         #         border='solid 1px black',
-        margin="0px 10px 10px 0px",
-        padding="5px 5px 5px 5px",
-        width="100%",
-        height="100%",
+        margin='0px 10px 10px 0px',
+        padding='5px 5px 5px 5px',
+        width='100%',
+        height='100%',
     )
 
 
 def create_expanded_button(description, button_style):
     return Button(
         description=description,
         button_style=button_style,
         layout=Layout(width="auto", height="auto"),
     )
 
 
 def update_map_layers(self):
     """
     Updates map to add new DEA layers, styles or basemap when selected
-    using menu options. Triggers data reload by resetting load params
+    using menu options. Triggers data reload by resetting load params 
     and output arrays.
     """
 
     # Clear data load params to trigger data re-load
     self.rgb_array = None
     self.sensor = None
     self.load_params = None
     self.query_params = None
 
     # Clear all layers and add basemap
     self.map_layers.clear_layers()
     self.map_layers.add_layer(self.basemap)
 
     # Get style name for specific satellite sensor
-    style = sat_params[self.dealayer]["styles"][self.style][0]
+    style = sat_params[self.dealayer]['styles'][self.style][0]
 
     # Add DEA layers over the top of the basemap
-    dea_layer = deawidgets.create_dea_wms_layer(self.dealayer, self.date, styles=style)
+    dea_layer = deawidgets.create_dea_wms_layer(self.dealayer,
+                                                self.date,
+                                                styles=style)
     self.map_layers.add_layer(dea_layer)
-
-
+    
+    
+    
 def extract_data(self):
-
+    
     # Connect to datacube database
     dc = datacube.Datacube(app="Exporting satellite images")
 
     # Configure local dask cluster
-    client = create_local_dask_cluster(return_client=True, display_client=True)
+    client = create_local_dask_cluster(return_client=True,
+                                       display_client=True)
 
     # Convert to geopolygon
-    geopolygon = Geometry(geom=self.gdf_drawn.geometry[0], crs=self.gdf_drawn.crs)
+    geopolygon = Geometry(geom=self.gdf_drawn.geometry[0],
+                          crs=self.gdf_drawn.crs)
 
     # Create query after adjusting interval time to UTC by
     # adding a UTC offset of -10 hours. This results issues
     # on the east coast of Australia where satelite overpasses
     # can occur on either side of 24:00 hours UTC
-    start_date = np.datetime64(self.date) - np.timedelta64(10, "h")
-    end_date = np.datetime64(self.date) + np.timedelta64(14, "h")
+    start_date = np.datetime64(self.date) - np.timedelta64(10, 'h')
+    end_date = np.datetime64(self.date) + np.timedelta64(14, 'h')
     self.query_params = {
-        "time": (str(start_date), str(end_date)),
-        "geopolygon": geopolygon,
+        'time': (str(start_date), str(end_date)),
+        'geopolygon': geopolygon
     }
 
     # Find matching datasets
     dss = [
         dc.find_datasets(product=i, **self.query_params)
-        for i in sat_params[self.dealayer]["products"]
+        for i in sat_params[self.dealayer]['products']
     ]
     dss = list(itertools.chain.from_iterable(dss))
-
+    
     # If data is found
     if len(dss) > 0:
 
         # Get CRS
         crs = str(dss[0].crs)
 
         # Get sensor (try/except to account for different S2 NRT metadata)
         try:
-            sensor = dss[0].metadata_doc["properties"]["eo:platform"].capitalize()
+            sensor = dss[0].metadata_doc['properties'][
+                'eo:platform'].capitalize()
         except:
-            sensor = dss[0].metadata_doc["platform"]["code"].capitalize()
-        self.sensor = sensor[0:-1].replace("_", "-") + sensor[-1].capitalize()
+            sensor = dss[0].metadata_doc['platform']['code'].capitalize(
+            )
+        self.sensor = sensor[0:-1].replace(
+            '_', '-') + sensor[-1].capitalize()
 
         # Meets pansharpening requirements
-        can_pansharpen = self.style == "True colour" and self.sensor in [
-            "Landsat-7",
-            "Landsat-8",
-            "Landsat-9",
+        can_pansharpen = self.style == 'True colour' and self.sensor in [
+            'Landsat-7', 'Landsat-8'
         ]
 
         # Set up load params
         if self.pansharpen and can_pansharpen:
             self.load_params = {
-                "measurements": sat_params[self.dealayer]["styles"][self.style][1]
-                + ["nbart_panchromatic"],
-                "resolution": (-self.resolution, self.resolution),
-                "align": (7.5, 7.5),
-                "output_crs": crs,
+                'measurements':
+                    sat_params[self.dealayer]['styles'][self.style][1] +
+                    ['nbart_panchromatic'],
+                'resolution': (-self.resolution, self.resolution),
+                'align': (7.5, 7.5),
+                'output_crs':
+                    crs
             }
 
         else:
 
             # Use resolution if provided, otherwise use default
             if self.resolution:
-                sat_params[self.dealayer]["resolution"] = (
-                    -self.resolution,
-                    self.resolution,
-                )
+                sat_params[self.dealayer]['resolution'] = (
+                    -self.resolution, self.resolution)
 
             self.load_params = {
-                "measurements": sat_params[self.dealayer]["styles"][self.style][1],
-                "resolution": (-self.resolution, self.resolution),
-                "output_crs": crs,
-                "skip_broken_datasets": True,
+                'measurements':
+                    sat_params[self.dealayer]['styles'][self.style][1],
+                'resolution': (-self.resolution, self.resolution),
+                'output_crs':
+                    crs
             }
 
         # Load data from datasets
-        print(f"Loading {self.sensor} satellite data")
-        ds = dc.load(
-            datasets=dss,
-            resampling="bilinear",
-            group_by="solar_day",
-            dask_chunks={"time": 1, "x": 2048, "y": 2048},
-            **self.load_params,
-            **self.query_params,
-        )
+        print(f'Loading {self.sensor} satellite data')
+        ds = dc.load(datasets=dss,
+                     resampling='bilinear',
+                     group_by='solar_day',
+                     dask_chunks={
+                         'time': 1,
+                         'x': 2048,
+                         'y': 2048
+                     },
+                     **self.load_params,
+                     **self.query_params)
         ds = masking.mask_invalid_data(ds)
 
         # Create plain numpy array, optionally after pansharpening
         if self.pansharpen and can_pansharpen:
 
-            # Perform Brovey pan-sharpening and return numpy.array
-            print(f"Pansharpening {self.sensor} image to 15 m resolution")
-            rgb_array = (
-                xr_pansharpen(ds, transform="brovey").to_array().squeeze("time").values
-            )
+            # Perform Brovey pan-sharpening and return three numpy.arrays
+            print(
+                f'Pansharpening {self.sensor} image to 15 m resolution')
+            red_sharpen, green_sharpen, blue_sharpen = pan_sharpen_brovey(
+                band_1=ds.nbart_red,
+                band_2=ds.nbart_green,
+                band_3=ds.nbart_blue,
+                pan_band=ds.nbart_panchromatic)
+            rgb_array = np.vstack(
+                [red_sharpen, green_sharpen, blue_sharpen])
+
+            # Match histogram to original array
+            from skimage.exposure import match_histograms
+            original_array = ds.drop(
+                'nbart_panchromatic').to_array().squeeze('time').values
+            rgb_array = match_histograms(image=rgb_array,
+                                         reference=original_array,
+                                         multichannel=True)
 
-        # If pansharpening is requested but not possible, deactivate
+        # If pansharpening is requested but not possible, deactivate 
         # pansharpening and reset to 30 m resolution
         elif self.pansharpen and not can_pansharpen:
-            print("\nUnable to pansharpen; reverting to 30 m resolution")
+            print(
+                '\nUnable to pansharpen; reverting to 30 m resolution'
+            )
             self.checkbox_pansharpen.value = False
             self.text_resolution.disabled = False
             self.text_resolution.value = 30
             rgb_array = ds.isel(time=0).to_array().values
 
         else:
             rgb_array = ds.isel(time=0).to_array().values
 
         # Transpose numpy array
         rgb_array = np.transpose(rgb_array, axes=[1, 2, 0])
-
+    
     # Else if no data is returned, return None
     else:
         rgb_array = None
-
+        
     # Close down the dask client
     client.close()
-
+        
     return rgb_array
 
 
 def plot_data(self, fname):
-
+    
     # Data to plot
     to_plot = self.rgb_array
 
     # If percentile stretch is supplied, calculate vmin and vmax
     # from percentiles
     if self.percentile_stretch:
         vmin, vmax = np.nanpercentile(to_plot, self.percentile_stretch)
     else:
         vmin, vmax = self.vmin, self.vmax
 
     # Raise by power to dampen bright features and enhance dark.
     # Raise vmin and vmax by same amount to ensure proper stretch
     if self.power < 1.0:
         with self.status_info:
-            print(f"\nApplying power transformation ({self.power})")
+            print(f'\nApplying power transformation ({self.power})')
         to_plot = to_plot ** self.power
         vmin, vmax = vmin ** self.power, vmax ** self.power
-
+        
     # Rescale/stretch imagery between vmin and vmax
-    to_plot = exposure.rescale_intensity(
-        to_plot.astype(float), in_range=(vmin, vmax), out_range=(0.0, 1.0)
-    )
-
+    to_plot = exposure.rescale_intensity(to_plot.astype(float),
+                                         in_range=(vmin, vmax),
+                                         out_range=(0.0, 1.0))
+    
     # Unsharp mask
     if self.unsharp_mask:
         with self.status_info:
-            print(
-                f"\nApplying unsharp masking with {self.unsharp_mask_radius} "
-                f"radius and {self.unsharp_mask_amount} amount"
-            )
-        to_plot = unsharp_mask(
-            to_plot, radius=self.unsharp_mask_radius, amount=self.unsharp_mask_amount
-        )
+            print(f'\nApplying unsharp masking with {self.unsharp_mask_radius} '
+                  f'radius and {self.unsharp_mask_amount} amount')
+        to_plot = unsharp_mask(to_plot, 
+                               radius=self.unsharp_mask_radius, 
+                               amount=self.unsharp_mask_amount)       
 
+    
     # Create figure with aspect ratio of data
     fig = plt.figure(dpi=100)
     fig.set_size_inches(10, 10 / (to_plot.shape[1] / to_plot.shape[0]))
 
     # Remove axes to plot just array data
-    ax = plt.Axes(
-        fig,
-        [0.0, 0.0, 1.0, 1.0],
-    )
+    ax = plt.Axes(fig, [0., 0., 1., 1.],)
     ax.set_axis_off()
     fig.add_axes(ax)
 
     # Add data to plot
     ax.imshow(to_plot)
-
+        
     # If a min DPI is specified and image is less than DPI
     if (self.dpi > 0) and (to_plot.shape[1] < self.dpi * 10):
-
+        
         # Export figure to file using exact DPI
         with self.status_info:
-            print(f"\nExporting image at {self.dpi} DPI")
-        fig.savefig(
-            fname.replace("resolution", f"resolution, {self.dpi} DPI"), dpi=self.dpi
-        )
-
+            print(f'\nExporting image at {self.dpi} DPI')
+        fig.savefig(fname.replace('resolution', 
+                                  f'resolution, {self.dpi} DPI'), 
+                    dpi=self.dpi)
+        
     # If no minumum DPI is specified, export raw array data in native
     # resolution
     else:
-        plt.imsave(
-            fname=fname, arr=np.ascontiguousarray(to_plot), format=self.output_format
-        )
-
+        plt.imsave(fname=fname,
+                   arr=np.ascontiguousarray(to_plot),
+                   format=self.output_format)
+        
     # Add plot preview below map and finish
     plt.show()
     with self.status_info:
-        print(f"\nImage successfully exported to:\n{fname}.")
+        print(f'\nImage successfully exported to:\n{fname}.')
+    
+
 
 
 class imageexport_app(HBox):
+
     def __init__(self):
         super().__init__()
 
         ######################
         # INITIAL ATTRIBUTES #
         ######################
 
         # Basemap
         self.basemap_list = [
-            ("Open Street Map", basemap_to_tiles(basemaps.OpenStreetMap.Mapnik)),
-            ("ESRI World Imagery", basemap_to_tiles(basemaps.Esri.WorldImagery)),
+            ("Open Street Map",
+             basemap_to_tiles(basemaps.OpenStreetMap.Mapnik)),
+            ("ESRI World Imagery",
+             basemap_to_tiles(basemaps.Esri.WorldImagery)),
         ]
         self.basemap = self.basemap_list[0][1]
 
-        # Satellite data using yesterday's date
-        date = datetime.datetime.today()
-        date = datetime.datetime(year=date.year, month=date.month, day=date.day - 1)
-        self.date = date.strftime("%Y-%m-%d")
+        # Satellite data
+        self.date = "2021-12-31"
         self.dealayer_list = [
-            ("Landsat", "ga_ls_ard_3"),
-            ("Sentinel-2", "ga_s2m_ard_3"),
+            ("Landsat", 'ga_ls_ard_3'),
+            ("Sentinel-2", 's2_ard_granule_nbar_t'),
+            ("Sentinel-2 NRT", 's2_nrt_granule_nbar_t'),
         ]
         self.dealayer = self.dealayer_list[0][1]
 
         # Styles
         self.styles_list = ["True colour", "False colour"]
         self.style = self.styles_list[0]
 
@@ -351,16 +377,16 @@
         self.resolution = 30
         self.pansharpen = False
         self.standardise_name = False
         self.vmin = 50
         self.vmax = 3000
         self.percentile_stretch = None  # (1, 99)
         self.power = 1.0
-        self.output_list = [("JPG", "jpg"), ("PNG", "png")]
-        self.output_format = self.output_list[0][1]
+        self.output_list = [("JPG", 'jpg'), ("PNG", 'png')]
+        self.output_format = self.output_list[0][1]        
         self.unsharp_mask = False
         self.unsharp_mask_radius = 20
         self.unsharp_mask_amount = 0.3
         self.max_size = False
         self.dpi = 0
 
         # Drawing params
@@ -376,22 +402,21 @@
 
         ##################
         # HEADER FOR APP #
         ##################
 
         # Create the Header widget
         header_title_text = "<h3>Digital Earth Australia satellite image export</h3>"
-        instruction_text = (
-            "<p>Select the desired satellite data, imagery "
-            "date and image style, zoom in until satellite "
-            "imagery appears on the map, then draw a "
-            "rectangle to select an area of imagery to "
-            "export as a high-resolution image file.</p>"
-        )
-        self.header = deawidgets.create_html(f"{header_title_text}{instruction_text}")
+        instruction_text = ("<p>Select the desired satellite data, imagery "
+                            "date and image style, zoom in until satellite "
+                            "imagery appears on the map, then draw a "
+                            "rectangle to select an area of imagery to "
+                            "export as a high-resolution image file.</p>")
+        self.header = deawidgets.create_html(
+            f"{header_title_text}{instruction_text}")
         self.header.layout = make_box_layout()
 
         #####################################
         # HANDLER FUNCTION FOR DRAW CONTROL #
         #####################################
 
         # Define the action to take once something is drawn on the map
@@ -412,75 +437,57 @@
             io = BytesIO(binary_data)
             io.seek(0)
             gdf = gpd.read_file(io)
             gdf.crs = "EPSG:4326"
 
             # Convert to Albers and compute area
             gdf_drawn_albers = gdf.copy().to_crs("EPSG:3577")
-            m2_per_km2 = 10 ** 6
+            m2_per_km2 = 10**6
             area = gdf_drawn_albers.area.values[0] / m2_per_km2
-            polyarea_label = "Total area of satellite data to extract"
+            polyarea_label = 'Total area of satellite data to extract'
             polyarea_text = f"<b>{polyarea_label}</b>: {area:.2f} km<sup>2</sup>"
 
             # Test area size
             if self.max_size:
-                confirmation_text = (
-                    '<span style="color: #33cc33"> '
-                    "<b>(Overriding maximum size limit; use with caution as may lead to memory issues)</b></span>"
-                )
-                self.header.value = (
-                    header_title_text
-                    + instruction_text
-                    + polyarea_text
-                    + confirmation_text
-                )
-                self.gdf_drawn = gdf
+                confirmation_text = ('<span style="color: #33cc33"> '
+                                     '<b>(Overriding maximum size limit; use with caution as may lead to memory issues)</b></span>')
+                self.header.value = header_title_text + instruction_text + polyarea_text + confirmation_text
+                self.gdf_drawn = gdf                
             elif area <= 10000:
-                confirmation_text = (
-                    '<span style="color: #33cc33"> '
-                    "<b>(Area to extract falls within "
-                    "recommended limit)</b></span>"
-                )
-                self.header.value = (
-                    header_title_text
-                    + instruction_text
-                    + polyarea_text
-                    + confirmation_text
-                )
+                confirmation_text = ('<span style="color: #33cc33"> '
+                                     '<b>(Area to extract falls within '
+                                     'recommended limit)</b></span>')
+                self.header.value = header_title_text + instruction_text + polyarea_text + confirmation_text
                 self.gdf_drawn = gdf
             else:
-                warning_text = (
-                    '<span style="color: #ff5050"> '
-                    "<b>(Area to extract is too large, "
-                    "please select an area less than 10000 "
-                    "km<sup>2)</b></span>"
-                )
-                self.header.value = (
-                    header_title_text + instruction_text + polyarea_text + warning_text
-                )
+                warning_text = ('<span style="color: #ff5050"> '
+                                '<b>(Area to extract is too large, '
+                                'please select an area less than 10000 '
+                                'km<sup>2)</b></span>')
+                self.header.value = header_title_text + instruction_text + polyarea_text + warning_text
                 self.gdf_drawn = None
 
         ###########################
         # WIDGETS FOR APP OUTPUTS #
         ###########################
 
         self.status_info = Output(layout=make_box_layout())
         self.output_plot = Output(layout=make_box_layout())
 
         #########################################
         # MAP WIDGET, DRAWING TOOLS, WMS LAYERS #
         #########################################
 
         # Create drawing tools
-        desired_drawtools = ["rectangle"]
+        desired_drawtools = ['rectangle']
         draw_control = deawidgets.create_drawcontrol(desired_drawtools)
 
         # Begin by displaying an empty layer group, and update the group with desired WMS on interaction.
         self.map_layers = LayerGroup(layers=())
-        self.map_layers.name = "Map Overlays"
+        self.map_layers.name = 'Map Overlays'
 
         # Create map widget
         self.m = deawidgets.create_map(map_center=(-28, 135), zoom_level=4)
         self.m.layout = make_box_layout()
 
         # Add tools to map widget
         self.m.add_control(draw_control)
@@ -490,109 +497,87 @@
         update_map_layers(self)
 
         ############################
         # WIDGETS FOR APP CONTROLS #
         ############################
 
         # Create parameter widgets
-        dropdown_basemap = deawidgets.create_dropdown(
-            self.basemap_list, self.basemap_list[0][1]
-        )
-        dropdown_dealayer = deawidgets.create_dropdown(
-            self.dealayer_list, self.dealayer_list[0][1]
-        )
-        dropdown_output = deawidgets.create_dropdown(
-            self.output_list, self.output_list[0][1]
-        )
-        date_picker = deawidgets.create_datepicker(value=date)
-        dropdown_styles = deawidgets.create_dropdown(
-            self.styles_list, self.styles_list[0]
-        )
-        slider_abs = widgets.IntRangeSlider(
-            value=[50, 3000],
-            min=0,
-            max=10000,
-            step=25,
-            description="",
-            layout={"width": "85%"},
-        )
+        dropdown_basemap = deawidgets.create_dropdown(self.basemap_list,
+                                                      self.basemap_list[0][1])
+        dropdown_dealayer = deawidgets.create_dropdown(self.dealayer_list,
+                                                       self.dealayer_list[0][1])
+        dropdown_output = deawidgets.create_dropdown(self.output_list,
+                                                     self.output_list[0][1])
+        date_picker = deawidgets.create_datepicker(
+            value=datetime.date(2021, 12, 31))
+        dropdown_styles = deawidgets.create_dropdown(self.styles_list,
+                                                     self.styles_list[0])
+        slider_abs = widgets.IntRangeSlider(value=[50, 3000],
+                                            min=0,
+                                            max=10000,
+                                            step=25,
+                                            description='',
+                                            layout={'width': '85%'})
         run_button = create_expanded_button("Export imagery", "info")
 
         # Expandable advanced section
-        text_resolution = widgets.FloatText(
-            value=30,
-            description="",
-            layout={"width": "100%", "margin": "0px", "padding": "0px"},
-        )
+        text_resolution = widgets.FloatText(value=30,
+                                            description='',
+                                            layout={'width': '100%',
+                                                    'margin': '0px',
+                                                    'padding': '0px'})
         checkbox_pansharpen = deawidgets.create_checkbox(
-            self.pansharpen, "Pansharpen Landsat"
-        )
-        slider_power = widgets.FloatSlider(
-            value=1.0,
-            min=0.01,
-            max=1.0,
-            step=0.01,
-            description="",
-            layout={"width": "85%"},
-        )
+            self.pansharpen, 'Pansharpen Landsat')
+        slider_power = widgets.FloatSlider(value=1.0,
+                                           min=0.01,
+                                           max=1.0,
+                                           step=0.01,
+                                           description='',
+                                            layout={'width': '85%'})
         checkbox_unsharp_mask = deawidgets.create_checkbox(
-            self.unsharp_mask, "Enable", layout={"width": "100%"}
-        )
-        text_unsharp_mask_radius = widgets.FloatText(
-            value=20,
-            step=1,
-            description="Radius",
-            layout={
-                "width": "100%",
-                "margin": "0px",
-                "padding": "0px",
-                "display": "none",
-            },
-        )
-        text_unsharp_mask_amount = widgets.FloatText(
-            value=0.3,
-            step=0.1,
-            description="Amount",
-            layout={
-                "width": "100%",
-                "margin": "0px",
-                "padding": "0px",
-                "display": "none",
-            },
-        )
-        checkbox_max_size = deawidgets.create_checkbox(self.max_size, "Enable")
-        text_dpi = widgets.IntText(
-            value=0, description="", step=50, layout={"width": "85%"}
-        )
-        html_dpi = HTML(
-            "</br>Minimum DPI for image export</br>(100 DPI = 1000 pixels wide):"
-        )
-        expand_box = widgets.VBox(
-            [
-                HTML("Resolution (metres):"),
-                text_resolution,
-                checkbox_pansharpen,
-                HTML("</br>Apply power transformation to darken bright features:"),
-                slider_power,
-                HTML("</br>Apply unsharp masking to sharpen image:"),
-                checkbox_unsharp_mask,
-                text_unsharp_mask_radius,
-                text_unsharp_mask_amount,
-                HTML(
-                    "</br>Override maximum size limit: (use with caution; may cause memory issues/crashes)"
-                ),
-                checkbox_max_size,
-                html_dpi,
-                text_dpi,
-            ],
-            layout={"overflow": "hidden"},
-        )
+            self.unsharp_mask, 'Enable', layout={'width': '100%'})
+        text_unsharp_mask_radius = widgets.FloatText(value=20,
+                                                     step=1,
+                                                     description='Radius',
+                                                     layout={'width': '100%',
+                                                             'margin': '0px',
+                                                             'padding': '0px',
+                                                             'display': 'none'})
+        text_unsharp_mask_amount = widgets.FloatText(value=0.3,
+                                                     step=0.1,
+                                                     description='Amount',
+                                                     layout={'width': '100%',
+                                                             'margin': '0px',
+                                                             'padding': '0px',
+                                                             'display': 'none'})
+        checkbox_max_size = deawidgets.create_checkbox(
+            self.max_size, 'Enable')        
+        text_dpi = widgets.IntText(value=0, 
+                                     description="", 
+                                     step=50, 
+                                     layout={'width': '85%'})
+        html_dpi = HTML('</br>Minimum DPI for image export</br>(100 DPI = 1000 pixels wide):')        
+        expand_box = widgets.VBox([HTML('Resolution (metres):'),
+                                   text_resolution,
+                                   checkbox_pansharpen,
+                                   HTML('</br>Apply power transformation to darken bright features:'),
+                                   slider_power,
+                                   HTML('</br>Apply unsharp masking to sharpen image:'),
+                                   checkbox_unsharp_mask,
+                                   text_unsharp_mask_radius,
+                                   text_unsharp_mask_amount,
+                                   HTML('</br>Override maximum size limit: (use with caution; may cause memory issues/crashes)'),
+                                   checkbox_max_size,
+                                   html_dpi,
+                                   text_dpi],
+                                  layout={'overflow': 'hidden'},
+                                 )
 
         expand = widgets.Accordion(children=[expand_box], selected_index=None)
-        expand.set_title(0, "Advanced")
+        expand.set_title(0, 'Advanced')
 
         # Add specific dialogs to class so they can be modified
         self.text_resolution = text_resolution
         self.checkbox_pansharpen = checkbox_pansharpen
         self.text_unsharp_mask_radius = text_unsharp_mask_radius
         self.text_unsharp_mask_amount = text_unsharp_mask_amount
         self.html_dpi = html_dpi
@@ -606,51 +591,48 @@
         dropdown_basemap.observe(self.update_basemap, "value")
         dropdown_dealayer.observe(self.update_dealayer, "value")
         dropdown_styles.observe(self.update_styles, "value")
         dropdown_output.observe(self.update_output, "value")
         run_button.on_click(self.run_app)
         draw_control.on_draw(update_geojson)
         slider_abs.observe(self.update_slider_abs, "value")
-
+        
         # Advanced params
         text_resolution.observe(self.update_text_resolution, "value")
         checkbox_pansharpen.observe(self.update_checkbox_pansharpen, "value")
         slider_power.observe(self.update_slider_power, "value")
         checkbox_unsharp_mask.observe(self.update_checkbox_unsharp_mask, "value")
         text_unsharp_mask_radius.observe(self.update_text_unsharp_mask_radius, "value")
         text_unsharp_mask_amount.observe(self.update_text_unsharp_mask_amount, "value")
         checkbox_max_size.observe(self.update_checkbox_max_size, "value")
         text_dpi.observe(self.update_dpi, "value")
+        
 
         ##################################
         # COLLECTION OF ALL APP CONTROLS #
         ##################################
 
-        parameter_selection = VBox(
-            [
-                HTML("<b>Date:</b>"),
-                date_picker,
-                HTML("<b>Satellite imagery:</b>"),
-                dropdown_dealayer,
-                HTML("<b>Style:</b>"),
-                dropdown_styles,
-                HTML("<b>Colour stretch:</b>"),
-                slider_abs,
-                HTML("<b>Output file format:</b>"),
-                dropdown_output,
-                HTML("</br>"),
-                expand,
-            ]
-        )
-        map_selection = VBox(
-            [
-                HTML("</br><b>Map overlay:</b>"),
-                dropdown_basemap,
-            ]
-        )
+        parameter_selection = VBox([
+            HTML("<b>Date:</b>"),
+            date_picker,
+            HTML('<b>Satellite imagery:</b>'),
+            dropdown_dealayer,
+            HTML('<b>Style:</b>'),
+            dropdown_styles,
+            HTML('<b>Colour stretch:</b>'),
+            slider_abs,
+            HTML('<b>Output file format:</b>'),
+            dropdown_output,
+            HTML('</br>'),
+            expand,
+        ])
+        map_selection = VBox([
+            HTML("</br><b>Map overlay:</b>"),
+            dropdown_basemap,
+        ])
         parameter_selection.layout = make_box_layout()
         map_selection.layout = make_box_layout()
 
         ###############################
         # SPECIFICATION OF APP LAYOUT #
         ###############################
 
@@ -697,15 +679,15 @@
     def update_date(self, change):
         self.date = str(change.new)
         update_map_layers(self)
 
     # Update colour stretch
     def update_slider_abs(self, change):
         self.vmin, self.vmax = change.new
-
+    
     # Update power transform
     def update_slider_power(self, change):
         self.power = change.new
 
     # Enable pansharpening and reset/deactivate resolution
     def update_checkbox_pansharpen(self, change):
         self.pansharpen = change.new
@@ -714,49 +696,47 @@
         # disable input if so
         if change.new:
             self.text_resolution.value = 15
             self.text_resolution.disabled = True
         else:
             self.text_resolution.value = 30
             self.text_resolution.disabled = False
-
+            
     # Enable unsharp masking and show/hide custom params
     def update_checkbox_unsharp_mask(self, change):
         self.unsharp_mask = change.new
-
+        
         # Show unsharp masking params in menu if activated
         if change.new:
-            self.text_unsharp_mask_radius.layout.display = "block"
-            self.text_unsharp_mask_amount.layout.display = "block"
+            self.text_unsharp_mask_radius.layout.display = 'block'
+            self.text_unsharp_mask_amount.layout.display = 'block'
         else:
-            self.text_unsharp_mask_radius.layout.display = "none"
-            self.text_unsharp_mask_amount.layout.display = "none"
-
+            self.text_unsharp_mask_radius.layout.display = 'none'
+            self.text_unsharp_mask_amount.layout.display = 'none'
+            
     # Change unsharp masking radius
     def update_text_unsharp_mask_radius(self, change):
         self.unsharp_mask_radius = change.new
-
+        
     # Change unsharp masking amount
     def update_text_unsharp_mask_amount(self, change):
         self.unsharp_mask_amount = change.new
-
+        
     # Override max size limit
     def update_checkbox_max_size(self, change):
         self.max_size = change.new
-
+        
     # Override min DPI
     def update_dpi(self, change):
         self.dpi = change.new
-
+        
         # Update DPI helper text to give output resolution
-        self.html_dpi.value = (
-            f"</br>Minimum DPI for image export</br>"
-            f"({change.new} DPI = {change.new * 10} "
-            f"pixels wide):"
-        )
+        self.html_dpi.value = (f'</br>Minimum DPI for image export</br>'
+                               f'({change.new} DPI = {change.new * 10} '
+                               f'pixels wide):')
 
     # Update resolution
     def update_text_resolution(self, change):
         self.resolution = change.new
 
         # Clear data load params to trigger data re-load
         self.rgb_array = None
@@ -764,15 +744,15 @@
         self.load_params = None
         self.query_params = None
 
     # Change layers shown on the map
     def update_dealayer(self, change):
         self.dealayer = change.new
 
-        if change.new == "ga_ls_ard_3":
+        if change.new == 'ga_ls_ard_3':
             self.text_resolution.value = 30
             self.checkbox_pansharpen.disabled = False
 
             if self.pansharpen:
                 self.text_resolution.value = 15
                 self.text_resolution.disabled = True
 
@@ -798,64 +778,54 @@
         self.output_format = change.new
 
     def run_app(self, change):
 
         # Clear progress bar and output areas before running
         self.status_info.clear_output()
         self.output_plot.clear_output()
-
+        
         # Verify that polygon was drawn
         if self.gdf_drawn is not None:
 
             with self.status_info:
 
-                # Load data and add to attribute
-                if self.rgb_array is None:
-                    self.rgb_array = extract_data(self)
-                else:
-                    print("Using previously loaded data")
+                    # Load data and add to attribute
+                    if self.rgb_array is None:
+                        self.rgb_array = extract_data(self)                            
+                    else:
+                        print('Using previously loaded data')                        
 
             if self.rgb_array is not None:
-
+                
                 with self.status_info:
 
                     # Create unique file name
                     centre_coords = self.gdf_drawn.geometry[0].centroid.coords[0][::-1]
                     site = reverse_geocode(coords=centre_coords)
-                    fname = (
-                        f"{self.sensor} - {self.date} - {site} - {self.style}, "
-                        f"{self.resolution:.0f} m resolution.{self.output_format}"
-                    )
+                    fname = (f"{self.sensor} - {self.date} - {site} - {self.style}, "
+                             f"{self.resolution:.0f} m resolution.{self.output_format}")
 
                     # Remove spaces and commas if requested
                     if self.standardise_name:
-                        fname = (
-                            fname.replace(" - ", "_")
-                            .replace(", ", "-")
-                            .replace(" ", "-")
-                            .lower()
-                        )
-
-                    print(
-                        f"\nExporting image for {site}.\nThis may take several minutes..."
-                    )
+                        fname = (fname
+                                 .replace(' - ', '_')
+                                 .replace(', ', '-')
+                                 .replace(' ', '-').lower())
+
+                    print(f'\nExporting image for {site}.\nThis may take several minutes...')
 
                 ############
                 # Plotting #
                 ############
 
-                with self.output_plot:
+                with self.output_plot:            
                     plot_data(self, fname)
-
+            
             else:
                 with self.status_info:
-                    print(
-                        "No satellite data found in the selected area. "
-                        "Please select a new rectangle over an area with "
-                        "satellite imagery visible on the map."
-                    )
-
+                    print('No satellite data found in the selected area. '
+                          'Please select a new rectangle over an area with '
+                          'satellite imagery visible on the map.')
+        
         else:
             with self.status_info:
-                print(
-                    'Please draw a valid rectangle on the map, then press "Export imagery"'
-                )
+                print('Please draw a valid rectangle on the map, then press "Export imagery"')
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/miningrehab.py` & `dea-tools-0.2.8.dev9/dea_tools/app/miningrehab.py`

 * *Files identical despite different names*

### Comparing `dea-tools-0.2.8.dev81/dea_tools/app/widgetconstructors.py` & `dea-tools-0.2.8.dev9/dea_tools/app/widgetconstructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 '''
-Functions for defining widgets for interactive Digital Earth Australia notebooks. 
-
-These functions are directly modified from 
+Description: Functions for easily defining widgets for Digital Earth 
+Australia notebooks. These functions are directly modified from 
 originals developed by Digital Earth Africa: 
 https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/blob/main/Tools/deafrica_tools/app/widgetconstructors.py
 
 License: The code in this notebook is licensed under the Apache License, 
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/bandindices.py` & `dea-tools-0.2.8.dev9/dea_tools/bandindices.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,88 +35,79 @@
     a set of remote sensing indices, and adds the resulting array as a 
     new variable in the original dataset.  
     
     Note: by default, this function will create a new copy of the data
     in memory. This can be a memory-expensive operation, so to avoid
     this, set `inplace=True`.
 
-    Last modified: April 2023
+    Last modified: March 2021
     
     Parameters
     ----------
     ds : xarray Dataset
         A two-dimensional or multi-dimensional array with containing the
         spectral bands required to calculate the index. These bands are
         used as inputs to calculate the selected water index.
     index : str or list of strs
         A string giving the name of the index to calculate or a list of
         strings giving the names of the indices to calculate:
-        
-        * ``'AWEI_ns'`` (Automated Water Extraction Index,
+        'AWEI_ns (Automated Water Extraction Index,
                   no shadows, Feyisa 2014)
-        * ``'AWEI_sh'`` (Automated Water Extraction Index,
+        'AWEI_sh' (Automated Water Extraction Index,
                    shadows, Feyisa 2014)
-        * ``'BAEI'`` (Built-Up Area Extraction Index, Bouzekri et al. 2015)
-        * ``'BAI'`` (Burn Area Index, Martin 1998)
-        * ``'BSI'`` (Bare Soil Index, Rikimaru et al. 2002)
-        * ``'BUI'`` (Built-Up Index, He et al. 2010)
-        * ``'CMR'`` (Clay Minerals Ratio, Drury 1987)
-        * ``'EVI'`` (Enhanced Vegetation Index, Huete 2002)
-        * ``'FMR'`` (Ferrous Minerals Ratio, Segal 1982)
-        * ``'IOR'`` (Iron Oxide Ratio, Segal 1982)
-        * ``'LAI'`` (Leaf Area Index, Boegh 2002)
-        * ``'MNDWI'`` (Modified Normalised Difference Water Index, Xu 1996)
-        * ``'MSAVI'`` (Modified Soil Adjusted Vegetation Index,
+        'BAEI' (Built-Up Area Extraction Index, Bouzekri et al. 2015)
+        'BAI' (Burn Area Index, Martin 1998)
+        'BSI' (Bare Soil Index, Rikimaru et al. 2002)
+        'BUI' (Built-Up Index, He et al. 2010)
+        'CMR' (Clay Minerals Ratio, Drury 1987)
+        'EVI' (Enhanced Vegetation Index, Huete 2002)
+        'FMR' (Ferrous Minerals Ratio, Segal 1982)
+        'IOR' (Iron Oxide Ratio, Segal 1982)
+        'LAI' (Leaf Area Index, Boegh 2002)
+        'MNDWI' (Modified Normalised Difference Water Index, Xu 1996)
+        'MSAVI' (Modified Soil Adjusted Vegetation Index,
                  Qi et al. 1994)              
-        * ``'NBI'`` (New Built-Up Index, Jieli et al. 2010)
-        * ``'NBR'`` (Normalised Burn Ratio, Lopez Garcia 1991)
-        * ``'NDBI'`` (Normalised Difference Built-Up Index, Zha 2003)
-        * ``'NDCI'`` (Normalised Difference Chlorophyll Index, 
+        'NBI' (New Built-Up Index, Jieli et al. 2010)
+        'NBR' (Normalised Burn Ratio, Lopez Garcia 1991)
+        'NDBI' (Normalised Difference Built-Up Index, Zha 2003)
+        'NDCI' (Normalised Difference Chlorophyll Index, 
                 Mishra & Mishra, 2012)
-        * ``'NDMI'`` (Normalised Difference Moisture Index, Gao 1996)        
-        * ``'NDSI'`` (Normalised Difference Snow Index, Hall 1995)
-        * ``'NDTI'`` (Normalise Difference Tillage Index,
+        'NDMI' (Normalised Difference Moisture Index, Gao 1996)        
+        'NDSI' (Normalised Difference Snow Index, Hall 1995)
+        'NDTI' (Normalise Difference Tillage Index,
                 Van Deventeret et al. 1997)
-        * ``'NDVI'`` (Normalised Difference Vegetation Index, Rouse 1973)
-        * ``'NDWI'`` (Normalised Difference Water Index, McFeeters 1996)
-        * ``'SAVI'`` (Soil Adjusted Vegetation Index, Huete 1988)
-        * ``'TCB'`` (Tasseled Cap Brightness, Crist 1985)
-        * ``'TCG'`` (Tasseled Cap Greeness, Crist 1985)
-        * ``'TCW'`` (Tasseled Cap Wetness, Crist 1985)        
-        * ``'TCB_GSO'`` (Tasseled Cap Brightness, Nedkov 2017)
-        * ``'TCG_GSO'`` (Tasseled Cap Greeness, Nedkov 2017)
-        * ``'TCW_GSO'`` (Tasseled Cap Wetness, Nedkov 2017)
-        * ``'TI'`` (Normalised Difference Turbidity Index, Lacaux et al 2007)
-        * ``'WI'`` (Water Index, Fisher 2016)
-        * ``'kNDVI'`` (Non-linear Normalised Difference Vegation Index,
+        'NDVI' (Normalised Difference Vegetation Index, Rouse 1973)
+        'NDWI' (Normalised Difference Water Index, McFeeters 1996)
+        'SAVI' (Soil Adjusted Vegetation Index, Huete 1988)
+        'TCB' (Tasseled Cap Brightness, Crist 1985)
+        'TCG' (Tasseled Cap Greeness, Crist 1985)
+        'TCW' (Tasseled Cap Wetness, Crist 1985)        
+        'TCB_GSO' (Tasseled Cap Brightness, Nedkov 2017)
+        'TCG_GSO' (Tasseled Cap Greeness, Nedkov 2017)
+        'TCW_GSO' (Tasseled Cap Wetness, Nedkov 2017)
+        'WI' (Water Index, Fisher 2016)
+        'kNDVI' (Non-linear Normalised Difference Vegation Index,
                  Camps-Valls et al. 2021)
-
     collection : str
         An string that tells the function what data collection is 
         being used to calculate the index. This is necessary because 
         different collections use different names for bands covering 
-        a similar spectra. 
-        
-        Valid options are: 
-        
-        * ``'ga_ls_3'`` (for GA Landsat Collection 3) 
-        * ``'ga_s2_3'`` (for GA Sentinel 2 Collection 3)
-        * ``'ga_gm_3'`` (for GA Geomedian Collection 3)
-
+        a similar spectra. Valid options are 'ga_ls_2' (for GA 
+        Landsat Collection 2), 'ga_ls_3' (for GA Landsat Collection 3) 
+        and 'ga_s2_1' (for GA Sentinel 2 Collection 1).
     custom_varname : str, optional
         By default, the original dataset will be returned with 
         a new index variable named after `index` (e.g. 'NDVI'). To 
         specify a custom name instead, you can supply e.g. 
         `custom_varname='custom_name'`. Defaults to None, which uses
         `index` to name the variable. 
     normalise : bool, optional
-        Some coefficient-based indices (e.g. ``'WI'``, ``'BAEI'``,
-        ``'AWEI_ns'``, ``'AWEI_sh'``, ``'TCW'``, ``'TCG'``, ``'TCB'``, 
-        ``'TCW_GSO'``, ``'TCG_GSO'``, ``'TCB_GSO'``, ``'EVI'``, 
-        ``'LAI'``, ``'SAVI'``, ``'MSAVI'``) produce different results if 
+        Some coefficient-based indices (e.g. 'WI', 'BAEI', 'AWEI_ns', 
+        'AWEI_sh', 'TCW', 'TCG', 'TCB', 'TCW_GSO', 'TCG_GSO', 'TCB_GSO', 
+        'EVI', 'LAI', 'SAVI', 'MSAVI') produce different results if 
         surface reflectance values are not scaled between 0.0 and 1.0 
         prior to calculating the index. Setting `normalise=True` first 
         scales values to a 0.0-1.0 range by dividing by 10000.0. 
         Defaults to True.  
     drop : bool, optional
         Provides the option to drop the original input data, thus saving 
         space. if drop = True, returns only the index and its values.
@@ -282,27 +273,22 @@
                   # Clay Minerals Ratio, Drury 1987
                   'CMR': lambda ds: (ds.swir1 / ds.swir2),
 
                   # Ferrous Minerals Ratio, Segal 1982
                   'FMR': lambda ds: (ds.swir1 / ds.nir),
 
                   # Iron Oxide Ratio, Segal 1982
-                  'IOR': lambda ds: (ds.red / ds.blue),
-      
-                  # Normalised Difference Turbidity Index , Lacaux et al 2007
-                  #NB. 'NDTI' key already used. 'TI' used in lieu.
-                  'TI': lambda ds:  (ds.red - ds.green) /
-                                    (ds.red + ds.green)
+                  'IOR': lambda ds: (ds.red / ds.blue)
     }
     
     # If index supplied is not a list, convert to list. This allows us to
     # iterate through either multiple or single indices in the loop below
     indices = index if isinstance(index, list) else [index]
     
-    # Calculate for each index in the list of indices supplied (indexes)
+    #calculate for each index in the list of indices supplied (indexes)
     for index in indices:
 
         # Select an index function from the dictionary
         index_func = index_dict.get(str(index))
 
         # If no index is provided or if no function is returned due to an 
         # invalid option being provided, raise an exception informing user to 
@@ -333,18 +319,18 @@
         # Rename bands to a consistent format if depending on what collection
         # is specified in `collection`. This allows the same index calculations
         # to be applied to all collections. If no collection was provided, 
         # raise an exception.
         if collection is None:
 
             raise ValueError("'No `collection` was provided. Please specify "
-                             "either 'ga_ls_3', 'ga_s2_3' or 'ga_gm_3' "
-                             "to ensure the function calculates indices "
-                             "using the correct spectral bands")            
-        
+                             "either 'ga_ls_2', 'ga_ls_3' or 'ga_s2_1' \nto "
+                             "ensure the function calculates indices using the "
+                             "correct spectral bands")
+
         elif collection == 'ga_ls_3':
 
             # Dictionary mapping full data names to simpler 'red' alias names
             bandnames_dict = {
                 'nbart_nir': 'nir',
                 'nbart_red': 'red',
                 'nbart_green': 'green',
@@ -360,15 +346,15 @@
             }
 
             # Rename bands in dataset to use simple names (e.g. 'red')
             bands_to_rename = {
                 a: b for a, b in bandnames_dict.items() if a in ds.variables
             }
 
-        elif collection == 'ga_s2_3':
+        elif collection == 'ga_s2_1':
 
             # Dictionary mapping full data names to simpler 'red' alias names
             bandnames_dict = {
                 'nbart_red': 'red',
                 'nbart_green': 'green',
                 'nbart_blue': 'blue',
                 'nbart_nir_1': 'nir',
@@ -386,25 +372,25 @@
                 'nbar_swir_3': 'swir2'
             }
 
             # Rename bands in dataset to use simple names (e.g. 'red')
             bands_to_rename = {
                 a: b for a, b in bandnames_dict.items() if a in ds.variables
             }
-           
-        elif collection == 'ga_gm_3':
-            
+
+        elif collection == 'ga_ls_2':
+
             # Pass an empty dict as no bands need renaming
             bands_to_rename = {}
 
         # Raise error if no valid collection name is provided:
         else:
             raise ValueError(f"'{collection}' is not a valid option for "
-                             "`collection`. Please specify either \n"
-                             "'ga_ls_3', 'ga_s2_3' or 'ga_gm_3'")
+                              "`collection`. Please specify either \n"
+                              "'ga_ls_2', 'ga_ls_3' or 'ga_s2_1'")
 
         # Apply index function 
         try:
             # If normalised=True, divide data by 10,000 before applying func
             mult = 10000.0 if normalise else 1.0
             index_array = index_func(ds.rename(bands_to_rename) / mult)
         except AttributeError:
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/bom.py` & `dea-tools-0.2.8.dev9/dea_tools/bom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,10 @@
 """
-Loading and processing Australian Bureau of Meteorology data.
-
-License: The code in this notebook is licensed under the Apache License,
-Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
-Australia data is licensed under the Creative Commons by Attribution 4.0
-license (https://creativecommons.org/licenses/by/4.0/).
-
-Contact: If you need assistance, please post a question on the Open Data
-Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack
-Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
-using the `open-data-cube` tag (you can view previously asked questions
-here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
-
-If you would like to report an issue with this script, you can file one
-on Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
-
-Last modified: March 2021
+Scraping some BOM data
 """
-
 import datetime
 import pytz
 import ciso8601
 from types import SimpleNamespace
 import requests
 import lxml
 import lxml.etree
@@ -127,15 +110,18 @@
 
 
 def ui_select_station(stations,
                       zoom=3,
                       center=(-24, 138),
                       **kw):
     """
-    Create an interactive map for selecting river gauging stations.
+    Returns
+    =======
+
+    (gauge_data, station)
     """
     import ipywidgets as W
     from IPython.display import display
     import matplotlib.pyplot as plt
     import ipyleaflet as L
     from odc.ui import ui_poll
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/classification.py` & `dea-tools-0.2.8.dev9/dea_tools/classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # classification.py
 """
-Machnine learning classification tools for analysing remote sensing data
-using the Open Data Cube.
+Description: This file contains a set of python functions for conducting
+machine learning classification on remote sensing data contained in an
+Open Data Cube instance.
 
 License: The code in this notebook is licensed under the Apache License,
-Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
-Australia data is licensed under the Creative Commons by Attribution 4.0
-license (https://creativecommons.org/licenses/by/4.0/).
+Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0).
 
 Contact: If you need assistance, please post a question on the Open Data
 Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
 using the `open-data-cube` tag (you can view previously asked questions
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
 
-If you would like to report an issue with this script, you can file one
-on Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
+If you would like to report an issue with this script, you can file one on
+Github https://github.com/GeoscienceAustralia/dea-notebooks/issues
 
 Last modified: May 2021
-"""
 
+
+"""
 import os
 import sys
 import joblib
 import datacube
 import rasterio
 import numpy as np
 import pandas as pd
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/climate.py` & `dea-tools-0.2.8.dev9/dea_tools/climate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # dea_climate.py
 '''
-Retrieving and manipulating gridded climate data.
+Description: A set of python functions to retrieve and manipulate 
+gridded climate data.
 
 Adapted from scripts by Andrew Cherry and Brian Killough.
 
 License: The code in this notebook is licensed under the Apache License,
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
@@ -14,15 +15,22 @@
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) 
 using the `open-data-cube` tag (you can view previously asked questions 
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube). 
 
 If you would like to report an issue with this script, you can file one on 
 Github https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues
 
+Functions included:
+    get_era5_daily
+    era5_area_crop
+    era5_area_nearest
+    load_era5    
+    
 Last modified: October 2020
+
 '''
 
 import os
 import datetime
 import numpy as np
 from dateutil.parser import parse
 import boto3
@@ -268,15 +276,15 @@
     
     if min(lon) < 0:
         # re-order along longitude to go from -180 to 180
         ds = ds.assign_coords({"lon": (((ds.lon + 180) % 360) - 180)})
         ds = ds.reindex({ "lon": np.sort(ds.lon)})
         
     # find the nearest lat lon boundary points
-    test = ds.sel(lat=list(lat), lon=list(lon), method='nearest')
+    test = ds.sel(lat=lat, lon=lon, method='nearest')
     
     # define the lat/lon grid
     lat_range = slice(test.lat.max().values, test.lat.min().values)
     lon_range = slice(test.lon.min().values, test.lon.max().values)
     
     # crop and keep attrs
     output = ds.sel(lat=lat_range, lon=lon_range)
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/coastal.py` & `dea-tools-0.2.8.dev9/dea_tools/coastal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## dea_coastaltools.py
-"""
-Coastal analysis and tide modelling tools.
+'''
+Description: This file contains a set of python functions for conducting 
+coastal analyses on Digital Earth Australia data.
 
 License: The code in this notebook is licensed under the Apache License, 
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, post a question on the Open Data Cube 
@@ -12,181 +13,538 @@
 (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) using 
 the `open-data-cube` tag (you can view previously asked questions here: 
 https://gis.stackexchange.com/questions/tagged/open-data-cube). 
 
 If you would like to report an issue with this script, you can file one 
 on Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
 
-Last modified: April 2023
+Functions included:
+    tidal_tag
+    tidal_stats
+    transect_distances
+    get_coastlines
+    model_tides
+    pixel_tides
 
-"""
+Last modified: August 2022
+
+'''
 
 # Import required packages
 import os
-import warnings
 import numpy as np
 import xarray as xr
 import pandas as pd
-import geopandas as gpd
+import geopandas as gpd 
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 from scipy import stats
 from shapely.geometry import box, shape
 from owslib.wfs import WebFeatureService
 
 import odc.algo
 from datacube.utils.geometry import CRS
 from dea_tools.datahandling import parallel_apply
 
+try:
+    from otps import TimePoint
+    from otps import predict_tide
+except ImportError:
+    from dea_tools.pyfes_model import TimePoint, predict_tide
+
 # Fix converters for tidal plot
 from pandas.plotting import register_matplotlib_converters
-
 register_matplotlib_converters()
 
 
 WFS_ADDRESS = "https://geoserver.dea.ga.gov.au/geoserver/wfs"
 
 
-def transect_distances(transects_gdf, lines_gdf, mode="distance"):
+def tidal_tag(ds,
+              tidepost_lat=None, 
+              tidepost_lon=None, 
+              ebb_flow=False, 
+              swap_dims=False,
+              return_tideposts=False):
+    """
+    Takes an xarray.Dataset and returns the same dataset with a new 
+    `tide_height` variable giving the height of the tide at the exact
+    moment of each satellite acquisition. 
+    
+    By default, the function models tides for the centroid of the 
+    dataset, but a custom tidal modelling location can be specified 
+    using `tidepost_lat` and `tidepost_lon`.
+    
+    Tides are modelled using the OTPS tidal modelling software based on
+    the TPXO8 tidal model: http://volkov.oce.orst.edu/tides/tpxo8_atlas.html
+    
+    Parameters
+    ----------     
+    ds : xarray.Dataset
+        An xarray.Dataset object with x, y and time dimensions  
+    tidepost_lat, tidepost_lon : float or int, optional
+        Optional coordinates used to model tides. The default is None,
+        which uses the centroid of the dataset as the tide modelling 
+        location.
+    ebb_flow : bool, optional
+        An optional boolean indicating whether to compute if the 
+        tide phase was ebbing (falling) or flowing (rising) for each 
+        observation. The default is False; if set to True, a new 
+        `ebb_flow` variable will be added to the dataset with each 
+        observation labelled with 'Ebb' or 'Flow'.
+    swap_dims : bool, optional
+        An optional boolean indicating whether to swap the `time` 
+        dimension in the original xarray.Dataset to the new 
+        `tide_height` variable. Defaults to False.
+    return_tideposts : bool, optional
+        An optional boolean indicating whether to return the `tidepost_lat`
+        and `tidepost_lon` location used to model tides in addition to the
+        xarray.Dataset. Defaults to False.
+        
+    Returns
+    -------
+    The original xarray.Dataset with a new `tide_height` variable giving
+    the height of the tide (and optionally, its ebb-flow phase) at the 
+    exact moment of each satellite acquisition.  
+    
+    (if `return_tideposts=True`, the function will also return the 
+    `tidepost_lon` and `tidepost_lat` location used in the analysis)
+    
+    """
+
+    # If custom tide modelling locations are not provided, use the
+    # dataset centroid
+    if not tidepost_lat or not tidepost_lon:
+
+        tidepost_lon, tidepost_lat = ds.extent.centroid.to_crs(
+            crs=CRS('EPSG:4326')).coords[0]
+        print(f'Setting tide modelling location from dataset centroid: '
+              f'{tidepost_lon:.2f}, {tidepost_lat:.2f}')
+
+    else:
+        print(f'Using user-supplied tide modelling location: '
+              f'{tidepost_lon:.2f}, {tidepost_lat:.2f}')
+
+    # Use the tidal model to compute tide heights for each observation:
+    obs_datetimes = ds.time.data.astype('M8[s]').astype('O').tolist()    
+    obs_timepoints = [TimePoint(tidepost_lon, tidepost_lat, dt) 
+                      for dt in obs_datetimes]
+    obs_predictedtides = predict_tide(obs_timepoints)   
+
+    # If tides cannot be successfully modeled (e.g. if the centre of the 
+    # xarray dataset is located is over land), raise an exception
+    if len(obs_predictedtides) > 0:
+
+        # Extract tide heights
+        obs_tideheights = [predictedtide.tide_m for predictedtide 
+                           in obs_predictedtides]   
+
+        # Assign tide heights to the dataset as a new variable
+        ds['tide_height'] = xr.DataArray(obs_tideheights, coords=[ds.time]) 
+
+        # Optionally calculate the tide phase for each observation
+        if ebb_flow:
+            
+            # Model tides for a time 15 minutes prior to each previously
+            # modelled satellite acquisition time. This allows us to compare
+            # tide heights to see if they are rising or falling.
+            print('Modelling tidal phase (e.g. ebb or flow)')
+            pre_times = (ds.time - pd.Timedelta('15 min'))
+            pre_datetimes = pre_times.data.astype('M8[s]').astype('O').tolist()   
+            pre_timepoints = [TimePoint(tidepost_lon, tidepost_lat, dt) 
+                              for dt in pre_datetimes]
+            pre_predictedtides = predict_tide(pre_timepoints)
+            
+            # Compare tides computed for each timestep. If the previous tide 
+            # was higher than the current tide, the tide is 'ebbing'. If the
+            # previous tide was lower, the tide is 'flowing'
+            tidal_phase = ['Ebb' if pre.tide_m > obs.tide_m else 'Flow'
+                           for pre, obs in zip(pre_predictedtides, 
+                                               obs_predictedtides)]
+            
+            # Assign tide phase to the dataset as a new variable
+            ds['ebb_flow'] = xr.DataArray(tidal_phase, coords=[ds.time]) 
+            
+        # If swap_dims = True, make tide height the primary dimension 
+        # instead of time
+        if swap_dims:
+
+            # Swap dimensions and sort by tide height
+            ds = ds.swap_dims({'time': 'tide_height'})          
+            ds = ds.sortby('tide_height')  
+            ds = ds.drop('time')
+            
+        if return_tideposts:
+            return ds, tidepost_lon, tidepost_lat
+        else:
+            return ds
+    
+    else:
+        
+        raise ValueError(
+            f'Tides could not be modelled for dataset centroid located '
+            f'at {tidepost_lon:.2f}, {tidepost_lat:.2f}. This can occur if '
+            f'this coordinate occurs over land. Please manually specify '
+            f'a tide modelling location located over water using the '
+            f'`tidepost_lat` and `tidepost_lon` parameters.'
+        )
+
+
+def tidal_stats(ds, 
+                tidepost_lat=None,
+                tidepost_lon=None,
+                plain_english=True, 
+                plot=True,
+                modelled_freq='2h',
+                round_stats=3): 
+    """
+    Takes an xarray.Dataset and statistically compares the tides 
+    modelled for each satellite observation against the full modelled 
+    tidal range. This comparison can be used to evaluate whether the 
+    tides observed by satellites (e.g. Landsat) are biased compared to 
+    the natural tidal range (e.g. fail to observe either the highest or 
+    lowest tides etc).    
+       
+    By default, the function models tides for the centroid of the 
+    dataset, but a custom tidal modelling location can be specified 
+    using `tidepost_lat` and `tidepost_lon`.
+    
+    Tides are modelled using the OTPS tidal modelling software based on
+    the TPXO8 tidal model: http://volkov.oce.orst.edu/tides/tpxo8_atlas.html
+    
+    For more information about the tidal statistics computed by this 
+    function, refer to Figure 8 in Bishop-Taylor et al. 2018:
+    https://www.sciencedirect.com/science/article/pii/S0272771418308783#fig8
+    
+    Parameters
+    ----------     
+    ds : xarray.Dataset
+        An xarray.Dataset object with x, y and time dimensions  
+    tidepost_lat, tidepost_lon : float or int, optional
+        Optional coordinates used to model tides. The default is None,
+        which uses the centroid of the dataset as the tide modelling 
+        location.
+    plain_english : bool, optional
+        An optional boolean indicating whether to print a plain english 
+        version of the tidal statistics to the screen. Defaults to True.
+    plot : bool, optional
+        An optional boolean indicating whether to plot how satellite-
+        observed tide heights compare against the full tidal range. 
+        Defaults to True.
+    modelled_freq : str, optional
+        An optional string giving the frequency at which to model tides 
+        when computing the full modelled tidal range. Defaults to '2h', 
+        which computes a tide height for every two hours across the
+        temporal extent of `ds`.        
+    round_stats : int, optional
+        The number of decimal places used to round the output statistics.
+        Defaults to 3.
+        
+    Returns
+    -------
+    A pandas.Series object containing the following statistics:
+    
+        tidepost_lat: latitude used for modelling tide heights
+        tidepost_lon: longitude used for modelling tide heights
+        observed_min_m: minimum tide height observed by the satellite
+        all_min_m: minimum tide height from full modelled tidal range
+        observed_max_m: maximum tide height observed by the satellite
+        all_max_m: maximum tide height from full modelled tidal range
+        observed_range_m: tidal range observed by the satellite
+        all_range_m: full modelled tidal range 
+        spread_m: proportion of the full modelled tidal range observed 
+                  by the satellite (see Bishop-Taylor et al. 2018)
+        low_tide_offset: proportion of the lowest tides never observed
+                  by the satellite (see Bishop-Taylor et al. 2018)
+        high_tide_offset: proportion of the highest tides never observed
+                  by the satellite (see Bishop-Taylor et al. 2018)
+        observed_slope: slope of any relationship between observed tide 
+                  heights and time
+        all_slope: slope of any relationship between all modelled tide 
+                  heights and time
+        observed_pval: significance/p-value of any relationship between 
+                  observed tide heights and time
+        all_pval: significance/p-value of any relationship between 
+                  all modelled tide heights and time
+    
+    """
+    
+    # Model tides for each observation in the supplied xarray object
+    ds_tides, tidepost_lon, tidepost_lat = tidal_tag(ds,
+                                                     tidepost_lat=tidepost_lat,
+                                                     tidepost_lon=tidepost_lon,
+                                                     return_tideposts=True)
+    
+    # Drop spatial ref for nicer plotting
+    if 'spatial_ref' in ds_tides:
+        ds_tides = ds_tides.drop('spatial_ref')
+
+    # Generate range of times covering entire period of satellite record
+    all_timerange = pd.date_range(start=ds_tides.time.min().item(),
+                                  end=ds_tides.time.max().item(),
+                                  freq=modelled_freq)
+    all_datetimes = all_timerange.values.astype('M8[s]').astype('O').tolist()  
+
+    # Use the tidal model to compute tide heights for each observation:  
+    all_timepoints = [TimePoint(tidepost_lon, tidepost_lat, dt) 
+                      for dt in all_datetimes]
+    all_predictedtides = predict_tide(all_timepoints)   
+    all_tideheights = [predictedtide.tide_m for predictedtide 
+                        in all_predictedtides]
+
+    # Get coarse statistics on all and observed tidal ranges
+    obs_mean = ds_tides.tide_height.mean().item()
+    all_mean = np.mean(all_tideheights)
+    obs_min, obs_max = ds_tides.tide_height.quantile([0.0, 1.0]).values
+    all_min, all_max = np.quantile(all_tideheights, [0.0, 1.0])
+
+    # Calculate tidal range
+    obs_range = (obs_max - obs_min)
+    all_range = (all_max - all_min)
+
+    # Calculate Bishop-Taylor et al. 2018 tidal metrics
+    spread = obs_range / all_range
+    low_tide_offset = abs(all_min - obs_min) / all_range
+    high_tide_offset = abs(all_max - obs_max) / all_range  
+    
+    # Extract x (time in decimal years) and y (distance) values
+    all_x = (all_timerange.year + 
+             ((all_timerange.dayofyear - 1) / 365) +
+             ((all_timerange.hour - 1) / 24))
+    all_y = all_tideheights
+    time_period = all_x.max() - all_x.min()
+
+    # Extract x (time in decimal years) and y (distance) values
+    obs_x = (ds_tides.time.dt.year + 
+             ((ds_tides.time.dt.dayofyear - 1) / 365) + 
+             ((ds_tides.time.dt.hour - 1) / 24))
+    obs_y = ds_tides.tide_height.values.astype(np.float)           
+
+    # Compute linear regression
+    obs_linreg = stats.linregress(x=obs_x, y=obs_y)  
+    all_linreg = stats.linregress(x=all_x, y=all_y)
+    
+    if plain_english:
+        
+        print(f'\n{spread:.0%} of the {all_range:.2f} m modelled astronomical '
+              f'tidal range is observed at this location.\nThe lowest '
+              f'{low_tide_offset:.0%} and highest {high_tide_offset:.0%} '
+              f'of astronomical tides are never observed.\n')
+        
+        # Plain english
+        if obs_linreg.pvalue > 0.05:
+            print(f'Observed tides show no significant trends '
+                  f'over the ~{time_period:.0f} year period.')
+        else:
+            obs_slope_desc = 'decrease' if obs_linreg.slope < 0 else 'increase'
+            print(f'Observed tides {obs_slope_desc} significantly '
+                  f'(p={obs_linreg.pvalue:.3f}) over time by '
+                  f'{obs_linreg.slope:.03f} m per year (i.e. a '
+                  f'~{time_period * obs_linreg.slope:.2f} m '
+                  f'{obs_slope_desc} over the ~{time_period:.0f} year period).')
+
+        if all_linreg.pvalue > 0.05:
+            print(f'All tides show no significant trends '
+                  f'over the ~{time_period:.0f} year period.')
+        else:
+            all_slope_desc = 'decrease' if all_linreg.slope < 0 else 'increase'
+            print(f'All tides {all_slope_desc} significantly '
+                  f'(p={all_linreg.pvalue:.3f}) over time by '
+                  f'{all_linreg.slope:.03f} m per year (i.e. a '
+                  f'~{time_period * all_linreg.slope:.2f} m '
+                  f'{all_slope_desc} over the ~{time_period:.0f} year period).')
+
+    if plot:
+        
+        # Create plot and add all time and observed tide data
+        fig, ax = plt.subplots(figsize=(10, 5))
+        ax.plot(all_timerange, all_tideheights, alpha=0.4)
+        ds_tides.tide_height.plot.line(ax=ax, 
+                                       marker='o',
+                                       linewidth=0.0, 
+                                       color='black',
+                                       markersize=2)
+
+        # Add horizontal lines for spread/offsets
+        ax.axhline(obs_min, color='black', linestyle=':', linewidth=1)
+        ax.axhline(obs_max, color='black', linestyle=':', linewidth=1)
+        ax.axhline(all_min, color='black', linestyle=':', linewidth=1)
+        ax.axhline(all_max, color='black', linestyle=':', linewidth=1)
+
+        # Add text annotations for spread/offsets
+        ax.annotate('    High tide\n    offset', 
+                     xy=(all_timerange.max(), 
+                         np.mean([all_max, obs_max])), 
+                     va='center')
+        ax.annotate('    Spread', 
+                     xy=(all_timerange.max(), 
+                         np.mean([obs_min, obs_max])), 
+                     va='center')
+        ax.annotate('    Low tide\n    offset', 
+                     xy=(all_timerange.max(), 
+                         np.mean([all_min, obs_min])))
+
+        # Remove top right axes and add labels
+        ax.spines['right'].set_visible(False)
+        ax.spines['top'].set_visible(False)
+        ax.set_ylabel('Tide height (m)')
+        ax.set_xlabel('');
+        ax.margins(x=0.015)
+        
+    # Export pandas.Series containing tidal stats
+    return pd.Series({'tidepost_lat': tidepost_lat,
+                      'tidepost_lon': tidepost_lon,
+                      'observed_mean_m': obs_mean,
+                      'all_mean_m': all_mean,
+                      'observed_min_m': obs_min,
+                      'all_min_m': all_min,
+                      'observed_max_m': obs_max,
+                      'all_max_m': all_max,
+                      'observed_range_m': obs_range,
+                      'all_range_m': all_range,
+                      'spread': spread,
+                      'low_tide_offset': low_tide_offset,
+                      'high_tide_offset': high_tide_offset,
+                      'observed_slope': obs_linreg.slope,
+                      'all_slope': all_linreg.slope,
+                      'observed_pval': obs_linreg.pvalue,
+                      'all_pval': all_linreg.pvalue}).round(round_stats)
+
+
+def transect_distances(transects_gdf, lines_gdf, mode='distance'):
     """
-    Take a set of transects (e.g. shore-normal beach survey lines), and
+    Take a set of transects (e.g. shore-normal beach survey lines), and 
     determine the distance along the transect to each object in a set of
-    lines (e.g. shorelines). Distances are measured in the CRS of the
+    lines (e.g. shorelines). Distances are measured in the CRS of the 
     input datasets.
-
-    For coastal applications, transects should be drawn from land to
+    
+    For coastal applications, transects should be drawn from land to 
     water (with the first point being on land so that it can be used
     as a consistent location from which to measure distances.
-
+        
     The distance calculation can be performed using two modes:
-        - 'distance': Distances are measured from the start of the
-          transect to where it intersects with each line. Any transect
-          that intersects a line more than once is ignored. This mode is
-          useful for measuring e.g. the distance to the shoreline over
+        - 'distance': Distances are measured from the start of the 
+          transect to where it intersects with each line. Any transect 
+          that intersects a line more than once is ignored. This mode is 
+          useful for measuring e.g. the distance to the shoreline over 
           time from a consistent starting location.
         - 'width' Distances are measured between the first and last
-          intersection between a transect and each line. Any transect
-          that intersects a line only once is ignored. This is useful
+          intersection between a transect and each line. Any transect 
+          that intersects a line only once is ignored. This is useful 
           for e.g. measuring the width of a narrow area of coastline over
           time, e.g. the neck of a spit or tombolo.
-
+          
     Parameters
-    ----------
+    ----------     
     transects_gdf : geopandas.GeoDataFrame
         A GeoDataFrame containing one or multiple vector profile lines.
         The GeoDataFrame's index column will be used to name the rows in
         the output distance table.
     lines_gdf : geopandas.GeoDataFrame
         A GeoDataFrame containing one or multiple vector line features
         that intersect the profile lines supplied to `transects_gdf`.
         The GeoDataFrame's index column will be used to name the columns
         in the output distance table.
     mode : string, optional
         Whether to use 'distance' (for measuring distances from the
-        start of a profile) or 'width' mode (for measuring the width
+        start of a profile) or 'width' mode (for measuring the width 
         between two profile intersections). See docstring above for more
         info; defaults to 'distance'.
-
+        
     Returns
     -------
     distance_df : pandas.DataFrame
         A DataFrame containing distance measurements for each profile
-        line (rows) and line feature (columns).
+        line (rows) and line feature (columns). 
     """
-
+    
     import warnings
     from shapely.errors import ShapelyDeprecationWarning
     from shapely.geometry import Point
 
     def _intersect_dist(transect_gdf, lines_gdf, mode=mode):
         """
         Take an individual transect, and determine the distance along
-        the transect to each object in a set of lines (e.g. shorelines).
+        the transect to each object in a set of lines (e.g. shorelines).        
         """
 
         # Identify intersections between transects and lines
         intersect_points = lines_gdf.apply(
-            lambda x: x.geometry.intersection(transect_gdf.geometry), axis=1
-        )
+            lambda x: x.geometry.intersection(transect_gdf.geometry), axis=1)
 
         # In distance mode, identify transects with one intersection only,
         # and use this as the end point and the start of the transect as the
         # start point when measuring distances
-        if mode == "distance":
+        if mode == 'distance':
             start_point = Point(transect_gdf.geometry.coords[0])
             point_df = intersect_points.apply(
-                lambda x: pd.Series({"start": start_point, "end": x})
-                if x.type == "Point"
-                else pd.Series({"start": None, "end": None})
-            )
+                lambda x: pd.Series({'start': start_point, 'end': x}) 
+                if x.type == 'Point'
+                else pd.Series({'start': None, 'end': None}))
 
         # In width mode, identify transects with multiple intersections, and
         # use the first intersection as the start point and the second
         # intersection for the end point when measuring distances
-        if mode == "width":
+        if mode == 'width':
             point_df = intersect_points.apply(
-                lambda x: pd.Series({"start": x.geoms[0], "end": x.geoms[-1]})
-                if x.type == "MultiPoint"
-                else pd.Series({"start": None, "end": None})
-            )
+                lambda x: pd.Series({'start': x.geoms[0], 'end': x.geoms[-1]})
+                if x.type == 'MultiPoint' 
+                else pd.Series({'start': None, 'end': None}))
 
         # Calculate distances between valid start and end points
         distance_df = point_df.apply(
-            lambda x: x.start.distance(x.end) if x.start else None, axis=1
-        )
-
+            lambda x: x.start.distance(x.end) if x.start else None, axis=1)
+            
         return distance_df
 
     # Run code after ignoring Shapely pre-v2.0 warnings
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
-
+    with warnings.catch_warnings():        
+        warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning) 
+        
         # Assert that both datasets use the same CRS
-        assert transects_gdf.crs == lines_gdf.crs, (
-            "Please ensure both " "input datasets use the same CRS."
-        )
-
+        assert transects_gdf.crs == lines_gdf.crs, ('Please ensure both '
+        'input datasets use the same CRS.')
+        
         # Run distance calculations
         distance_df = transects_gdf.apply(
-            lambda x: _intersect_dist(x, lines_gdf), axis=1
-        )
-
+            lambda x: _intersect_dist(x, lines_gdf), axis=1)   
+        
         return pd.DataFrame(distance_df)
 
-
-def get_coastlines(
-    bbox: tuple, crs="EPSG:4326", layer="shorelines_annual", drop_wms=True
-) -> gpd.GeoDataFrame:
+    
+def get_coastlines(bbox: tuple,
+                   crs="EPSG:4326",
+                   layer="shorelines",
+                   drop_wms=True) -> gpd.GeoDataFrame:
     """
-    Load DEA Coastlines annual shorelines or rates of change points data
-    for a provided bounding box using WFS.
-
-    For a full description of the DEA Coastlines dataset, refer to the
+    Get DEA Coastlines data for a provided bounding box using WFS.
+    
+    For a full description of the DEA Coastlines dataset, refer to the 
     official Geoscience Australia product description:
     https://cmi.ga.gov.au/data-products/dea/581/dea-coastlines
-
+    
     Parameters
     ----------
     bbox : (xmin, ymin, xmax, ymax), or geopandas object
-        Bounding box expressed as a tutple. Alternatively, a bounding
-        box can be automatically extracted by suppling a
+        Bounding box expressed as a tutple. Alternatively, a bounding 
+        box can be automatically extracted by suppling a 
         geopandas.GeoDataFrame or geopandas.GeoSeries.
     crs : str, optional
         Optional CRS for the bounding box. This is ignored if `bbox`
         is provided as a geopandas object.
     layer : str, optional
         Which DEA Coastlines layer to load. Options include the annual
-        shoreline vectors ("shorelines_annual") and the rates of change
-        points ("rates_of_change"). Defaults to "shorelines_annual".
+        shoreline vectors ("shorelines") and the rates of change 
+        statistics points ("statistics"). Defaults to "shorelines".
     drop_wms : bool, optional
         Whether to drop WMS-specific attribute columns from the data.
         These columns are used for visualising the dataset on DEA Maps,
         and are unlikely to be useful for scientific analysis. Defaults
         to True.
-
+    
     Returns
     -------
     gpd.GeoDataFrame
         A GeoDataFrame containing shoreline or point features and
         associated metadata.
     """
 
@@ -195,43 +553,41 @@
         crs = str(bbox.crs)
         bbox = bbox.total_bounds
     except:
         pass
 
     # Query WFS
     wfs = WebFeatureService(url=WFS_ADDRESS, version="1.1.0")
-    layer_name = f"dea:{layer}"
+    layer_name = "dea:coastlines" if layer == "shorelines" else "dea:coastlines_statistics"
     response = wfs.getfeature(
         typename=layer_name,
         bbox=tuple(bbox) + (crs,),
         outputFormat="json",
     )
 
     # Load data as a geopandas.GeoDataFrame
     coastlines_gdf = gpd.read_file(response)
 
     # Clip to extent of bounding box
     extent = gpd.GeoSeries(box(*bbox), crs=crs).to_crs(coastlines_gdf.crs)
     coastlines_gdf = coastlines_gdf.clip(extent)
-
+    
     # Optionally drop WMS-specific columns
     if drop_wms:
-        coastlines_gdf = coastlines_gdf.loc[
-            :, ~coastlines_gdf.columns.str.contains("wms_")
-        ]
+        coastlines_gdf = coastlines_gdf.loc[:, ~coastlines_gdf.columns.str.contains("wms_")]
 
     return coastlines_gdf
 
 
 def model_tides(
     x,
     y,
     time,
     model="FES2014",
-    directory="/var/share/tide_models",
+    directory="~/tide_models_clipped",
     epsg=4326,
     method="bilinear",
     extrapolate=True,
     cutoff=10.0,
 ):
     """
     Compute tides at points and times using tidal harmonics.
@@ -273,15 +629,15 @@
         are in a custom coordinate reference system.
     time : A datetime array or pandas.DatetimeIndex
         An array containing 'datetime64[ns]' values or a
         'pandas.DatetimeIndex' providing the times at which to
         model tides in UTC time.
     model : string
         The tide model used to model tides. Options include:
-        - "FES2014" (only pre-configured option on DEA Sandbox)
+        - "FES2014"
         - "TPXO8-atlas"
         - "TPXO9-atlas-v5"
     directory : string
         The directory containing tide model data files. These
         data files should be stored in sub-folders for each
         model that match the structure provided by `pyTMD`:
         https://pytmd.readthedocs.io/en/latest/getting_started/Getting-Started.html#directories
@@ -307,15 +663,15 @@
         to extrapolate for all points.
 
     Returns
     -------
     A pandas.DataFrame containing tide heights for every
     combination of time and point coordinates.
     """
-
+    
     import os
     import pyproj
     import numpy as np
     import pyTMD.time
     import pyTMD.model
     import pyTMD.utilities
     from pyTMD.calc_delta_time import calc_delta_time
@@ -448,31 +804,16 @@
         np.tile(deltat, n_points),
     )
 
     # Predict tidal elevations at time and infer minor corrections
     npts = len(t)
     tide = np.ma.zeros((npts), fill_value=np.nan)
     tide.mask = np.any(hc.mask, axis=1)
-
-    # Depending on pyTMD version (<=1.06 vs > 1.06), use different params
-    # TODO: Remove once Sandbox is updated to use pyTMD version 1.0.9
-    try:
-        tide.data[:] = predict_tide_drift(
-            t, hc, c, deltat=deltat, corrections=model.format
-        )
-        minor = infer_minor_corrections(
-            t, hc, c, deltat=deltat, corrections=model.format
-        )
-    except:
-        tide.data[:] = predict_tide_drift(
-            t, hc, c, DELTAT=deltat, CORRECTIONS=model.format
-        )
-        minor = infer_minor_corrections(
-            t, hc, c, DELTAT=deltat, CORRECTIONS=model.format
-        )
+    tide.data[:] = predict_tide_drift(t, hc, c, DELTAT=deltat, CORRECTIONS=model.format)
+    minor = infer_minor_corrections(t, hc, c, DELTAT=deltat, CORRECTIONS=model.format)
     tide.data[:] += minor.data[:]
 
     # Replace invalid values with fill value
     tide.data[tide.mask] = tide.fill_value
 
     # Export data as a dataframe
     return pd.DataFrame(
@@ -486,75 +827,79 @@
 
 
 def pixel_tides(
     ds,
     times=None,
     resample=True,
     calculate_quantiles=None,
-    resolution=None,
-    buffer=None,
+    resolution=5000,
+    buffer=12000,
     resample_method="bilinear",
-    **model_tides_kwargs,
+    model="FES2014",
+    directory="~/tide_models_clipped",
 ):
     """
     Obtain tide heights for each pixel in a dataset by modelling
     tides into a low-resolution grid surrounding the dataset,
-    then (optionally) spatially resample this low-res data back
+    then (optionally) spatially reprojecting this low-res data back
     into the original higher resolution dataset extent and resolution.
 
     Parameters:
     -----------
     ds : xarray.Dataset
         A dataset whose geobox (`ds.odc.geobox`) will be used to define
         the spatial extent of the low resolution tide modelling grid.
-    times : pandas.DatetimeIndex or list of pandas.Timestamps, optional
+    times : list or pandas.Series, optional
         By default, the function will model tides using the times
-        contained in the `time` dimension of `ds`. Alternatively, this 
-        param can be used to model tides for a custom set of times 
-        instead. For example:
-        `times=pd.date_range(start="2000", end="2001", freq="5h")`
+        contained in the `time` dimension of `ds`. This param can be used
+        to model tides for a custom set of times instead, for example:
+        `times=pd.date_range(start="2000", end="2020", freq="30min")`
     resample : bool, optional
         Whether to resample low resolution tides back into `ds`'s original
         higher resolution grid. Set this to `False` if you do not want
         low resolution tides to be re-projected back to higher resolution.
     calculate_quantiles : list or np.array, optional
         Rather than returning all individual tides, low-resolution tides
         can be first aggregated using a quantile calculation by passing in
         a list or array of quantiles to compute. For example, this could
         be used to calculate the min/max tide across all times:
         `calculate_quantiles=[0.0, 1.0]`.
     resolution: int, optional
         The desired resolution of the low-resolution grid used for tide
-        modelling. The default None will create a 5000 m resolution grid
-        if `ds` has a projected CRS (i.e. metre units), or a 0.05 degree
-        resolution grid if `ds` has a geographic CRS (e.g. degree units).
-        Note: higher resolutions do not necessarily provide better
-        tide modelling performance, as results will be limited by the
-        resolution of the underlying global tide model (e.g. 1/16th 
-        degree / ~5 km resolution grid for FES2014).
+        modelling. Defaults to 5000 for a 5,000 m grid (assuming `ds`'s
+        CRS uses project/metre units).
     buffer : int, optional
         The amount by which to buffer the higher resolution grid extent
         when creating the new low resolution grid. This buffering is
         important as it ensures that ensure pixel-based tides are seamless
         across dataset boundaries. This buffer will eventually be clipped
         away when the low-resolution data is re-projected back to the
-        resolution and extent of the higher resolution dataset. To 
-        ensure that at least two pixels occur outside of the dataset 
-        bounds, the default None applies a 12000 m buffer if `ds` has a 
-        projected CRS (i.e. metre units), or a 0.12 degree buffer if 
-        `ds` has a geographic CRS (e.g. degree units).
+        resolution and extent of the higher resolution dataset. Defaults
+        to 12,000 m to ensure that at least two 5,000 m pixels occur
+        outside of the dataset bounds.
     resample_method : string, optional
         If resampling is requested (see `resample` above), use this
         resampling method when converting from low resolution to high
         resolution pixels. Defaults to "bilinear"; valid options include
         "nearest", "cubic", "min", "max", "average" etc.
-    **model_tides_kwargs :
-        Optional parameters passed to the `dea_tools.coastal.model_tides`
-        function. Important parameters include "model" and "directory",
-        used to specify the tide model to use and the location of its files.
+    model : string, optional
+        The tide model used to model tides. Options include:
+        - "FES2014"
+        - "TPXO8-atlas"
+        - "TPXO9-atlas-v5"
+    directory : string, optional
+        The directory containing tide model data files. These
+        data files should be stored in sub-folders for each
+        model that match the structure provided by `pyTMD`:
+        https://pytmd.readthedocs.io/en/latest/getting_started/Getting-Started.html#directories
+        For example:
+        - {directory}/fes2014/ocean_tide/
+          {directory}/fes2014/load_tide/
+        - {directory}/tpxo8_atlas/
+        - {directory}/TPXO9_atlas_v5/
 
     Returns:
     --------
     If `resample` is True:
 
         tides_lowres : xr.DataArray
             A low resolution data array giving either tide heights every
@@ -573,107 +918,47 @@
             or tide height quantiles for every quantile provided by
             `calculate_quantiles`.
     """
 
     import odc.geo.xr
     from odc.geo.geobox import GeoBox
 
-    # First test if no time dimension and nothing passed to `times`
-    if ('time' not in ds.dims) & (times is None):
-        raise ValueError(
-            "`ds` does not contain a 'time' dimension. Times are required "
-            "for modelling tides: please pass in a set of custom tides "
-            "using the `times` parameter. For example: "
-            "`times=pd.date_range(start='2000', end='2001', freq='5h')`"
-        )
-
-    # If custom times are provided, convert them to a consistent 
-    # pandas.DatatimeIndex format
-    if times is not None:
-        if isinstance(times, list):
-            time_coords = pd.DatetimeIndex(times)
-        elif isinstance(times, pd.Timestamp):
-            time_coords = pd.DatetimeIndex([times])
-        else: 
-            time_coords = times
-
-    # Otherwise, use times from `ds` directly
-    else:
-        time_coords = ds.coords["time"]
-        
-    # Determine spatial dimensions
-    y_dim, x_dim = ds.odc.spatial_dims
-    
-    # Determine resolution and buffer, using different defaults for
-    # geographic (i.e. degrees) and projected (i.e. metres) CRSs:
-    crs_units = ds.odc.geobox.crs.units[0][0:6]
-    if ds.odc.geobox.crs.geographic:
-        if resolution is None:
-            resolution = 0.05
-        elif resolution > 360:
-            raise ValueError(f"A resolution of greater than 360 was "
-                             f"provided, but `ds` has a geographic CRS "
-                             f"in {crs_units} units. Did you accidently "
-                             f"provide a resolution in projected "
-                             f"(i.e. metre) units?")
-        if buffer is None:
-            buffer = 0.12
-    else:
-        if resolution is None:
-            resolution = 5000
-        elif resolution < 1:
-            raise ValueError(f"A resolution of less than 1 was provided, "
-                             f"but `ds` has a projected CRS in "
-                             f"{crs_units} units. Did you accidently "
-                             f"provide a resolution in geographic "
-                             f"(degree) units?")
-        if buffer is None:
-            buffer = 12000
-
-    # Create a new reduced resolution tide modelling grid after
-    # first buffering the grid
-    print(f"Creating reduced resolution {resolution} x {resolution} "
-          f"{crs_units} tide modelling array")
+    # Create a new reduced resolution (5km) tide modelling grid after
+    # first buffering the grid by 12km (i.e. at least two 5km pixels)
+    print("Creating reduced resolution tide modelling array")
     buffered_geobox = ds.odc.geobox.buffered(buffer)
     rescaled_geobox = GeoBox.from_bbox(
         bbox=buffered_geobox.boundingbox, resolution=resolution
     )
     rescaled_ds = odc.geo.xr.xr_zeros(rescaled_geobox)
 
-    # Flatten grid to 1D, then add time dimension  
-    flattened_ds = rescaled_ds.stack(z=(x_dim, y_dim))    
+    # Flatten grid to 1D, then add time dimension. If custom times are
+    # provided use these, otherwise use times from `ds`
+    time_coords = ds.coords["time"] if times is None else times
+    flattened_ds = rescaled_ds.stack(z=("x", "y"))
     flattened_ds = flattened_ds.expand_dims(dim={"time": time_coords.values})
 
-    # Model tides for each timestep
-    model = (
-        "FES2014" if "model" not in model_tides_kwargs else model_tides_kwargs["model"]
-    )
+    # Model tides for each timestep and x/y grid cell
     print(f"Modelling tides using {model} tide model")
     tide_df = model_tides(
-        x=flattened_ds[x_dim],
-        y=flattened_ds[y_dim],
+        x=flattened_ds.x,
+        y=flattened_ds.y,
         time=flattened_ds.time,
+        model=model,
+        directory=directory,
         epsg=ds.odc.geobox.crs.epsg,
-        **model_tides_kwargs,
     )
-    
-    # Rename x and y coordinates to match satellite array
-    tide_df = tide_df.rename({"x": x_dim, "y": y_dim}, axis=1)
 
     # Insert modelled tide values back into flattened array, then unstack
-    # back to 3D (y, x, time)
+    # back to 3D (x, y, time)
     tides_lowres = (
-
-        # Convert dataframe to xarray format
-        tide_df.set_index([x_dim, y_dim], append=True)
+        tide_df.set_index(["x", "y"], append=True)
         .to_xarray()
-
-        # Re-index and transpose back into 3D
         .tide_m.reindex_like(rescaled_ds)
-        .transpose(y_dim, x_dim, "time")
+        .transpose(*list(ds.dims.keys()))
         .astype(np.float32)
     )
 
     # Optionally calculate and return quantiles rather than raw data
     if calculate_quantiles is not None:
 
         print("Computing tide quantiles")
@@ -699,838 +984,7 @@
         )
 
         return tides_highres, tides_lowres
 
     else:
         print("Returning low resolution tide array")
         return tides_lowres
-
-
-def tidal_tag(
-    ds,
-    ebb_flow=False,
-    swap_dims=False,
-    tidepost_lat=None,
-    tidepost_lon=None,
-    return_tideposts=False,
-    **model_tides_kwargs,
-):
-    """
-    Takes an xarray.Dataset and returns the same dataset with a new
-    `tide_m` variable giving the height of the tide at the exact
-    moment of each satellite acquisition.
-
-    The function models tides at the centroid of the dataset by default, 
-    but a custom tidal modelling location can be specified using 
-    `tidepost_lat` and `tidepost_lon`.
-
-    The default settings use the FES2014 global tidal model, implemented
-    using the pyTMD Python package. FES2014 was produced by NOVELTIS, 
-    LEGOS, CLS Space Oceanography Division and CNES. It is distributed 
-    by AVISO, with support from CNES (http://www.aviso.altimetry.fr/).
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        An xarray.Dataset object with x, y and time dimensions
-    ebb_flow : bool, optional
-        An optional boolean indicating whether to compute if the
-        tide phase was ebbing (falling) or flowing (rising) for each
-        observation. The default is False; if set to True, a new
-        `ebb_flow` variable will be added to the dataset with each
-        observation labelled with 'Ebb' or 'Flow'.
-    swap_dims : bool, optional
-        An optional boolean indicating whether to swap the `time`
-        dimension in the original xarray.Dataset to the new
-        `tide_m` variable. Defaults to False.
-    tidepost_lat, tidepost_lon : float or int, optional
-        Optional coordinates used to model tides. The default is None,
-        which uses the centroid of the dataset as the tide modelling
-        location.
-    return_tideposts : bool, optional
-        An optional boolean indicating whether to return the `tidepost_lat`
-        and `tidepost_lon` location used to model tides in addition to the
-        xarray.Dataset. Defaults to False.
-    **model_tides_kwargs :
-        Optional parameters passed to the `dea_tools.coastal.model_tides`
-        function. Important parameters include "model" and "directory",
-        used to specify the tide model to use and the location of its files.
-
-    Returns
-    -------
-    The original xarray.Dataset with a new `tide_m` variable giving
-    the height of the tide (and optionally, its ebb-flow phase) at the
-    exact moment of each satellite acquisition (if `return_tideposts=True`,
-    the function will also return the `tidepost_lon` and `tidepost_lat`
-    location used in the analysis).
-
-    """
-
-    import odc.geo.xr
-
-    # If custom tide modelling locations are not provided, use the
-    # dataset centroid
-    if not tidepost_lat or not tidepost_lon:
-
-        tidepost_lon, tidepost_lat = ds.odc.geobox.geographic_extent.centroid.coords[0]
-        print(
-            f"Setting tide modelling location from dataset centroid: "
-            f"{tidepost_lon:.2f}, {tidepost_lat:.2f}"
-        )
-
-    else:
-        print(
-            f"Using user-supplied tide modelling location: "
-            f"{tidepost_lon:.2f}, {tidepost_lat:.2f}"
-        )
-
-    # Use tidal model to compute tide heights for each observation:
-    model = (
-        "FES2014" if "model" not in model_tides_kwargs else model_tides_kwargs["model"]
-    )
-    print(f"Modelling tides using {model} tidal model")
-    tide_df = model_tides(
-        x=tidepost_lon,
-        y=tidepost_lat,
-        time=ds.time,
-        epsg="EPSG:4326",
-        **model_tides_kwargs,
-    )
-
-    # If tides cannot be successfully modeled (e.g. if the centre of the
-    # xarray dataset is located is over land), raise an exception
-    if tide_df.tide_m.isnull().all():
-
-        raise ValueError(
-            f"Tides could not be modelled for dataset centroid located "
-            f"at {tidepost_lon:.2f}, {tidepost_lat:.2f}. This can occur if "
-            f"this coordinate occurs over land. Please manually specify "
-            f"a tide modelling location located over water using the "
-            f"`tidepost_lat` and `tidepost_lon` parameters."
-        )
-
-    # Assign tide heights to the dataset as a new variable
-    ds["tide_m"] = xr.DataArray(tide_df.tide_m, coords=[ds.time])
-
-    # Optionally calculate the tide phase for each observation
-    if ebb_flow:
-
-        # Model tides for a time 15 minutes prior to each previously
-        # modelled satellite acquisition time. This allows us to compare
-        # tide heights to see if they are rising or falling.
-        print("Modelling tidal phase (e.g. ebb or flow)")
-        tide_pre_df = model_tides(
-            x=tidepost_lon,
-            y=tidepost_lat,
-            time=(ds.time - pd.Timedelta("15 min")),
-            epsg="EPSG:4326",
-            **model_tides_kwargs,
-        )
-
-        # Compare tides computed for each timestep. If the previous tide
-        # was higher than the current tide, the tide is 'ebbing'. If the
-        # previous tide was lower, the tide is 'flowing'
-        tidal_phase = [
-            "Ebb" if i else "Flow"
-            for i in tide_pre_df.tide_m.values > tide_df.tide_m.values
-        ]
-
-        # Assign tide phase to the dataset as a new variable
-        ds["ebb_flow"] = xr.DataArray(tidal_phase, coords=[ds.time])
-
-    # If swap_dims = True, make tide height the primary dimension
-    # instead of time
-    if swap_dims:
-
-        # Swap dimensions and sort by tide height
-        ds = ds.swap_dims({"time": "tide_m"})
-        ds = ds.sortby("tide_m")
-        ds = ds.drop("time")
-
-    if return_tideposts:
-        return ds, tidepost_lon, tidepost_lat
-    else:
-        return ds
-
-
-def tidal_stats(
-    ds,
-    tidepost_lat=None,
-    tidepost_lon=None,
-    plain_english=True,
-    plot=True,
-    modelled_freq="2h",
-    linear_reg=False,
-    round_stats=3,
-    **model_tides_kwargs,
-):
-    """
-    Takes an xarray.Dataset and statistically compares the tides
-    modelled for each satellite observation against the full modelled
-    tidal range. This comparison can be used to evaluate whether the
-    tides observed by satellites (e.g. Landsat) are biased compared to
-    the natural tidal range (e.g. fail to observe either the highest or
-    lowest tides etc).
-    
-    For more information about the tidal statistics computed by this
-    function, refer to Figure 8 in Bishop-Taylor et al. 2018:
-    https://www.sciencedirect.com/science/article/pii/S0272771418308783#fig8
-
-    The function models tides at the centroid of the dataset by default, 
-    but a custom tidal modelling location can be specified using 
-    `tidepost_lat` and `tidepost_lon`.
-    
-    The default settings use the FES2014 global tidal model, implemented
-    using the pyTMD Python package. FES2014 was produced by NOVELTIS, 
-    LEGOS, CLS Space Oceanography Division and CNES. It is distributed 
-    by AVISO, with support from CNES (http://www.aviso.altimetry.fr/).
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        An xarray.Dataset object with x, y and time dimensions
-    tidepost_lat, tidepost_lon : float or int, optional
-        Optional coordinates used to model tides. The default is None,
-        which uses the centroid of the dataset as the tide modelling
-        location.
-    plain_english : bool, optional
-        An optional boolean indicating whether to print a plain english
-        version of the tidal statistics to the screen. Defaults to True.
-    plot : bool, optional
-        An optional boolean indicating whether to plot how satellite-
-        observed tide heights compare against the full tidal range.
-        Defaults to True.
-    modelled_freq : str, optional
-        An optional string giving the frequency at which to model tides
-        when computing the full modelled tidal range. Defaults to '2h',
-        which computes a tide height for every two hours across the
-        temporal extent of `ds`.
-    linear_reg: bool, optional
-        Experimental: whether to return linear regression stats that
-        assess whether dstellite-observed and all available tides show
-        any decreasing or increasing trends over time. Not currently
-        recommended as all observed regressions always return as
-        significant due to far larger sample size.
-    round_stats : int, optional
-        The number of decimal places used to round the output statistics.
-        Defaults to 3.
-    **model_tides_kwargs :
-        Optional parameters passed to the `dea_tools.coastal.model_tides`
-        function. Important parameters include "model" and "directory",
-        used to specify the tide model to use and the location of its files.
-
-    Returns
-    -------
-    A pandas.Series object containing the following statistics:
-
-        tidepost_lat: latitude used for modelling tide heights
-        tidepost_lon: longitude used for modelling tide heights
-        observed_min_m: minimum tide height observed by the satellite
-        all_min_m: minimum tide height from all available tides
-        observed_max_m: maximum tide height observed by the satellite
-        all_max_m: maximum tide height from all available tides
-        observed_range_m: tidal range observed by the satellite
-        all_range_m: full astronomical tidal range based on all
-                  available tides
-        spread_m: proportion of the full astronomical tidal range observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-        low_tide_offset: proportion of the lowest tides never observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-        high_tide_offset: proportion of the highest tides never observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-
-    If `linear_reg = True`, the output will also contain:
-
-        observed_slope: slope of any relationship between observed tide
-                  heights and time
-        all_slope: slope of any relationship between all available tide
-                  heights and time
-        observed_pval: significance/p-value of any relationship between
-                  observed tide heights and time
-        all_pval: significance/p-value of any relationship between
-                  all available tide heights and time
-
-    """
-
-    # Model tides for each observation in the supplied xarray object
-    ds_tides, tidepost_lon, tidepost_lat = tidal_tag(
-        ds,
-        tidepost_lat=tidepost_lat,
-        tidepost_lon=tidepost_lon,
-        return_tideposts=True,
-        **model_tides_kwargs,
-    )
-
-    # Drop spatial ref for nicer plotting
-    if "spatial_ref" in ds_tides:
-        ds_tides = ds_tides.drop("spatial_ref")
-
-    # Generate range of times covering entire period of satellite record
-    all_timerange = pd.date_range(
-        start=ds_tides.time.min().item(),
-        end=ds_tides.time.max().item(),
-        freq=modelled_freq,
-    )
-
-    # Model tides for each timestep
-    all_tides_df = model_tides(
-        x=tidepost_lon,
-        y=tidepost_lat,
-        time=all_timerange,
-        epsg="EPSG:4326",
-        **model_tides_kwargs,
-    )
-
-    # Get coarse statistics on all and observed tidal ranges
-    obs_mean = ds_tides.tide_m.mean().item()
-    all_mean = all_tides_df.tide_m.mean()
-    obs_min, obs_max = ds_tides.tide_m.quantile([0.0, 1.0]).values
-    all_min, all_max = all_tides_df.tide_m.quantile([0.0, 1.0]).values
-
-    # Calculate tidal range
-    obs_range = obs_max - obs_min
-    all_range = all_max - all_min
-
-    # Calculate Bishop-Taylor et al. 2018 tidal metrics
-    spread = obs_range / all_range
-    low_tide_offset = abs(all_min - obs_min) / all_range
-    high_tide_offset = abs(all_max - obs_max) / all_range
-
-    # Extract x (time in decimal years) and y (distance) values
-    all_x = (
-        all_tides_df.index.year
-        + ((all_tides_df.index.dayofyear - 1) / 365)
-        + ((all_tides_df.index.hour - 1) / 24)
-    )
-    all_y = all_tides_df.tide_m.values.astype(np.float)
-    time_period = all_x.max() - all_x.min()
-
-    # Extract x (time in decimal years) and y (distance) values
-    obs_x = (
-        ds_tides.time.dt.year
-        + ((ds_tides.time.dt.dayofyear - 1) / 365)
-        + ((ds_tides.time.dt.hour - 1) / 24)
-    )
-    obs_y = ds_tides.tide_m.values.astype(np.float)
-
-    # Compute linear regression
-    obs_linreg = stats.linregress(x=obs_x, y=obs_y)
-    all_linreg = stats.linregress(x=all_x, y=all_y)
-
-    if plain_english:
-
-        print(
-            f"\n{spread:.0%} of the {all_range:.2f} m modelled astronomical "
-            f"tidal range is observed at this location.\nThe lowest "
-            f"{low_tide_offset:.0%} and highest {high_tide_offset:.0%} "
-            f"of astronomical tides are never observed.\n"
-        )
-
-        if linear_reg:
-
-            if obs_linreg.pvalue > 0.05:
-                print(
-                    f"Observed tides show no significant trends "
-                    f"over the ~{time_period:.0f} year period."
-                )
-            else:
-                obs_slope_desc = "decrease" if obs_linreg.slope < 0 else "increase"
-                print(
-                    f"Observed tides {obs_slope_desc} significantly "
-                    f"(p={obs_linreg.pvalue:.3f}) over time by "
-                    f"{obs_linreg.slope:.03f} m per year (i.e. a "
-                    f"~{time_period * obs_linreg.slope:.2f} m "
-                    f"{obs_slope_desc} over the ~{time_period:.0f} year period)."
-                )
-
-            if all_linreg.pvalue > 0.05:
-                print(
-                    f"All tides show no significant trends "
-                    f"over the ~{time_period:.0f} year period."
-                )
-            else:
-                all_slope_desc = "decrease" if all_linreg.slope < 0 else "increase"
-                print(
-                    f"All tides {all_slope_desc} significantly "
-                    f"(p={all_linreg.pvalue:.3f}) over time by "
-                    f"{all_linreg.slope:.03f} m per year (i.e. a "
-                    f"~{time_period * all_linreg.slope:.2f} m "
-                    f"{all_slope_desc} over the ~{time_period:.0f} year period)."
-                )
-
-    if plot:
-
-        # Create plot and add all time and observed tide data
-        fig, ax = plt.subplots(figsize=(10, 5))
-        all_tides_df.tide_m.plot(ax=ax, alpha=0.4)
-        ds_tides.tide_m.plot.line(
-            ax=ax, marker="o", linewidth=0.0, color="black", markersize=2
-        )
-
-        # Add horizontal lines for spread/offsets
-        ax.axhline(obs_min, color="black", linestyle=":", linewidth=1)
-        ax.axhline(obs_max, color="black", linestyle=":", linewidth=1)
-        ax.axhline(all_min, color="black", linestyle=":", linewidth=1)
-        ax.axhline(all_max, color="black", linestyle=":", linewidth=1)
-
-        # Add text annotations for spread/offsets
-        ax.annotate(
-            f"    High tide\n    offset ({high_tide_offset:.0%})",
-            xy=(all_timerange.max(), np.mean([all_max, obs_max])),
-            va="center",
-        )
-        ax.annotate(
-            f"    Spread\n    ({spread:.0%})",
-            xy=(all_timerange.max(), np.mean([obs_min, obs_max])),
-            va="center",
-        )
-        ax.annotate(
-            f"    Low tide\n    offset ({low_tide_offset:.0%})",
-            xy=(all_timerange.max(), np.mean([all_min, obs_min])),
-        )
-
-        # Remove top right axes and add labels
-        ax.spines["right"].set_visible(False)
-        ax.spines["top"].set_visible(False)
-        ax.set_ylabel("Tide height (m)")
-        ax.set_xlabel("")
-        ax.margins(x=0.015)
-
-    # Export pandas.Series containing tidal stats
-    output_stats = {
-        "tidepost_lat": tidepost_lat,
-        "tidepost_lon": tidepost_lon,
-        "observed_mean_m": obs_mean,
-        "all_mean_m": all_mean,
-        "observed_min_m": obs_min,
-        "all_min_m": all_min,
-        "observed_max_m": obs_max,
-        "all_max_m": all_max,
-        "observed_range_m": obs_range,
-        "all_range_m": all_range,
-        "spread": spread,
-        "low_tide_offset": low_tide_offset,
-        "high_tide_offset": high_tide_offset,
-    }
-
-    if linear_reg:
-        output_stats.update(
-            {
-                "observed_slope": obs_linreg.slope,
-                "all_slope": all_linreg.slope,
-                "observed_pval": obs_linreg.pvalue,
-                "all_pval": all_linreg.pvalue,
-            }
-        )
-
-    return pd.Series(output_stats).round(round_stats)
-
-
-def tidal_tag_otps(
-    ds,
-    tidepost_lat=None,
-    tidepost_lon=None,
-    ebb_flow=False,
-    swap_dims=False,
-    return_tideposts=False,
-):
-    """
-    Takes an xarray.Dataset and returns the same dataset with a new
-    `tide_m` variable giving the height of the tide at the exact
-    moment of each satellite acquisition.
-
-    By default, the function models tides for the centroid of the
-    dataset, but a custom tidal modelling location can be specified
-    using `tidepost_lat` and `tidepost_lon`.
-
-    Tides are modelled using the OTPS tidal modelling software based on
-    the TPXO8 tidal model: http://volkov.oce.orst.edu/tides/tpxo8_atlas.html
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        An xarray.Dataset object with x, y and time dimensions
-    tidepost_lat, tidepost_lon : float or int, optional
-        Optional coordinates used to model tides. The default is None,
-        which uses the centroid of the dataset as the tide modelling
-        location.
-    ebb_flow : bool, optional
-        An optional boolean indicating whether to compute if the
-        tide phase was ebbing (falling) or flowing (rising) for each
-        observation. The default is False; if set to True, a new
-        `ebb_flow` variable will be added to the dataset with each
-        observation labelled with 'Ebb' or 'Flow'.
-    swap_dims : bool, optional
-        An optional boolean indicating whether to swap the `time`
-        dimension in the original xarray.Dataset to the new
-        `tide_m` variable. Defaults to False.
-    return_tideposts : bool, optional
-        An optional boolean indicating whether to return the `tidepost_lat`
-        and `tidepost_lon` location used to model tides in addition to the
-        xarray.Dataset. Defaults to False.
-
-    Returns
-    -------
-    The original xarray.Dataset with a new `tide_m` variable giving
-    the height of the tide (and optionally, its ebb-flow phase) at the
-    exact moment of each satellite acquisition (if `return_tideposts=True`,
-    the function will also return the `tidepost_lon` and `tidepost_lat`
-    location used in the analysis).
-
-    """
-
-    # Load tide modelling functions from either OTPS for pyfes
-    try:
-        from otps import TimePoint
-        from otps import predict_tide
-    except ImportError:
-        from dea_tools.pyfes_model import TimePoint, predict_tide
-
-    # If custom tide modelling locations are not provided, use the
-    # dataset centroid
-    if not tidepost_lat or not tidepost_lon:
-
-        tidepost_lon, tidepost_lat = ds.extent.centroid.to_crs(
-            crs=CRS("EPSG:4326")
-        ).coords[0]
-        print(
-            f"Setting tide modelling location from dataset centroid: "
-            f"{tidepost_lon:.2f}, {tidepost_lat:.2f}"
-        )
-
-    else:
-        print(
-            f"Using user-supplied tide modelling location: "
-            f"{tidepost_lon:.2f}, {tidepost_lat:.2f}"
-        )
-
-    # Use the tidal model to compute tide heights for each observation:
-    print(f"Modelling tides using OTPS and the TPXO8 tidal model")
-    obs_datetimes = ds.time.data.astype("M8[s]").astype("O").tolist()
-    obs_timepoints = [TimePoint(tidepost_lon, tidepost_lat, dt) for dt in obs_datetimes]
-    obs_predictedtides = predict_tide(obs_timepoints)
-
-    # If tides cannot be successfully modeled (e.g. if the centre of the
-    # xarray dataset is located is over land), raise an exception
-    if len(obs_predictedtides) > 0:
-
-        # Extract tide heights
-        obs_tideheights = [predictedtide.tide_m for predictedtide in obs_predictedtides]
-
-        # Assign tide heights to the dataset as a new variable
-        ds["tide_m"] = xr.DataArray(obs_tideheights, coords=[ds.time])
-
-        # Optionally calculate the tide phase for each observation
-        if ebb_flow:
-
-            # Model tides for a time 15 minutes prior to each previously
-            # modelled satellite acquisition time. This allows us to compare
-            # tide heights to see if they are rising or falling.
-            print("Modelling tidal phase (e.g. ebb or flow)")
-            pre_times = ds.time - pd.Timedelta("15 min")
-            pre_datetimes = pre_times.data.astype("M8[s]").astype("O").tolist()
-            pre_timepoints = [
-                TimePoint(tidepost_lon, tidepost_lat, dt) for dt in pre_datetimes
-            ]
-            pre_predictedtides = predict_tide(pre_timepoints)
-
-            # Compare tides computed for each timestep. If the previous tide
-            # was higher than the current tide, the tide is 'ebbing'. If the
-            # previous tide was lower, the tide is 'flowing'
-            tidal_phase = [
-                "Ebb" if pre.tide_m > obs.tide_m else "Flow"
-                for pre, obs in zip(pre_predictedtides, obs_predictedtides)
-            ]
-
-            # Assign tide phase to the dataset as a new variable
-            ds["ebb_flow"] = xr.DataArray(tidal_phase, coords=[ds.time])
-
-        # If swap_dims = True, make tide height the primary dimension
-        # instead of time
-        if swap_dims:
-
-            # Swap dimensions and sort by tide height
-            ds = ds.swap_dims({"time": "tide_m"})
-            ds = ds.sortby("tide_m")
-            ds = ds.drop("time")
-
-        if return_tideposts:
-            return ds, tidepost_lon, tidepost_lat
-        else:
-            return ds
-
-    else:
-
-        raise ValueError(
-            f"Tides could not be modelled for dataset centroid located "
-            f"at {tidepost_lon:.2f}, {tidepost_lat:.2f}. This can occur if "
-            f"this coordinate occurs over land. Please manually specify "
-            f"a tide modelling location located over water using the "
-            f"`tidepost_lat` and `tidepost_lon` parameters."
-        )
-
-
-def tidal_stats_otps(
-    ds,
-    tidepost_lat=None,
-    tidepost_lon=None,
-    plain_english=True,
-    plot=True,
-    modelled_freq="2h",
-    linear_reg=False,
-    round_stats=3,
-):
-    """
-    Takes an xarray.Dataset and statistically compares the tides
-    modelled for each satellite observation against the full modelled
-    tidal range. This comparison can be used to evaluate whether the
-    tides observed by satellites (e.g. Landsat) are biased compared to
-    the natural tidal range (e.g. fail to observe either the highest or
-    lowest tides etc).
-
-    By default, the function models tides for the centroid of the
-    dataset, but a custom tidal modelling location can be specified
-    using `tidepost_lat` and `tidepost_lon`.
-
-    For more information about the tidal statistics computed by this
-    function, refer to Figure 8 in Bishop-Taylor et al. 2018:
-    https://www.sciencedirect.com/science/article/pii/S0272771418308783#fig8
-    
-    Tides are modelled using the OTPS tidal modelling software based on
-    the TPXO8 tidal model: http://volkov.oce.orst.edu/tides/tpxo8_atlas.html
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        An xarray.Dataset object with x, y and time dimensions
-    tidepost_lat, tidepost_lon : float or int, optional
-        Optional coordinates used to model tides. The default is None,
-        which uses the centroid of the dataset as the tide modelling
-        location.
-    plain_english : bool, optional
-        An optional boolean indicating whether to print a plain english
-        version of the tidal statistics to the screen. Defaults to True.
-    plot : bool, optional
-        An optional boolean indicating whether to plot how satellite-
-        observed tide heights compare against the full tidal range.
-        Defaults to True.
-    modelled_freq : str, optional
-        An optional string giving the frequency at which to model tides
-        when computing the full modelled tidal range. Defaults to '2h',
-        which computes a tide height for every two hours across the
-        temporal extent of `ds`.
-    linear_reg: bool, optional
-        Experimental: whether to return linear regression stats that
-        assess whether dstellite-observed and all available tides show
-        any decreasing or increasing trends over time. Not currently
-        recommended as all observed regressions always return as
-        significant due to far larger sample size.
-    round_stats : int, optional
-        The number of decimal places used to round the output statistics.
-        Defaults to 3.
-
-    Returns
-    -------
-    A pandas.Series object containing the following statistics:
-
-        tidepost_lat: latitude used for modelling tide heights
-        tidepost_lon: longitude used for modelling tide heights
-        observed_min_m: minimum tide height observed by the satellite
-        all_min_m: minimum tide height from all available tides
-        observed_max_m: maximum tide height observed by the satellite
-        all_max_m: maximum tide height from all available tides
-        observed_range_m: tidal range observed by the satellite
-        all_range_m: full astronomical tidal range based on all
-                  available tides
-        spread_m: proportion of the full astronomical tidal range observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-        low_tide_offset: proportion of the lowest tides never observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-        high_tide_offset: proportion of the highest tides never observed
-                  by the satellite (see Bishop-Taylor et al. 2018)
-
-    If `linear_reg = True`, the output will also contain:
-
-        observed_slope: slope of any relationship between observed tide
-                  heights and time
-        all_slope: slope of any relationship between all available tide
-                  heights and time
-        observed_pval: significance/p-value of any relationship between
-                  observed tide heights and time
-        all_pval: significance/p-value of any relationship between
-                  all available tide heights and time
-
-    """
-
-    # Load tide modelling functions from either OTPS for pyfes
-    try:
-        from otps import TimePoint
-        from otps import predict_tide
-    except ImportError:
-        from dea_tools.pyfes_model import TimePoint, predict_tide
-
-    # Model tides for each observation in the supplied xarray object
-    ds_tides, tidepost_lon, tidepost_lat = tidal_tag_otps(
-        ds, tidepost_lat=tidepost_lat, tidepost_lon=tidepost_lon, return_tideposts=True
-    )
-
-    # Drop spatial ref for nicer plotting
-    if "spatial_ref" in ds_tides:
-        ds_tides = ds_tides.drop("spatial_ref")
-
-    # Generate range of times covering entire period of satellite record
-    all_timerange = pd.date_range(
-        start=ds_tides.time.min().item(),
-        end=ds_tides.time.max().item(),
-        freq=modelled_freq,
-    )
-    all_datetimes = all_timerange.values.astype("M8[s]").astype("O").tolist()
-
-    # Use the tidal model to compute tide heights for each observation:
-    all_timepoints = [TimePoint(tidepost_lon, tidepost_lat, dt) for dt in all_datetimes]
-    all_predictedtides = predict_tide(all_timepoints)
-    all_tideheights = [predictedtide.tide_m for predictedtide in all_predictedtides]
-
-    # Get coarse statistics on all and observed tidal ranges
-    obs_mean = ds_tides.tide_m.mean().item()
-    all_mean = np.mean(all_tideheights)
-    obs_min, obs_max = ds_tides.tide_m.quantile([0.0, 1.0]).values
-    all_min, all_max = np.quantile(all_tideheights, [0.0, 1.0])
-
-    # Calculate tidal range
-    obs_range = obs_max - obs_min
-    all_range = all_max - all_min
-
-    # Calculate Bishop-Taylor et al. 2018 tidal metrics
-    spread = obs_range / all_range
-    low_tide_offset = abs(all_min - obs_min) / all_range
-    high_tide_offset = abs(all_max - obs_max) / all_range
-
-    # Extract x (time in decimal years) and y (distance) values
-    all_x = (
-        all_timerange.year
-        + ((all_timerange.dayofyear - 1) / 365)
-        + ((all_timerange.hour - 1) / 24)
-    )
-    all_y = all_tideheights
-    time_period = all_x.max() - all_x.min()
-
-    # Extract x (time in decimal years) and y (distance) values
-    obs_x = (
-        ds_tides.time.dt.year
-        + ((ds_tides.time.dt.dayofyear - 1) / 365)
-        + ((ds_tides.time.dt.hour - 1) / 24)
-    )
-    obs_y = ds_tides.tide_m.values.astype(np.float)
-
-    # Compute linear regression
-    obs_linreg = stats.linregress(x=obs_x, y=obs_y)
-    all_linreg = stats.linregress(x=all_x, y=all_y)
-
-    if plain_english:
-
-        print(
-            f"\n{spread:.0%} of the {all_range:.2f} m modelled astronomical "
-            f"tidal range is observed at this location.\nThe lowest "
-            f"{low_tide_offset:.0%} and highest {high_tide_offset:.0%} "
-            f"of astronomical tides are never observed.\n"
-        )
-        
-        if linear_reg:
-
-            # Plain english
-            if obs_linreg.pvalue > 0.05:
-                print(
-                    f"Observed tides show no significant trends "
-                    f"over the ~{time_period:.0f} year period."
-                )
-            else:
-                obs_slope_desc = "decrease" if obs_linreg.slope < 0 else "increase"
-                print(
-                    f"Observed tides {obs_slope_desc} significantly "
-                    f"(p={obs_linreg.pvalue:.3f}) over time by "
-                    f"{obs_linreg.slope:.03f} m per year (i.e. a "
-                    f"~{time_period * obs_linreg.slope:.2f} m "
-                    f"{obs_slope_desc} over the ~{time_period:.0f} year period)."
-                )
-
-            if all_linreg.pvalue > 0.05:
-                print(
-                    f"All tides show no significant trends "
-                    f"over the ~{time_period:.0f} year period."
-                )
-            else:
-                all_slope_desc = "decrease" if all_linreg.slope < 0 else "increase"
-                print(
-                    f"All tides {all_slope_desc} significantly "
-                    f"(p={all_linreg.pvalue:.3f}) over time by "
-                    f"{all_linreg.slope:.03f} m per year (i.e. a "
-                    f"~{time_period * all_linreg.slope:.2f} m "
-                    f"{all_slope_desc} over the ~{time_period:.0f} year period)."
-                )
-
-    if plot:
-
-        # Create plot and add all time and observed tide data
-        fig, ax = plt.subplots(figsize=(10, 5))
-        ax.plot(all_timerange, all_tideheights, alpha=0.4)
-        ds_tides.tide_m.plot.line(
-            ax=ax, marker="o", linewidth=0.0, color="black", markersize=2
-        )
-
-        # Add horizontal lines for spread/offsets
-        ax.axhline(obs_min, color="black", linestyle=":", linewidth=1)
-        ax.axhline(obs_max, color="black", linestyle=":", linewidth=1)
-        ax.axhline(all_min, color="black", linestyle=":", linewidth=1)
-        ax.axhline(all_max, color="black", linestyle=":", linewidth=1)
-
-        # Add text annotations for spread/offsets
-        ax.annotate(
-            f"    High tide\n    offset ({high_tide_offset:.0%})",
-            xy=(all_timerange.max(), np.mean([all_max, obs_max])),
-            va="center",
-        )
-        ax.annotate(
-            f"    Spread\n    ({spread:.0%})",
-            xy=(all_timerange.max(), np.mean([obs_min, obs_max])),
-            va="center",
-        )
-        ax.annotate(
-            f"    Low tide\n    offset ({low_tide_offset:.0%})",
-            xy=(all_timerange.max(), np.mean([all_min, obs_min])),
-        )
-
-        # Remove top right axes and add labels
-        ax.spines["right"].set_visible(False)
-        ax.spines["top"].set_visible(False)
-        ax.set_ylabel("Tide height (m)")
-        ax.set_xlabel("")
-        ax.margins(x=0.015)
-
-    # Export pandas.Series containing tidal stats
-    output_stats = {
-        "tidepost_lat": tidepost_lat,
-        "tidepost_lon": tidepost_lon,
-        "observed_mean_m": obs_mean,
-        "all_mean_m": all_mean,
-        "observed_min_m": obs_min,
-        "all_min_m": all_min,
-        "observed_max_m": obs_max,
-        "all_max_m": all_max,
-        "observed_range_m": obs_range,
-        "all_range_m": all_range,
-        "spread": spread,
-        "low_tide_offset": low_tide_offset,
-        "high_tide_offset": high_tide_offset,
-    }
-
-    if linear_reg:
-        output_stats.update(
-            {
-                "observed_slope": obs_linreg.slope,
-                "all_slope": all_linreg.slope,
-                "observed_pval": obs_linreg.pvalue,
-                "all_pval": all_linreg.pvalue,
-            }
-        )
-
-    return pd.Series(output_stats).round(round_stats)
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/dask.py` & `dea-tools-0.2.8.dev9/dea_tools/dask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## dea_dask.py
 '''
-Tools for simplifying the creation of Dask clusters for parallelised computing.
+Description: A set of python functions for simplifying the creation of a
+local dask cluster.
 
 License: The code in this notebook is licensed under the Apache License,
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
 Australia data is licensed under the Creative Commons by Attribution 4.0
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data
@@ -12,14 +13,18 @@
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
 using the `open-data-cube` tag (you can view previously asked questions
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
 
 If you would like to report an issue with this script, you can file one on
 Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
 
+Functions included:
+    create_local_dask_cluster
+    create_dask_gateway_cluster
+
 Last modified: June 2022
 
 '''
 
 
 from importlib.util import find_spec
 import os
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/datahandling.py` & `dea-tools-0.2.8.dev9/dea_tools/datahandling.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 ## dea_datahandling.py
-"""
-Loading and manipulating Digital Earth Australia products and data
-using the Open Data Cube and xarray.
+'''
+Description: This file contains a set of python functions for handling
+Digital Earth Australia data.
 
 License: The code in this notebook is licensed under the Apache License,
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
 Australia data is licensed under the Creative Commons by Attribution 4.0
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data
 Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
 using the `open-data-cube` tag (you can view previously asked questions
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
 
-If you would like to report an issue with this script, you can file one
-on Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
+If you would like to report an issue with this script, you can file one on
+Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
 
-Last modified: February 2023
-"""
+Functions included:
+    load_ard
+    array_to_geotiff
+    mostcommon_crs
+    download_unzip
+    wofs_fuser
+    dilate
+    pan_sharpen_brovey
+    paths_to_datetimeindex
+    nearest
+    last
+    first
+    parallel_apply
+
+Last modified: August 2022
+
+'''
 
 # Import required packages
 import os
 import zipfile
+import numexpr
 import datetime
 import requests
 import warnings
 import odc.algo
 import dask
 import numpy as np
 import pandas as pd
+import numexpr as ne
 import dask.array as da
 import xarray as xr
-import skimage.transform
-import sklearn.decomposition
-from skimage.exposure import match_histograms
-from skimage.color import rgb2hsv, hsv2rgb
+from osgeo import gdal
 from random import randint
 from collections import Counter
 from odc.algo import mask_cleanup
 from datacube.utils import masking
 from scipy.ndimage import binary_dilation
 from datacube.utils.dates import normalise_dt
 
 
 def _dc_query_only(**kw):
     """
-    Remove load-only datacube parameters, the rest can be
-    passed to Query/dc.find_datasets.
+    Remove load-only parameters, the rest can be passed to Query
 
     Returns
     -------
     dict of query parameters
     """
 
-    def _impl(
-        measurements=None,
-        output_crs=None,
-        resolution=None,
-        resampling=None,
-        skip_broken_datasets=None,
-        dask_chunks=None,
-        fuse_func=None,
-        align=None,
-        datasets=None,
-        progress_cbk=None,
-        group_by=None,
-        **query,
-    ):
+    def _impl(measurements=None,
+              output_crs=None,
+              resolution=None,
+              resampling=None,
+              skip_broken_datasets=None,
+              dask_chunks=None,
+              fuse_func=None,
+              align=None,
+              datasets=None,
+              progress_cbk=None,
+              group_by=None,
+              **query):
         return query
 
     return _impl(**kw)
 
 
 def _common_bands(dc, products):
     """
@@ -91,428 +102,314 @@
             common = set(p.measurements)
             bands = list(p.measurements)
         else:
             common = common.intersection(set(p.measurements))
     return [band for band in bands if band in common]
 
 
-def load_ard(
-    dc,
-    products=None,
-    cloud_mask='fmask',
-    min_gooddata=0.00,
-    mask_pixel_quality=True,
-    mask_filters=None,
-    mask_contiguity=False,
-    fmask_categories=["valid", "snow", "water"],
-    s2cloudless_categories=["valid"],
-    ls7_slc_off=True,
-    dtype="auto",
-    predicate=None,
-    **kwargs,
-):
-
-    """
-    Load multiple Geoscience Australia Landsat or Sentinel 2
-    Collection 3 products (e.g. Landsat 5, 7, 8, 9; Sentinel 2A and 2B),
-    optionally apply pixel quality/cloud masking and contiguity masks, 
-    and drop time steps that contain greater than a minimum proportion 
-    of good quality (e.g. non-cloudy or shadowed) pixels.
-
-    The function supports loading the following Landsat products:
-        * ga_ls5t_ard_3
-        * ga_ls7e_ard_3
-        * ga_ls8c_ard_3
-        * ga_ls9c_ard_3
-
-    And Sentinel-2 products:
-        * ga_s2am_ard_3
-        * ga_s2bm_ard_3
-        
-    Cloud masking can be performed using the Fmask (Function of Mask)
-    cloud mask for Landsat and Sentinel-2, and the s2cloudless 
-    (Sentinel Hub cloud detector for Sentinel-2 imagery) cloud mask for 
-    Sentinel-2.
+def load_ard(dc,
+             products=None,
+             min_gooddata=0.0,
+             fmask_categories=['valid', 'snow', 'water'],
+             mask_pixel_quality=True,
+             mask_filters=None,
+             mask_contiguity=False,
+             ls7_slc_off=True,
+             predicate=None,
+             dtype='auto',
+             **kwargs):
+
+    """
+    Loads and combines Landsat Collection 3 or Sentinel 2 Definitive
+    and Near Real Time data for multiple sensors (i.e. ls5t, ls7e and
+    ls8c for Landsat; s2a and s2b for Sentinel 2), optionally applies
+    pixel quality and contiguity masks, and drops time steps that
+    contain greater than a minimum proportion of good quality (e.g. non-
+    cloudy or shadowed) pixels.
+
+    The function supports loading the following DEA products:
+
+        ga_ls5t_ard_3
+        ga_ls7e_ard_3
+        ga_ls8c_ard_3
+        s2a_ard_granule
+        s2b_ard_granule
+        s2a_nrt_granule
+        s2b_nrt_granule
 
-    Last modified: February 2023
+    Last modified: April 2022
 
     Parameters
     ----------
     dc : datacube Datacube object
-        The Datacube to connect to, i.e. ``dc = datacube.Datacube()``.
+        The Datacube to connect to, i.e. `dc = datacube.Datacube()`.
         This allows you to also use development datacubes if required.
     products : list
-        A list of product names to load. Valid options are
-        ['ga_ls5t_ard_3', 'ga_ls7e_ard_3', 'ga_ls8c_ard_3', 'ga_ls9c_ard_3']
-        for Landsat, ['ga_s2am_ard_3', 'ga_s2bm_ard_3'] for Sentinel 2.
-    cloud_mask : string, optional
-        The cloud mask used by the function. This is used for both 
-        masking out poor quality pixels (e.g. clouds) if
-        ``mask_pixel_quality=True``, and for calculating the 
-        ``min_gooddata`` percentage when dropping cloudy or low quality
-        satellite observations. Two cloud masks are supported:
-            * 'fmask': (default; available for Landsat, Sentinel-2)
-            * 's2cloudless' (Sentinel-2 only)
+        A list of product names to load data from. Valid options are
+        ['ga_ls5t_ard_3', 'ga_ls7e_ard_3', 'ga_ls8c_ard_3'] for Landsat,
+        ['s2a_ard_granule', 's2b_ard_granule'] for Sentinel 2 Definitive,
+        and ['s2a_nrt_granule', 's2b_nrt_granule'] for Sentinel 2 Near
+        Real Time (on the DEA Sandbox only).
     min_gooddata : float, optional
-        The minimum percentage of good quality pixels required for a 
-        satellite observation to be loaded. Defaults to 0.00 which will
-        return all observations regardless of pixel quality (set to e.g.
-        0.99 to return only observations with more than 99% good quality
-        pixels).
-    mask_pixel_quality : str or bool, optional
-        Whether to mask out poor quality (e.g. cloudy) pixels by setting 
-        them as nodata. Depending on the choice of cloud mask, the 
-        function will identify good quality pixels using the categories 
-        passed to the ``fmask_categories`` or ``s2cloudless_categories``
-        params. Set to False to turn off pixel quality masking completely. 
-        Poor quality pixels will be set to NaN (and convert all data to 
-        `float32`) if  ``dtype='auto'``, or be set to the data's native 
-        nodata value (usually -999) if ``dtype='native'`` (see 'dtype' 
-        below for more details).
+        An optional float giving the minimum percentage of good quality
+        pixels required for a satellite observation to be loaded.
+        Defaults to 0.0 which will return all observations regardless of
+        pixel quality (set to e.g. 0.99 to return only observations with
+        more than 99% good quality pixels).
+    fmask_categories : list, optional
+        An optional list of fmask category names to treat as good
+        quality pixels in the above `min_gooddata` calculation, and for
+        masking data by pixel quality (if `mask_pixel_quality=True`).
+        The default is `['valid', 'snow', 'water']` which will return
+        non-cloudy or shadowed land, snow and water pixels. Choose from:
+        'nodata', 'valid', 'cloud', 'shadow', 'snow', and 'water'.
+    mask_pixel_quality : bool, optional
+        An optional boolean indicating whether to mask out poor quality
+        pixels using fmask based on the `fmask_categories` provided
+        above. The default is True, which will set poor quality pixels
+        to NaN if `dtype='auto'` (which will convert the data to
+        'float32'), or set poor quality pixels to the data's native
+        nodata value if `dtype='native' (which can be useful for
+        reducing memory).
     mask_filters : iterable of tuples, optional
         Iterable tuples of morphological operations - ("<operation>", <radius>)
-        to apply to the inverted pixel quality mask, where:
-        operation: string; one of these morphological operations:
-            * ``'dilation'`` = Expands poor quality pixels/clouds outwards
-            * ``'erosion'``  = Shrinks poor quality pixels/clouds inwards
-            * ``'closing'``  = Remove small holes in clouds by expanding
-                               then shrinking poor quality pixels
-            * ``'opening'``  = Remove small or narrow clouds by shrinking
-                               then expanding poor quality pixels
+        to apply to the pixel quality mask, where:
+        operation: string, can be one of these morphological operations:
+            * ``'closing'``  = remove small holes in cloud - morphological closing
+            * ``'opening'``  = shrinks away small areas of the mask
+            * ``'dilation'`` = adds padding to the mask
+            * ``'erosion'``  = shrinks bright regions and enlarges dark regions
         radius: int
-        e.g. ``mask_filters=[('erosion', 5), ("opening", 2), ("dilation", 2)]``
+        e.g. ``mask_filters=[('erosion', 5),("opening", 2),("dilation", 2)]``
     mask_contiguity : str or bool, optional
-        Whether to mask out pixels that are missing data in any band
-        (i.e. "non-contiguous" pixels). This can be important for
-        generating clean composite datasets. The default of False will
-        not apply any contiguity mask.
-        If loading NBART data, set:
-            * ``mask_contiguity='nbart'`` (or ``mask_contiguity=True``)
-        If loading NBAR data, specify:
-            * ``mask_contiguity='nbar'``
+        An optional string or boolean indicating whether to mask out
+        pixels missing data in any band (i.e. "non-contiguous" values).
+        This can be important for generating clean composite datasets.
+        The default is False, which will ignore non-contiguous values
+        completely. If loading NBART data, set the parameter to:
+        `mask_contiguity='nbart_contiguity'`. If loading NBAR data,
+        specify `mask_contiguity='nbar_contiguity'` instead.
         Non-contiguous pixels will be set to NaN if `dtype='auto'`, or
-        set to the data's native nodata value if `dtype='native'` (see
-        'dtype' below).
-    fmask_categories : list, optional
-        A list of Fmask cloud mask categories to consider as good
-        quality pixels when calculating `min_gooddata` and when masking
-        data by pixel quality if ``mask_pixel_quality=True``.
-        The default is ``['valid', 'snow', 'water']``; all other Fmask
-        categories ('cloud', 'shadow', 'nodata') will be treated as low
-        quality pixels. Choose from: 'nodata', 'valid', 'cloud',
-        'shadow', 'snow', and 'water'.
-    s2cloudless_categories : list, optional
-        A list of s2cloudless cloud mask categories to consider as good
-        quality pixels when calculating `min_gooddata` and when masking
-        data by pixel quality if ``mask_pixel_quality=True``. The default
-        is `['valid']`; all other s2cloudless categories ('cloud',
-        'nodata') will be treated as low quality pixels. Choose from:
-        'nodata', 'valid', or 'cloud'.
+        set to the data's native nodata value if `dtype='native'`
+        (which can be useful for reducing memory).
+    dtype : string, optional
+        An optional parameter that controls the data type/dtype that
+        layers are coerced to after loading. Valid values: 'native',
+        'auto', 'float{16|32|64}'. When 'auto' is used, the data will be
+        converted to `float32` if masking is used, otherwise data will
+        be returned in the native data type of the data. Be aware that
+        if data is loaded in its native dtype, nodata and masked
+        pixels will be returned with the data's native nodata value
+        (typically -999), not NaN.
     ls7_slc_off : bool, optional
         An optional boolean indicating whether to include data from
         after the Landsat 7 SLC failure (i.e. SLC-off). Defaults to
         True, which keeps all Landsat 7 observations > May 31 2003.
-    dtype : string, optional
-        Controls the data type/dtype that layers are coerced to after
-        loading. Valid values: 'native', 'auto', and 'float{16|32|64}'.
-        When 'auto' is used, the data will be converted to `float32`
-        if masking is used, otherwise data will be returned in the
-        native data type of the data. Be aware that if data is loaded
-        in its native dtype, nodata and masked pixels will be returned
-        with the data's native nodata value (typically -999), not NaN.
     predicate : function, optional
-        DEPRECATED: Please use `dataset_predicate` instead.
-        An optional function that can be passed in to restrict the datasets that
-        are loaded. A predicate function should take a
-        `datacube.model.Dataset` object as an input (i.e. as returned
-        from `dc.find_datasets`), and return a boolean. For example,
-        a predicate function could be used to return True for only
-        datasets acquired in January: `dataset.time.begin.month == 1`
+        An optional function that can be passed in to restrict the
+        datasets that are loaded by the function. A predicate function
+        should take a `datacube.model.Dataset` object as an input (i.e.
+        as returned from `dc.find_datasets`), and return a boolean.
+        For example, a predicate function could be used to return True
+        for only datasets acquired in January:
+        `dataset.time.begin.month == 1`
     **kwargs :
         A set of keyword arguments to `dc.load` that define the
         spatiotemporal query and load parameters used to extract data.
         Keyword arguments can either be listed directly in the
         `load_ard` call like any other parameter (e.g.
         `measurements=['nbart_red']`), or by passing in a query kwarg
         dictionary (e.g. `**query`). Keywords can include `measurements`,
         `x`, `y`, `time`, `resolution`, `resampling`, `group_by`, `crs`;
         see the `dc.load` documentation for all possible options:
         https://datacube-core.readthedocs.io/en/latest/dev/api/generate/datacube.Datacube.load.html
 
     Returns
     -------
-    combined_ds : xarray.Dataset
-        An xarray.Dataset containing only satellite observations with
-        a proportion of good quality pixels greater than `min_gooddata`.
+    combined_ds : xarray Dataset
+        An xarray dataset containing only satellite observations that
+        contains greater than `min_gooddata` proportion of good quality
+        pixels.
 
     """
 
     #########
     # Setup #
     #########
 
-    # Verify that products were provided
-    if not products:
-        raise ValueError(
-            "Please provide a list of product names to load data from. "
-            "Valid options are: ['ga_ls5t_ard_3', 'ga_ls7e_ard_3', "
-            "'ga_ls8c_ard_3', 'ga_ls9c_ard_3'] for Landsat, and "
-            "['ga_s2am_ard_3', 'ga_s2bm_ard_3'] for Sentinel 2."
-        )
-
-    # Determine whether products are all Landsat, all S2, or mixed
-    elif all(["ls" in product for product in products]):
-        product_type = "ls"
-    elif all(["s2" in product for product in products]):
-        product_type = "s2"
-    else:
-        product_type = "mixed"
-
-        warnings.warn(
-            "You have selected a combination of Landsat and Sentinel-2 "
-            "products. This can produce unexpected results as these "
-            "products use the same names for different spectral bands "
-            "(e.g. Landsat and Sentinel-2's 'nbart_swir_2'); use with "
-            "caution."
-        )
-
-    # Set contiguity band depending on `mask_contiguity`;
-    # "oa_nbart_contiguity" if True, False or "nbart",
-    # "oa_nbar_contiguity" if "nbar"
-    if mask_contiguity in (True, False, "nbart"):
-        contiguity_band = "oa_nbart_contiguity"
+    # Use 'nbart_contiguity' by default if mask_contiguity is true
+    if mask_contiguity is True:
+        mask_contiguity = 'nbart_contiguity'
+
+    # We deal with `dask_chunks` separately
+    dask_chunks = kwargs.pop('dask_chunks', None)
+    requested_measurements = kwargs.pop('measurements', None)
+
+    # Warn user if they combine lazy load with min_gooddata
+    if (min_gooddata > 0.0) and dask_chunks is not None:
+        warnings.warn("Setting 'min_gooddata' percentage to > 0.0 "
+                      "will cause dask arrays to compute when "
+                      "loading pixel-quality data to calculate "
+                      "'good pixel' percentage. This can "
+                      "slow the return of your dataset.")
 
-    elif mask_contiguity == "nbar":
-        contiguity_band = "oa_nbar_contiguity"
-
-    else:
-
-        raise ValueError(
-            f"Unsupported value '{mask_contiguity}' passed to "
-            "`mask_contiguity`. Please provide either 'nbart', 'nbar', "
-            "True, or False."
-        )
-
-    # Set pixel quality (PQ) band depending on `cloud_mask`
-    if cloud_mask == 'fmask': 
-        pq_band = "oa_fmask"
-        pq_categories = fmask_categories
-
-    elif cloud_mask == "s2cloudless":
-        pq_band = "oa_s2cloudless_mask"
-        pq_categories = s2cloudless_categories
-
-        # Raise error if s2cloudless is requested for Landsat products
-        if product_type in ["ls", "mixed"]:
-
-            raise ValueError(
-                "The 's2cloudless' cloud mask is not available for "
-                "Landsat products. Please set `mask_pixel_quality` to "
-                "'fmask' or False."
-            )
-    else:
-
-        raise ValueError(
-            f"Unsupported value '{cloud_mask}' passed to "
-            "`cloud_mask`. Please provide either 'fmask', "
-            "'s2cloudless', True, or False."
-        )
-
-    # To ensure that the categorical PQ/contiguity masking bands are
-    # loaded using nearest neighbour resampling, we need to add these to
-    # the resampling kwarg if it exists and is not "nearest". 
-    # This only applies if a string resampling method is supplied; 
-    # if a resampling dictionary (e.g. `resampling={'*': 'bilinear',
-    # 'oa_fmask': 'mode'}` is passed instead we assume the user wants 
-    # to select custom resampling methods for each of their bands.
-    resampling = kwargs.get("resampling", None)
-
-    if isinstance(resampling, str) and resampling not in (None, "nearest"):
-        kwargs["resampling"] = {
-            "*": resampling,
-            pq_band: "nearest",
-            contiguity_band: "nearest",
-        }
-
-    # We extract and deal with `dask_chunks` separately as every
-    # function call uses dask internally regardless of whether the user
-    # sets `dask_chunks` themselves
-    dask_chunks = kwargs.pop("dask_chunks", None)
-
-    # Create a list of requested measurements so that we can eventually
-    # return only the measurements the user orignally asked for
-    requested_measurements = kwargs.pop("measurements", None)
-
-    # Copy our measurements list so we can temporarily append extra PQ
-    # and/or contiguity masking bands when loading our data
-    measurements = requested_measurements.copy() if requested_measurements else None
+    # Verify that products were provided, and determine if Sentinel-2
+    # or Landsat data is being loaded
+    if not products:
+        raise ValueError("Please provide a list of product names "
+                         "to load data from. Valid options are: \n"
+                         "['ga_ls5t_ard_3', 'ga_ls7e_ard_3', 'ga_ls8c_ard_3'] "
+                         "for Landsat, ['s2a_ard_granule', "
+                         "'s2b_ard_granule'] \nfor Sentinel 2 Definitive, or "
+                         "['s2a_nrt_granule', 's2b_nrt_granule'] for "
+                         "Sentinel 2 Near Real Time")
+    elif all(['ls' in product for product in products]):
+        product_type = 'ls'
+    elif all(['s2' in product for product in products]):
+        product_type = 's2'
+
+    fmask_band = 'fmask'
+    measurements = (requested_measurements.copy() if
+                    requested_measurements else None)
 
-    # Deal with "load all" case: pick a set of bands that are common
-    # across requested products
     if measurements is None:
 
+        # Deal with "load all" case: pick a set of bands common across
+        # all products
         measurements = _common_bands(dc, products)
 
-    # Deal with edge case where user supplies alias for PQ/contiguity
-    # by stripping PQ/contiguity masks of their "oa_" prefix
-    else:
-
-        contiguity_band = (
-            contiguity_band.replace("oa_", "")
-            if contiguity_band.replace("oa_", "") in measurements
-            else contiguity_band
-        )
-        pq_band = (
-            pq_band.replace("oa_", "")
-            if pq_band.replace("oa_", "") in measurements
-            else pq_band
-        )
+        # If no `measurements` are specified, Landsat ancillary bands are
+        # loaded with a 'oa_' prefix, but Sentinel-2 bands are not. As a
+        # work-around, we need to rename the default contiguity and fmask
+        # bands if loading Landsat data without specifying `measurements`
+        if product_type == 'ls':
+            mask_contiguity = (f'oa_{mask_contiguity}' if
+                               mask_contiguity else False)
+            fmask_band = f'oa_{fmask_band}'
 
-    # If `measurements` are specified but do not include PQ or
+    # If `measurements` are specified but do not include fmask or
     # contiguity variables, add these to `measurements`
-    if pq_band not in measurements:
-        measurements.append(pq_band)
-    if mask_contiguity and contiguity_band not in measurements:
-        measurements.append(contiguity_band)
+    if fmask_band not in measurements:
+        measurements.append(fmask_band)
+    if mask_contiguity and mask_contiguity not in measurements:
+        measurements.append(mask_contiguity)
 
     # Get list of data and mask bands so that we can later exclude
     # mask bands from being masked themselves
-    data_bands = [
-        band for band in measurements if band not in (pq_band, contiguity_band)
-    ]
+    data_bands = [band for band in measurements if
+                  band not in (fmask_band, mask_contiguity)]
     mask_bands = [band for band in measurements if band not in data_bands]
 
     #################
     # Find datasets #
     #################
 
     # Pull out query params only to pass to dc.find_datasets
     query = _dc_query_only(**kwargs)
 
-    # If predicate is specified, use this function to filter the list
-    # of datasets prior to load
-    if predicate:
-        print(
-            "The 'predicate' parameter will be deprecated in future "
-            "versions of this function as this functionality has now "
-            "been added to Datacube itself. Please use "
-            "`dataset_predicate=...` instead."
-        )
-        query["dataset_predicate"] = predicate
-
-    # Extract list of datasets for each product using query params
+    # Extract datasets for each product using subset of dcload_kwargs
     dataset_list = []
 
     # Get list of datasets for each product
-    print("Finding datasets")
+    print('Finding datasets')
     for product in products:
 
         # Obtain list of datasets for product
-        print(
-            f"    {product} (ignoring SLC-off observations)"
-            if not ls7_slc_off and product == "ga_ls7e_ard_3"
-            else f"    {product}"
-        )
+        print(f'    {product} (ignoring SLC-off observations)'
+              if not ls7_slc_off and product == 'ga_ls7e_ard_3'
+              else f'    {product}')
         datasets = dc.find_datasets(product=product, **query)
 
         # Remove Landsat 7 SLC-off observations if ls7_slc_off=False
-        if not ls7_slc_off and product == "ga_ls7e_ard_3":
-            datasets = [
-                i
-                for i in datasets
-                if normalise_dt(i.time.begin) < datetime.datetime(2003, 5, 31)
-            ]
+        if not ls7_slc_off and product == 'ga_ls7e_ard_3':
+            datasets = [i for i in datasets if
+                        normalise_dt(i.time.begin) <
+                        datetime.datetime(2003, 5, 31)]
 
         # Add any returned datasets to list
         dataset_list.extend(datasets)
 
     # Raise exception if no datasets are returned
     if len(dataset_list) == 0:
-        raise ValueError(
-            "No data available for query: ensure that "
-            "the products specified have data for the "
-            "time and location requested"
-        )
+        raise ValueError("No data available for query: ensure that "
+                         "the products specified have data for the "
+                         "time and location requested")
+
+    # If predicate is specified, use this function to filter the list
+    # of datasets prior to load
+    if predicate:
+        print(f'Filtering datasets using predicate function')
+        dataset_list = [ds for ds in dataset_list if predicate(ds)]
+
+    # Raise exception if filtering removes all datasets
+    if len(dataset_list) == 0:
+        raise ValueError("No data available after filtering with "
+                         "predicate function")
 
     #############
     # Load data #
     #############
 
     # Note we always load using dask here so that we can lazy load data
-    # before filtering by `min_gooddata`
-    ds = dc.load(
-        datasets=dataset_list,
-        measurements=measurements,
-        dask_chunks={} if dask_chunks is None else dask_chunks,
-        **kwargs,
-    )
+    # before filtering by good data
+    ds = dc.load(datasets=dataset_list,
+                 measurements=measurements,
+                 dask_chunks={} if dask_chunks is None else dask_chunks,
+                 **kwargs)
 
     ####################
     # Filter good data #
     ####################
 
     # Calculate pixel quality mask
-    pq_mask = odc.algo.fmask_to_bool(ds[pq_band], categories=pq_categories)
+    pq_mask = odc.algo.fmask_to_bool(ds[fmask_band],
+                                     categories=fmask_categories)
 
-    # The good data percentage calculation has to load all pixel quality
+    # The good data percentage calculation has to load in all `fmask`
     # data, which can be slow. If the user has chosen no filtering
     # by using the default `min_gooddata = 0`, we can skip this step
     # completely to save processing time
     if min_gooddata > 0.0:
 
         # Compute good data for each observation as % of total pixels
-        print(f"Counting good quality pixels for each time step using {cloud_mask}")
-        data_perc = pq_mask.sum(axis=[1, 2], dtype="int32") / (
-            pq_mask.shape[1] * pq_mask.shape[2]
-        )
+        print('Counting good quality pixels for each time step')
+        data_perc = (pq_mask.sum(axis=[1, 2], dtype='int32') /
+                     (pq_mask.shape[1] * pq_mask.shape[2]))
         keep = (data_perc >= min_gooddata).persist()
 
         # Filter by `min_gooddata` to drop low quality observations
         total_obs = len(ds.time)
         ds = ds.sel(time=keep)
         pq_mask = pq_mask.sel(time=keep)
 
-        print(
-            f"Filtering to {len(ds.time)} out of {total_obs} "
-            f"time steps with at least {min_gooddata:.1%} "
-            f"good quality pixels"
-        )
-
+        print(f'Filtering to {len(ds.time)} out of {total_obs} '
+              f'time steps with at least {min_gooddata:.1%} '
+              f'good quality pixels')
+    
     # Morphological filtering on cloud masks
-    if (mask_filters is not None) & (mask_pixel_quality != False):
+    if (mask_filters is not None) & (mask_pixel_quality):
         print(f"Applying morphological filters to pixel quality mask: {mask_filters}")
-        pq_mask = ~mask_cleanup(~pq_mask, mask_filters=mask_filters)
-
-        warnings.warn(
-            "As of `dea_tools` v1.0.0, pixel quality masks are "
-            "inverted before being passed to `mask_filters` (i.e. so "
-            "that good quality/clear pixels are False and poor quality "
-            "pixels/clouds are True). This means that 'dilation' will "
-            "now expand cloudy pixels, rather than shrink them as in "
-            "previous versions."
-        )
-
+        pq_mask = mask_cleanup(pq_mask, mask_filters=mask_filters)
+    
     ###############
     # Apply masks #
     ###############
 
-    # Create a combined mask to hold both pixel quality and contiguity.
-    # This is more efficient than creating multiple dask tasks for 
-    # similar masking operations.
+    # Create an overall mask to hold both pixel quality and contiguity
     mask = None
 
-    # Add pixel quality mask to combined mask
+    # Add pixel quality mask to overall mask
     if mask_pixel_quality:
-        print(f"Applying {cloud_mask} pixel quality/cloud mask")
+        print('Applying pixel quality/cloud mask')
         mask = pq_mask
 
-    # Add contiguity mask to combined mask
+    # Add contiguity mask to overall mask
     if mask_contiguity:
-        print(f"Applying contiguity mask ({contiguity_band})")
-        cont_mask = ds[contiguity_band] == 1
+        print('Applying contiguity mask')
+        cont_mask = ds[mask_contiguity] == 1
 
         # If mask already has data if mask_pixel_quality == True,
         # multiply with cont_mask to perform a logical 'or' operation
         # (keeping only pixels good in both)
         mask = cont_mask if mask is None else mask * cont_mask
 
     # Split into data/masks bands, as conversion to float and masking
@@ -522,20 +419,20 @@
 
     # Mask data if either of the above masks were generated
     if mask is not None:
         ds_data = odc.algo.keep_good_only(ds_data, where=mask)
 
     # Automatically set dtype to either native or float32 depending
     # on whether masking was requested
-    if dtype == "auto":
-        dtype = "native" if mask is None else "float32"
+    if dtype == 'auto':
+        dtype = 'native' if mask is None else 'float32'
 
     # Set nodata values using odc.algo tools to reduce peak memory
     # use when converting data dtype
-    if dtype != "native":
+    if dtype != 'native':
         ds_data = odc.algo.to_float(ds_data, dtype=dtype)
 
     # Put data and mask bands back together
     attrs = ds.attrs
     ds = xr.merge([ds_data, ds_masks])
     ds.attrs.update(attrs)
 
@@ -543,24 +440,83 @@
     # Return data #
     ###############
 
     # Drop bands not originally requested by user
     if requested_measurements:
         ds = ds[requested_measurements]
 
-    # If user supplied `dask_chunks`, return data as a dask array
-    # without actually loading it into memory
+    # If user supplied dask_chunks, return data as a dask array without
+    # actually loading it in
     if dask_chunks is not None:
-        print(f"Returning {len(ds.time)} time steps as a dask array")
+        print(f'Returning {len(ds.time)} time steps as a dask array')
         return ds
     else:
-        print(f"Loading {len(ds.time)} time steps")
+        print(f'Loading {len(ds.time)} time steps')
         return ds.compute()
 
 
+def array_to_geotiff(fname, data, geo_transform, projection,
+                     nodata_val=0, dtype=gdal.GDT_Float32):
+    """
+    Create a single band GeoTIFF file with data from an array.
+
+    Because this works with simple arrays rather than xarray datasets
+    from DEA, it requires geotransform info ("(upleft_x, x_size,
+    x_rotation, upleft_y, y_rotation, y_size)") and projection data
+    (in "WKT" format) for the output raster. These are typically
+    obtained from an existing raster using the following GDAL calls:
+
+        import gdal
+        gdal_dataset = gdal.Open(raster_path)
+        geotrans = gdal_dataset.GetGeoTransform()
+        prj = gdal_dataset.GetProjection()
+
+    ...or alternatively, directly from an xarray dataset:
+
+        geotrans = xarraydataset.geobox.transform.to_gdal()
+        prj = xarraydataset.geobox.crs.wkt
+
+    Parameters
+    ----------
+    fname : str
+        Output geotiff file path including extension
+    data : numpy array
+        Input array to export as a geotiff
+    geo_transform : tuple
+        Geotransform for output raster; e.g. "(upleft_x, x_size,
+        x_rotation, upleft_y, y_rotation, y_size)"
+    projection : str
+        Projection for output raster (in "WKT" format)
+    nodata_val : int, optional
+        Value to convert to nodata in the output raster; default 0
+    dtype : gdal dtype object, optional
+        Optionally set the dtype of the output raster; can be
+        useful when exporting an array of float or integer values.
+        Defaults to gdal.GDT_Float32
+
+    """
+
+    # Set up driver
+    driver = gdal.GetDriverByName('GTiff')
+
+    # Create raster of given size and projection
+    rows, cols = data.shape
+    dataset = driver.Create(fname, cols, rows, 1, dtype)
+    dataset.SetGeoTransform(geo_transform)
+    dataset.SetProjection(projection)
+
+    # Write data to array and set nodata values
+    band = dataset.GetRasterBand(1)
+    band.WriteArray(data)
+    band.SetNoDataValue(nodata_val)
+
+    # Close file
+    dataset = None
+
+
 def mostcommon_crs(dc, product, query):
     """
     Takes a given query and returns the most common CRS for observations
     returned for that spatial extent. This can be useful when your study
     area lies on the boundary of two UTM zones, forcing you to decide
     which CRS to use for your `output_crs` in `dc.load`.
 
@@ -573,65 +529,63 @@
         A product name (or list of product names) to load CRSs from.
     query : dict
         A datacube query including x, y and time range to assess for the
         most common CRS
 
     Returns
     -------
-    epsg_string : str
-        An EPSG string giving the most common CRS from all datasets
-        returned by the query above
+    A EPSG string giving the most common CRS from all datasets returned
+    by the query above
 
     """
-
-    # Find list of datasets matching query for either product or
+    
+    # Find list of datasets matching query for either product or 
     # list of products
     if isinstance(product, list):
         matching_datasets = []
         for i in product:
-            matching_datasets.extend(dc.find_datasets(product=i, **query))
+            matching_datasets.extend(dc.find_datasets(product=i, 
+                                                      **query))        
     else:
         matching_datasets = dc.find_datasets(product=product, **query)
 
     # Extract all CRSs
     crs_list = [str(i.crs) for i in matching_datasets]
-
+    
     # If CRSs are returned
     if len(crs_list) > 0:
 
         # Identify most common CRS
         crs_counts = Counter(crs_list)
         crs_mostcommon = crs_counts.most_common(1)[0][0]
 
         # Warn user if multiple CRSs are encountered
         if len(crs_counts.keys()) > 1:
 
-            warnings.warn(
-                f"Multiple UTM zones {list(crs_counts.keys())} "
-                f"were returned for this query. Defaulting to "
-                f"the most common zone: {crs_mostcommon}",
-                UserWarning,
-            )
+            warnings.warn(f'Multiple UTM zones {list(crs_counts.keys())} '
+                          f'were returned for this query. Defaulting to '
+                          f'the most common zone: {crs_mostcommon}',
+                          UserWarning)
 
         return crs_mostcommon
-
+    
     else:
-
-        raise ValueError(
-            f"No CRS was returned as no data was found for "
-            f"the supplied product ({product}) and query. "
-            f"Please ensure that data is available for "
-            f"{product} for the spatial extents and time "
-            f"period specified in the query (e.g. by using "
-            f"the Data Cube Explorer for this datacube "
-            f"instance)."
-        )
+        
+        raise ValueError(f'No CRS was returned as no data was found for '
+                         f'the supplied product ({product}) and query. '
+                         f'Please ensure that data is available for '
+                         f'{product} for the spatial extents and time '
+                         f'period specified in the query (e.g. by using '
+                         f'the Data Cube Explorer for this datacube '
+                         f'instance).')
 
 
-def download_unzip(url, output_dir=None, remove_zip=True):
+def download_unzip(url,
+                   output_dir=None,
+                   remove_zip=True):
     """
     Downloads and unzips a .zip file from an external URL to a local
     directory.
 
     Parameters
     ----------
     url : str
@@ -648,43 +602,39 @@
 
     """
 
     # Get basename for zip file
     zip_name = os.path.basename(url)
 
     # Raise exception if the file is not of type .zip
-    if not zip_name.endswith(".zip"):
-        raise ValueError(
-            f"The URL provided does not point to a .zip "
-            f"file (e.g. {zip_name}). Please specify a "
-            f"URL path to a valid .zip file"
-        )
+    if not zip_name.endswith('.zip'):
+        raise ValueError(f'The URL provided does not point to a .zip '
+                         f'file (e.g. {zip_name}). Please specify a '
+                         f'URL path to a valid .zip file')
 
     # Download zip file
-    print(f"Downloading {zip_name}")
+    print(f'Downloading {zip_name}')
     r = requests.get(url)
-    with open(zip_name, "wb") as f:
+    with open(zip_name, 'wb') as f:
         f.write(r.content)
 
     # Extract into output_dir
-    with zipfile.ZipFile(zip_name, "r") as zip_ref:
+    with zipfile.ZipFile(zip_name, 'r') as zip_ref:
         zip_ref.extractall(output_dir)
-        print(
-            f"Unzipping output files to: "
-            f"{output_dir if output_dir else os.getcwd()}"
-        )
+        print(f'Unzipping output files to: '
+              f'{output_dir if output_dir else os.getcwd()}')
 
     # Optionally cleanup
     if remove_zip:
         os.remove(zip_name)
 
 
 def wofs_fuser(dest, src):
     """
-    Fuse two WOfS water measurements represented as ``ndarray``s.
+    Fuse two WOfS water measurements represented as `ndarray`s.
 
     Note: this is a copy of the function located here:
     https://github.com/GeoscienceAustralia/digitalearthau/blob/develop/digitalearthau/utils.py
     """
     empty = (dest & 1).astype(np.bool)
     both = ~empty & ~((src & 1).astype(np.bool))
     dest[empty] = src[empty]
@@ -716,28 +666,68 @@
     Returns
     -------
     An array of the same shape as `array`, with valid data pixels
     dilated by the number of pixels specified by `dilation`.
     """
 
     y, x = np.ogrid[
-        -dilation : (dilation + 1),
-        -dilation : (dilation + 1),
+        -dilation: (dilation + 1),
+        -dilation: (dilation + 1),
     ]
 
     # disk-like radial dilation
     kernel = (x * x) + (y * y) <= (dilation + 0.5) ** 2
 
     # If invert=True, invert True values to False etc
     if invert:
         array = ~array
 
-    return ~binary_dilation(
-        array.astype(np.bool), structure=kernel.reshape((1,) + kernel.shape)
-    )
+    return ~binary_dilation(array.astype(np.bool),
+                            structure=kernel.reshape((1,) + kernel.shape))
+
+
+def pan_sharpen_brovey(band_1, band_2, band_3, pan_band):
+    """
+    Brovey pan sharpening on surface reflectance input using numexpr
+    and return three xarrays.
+
+    Parameters
+    ----------
+    band_1, band_2, band_3 : xarray.DataArray or numpy.array
+        Three input multispectral bands, either as xarray.DataArrays or
+        numpy.arrays. These bands should have already been resampled to
+        the spatial resolution of the panchromatic band.
+    pan_band : xarray.DataArray or numpy.array
+        A panchromatic band corresponding to the above multispectral
+        bands that will be used to pan-sharpen the data.
+
+    Returns
+    -------
+    band_1_sharpen, band_2_sharpen, band_3_sharpen : numpy.arrays
+        Three numpy arrays equivelent to `band_1`, `band_2` and `band_3`
+        pan-sharpened to the spatial resolution of `pan_band`.
+
+    """
+    # Calculate total
+    exp = 'band_1 + band_2 + band_3'
+    total = numexpr.evaluate(exp)
+
+    # Perform Brovey Transform in form of: band/total*panchromatic
+    exp = 'a/b*c'
+    band_1_sharpen = numexpr.evaluate(exp, local_dict={'a': band_1,
+                                                       'b': total,
+                                                       'c': pan_band})
+    band_2_sharpen = numexpr.evaluate(exp, local_dict={'a': band_2,
+                                                       'b': total,
+                                                       'c': pan_band})
+    band_3_sharpen = numexpr.evaluate(exp, local_dict={'a': band_3,
+                                                       'b': total,
+                                                       'c': pan_band})
+
+    return band_1_sharpen, band_2_sharpen, band_3_sharpen
 
 
 def paths_to_datetimeindex(paths, string_slice=(0, 10)):
     """
     Helper function to generate a Pandas datetimeindex object
     from dates contained in a file path string.
 
@@ -749,30 +739,32 @@
         An optional tuple giving the start and stop position that
         contains the time information in the provided paths. These are
         applied to the basename (i.e. file name) in each path, not the
         path itself. Defaults to (0, 10).
 
     Returns
     -------
-    datetime : pandas.DatetimeIndex
-        A pandas.DatetimeIndex object containing a 'datetime64[ns]' derived
-        from the file paths provided by `paths`.
+    A pandas.DatetimeIndex object containing a 'datetime64[ns]' derived
+    from the file paths provided by `paths`.
     """
 
-    date_strings = [os.path.basename(i)[slice(*string_slice)] for i in paths]
+    date_strings = [os.path.basename(i)[slice(*string_slice)]
+                    for i in paths]
     return pd.to_datetime(date_strings)
 
 
 def _select_along_axis(values, idx, axis):
     other_ind = np.ix_(*[np.arange(s) for s in idx.shape])
     sl = other_ind[:axis] + (idx,) + other_ind[axis:]
     return values[sl]
 
 
-def first(array: xr.DataArray, dim: str, index_name: str = None) -> xr.DataArray:
+def first(array: xr.DataArray,
+          dim: str,
+          index_name: str = None) -> xr.DataArray:
     """
     Finds the first occuring non-null value along the given dimension.
 
     Parameters
     ----------
     array : xr.DataArray
          The array to search.
@@ -788,21 +780,24 @@
         of the same name, containing the value of that dimension where
         the last value was found.
     """
 
     axis = array.get_axis_num(dim)
     idx_first = np.argmax(~pd.isnull(array), axis=axis)
     reduced = array.reduce(_select_along_axis, idx=idx_first, axis=axis)
-    reduced[dim] = array[dim].isel({dim: xr.DataArray(idx_first, dims=reduced.dims)})
+    reduced[dim] = array[dim].isel({dim: xr.DataArray(idx_first,
+                                                      dims=reduced.dims)})
     if index_name is not None:
         reduced[index_name] = xr.DataArray(idx_first, dims=reduced.dims)
     return reduced
 
 
-def last(array: xr.DataArray, dim: str, index_name: str = None) -> xr.DataArray:
+def last(array: xr.DataArray,
+         dim: str,
+         index_name: str = None) -> xr.DataArray:
     """
     Finds the last occuring non-null value along the given dimension.
 
     Parameters
     ----------
     array : xr.DataArray
          The array to search.
@@ -822,23 +817,24 @@
         the last value was found.
     """
 
     axis = array.get_axis_num(dim)
     rev = (slice(None),) * axis + (slice(None, None, -1),)
     idx_last = -1 - np.argmax(~pd.isnull(array)[rev], axis=axis)
     reduced = array.reduce(_select_along_axis, idx=idx_last, axis=axis)
-    reduced[dim] = array[dim].isel({dim: xr.DataArray(idx_last, dims=reduced.dims)})
+    reduced[dim] = array[dim].isel({dim: xr.DataArray(idx_last,
+                                                      dims=reduced.dims)})
     if index_name is not None:
         reduced[index_name] = xr.DataArray(idx_last, dims=reduced.dims)
     return reduced
 
 
-def nearest(
-    array: xr.DataArray, dim: str, target, index_name: str = None
-) -> xr.DataArray:
+def nearest(array: xr.DataArray,
+            dim: str, target,
+            index_name: str = None) -> xr.DataArray:
     """
     Finds the nearest values to a target label along the given
     dimension, for all other dimensions.
 
     E.g. For a DataArray with dimensions ('time', 'x', 'y')
 
         nearest_array = nearest(array, 'time', '2017-03-12')
@@ -873,64 +869,68 @@
 
     before_target = slice(None, target)
     after_target = slice(target, None)
 
     da_before = array.sel({dim: before_target})
     da_after = array.sel({dim: after_target})
 
-    da_before = last(da_before, dim, index_name) if da_before[dim].shape[0] else None
-    da_after = first(da_after, dim, index_name) if da_after[dim].shape[0] else None
+    da_before = (last(da_before, dim, index_name) if
+                 da_before[dim].shape[0] else None)
+    da_after = (first(da_after, dim, index_name) if
+                da_after[dim].shape[0] else None)
 
     if da_before is None and da_after is not None:
         return da_after
     if da_after is None and da_before is not None:
         return da_before
 
     target = array[dim].dtype.type(target)
-    is_before_closer = abs(target - da_before[dim]) < abs(target - da_after[dim])
-    nearest_array = xr.where(is_before_closer, da_before, da_after, keep_attrs=True)
-    nearest_array[dim] = xr.where(is_before_closer, da_before[dim], da_after[dim], keep_attrs=True)
+    is_before_closer = (abs(target - da_before[dim]) <
+                        abs(target - da_after[dim]))
+    nearest_array = xr.where(is_before_closer, da_before, da_after)
+    nearest_array[dim] = xr.where(is_before_closer,
+                                  da_before[dim],
+                                  da_after[dim])
 
     if index_name is not None:
-        nearest_array[index_name] = xr.where(
-            is_before_closer, da_before[index_name], da_after[index_name], keep_attrs=True
-        )
-
+        nearest_array[index_name] = xr.where(is_before_closer,
+                                             da_before[index_name],
+                                             da_after[index_name])
     return nearest_array
 
 
 def parallel_apply(ds, dim, func, *args):
     """
-    Applies a custom function in parallel along the dimension of an
+    Applies a custom function in parallel along the dimension of an 
     xarray.Dataset or xarray.DataArray.
-
+    
     The function can be any function that can be applied to an
-    individual xarray.Dataset or xarray.DataArray (e.g. data for a
-    single timestep). The function should also return data in
+    individual xarray.Dataset or xarray.DataArray (e.g. data for a 
+    single timestep). The function should also return data in 
     xarray.Dataset or xarray.DataArray format.
-
+    
     This function is useful as a simple method for parallising code
     that cannot easily be parallised using Dask.
-
-    Parameters
-    ----------
+    
+    Parameters:
+    -----------
     ds : xarray.Dataset or xarray.DataArray
         xarray data with a dimension `dim` to apply the custom function
         along.
     dim : string
         The dimension along which the custom function will be applied.
     func : function
         The function that will be applied in parallel to each array
         along dimension `dim`. The first argument passed to this
         function should be the array along `dim`.
     *args :
         Any number of arguments that will be passed to `func`.
-
-    Returns
-    -------
+        
+    Returns:
+    --------
     xarray.Dataset
         A concatenated dataset containing an output for each array
         along the input `dim` dimension.
     """
 
     from concurrent.futures import ProcessPoolExecutor
     from tqdm import tqdm
@@ -941,463 +941,7 @@
         # Apply func in parallel
         groups = [group for (i, group) in ds.groupby(dim)]
         to_iterate = (groups, *(repeat(i, len(groups)) for i in args))
         out_list = list(tqdm(executor.map(func, *to_iterate), total=len(groups)))
 
     # Combine to match the original dataset
     return xr.concat(out_list, dim=ds[dim])
-
-
-def _apply_weights(da, band_weights):
-    """
-    Apply weights from a dictionary to the bands of a
-    multispectral xarray.DataArray.  Raises a ValueError if any
-    bands in `da` are not present in the `band_weights` dictionary.
-
-    Parameters
-    ----------
-    da : xarray.DataArray object
-        DataArray containing multispectral data. The dataarray
-        should contain a "variable" dimension that corresponds
-        to the different bands of the data.
-    band_weights : dict
-        Mapping of band names to weights to be applied. The keys
-        of the dictionary should be the names of the bands in the
-        "variable" dimension of `da`, and the values should be
-        the weights to be applied to each band.
-
-    Returns
-    -------
-    xarray.DataArray object
-        DataArray with weights applied to the bands.
-    """
-
-    # Identify any bands without weights, and raise an
-    # error if they exist
-    bands_without_weights = set(da["variable"].values) - set(band_weights.keys())
-    if len(bands_without_weights) > 0:
-        raise ValueError(
-            f"The following multispectral bands are missing from the "
-            f"`band_weights` dictionary: {bands_without_weights}.\n"
-            f"Ensure that weights are supplied for all multispectral "
-            f"bands in `ds`, or set `band_weights=None`."
-        )
-
-    # Create xr.DataArray with weights for each variable
-    # along the "variable" dimension
-    weights_da = xr.DataArray(
-        data=list(band_weights.values()),
-        coords={"variable": list(band_weights.keys())},
-        dims="variable",
-    )
-
-    # Apply weights
-    return da.weighted(weights_da)
-
-
-def _brovey_pansharpen(ds, pan_band, band_weights=None):
-    """
-    Perform pansharpening on multiple timesteps of a multispectral
-    dataset using the Brovey transform (with optional per-band weights).
-
-    Source: https://pro.arcgis.com/en/pro-app/latest/help/analysis/
-            raster-functions/fundamentals-of-pan-sharpening-pro.htm
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        Dataset containing multispectral and panchromatic bands.
-    pan_band : str
-        Name of the panchromatic band in the dataset.
-    band_weights : dict, optional
-        Mapping of band names to weights to be applied to each band when
-        calculating the sum of all multispectral bands. The keys of
-        the dictionary should be the names of the bands, and the values
-        should be the weights to apply to each band, e.g.:
-        ``{"nbart_red": 0.4, "nbart_green": 0.4, "nbart_blue": 0.2}``.
-        The default accounts for Landsat 8 and 9's pan band only
-        partially overlapping with the blue band; this may not be
-        suitable for all applications. Setting `band_weights=None`
-        will use a simple unweighted sum.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        Pansharpened dataset with the same dimensions as the input dataset.
-    """
-
-    # Create new dataarrays with and without pan band
-    da_nopan = ds.drop(pan_band).to_array()
-    da_pan = ds[pan_band]
-
-    # Calculate weighted sum
-    if band_weights is not None:
-        da_total = _apply_weights(da_nopan, band_weights).sum(dim="variable")
-    else:
-        da_total = da_nopan.sum(dim="variable")
-
-    # Perform Brovey Transform in form of: band / total * panchromatic
-    da_pansharpened = da_nopan / da_total * da_pan
-    ds_pansharpened = da_pansharpened.to_dataset("variable")
-
-    return ds_pansharpened
-
-
-def _esri_pansharpen(ds, pan_band, band_weights=None):
-    """
-    Perform pansharpening on multiple timesteps of a multispectral
-    dataset using the ESRI transform (with optional per-band weights).
-
-    Source: https://pro.arcgis.com/en/pro-app/latest/help/analysis/
-            raster-functions/fundamentals-of-pan-sharpening-pro.htm
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        Dataset containing multispectral and panchromatic bands.
-    pan_band : str
-        Name of the panchromatic band in the dataset.
-    band_weights : dict, optional
-        Mapping of band names to weights to be applied to each band when
-        calculating the mean of all multispectral bands. The keys of
-        the dictionary should be the names of the bands, and the values
-        should be the weights to apply to each band, e.g.:
-        ``{"nbart_red": 0.4, "nbart_green": 0.4, "nbart_blue": 0.2}``.
-        The default accounts for Landsat 8 and 9's pan band only
-        partially overlapping with the blue band; this may not be
-        suitable for all applications. Setting `band_weights=None`
-        will use a simple unweighted mean.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        Pansharpened dataset with the same dimensions as the input dataset.
-    """
-
-    # Create new dataarrays with and without pan band
-    da_nopan = ds.drop(pan_band).to_array()
-    da_pan = ds[pan_band]
-
-    # Calculate weighted sum
-    if band_weights is not None:
-        da_mean = _apply_weights(da_nopan, band_weights).mean(dim="variable")
-    else:
-        da_mean = da_nopan.mean(dim="variable")
-
-    # Calculate adjustment and apply to multispectral bands
-    adj = da_pan - da_mean
-    da_pansharpened = da_nopan + adj
-    ds_pansharpened = da_pansharpened.to_dataset("variable")
-
-    return ds_pansharpened
-
-
-def _simple_mean_pansharpen(ds, pan_band):
-    """
-    Perform pansharpening on multiple timesteps of a multispectral
-    dataset using the Simple Mean transform.
-
-    Source: https://pro.arcgis.com/en/pro-app/latest/help/analysis/
-            raster-functions/fundamentals-of-pan-sharpening-pro.htm
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        Dataset containing multispectral and panchromatic bands.
-    pan_band : str
-        Name of the panchromatic band in the dataset.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        Pansharpened dataset with the same dimensions as the input dataset.
-    """
-
-    # Create new dataarrays with and without pan band
-    ds_nopan = ds.drop(pan_band)
-    da_pan = ds[pan_band]
-
-    # Take mean of pan band and RGBs
-    ds_pansharpened = (ds_nopan + da_pan) / 2.0
-
-    return ds_pansharpened
-
-
-def _hsv_timestep_pansharpen(ds_i, pan_band):
-    """
-    Perform pansharpening on a single timestep of a multispectral
-    dataset using the Hue Saturation Value (HSV) transform.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        Dataset containing multispectral and panchromatic bands.
-    pan_band : str
-        Name of the panchromatic band in the dataset.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        Pansharpened dataset with the same dimensions as the input dataset.
-    """
-
-    # Convert to an xr.DataArray and move "variable" to end
-    da_i = ds_i.to_array().transpose(..., "variable")
-
-    # Create new dataarrays with and without pan band
-    da_i_nopan = da_i.drop(pan_band, dim="variable")
-    da_i_pan = da_i.sel(variable=pan_band)
-
-    # Convert to HSV colour space
-    hsv = rgb2hsv(da_i_nopan)
-
-    # Replace value (lightness) channel with pan band data
-    hsv[:, :, 2] = da_i_pan.values
-
-    # Convert back to RGB colour space
-    pansharped_array = hsv2rgb(hsv)
-
-    # Add back into original array, reshape and return dataframe
-    da_i_nopan[:] = pansharped_array
-    ds_pansharpened = da_i_nopan.to_dataset("variable")
-
-    return ds_pansharpened
-
-
-def _pca_timestep_pansharpen(ds_i, pan_band, pca_rescaling="histogram"):
-    """
-    Perform pansharpening on a single timestep of a multispectral
-    dataset using the principal component analysis (PCA) transform.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        Dataset containing multispectral and panchromatic bands.
-    pan_band : str
-        Name of the panchromatic band in the dataset.
-    pca_rescaling : str, optional
-        Method to use for rescaling pan band to more closely match the
-        distribution of values in the first PCA component. "simple"
-        scales the pan band values to more closely match the first PCA
-        component by subtracting the mean of the pan band values from
-        each value, scaling the resulting values by the ratio of the
-        standard deviations of the first PCA component and the pan band,
-        and adding back the mean of the first PCA component.
-        "histogram" uses a histogram matching technique to adjust the
-        pan band values so that the resulting histogram more closely
-        matches the histogram of the first PCA component.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        Pansharpened dataset with the same dimensions as the input dataset.
-    """
-
-    # Reshape to 2D by stacking x and y dimensions to prepare it
-    # as an input to PCA. Drop NA rows as these are not supported
-    # by `pca.fit_transform`.
-    da_2d = (
-        ds_i.to_array()
-        .stack(pixel=("y", "x"))
-        .transpose("pixel", "variable")
-        .dropna(dim="pixel")
-    )
-
-    # Create new dataarrays with and without pan band
-    da_2d_nopan = da_2d.drop(pan_band, dim="variable")
-    da_2d_pan = da_2d.sel(variable=pan_band)
-
-    # Apply PCA transformation
-    pca = sklearn.decomposition.PCA()
-    pca_array = pca.fit_transform(da_2d_nopan)
-
-    # Rescale pan band to more closely match the first PCA component
-    if pca_rescaling == "simple":
-        pca_array[:, 0] = (da_2d_pan.values - da_2d_pan.values.mean()) * (
-            pca_array[:, 0].std() / da_2d_pan.values.std()
-        ) + pca_array[:, 0].mean()
-    elif pca_rescaling == "histogram":
-        pca_array[:, 0] = match_histograms(da_2d_pan.values, pca_array[:, 0])
-
-    # Apply reverse PCA transform to restore multispectral array
-    pansharped_array = pca.inverse_transform(pca_array)
-
-    # Add back into original array, reshape and return dataframe
-    da_2d_nopan[:] = pansharped_array
-    ds_pansharpened = da_2d_nopan.unstack("pixel").to_dataset("variable")
-
-    return ds_pansharpened
-
-
-def xr_pansharpen(
-    ds,
-    transform,
-    pan_band="nbart_panchromatic",
-    return_pan=False,
-    output_dtype=None,
-    parallelise=False,
-    band_weights={"nbart_red": 0.4, "nbart_green": 0.4, "nbart_blue": 0.2},
-    pca_rescaling="histogram",
-):
-
-    """
-    Apply pan-sharpening to multispectral satellite data with one
-    or more timesteps. The following pansharpening transforms are
-    currently supported:
-
-        - Brovey ("brovey"), with optional band weighting
-        - ESRI ("esri"), with optional band weighting
-        - Simple mean ("simple mean")
-        - PCA ("pca")
-        - HSV ("hsv"), similar to IHS
-
-    Note: Pan-sharpening transforms do not necessarily maintain
-    the spectral integrity of the input satellite data, and may
-    be more suitable for visualisation than quantitative work.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        An xarrray dataset containing the three input multispectral
-        bands, and a panchromatic band. This dataset should have
-        already been resampled to the spatial resolution of the
-        panchromatic band (15 m for Landsat). Due to differences in
-        the electromagnetic spectrum covered by the panchromatic band,
-        Landsat 8 and 9 data should be supplied with 'blue', 'green',
-        and 'red' multispectral bands, while Landsat 7 should be
-        supplied with 'green', 'red' and 'NIR'.
-    transform : string
-        The pansharpening transform to apply to the data. Valid options
-        include "brovey", "esri", "simple mean", "pca", "hsv".
-    pan_band : string, optional
-        The name of the panchromatic band that will be used to
-        pansharpen the multispectral data.
-    return_pan : bool, optional
-        Whether to return the panchromatic band in the output dataset.
-        Defaults to False.
-    output_dtype : string or numpy.dtype, optional
-        The dtype used for the output values. Defaults to the input
-        dtype of the multispectral bands in `ds`.
-    parallelise: bool, optional
-        Whether to parallelise transformations across multiple cores.
-        Used for PCA and HSV transforms that are applied to each
-        timestep in `ds` individually; defaults to False.
-    band_weights : dict, optional
-        Used for the Brovey and ESRI transforms. Mapping of band
-        names to weights to be applied to each band when calculating
-        the sum (Brovey) or mean (ESRI) of all multispectral bands.
-        The keys of the dictionary should be the names of the bands,
-        and the values should be the weights to apply to each band, e.g.:
-        ``{"nbart_red": 0.4, "nbart_green": 0.4, "nbart_blue": 0.2}``.
-        The default accounts for Landsat 8 and 9's pan band only
-        partially overlapping with the blue band; this may not be
-        suitable for all applications. Setting `band_weights=None`
-        will use a simple unweighted sum (for the Brovey transform)
-        or unweighted mean (for the ESRI transform).
-    pca_rescaling : str, optional
-        Used for the PCA transform. The method to use for rescaling
-        pan band to more closely match the distribution of values
-        in the first PCA component. "simple" scales the pan band
-        values to more closely match the first PCA component by
-        subtracting the mean of the pan band values from each value,
-        scaling the resulting values by the ratio of the standard
-        deviations of the first PCA component and the pan band, and
-        adding back the mean of the first PCA component.
-        "histogram" uses a histogram matching technique to adjust the
-        pan band values so that the resulting histogram more closely
-        matches the histogram of the first PCA component.
-
-    Returns
-    -------
-    ds_pansharpened : xarray.Dataset
-        An xarrray dataset containing the three pansharpened input
-        multispectral bands and optionally the panchromatic band
-        (if `return_pan=True`).
-    """
-
-    # Assert whether pan band exists in the dataset
-    if pan_band not in ds.data_vars:
-        raise ValueError(
-            f"The specified panchromatic band '{pan_band}' cannot be found in `ds`. "
-            f"Specify a panchromatic band name that exists in the dataset using `pan_band=...`."
-        )
-
-    # Assert whether exactly three multispectral bands are included in `ds`
-    n_multi = len(ds.drop(pan_band).data_vars)
-    if n_multi != 3:
-        raise ValueError(
-            f"`ds` should contain exactly three multispectral bands (not "
-            f"including the panchromatic band). However, {n_multi} "
-            f"multispectral bands were found: {list(ds.drop(pan_band).data_vars)}. "
-        )
-
-    # Define dict linking functions to each transform
-    transform_dict = {
-        "brovey": _brovey_pansharpen,
-        "esri": _esri_pansharpen,
-        "simple mean": _simple_mean_pansharpen,
-        "pca": _pca_timestep_pansharpen,
-        "hsv": _hsv_timestep_pansharpen,
-    }
-
-    # If Brovey, ESRI or Simple Mean pansharpening is specified, apply to
-    # entire `xr.Dataset` in one go (with optional weights for Brovey, ESRI)
-    if transform in ("brovey", "esri", "simple mean"):
-        print(f"Applying {transform.capitalize()} pansharpening")
-        extra_params = (
-            {"band_weights": band_weights} if transform in ("brovey", "esri") else {}
-        )
-        ds_pansharpened = transform_dict[transform](
-            ds,
-            pan_band=pan_band,
-            **extra_params,
-        )
-
-    # Otherwise, apply PCA or HSV pansharpening to each
-    # timestep in the `xr.Dataset` using `.apply`
-    elif transform in ("pca", "hsv"):
-
-        extra_params = {"pca_rescaling": pca_rescaling} if transform == "pca" else {}
-
-        # Apply pansharpening to all timesteps in data in parallel
-        if ("time" in ds.dims) and parallelise:
-            print(
-                f"Applying {transform.upper()} pansharpening in parallel"
-            )
-            ds_pansharpened = parallel_apply(
-                ds,
-                "time",
-                transform_dict[transform],
-                pan_band,
-                *extra_params.values(),  # TODO: Update once `parallel_apply` supports kwargs
-            )
-
-        # Apply pansharpening to all timesteps in data sequentially
-        elif ("time" in ds.dims) and not parallelise:
-            print(f"Applying {transform.upper()} pansharpening")
-            ds_pansharpened = ds.groupby("time").apply(
-                transform_dict[transform],
-                pan_band=pan_band,
-                **extra_params,
-            )
-
-        # Otherwise, apply func directly if only one timestep
-        else:
-            print(f"Applying {transform.upper()} pansharpening")
-            ds_pansharpened = transform_dict[transform](
-                ds, pan_band=pan_band, **extra_params
-            )
-
-    else:
-        raise ValueError(
-            f"Unsupported value '{transform}' passed to `method`. Please "
-            f"provide one of {list(transform_dict.keys())}."
-        )
-
-    # Optionally insert pan band back into dataset
-    if return_pan:
-        ds_pansharpened[pan_band] = ds[pan_band]
-
-    # Return data in original or requested dtype
-    return ds_pansharpened.astype(
-        ds.to_array().dtype if output_dtype is None else output_dtype
-    )
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/landcover.py` & `dea-tools-0.2.8.dev9/dea_tools/landcover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 # Land_cover_plotting.py
 """
-Plotting and animating Digital Earth Australia Land Cover data.
-
-License: The code in this notebook is licensed under the Apache License,
-Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
-Australia data is licensed under the Creative Commons by Attribution 4.0
+Description: This file contains a set of python functions for plotting 
+Digital Earth Australia Land Cover data.
+License: The code in this notebook is licensed under the Apache License, 
+Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
+Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
-
 Contact: If you need assistance, please post a question on the Open Data
-Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack
-Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
-using the `open-data-cube` tag (you can view previously asked questions
-here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
-
-If you would like to report an issue with this script, you can file one
-on Github (https://github.com/GeoscienceAustralia/dea-notebooks/issues/new).
-
+Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack 
+Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) 
+using the `open-data-cube` tag (you can view previously asked questions 
+here: https://gis.stackexchange.com/questions/tagged/open-data-cube). 
+If you would like to report an issue with this script, file one on 
+Github: https://github.com/GeoscienceAustralia/dea-notebooks/issues/new
+Functions included:
+    get_layer_name
+    lc_colourmap
+    plot_land_cover
+    lc_animation
 Last modified: January 2022
 """
 
 import numpy as np
 import pandas as pd
 import ast
 import sys
@@ -267,29 +269,20 @@
     measurement = aliases[measurement] if measurement in aliases.keys(
     ) else measurement
     return measurement
 
 
 def make_colorbar(fig, ax, measurement, horizontal=False, animation=False):
     """
-    Adds a new colorbar with appropriate land cover colours and labels.
-
-    For DEA Land Cover Level 4 data, this function must be used with a double plot. 
-    The 'ax' should be on the left side of the figure, and the colour bar will added 
-    on the right hand side.
+    Adds a new colorbar with appropriate land cover colours and labels
     
-    Parameters
-    ----------
-    fig : matplotlib figure
-        Figure to add colourbar to
-    ax : matplotlib ax
-        Matplotlib figure ax to add colorbar to.
-    measurement : str
-        Land cover measurement to use for colour map and labels. 
+    measurement = land cover measurement to use for colour map and lables
     
+    for level 4, must be used with a double plot, ax should be the left side canvas
+    the colour bar will go over thr right hand side.
     """
     # Create new axis object for colorbar
     # parameters for add_axes are [left, bottom, width, height], in
     # fractions of total plot
     
     if measurement == 'level4' and animation == True:
         
@@ -339,27 +332,25 @@
 
 
 
 def lc_colourmap(colour_scheme, colour_bar=False):
     """
     Returns colour map and normalisation for the provided DEA Land Cover
     measurement, for use in plotting with Matplotlib library
-    
     Parameters
     ----------
     colour_scheme : string
         Name of land cover colour scheme to use
         Valid options: 'level3', 'level4', 'lifeform_veg_cat_l4a', 
         'canopyco_veg_cat_l4d', 'watersea_veg_cat_l4a_au',
         'waterstt_wat_cat_l4a', 'inttidal_wat_cat_l4a', 
         'waterper_wat_cat_l4d_au', 'baregrad_phy_cat_l4d_au'.
     colour_bar : bool, optional
         Controls if colour bar labels are returned as a list for 
         plotting a colour bar. Default: False.
-        
     Returns
     ---------
     cmap : matplotlib colormap
         Matplotlib colormap containing the colour scheme for the
         specified DEA Land Cover measurement.
     norm : matplotlib colormap index
         Matplotlib colormap index based on the discrete intervals of the
@@ -418,15 +409,15 @@
     data : xarray.DataArray
         A dataArray containing a DEA Land Cover classification.
     year : int, optional
         Can be used to select to plot a specific year. If not provided,
         all time slices are plotted.
     measurement : string, optional
         Name of the DEA land cover classification to be plotted. Passed to 
-        lc_colourmap to specify which colour scheme will be used. If non 
+        lc_colourmap to specify which colour scheme will ve used. If non 
         provided, reads data array name from `da` to determine.
     """
     # get measurement name
     measurement = get_layer_name(measurement, data)
 
     # get colour map, normalisation
     try:
@@ -482,55 +473,53 @@
         dpi=150,
         font_size=15,
         label_ax=True):
     """
     Creates an animation of DEA Landcover though time beside 
     corresponding stacked plots of the landcover classes. Saves the
     animation to a file and displays the animation in notebook.
-    
-    Parameters
-    ----------
+    Inputs
+    -------
     da : xarray.DataArray
         An xarray.DataArray containing a multi-date stack of 
         observations of a single landcover level.
     file_name: string, optional.
         string used to create filename for saved animation file.
         Default: "default_animation" code adds .gif suffix.
     measurement : string, optional
         Name of the DEA land cover classification to be plotted. Passed to 
         lc_colourmap to specify which colour scheme will ve used. If non 
         provided, reads data array name from `da` to determine.
-    stacked_plot: boolean, optional
+    Stacked_plot: boolean, optional
         Determines if a stacked plot showing the percentage of area
         taken up by each class in each time slice is added to the
         animation. Default: False.
     colour_bar : boolean, Optional
         Determines if a colour bar is generated for the stand alone 
         animation. This is NOT recommended for use with level 4 data. 
         Does not work with stacked plot. Default: False.
     animation_interval : int , optional
         How quickly the frames of the animations should be re-drawn. 
         Default: 500.
-    width_pixels : int, optional
+    Width_pixels : int, optional
         How wide in pixles the animation plot should be. Default: 10.
     dpi : int, optional
         Stands for 'Dots Per Inch'. Passed to the fuction that saves the
         animation and determines the resolution. A higher number will
         produce a higher resolution image but a larger file size and
         slower processing. Default: 150.
     font_size : int, optional. 
         Controls the size of the text which indicates the year
         displayed. Default: 15.
     label_ax : boolean, optional
         Determines if animation plot should have tick marks and numbers
         on axes. Also removes white space around plot. default: True
-        
     Returns
-    -------
-    A GIF (.gif) animation file.
+    ---------
+    A .gif file animation.
     """
 
     def calc_class_ratio(da):
         """
         Creates a table listing year by year what percentage of the
         total area is taken up by each class.
         Parameters
@@ -759,8 +748,8 @@
         frames=len(da.time),
         interval=animation_interval,
         repeat=False,
     )
 
     anim.save(file_name, writer="pillow", dpi=dpi)
     plt.close()
-    return Image(filename=file_name)
+    return Image(filename=file_name)
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/plotting.py` & `dea-tools-0.2.8.dev9/dea_tools/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## dea_plotting.py
 '''
-Plotting and animating Digital Earth Australia products and data.
+Description: This file contains a set of python functions for plotting 
+Digital Earth Australia data.
 
 License: The code in this notebook is licensed under the Apache License, 
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data
@@ -12,38 +13,57 @@
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) 
 using the `open-data-cube` tag (you can view previously asked questions 
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube). 
 
 If you would like to report an issue with this script, file one on 
 Github: https://github.com/GeoscienceAustralia/dea-notebooks/issues/new
 
-Last modified: April 2023
+Functions included:
+    rgb
+    display_map
+    xr_animation
+    plot_wo
+    plot_fmask
+
+Last modified: October 2021
 
 '''
 
 # Import required packages
 import math
+import branca
 import folium
+import calendar
+import ipywidgets
 import numpy as np
-import pandas as pd
 import geopandas as gpd
+import matplotlib as mpl
+import matplotlib.cm as cm
+from matplotlib import colors as mcolours
 import matplotlib.patheffects as PathEffects
 import matplotlib.pyplot as plt
-import xarray as xr
-from matplotlib import colors as mcolours
+import matplotlib.animation as animation
+from datetime import datetime
+from pyproj import Proj, transform
+from IPython.display import display
+from matplotlib.colors import ListedColormap
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+from ipyleaflet import Map, Marker, Popup, GeoJSON, basemaps, Choropleth
+from skimage import exposure
+from odc.ui import image_aspect
+import warnings
+
 from matplotlib.animation import FuncAnimation
+import pandas as pd
 from pathlib import Path
-from pyproj import Transformer
 from shapely.geometry import box
 from skimage.exposure import rescale_intensity
 from tqdm.auto import tqdm
-
-import odc.geo.xr
-from odc.ui import image_aspect
-from dea_tools.spatial import add_geobox
+import warnings
 
 
 def rgb(ds,
         bands=['nbart_red', 'nbart_green', 'nbart_blue'],
         index=None,
         index_dim='time',
         robust=True,
@@ -124,27 +144,32 @@
         
     Returns
     -------
     An RGB plot of one or multiple observations, and optionally an image
     file written to file.
     
     """
-    
+
     # Get names of x and y dims
-    y_dim, x_dim = ds.odc.spatial_dims
+    # TODO: remove geobox and try/except once datacube 1.8 is default
+    try:
+        y_dim, x_dim = ds.geobox.dimensions
+    except AttributeError:
+        from datacube.utils import spatial_dims
+        y_dim, x_dim = spatial_dims(ds)
 
     # If ax is supplied via kwargs, ignore aspect and size
     if 'ax' in kwargs:
 
         # Create empty aspect size kwarg that will be passed to imshow
         aspect_size_kwarg = {}
     else:
         # Compute image aspect
         if not aspect:
-            aspect = ds.odc.geobox.aspect
+            aspect = image_aspect(ds)
 
         # Populate aspect size kwarg with aspect and size data
         aspect_size_kwarg = {'aspect': aspect, 'size': size}
 
     # If no value is supplied for `index` (the default), plot using default
     # values and arguments passed via `**kwargs`
     if index is None:
@@ -245,15 +270,15 @@
 
 def display_map(x, y, crs='EPSG:4326', margin=-0.5, zoom_bias=0):
     """ 
     Given a set of x and y coordinates, this function generates an 
     interactive map with a bounded rectangle overlayed on Google Maps 
     imagery.        
     
-    Last modified: February 2023
+    Last modified: September 2019
     
     Modified from function written by Otto Wagner available here: 
     https://github.com/ceos-seo/data_cube_utilities/tree/master/data_cube_utilities
     
     Parameters
     ----------  
     x : (float, float)
@@ -281,16 +306,16 @@
     viewport is the closest it can possibly get to the centered 
     bounding rectangle without clipping it. 
     """
 
     # Convert each corner coordinates to lat-lon
     all_x = (x[0], x[1], x[0], x[1])
     all_y = (y[0], y[0], y[1], y[1])
-    transformer = Transformer.from_crs(crs, "EPSG:4326")
-    all_longitude, all_latitude = transformer.transform(all_x, all_y)
+    all_longitude, all_latitude = transform(Proj(crs), Proj('EPSG:4326'), all_x,
+                                            all_y)
 
     # Calculate zoom level based on coordinates
     lat_zoom_level = _degree_to_zoom_level(
         min(all_latitude), max(all_latitude), margin=margin) + zoom_bias
     lon_zoom_level = _degree_to_zoom_level(
         min(all_longitude), max(all_longitude), margin=margin) + zoom_bias
     zoom_level = min(lat_zoom_level, lon_zoom_level)
@@ -320,14 +345,203 @@
 
     # Add clickable lat-lon popup box
     interactive_map.add_child(folium.features.LatLngPopup())
 
     return interactive_map
 
 
+def map_shapefile(gdf,
+                  attribute,
+                  continuous=False,
+                  cmap='viridis',
+                  basemap=basemaps.Esri.WorldImagery,
+                  default_zoom=None,
+                  hover_col=True,
+                  **style_kwargs):
+    """
+    Plots a geopandas GeoDataFrame over an interactive ipyleaflet 
+    basemap, with features coloured based on attribute column values. 
+    Optionally, can be set up to print selected data from features in 
+    the GeoDataFrame. 
+
+    Last modified: February 2020
+
+    Parameters
+    ----------  
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame containing the spatial features to be plotted 
+        over the basemap.
+    attribute: string, required
+        An required string giving the name of any column in the
+        GeoDataFrame you wish to have coloured on the choropleth.
+    continuous: boolean, optional
+        Whether to plot data as a categorical or continuous variable. 
+        Defaults to remapping the attribute which is suitable for 
+        categorical data. For continuous data set `continuous` to True.
+    cmap : string, optional
+        A string giving the name of a `matplotlib.cm` colormap that will
+        be used to style the features in the GeoDataFrame. Features will
+        be coloured based on the selected attribute. Defaults to the 
+        'viridis' colormap.
+    basemap : ipyleaflet.basemaps object, optional
+        An optional `ipyleaflet.basemaps` object used as the basemap for 
+        the interactive plot. Defaults to `basemaps.Esri.WorldImagery`.
+    default_zoom : int, optional
+        An optional integer giving a default zoom level for the 
+        interactive ipyleaflet plot. Defaults to None, which infers
+        the zoom level from the extent of the data.
+    hover_col : boolean or str, optional
+        If True (the default), the function will print  values from the 
+        GeoDataFrame's `attribute` column above the interactive map when 
+        a user hovers over the features in the map. Alternatively, a 
+        custom shapefile field can be specified by supplying a string
+        giving the name of the field to print. Set to False to prevent 
+        any attributes from being printed.
+    **style_kwargs :
+        Optional keyword arguments to pass to the `style` paramemter of
+        the `ipyleaflet.Choropleth` function. This can be used to 
+        control the appearance of the shapefile, for example 'stroke' 
+        and 'weight' (controlling line width), 'fillOpacity' (polygon 
+        transparency) and 'dashArray' (whether to plot lines/outlines
+        with dashes). For more information:
+        https://ipyleaflet.readthedocs.io/en/latest/api_reference/choropleth.html
+
+    """
+
+    warnings.warn(
+        "The `map_shapefile` function is deprecated, and will "
+        "be removed from future versions of `dea-tools`. Please "
+        "use Geopanda's built-in `.explore` functionality instead.",
+        FutureWarning)
+
+    def on_hover(event, id, properties):
+        with dbg:
+            text = properties.get(hover_col, '???')
+            lbl.value = f'{hover_col}: {text}'
+
+    # Verify that attribute exists in shapefile
+    if attribute not in gdf.columns:
+        raise ValueError(f"The `attribute` {attribute} does not exist "
+                         f"in the geopandas.GeoDataFrame. "
+                         f"Valid attributes include {gdf.columns.values}.")
+
+    # If hover_col is True, use 'attribute' as the default hover attribute.
+    # Otherwise, hover_col will use the supplied attribute field name
+    if hover_col and (hover_col is True):
+        hover_col = attribute
+
+    # If a custom string if supplied to hover_col, check this exists
+    elif hover_col and (type(hover_col) == str):
+        if hover_col not in gdf.columns:
+            raise ValueError(f"The `hover_col` field {hover_col} does "
+                             f"not exist in the geopandas.GeoDataFrame. "
+                             f"Valid attributes include "
+                             f"{gdf.columns.values}.")
+
+    # Convert to WGS 84 and GeoJSON format
+    gdf_wgs84 = gdf.to_crs(epsg=4326)
+    data_geojson = gdf_wgs84.__geo_interface__
+
+    # If continuous is False, remap categorical classes for visualisation
+    if not continuous:
+
+        # Zip classes data together to make a dictionary
+        classes_uni = list(gdf[attribute].unique())
+        classes_clean = list(range(0, len(classes_uni)))
+        classes_dict = dict(zip(classes_uni, classes_clean))
+
+        # Get values to colour by as a list
+        classes = gdf[attribute].map(classes_dict).tolist()
+
+    # If continuous is True then do not remap
+    else:
+
+        # Get values to colour by as a list
+        classes = gdf[attribute].tolist()
+
+    # Create the dictionary to colour map by
+    keys = gdf.index
+    id_class_dict = dict(zip(keys.astype(str), classes))
+
+    # Get centroid to focus map on
+    lon1, lat1, lon2, lat2 = gdf_wgs84.total_bounds
+    lon = (lon1 + lon2) / 2
+    lat = (lat1 + lat2) / 2
+
+    if default_zoom is None:
+
+        # Calculate default zoom from latitude of features
+        default_zoom = _degree_to_zoom_level(lat1, lat2, margin=-0.5)
+
+    # Plot map
+    m = Map(center=(lat, lon),
+            zoom=default_zoom,
+            basemap=basemap,
+            layout=dict(width='800px', height='600px'))
+
+    # Define default plotting parameters for the choropleth map.
+    # The nested dict structure sets default values which can be
+    # overwritten/customised by `choropleth_kwargs` values
+    style_kwargs = dict({'fillOpacity': 0.8}, **style_kwargs)
+
+    # Get `branca.colormap` object from matplotlib string
+    cm_cmap = cm.get_cmap(cmap, 30)
+    colormap = branca.colormap.LinearColormap(
+        [cm_cmap(i) for i in np.linspace(0, 1, 30)])
+
+    # Create the choropleth
+    choropleth = Choropleth(geo_data=data_geojson,
+                            choro_data=id_class_dict,
+                            colormap=colormap,
+                            style=style_kwargs)
+
+    # If the vector data contains line features, they will not be
+    # be coloured by default. To resolve this, we need to manually copy
+    # across the 'fillColor' attribute to the 'color' attribute for each
+    # feature, then plot the data as a GeoJSON layer rather than the
+    # choropleth layer that we use for polygon data.
+    linefeatures = any(x in ['LineString', 'MultiLineString']
+                       for x in gdf.geometry.type.values)
+    if linefeatures:
+
+        # Copy colour from fill to line edge colour
+        for i in keys:
+            choropleth.data['features'][i]['properties']['style']['color'] = \
+            choropleth.data['features'][i]['properties']['style']['fillColor']
+
+        # Add GeoJSON layer to map
+        feature_layer = GeoJSON(data=choropleth.data, style=style_kwargs)
+        m.add_layer(feature_layer)
+
+    else:
+
+        # Add Choropleth layer to map
+        m.add_layer(choropleth)
+
+    # If a column is specified by `hover_col`, print data from the
+    # hovered feature above the map
+    if hover_col and not linefeatures:
+
+        # Use cholopleth object if data is polygon
+        lbl = ipywidgets.Label()
+        dbg = ipywidgets.Output()
+        choropleth.on_hover(on_hover)
+        display(lbl)
+
+    else:
+
+        lbl = ipywidgets.Label()
+        dbg = ipywidgets.Output()
+        feature_layer.on_hover(on_hover)
+        display(lbl)
+
+    # Display the map
+    display(m)
+
+
 def xr_animation(ds,
                  bands=None,
                  output_path='animation.mp4',
                  width_pixels=500,
                  interval=100,
                  percentile_stretch=(0.02, 0.98),
                  image_proc_funcs=None,
@@ -349,15 +563,15 @@
     or use specific combinations of input bands. Vector data can be 
     overlaid and animated on top of imagery, and custom image 
     processing functions can be applied to each frame.
     
     Supports .mp4 (ideal for Twitter/social media) and .gif (ideal 
     for all purposes, but can have large file sizes) format files. 
     
-    Last modified: April 2023
+    Last modified: October 2020
     
     Parameters
     ----------  
     ds : xarray.Dataset
         An xarray dataset with multiple time steps (i.e. multiple 
         observations along the `time` dimension).        
     bands : list of strings
@@ -584,24 +798,14 @@
 
         # Remove axes to show imagery only
         ax.axis('off')
 
         # Update progress bar
         progress_bar.update(1)
 
-    # Add GeoBox and odc.* accessor to array using `odc-geo`
-    try:
-        ds = add_geobox(ds)
-    except ValueError:
-        raise ValueError("Unable to determine `ds`'s coordinate "
-                         "reference system (CRS). Please assign a CRS "
-                         "to the array before passing it to this "
-                         "function, e.g.: "
-                         "`ds.odc.assign_crs(crs='EPSG:3577')`")
-    
     # Test if bands have been supplied, or convert to list to allow
     # iteration if a single band is provided as a string
     if bands is None:
         raise ValueError(f'Please use the `bands` parameter to supply '
                          f'a list of one or three bands that exist as '
                          f'variables in `ds`, e.g. {list(ds.data_vars)}')
     elif isinstance(bands, str):
@@ -638,24 +842,24 @@
     # Update defaults with kwargs
     annotation_defaults.update(annotation_kwargs)
     imshow_defaults.update(imshow_kwargs)
     colorbar_defaults.update(colorbar_kwargs)
     gdf_defaults.update(gdf_kwargs)
 
     # Get info on dataset dimensions
-    height, width = ds.odc.geobox.shape
+    height, width = ds.geobox.shape
     scale = width_pixels / width
-    left, bottom, right, top = ds.odc.geobox.extent.boundingbox
+    left, bottom, right, top = ds.geobox.extent.boundingbox
 
     # Prepare annotations
     annotation_list = _frame_annotation(ds.time, show_date, show_text)
 
     # Prepare geodataframe
     if show_gdf is not None:
-        show_gdf = show_gdf.to_crs(ds.odc.geobox.crs)
+        show_gdf = show_gdf.to_crs(ds.geobox.crs)
         show_gdf = gpd.clip(show_gdf, mask=box(
             left, bottom, right, top)).reindex(show_gdf.index).dropna(how='all')
         show_gdf = _start_end_times(show_gdf, ds)
 
     # Convert data to 4D numpy array of shape [time, y, x, bands]
     ds = ds[bands].to_array().transpose(..., 'variable')[0:limit, ...]
     array = ds.astype(np.float32).values
@@ -802,15 +1006,15 @@
 
     if legend:
         try:
             cb = im.colorbar
         except AttributeError:
             cb = im.cbar
         ticks = cb.get_ticks()
-        cb.set_ticks(ticks[:-1] + np.diff(ticks) / 2)
+        cb.set_ticks(ticks + np.diff(ticks, append=256) / 2)
         cb.set_ticklabels(cblabels)
     return im
 
 
 def plot_fmask(fmask, legend=True, **plot_kwargs):
     """
     Plot an enumerated FMask flag image with human-readable colours.
@@ -853,92 +1057,10 @@
 
     if legend:
         try:
             cb = im.colorbar
         except AttributeError:
             cb = im.cbar
         ticks = cb.get_ticks()
-        cb.set_ticks(ticks[:-1] + np.diff(ticks) / 2)
+        cb.set_ticks(ticks + np.diff(ticks, append=256) / 2)
         cb.set_ticklabels(cblabels)
     return im
-
-
-def plot_variable_images(img_collection):
-    """
-    Plot a dynamic number of images from a xarray dataset that
-    includes Date and Index in the title. Optional ability to
-    also include the sensor in the title if a 'sensor' attribute
-    is added to the dataset using dataset.assign_attrs
-    Parameters
-    ----------
-    img_collection : xr.Dataset
-        A Dataset containing imagery with RBG bands
-    Returns
-    -------
-    plot
-    """
-    # Check that img_collection is a xarray dataset
-    if not isinstance(img_collection, xr.Dataset):
-        raise TypeError("img_collection must be a xarray dataset.")
-
-    # Calculate number of images in `img_collection`
-    plot_count = img_collection.dims["time"]
-    
-    # Check if dataset has 0 images
-    if plot_count == 0:
-        if hasattr(img_collection, "sensor"):
-            raise ValueError("The {} dataset has no images to display for the " 
-            "given query parameters".format(img_collection.sensor))
-        else:
-            raise ValueError("The supplied xarray dataset has no images to "
-            "display for the given query parameters")
-                  
-    # Divide the number of images by 2 rounding up to calculate the
-    # number of rows for the below figure are needed
-    plot_rows = math.ceil(plot_count / 2)
-
-    # Construct a figure to visualise the imagery
-    f, axarr = plt.subplots(plot_rows, 2, figsize=(10, plot_rows * 4.5),
-                            squeeze=False)
-
-    # Flatten the subplots so they can easily be enumerated through
-    axarr = axarr.flatten()
-
-    # Iterate through each image in the dataset and plot
-    # each image as a RGB on a subplot
-    for t in range(plot_count):
-        rgb(
-            img_collection.isel(time=t),
-            bands=["nbart_red", "nbart_green", "nbart_blue"],
-            ax=axarr[t],
-            robust=True,
-        )
-        # Test to see if the dataset has a custom 'sensor' attribute.
-        # If so, include the string in each subplot title.
-        if hasattr(img_collection, "sensor"):
-            title = (
-                str(img_collection.time[t].values)[:10]
-                + "  ||  Index: "
-                + str(t)
-                + "  ||  Sensor: "
-                + img_collection.sensor
-            )
-        else:
-            title = (
-                str(img_collection.time[t].values)[:10]
-                + "  ||  Index: "
-                + str(t)
-            )
-        # Set subplot title, axis label, and shrink offset text
-        axarr[t].set_title(title)
-        axarr[t].set_xlabel("X coordinate")
-        axarr[t].set_ylabel("Y coordinate")
-        axarr[t].yaxis.offsetText.set_fontsize(6)
-        axarr[t].xaxis.offsetText.set_fontsize(6)
-
-    # Adjust padding arround subplots to prevent overlapping elements
-    plt.tight_layout()
-
-    # Remove the last subplot if an odd number of images are being displayed
-    if plot_count % 2 != 0:
-        f.delaxes(axarr[plot_count])
-
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/pyfes_model.py` & `dea-tools-0.2.8.dev9/dea_tools/pyfes_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 
 from os import environ
 from pathlib import Path
 from types import SimpleNamespace
 
 import numpy as np
 
+from pyfes import Handler
+
+
 def initialise_handler():
     """Initialise Aviso FES Handler from INI file.
 
     The path to the INI file must be set in the `FES2014_OCEAN_INI` environment
     variable.
     """
-    from pyfes import Handler
-    
     ini_path = Path(environ.get("FES2014_OCEAN_INI", "."))
     if not ini_path.exists() or not ini_path.is_file():
         raise ValueError("FES2014_OCEAN_INI environment variable must be set")
     short_tide = Handler("ocean", "io", str(ini_path))
     print(f"Initialised FES2014 from {ini_path}")
     return short_tide
 
@@ -43,17 +44,15 @@
     `TimePoint` i.e., tuples of (lon, lat, time).
 
     It returns a list of SimpleNamespaces, each containing the "pure tide" as
     seen by a tide gauge, expressed in meters at the corresponding time.
     This is the sum of the computed height of the diurnal and semi-diurnal
     constituents of the tidal spectrum and of the long period wave constituents
     of the tidal spectrum.
-    """
-    from pyfes import Handler
-    
+    """        
     lons, lats, times = tuple(np.array(timepoints).T)
     # aviso-fes requires naive UTC times in microseconds
     times_us = times.astype("datetime64[us]")
     tide, lp, _ = SHORT_TIDE.calculate(lons, lats, times_us)
 
     # Heights correspond to tide + lp converted from cm to m
     heights = (tide + lp) / 100
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/spatial.py` & `dea-tools-0.2.8.dev9/dea_tools/spatial.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## dea_spatialtools.py
 '''
-Tools for spatially manipulating Digital Earth Australia data.
+Description: This file contains a set of python functions for conducting 
+spatial analyses on Digital Earth Australia data.
 
 License: The code in this notebook is licensed under the Apache License, 
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data 
@@ -12,311 +13,345 @@
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) 
 using the `open-data-cube` tag (you can view previously asked questions 
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube). 
 
 If you would like to report an issue with this script, file one on 
 Github: https://github.com/GeoscienceAustralia/dea-notebooks/issues/new
 
-Last modified: March 2023
+Functions included:
+    xr_vectorize
+    xr_rasterize
+    subpixel_contours
+    interpolate_2d
+    contours_to_array
+    largest_region
+    transform_geojson_wgs_to_epsg
+    zonal_stats_parallel
+    reverse_geocode
+    hillshade
+    sun_angles
+
+Last modified: August 2022
 
 '''
 
 # Import required packages
-import dask
 import fiona
-import warnings
 import collections
-import odc.geo.xr
 import numpy as np
 import xarray as xr
 import geopandas as gpd
 import rasterio.features
 import scipy.interpolate
 import multiprocessing as mp
 from scipy import ndimage as nd
 from skimage.measure import label
 from rasterstats import zonal_stats
 from skimage.measure import find_contours
 from geopy.geocoders import Nominatim
-from geopy.exc import GeocoderUnavailable, GeocoderServiceError
 from datacube.utils.cog import write_cog
 from datacube.utils.geometry import assign_crs
 from datacube.utils.geometry import CRS, Geometry
 from shapely.geometry import LineString, MultiLineString, shape, mapping
 
-
-def points_on_line(gdf, index, distance=30):
-    """
-    Generates evenly-spaced point features along a specific line feature
-    in a `geopandas.GeoDataFrame`.
-    Parameters:
-    -----------
-    gdf : geopandas.GeoDataFrame
-        A `geopandas.GeoDataFrame` containing line features with an
-        index and CRS.
-    index : string or int
-        An value giving the index of the line to generate points along
-    distance : integer or float, optional
-        A number giving the interval at which to generate points along
-        the line feature. Defaults to 30, which will generate a point
-        at every 30 metres along the line.
-    Returns:
-    --------
-    points_gdf : geopandas.GeoDataFrame
-        A `geopandas.GeoDataFrame` containing point features at every
-        `distance` along the selected line.
-    """
-
-    # Select individual line to generate points along
-    line_feature = gdf.loc[[index]].geometry
-
-    # If multiple features are returned, take unary union
-    if line_feature.shape[0] > 0:
-        line_feature = line_feature.unary_union
-    else:
-        line_feature = line_feature.iloc[0]
-
-    # Generate points along line and convert to geopandas.GeoDataFrame
-    points_line = [
-        line_feature.interpolate(i)
-        for i in range(0, int(line_feature.length), distance)
-    ]
-    points_gdf = gpd.GeoDataFrame(geometry=points_line, crs=gdf.crs)
-
-    return points_gdf
-
-
-def add_geobox(ds, crs=None):
-    """
-    Ensure that an xarray DataArray has a GeoBox and .odc.* accessor
-    using `odc.geo`.
-    
-    If `ds` is missing a Coordinate Reference System (CRS), this can be
-    supplied using the `crs` param.
-    
-    Parameters
-    ----------
-    ds : xarray.Dataset or xarray.DataArray
-        Input xarray object that needs to be checked for spatial 
-        information.
-    crs : str, optional
-        Coordinate Reference System (CRS) information for the input `ds` 
-        array. If `ds` already has a CRS, then `crs` is not required. 
-        Default is None.
-        
-    Returns
-    -------
-    xarray.Dataset or xarray.DataArray
-        The input xarray object with added `.odc.x` attributes to access
-        spatial information.
-    
+def xr_vectorize(da, 
+                 attribute_col='attribute', 
+                 transform=None, 
+                 crs=None, 
+                 dtype='float32',
+                 export_shp=False,
+                 verbose=False,
+                 **rasterio_kwargs):    
     """
+    Vectorises a xarray.DataArray into a geopandas.GeoDataFrame.
     
-    # Import the odc-geo package to add `.odc.x` attributes
-    # to our input xarray object
-    import odc.geo.xr
-
-    # If a CRS is not found, use custom provided CRS
-    if ds.odc.crs is None and crs is not None:
-        ds = ds.odc.assign_crs(crs)
-    elif ds.odc.crs is None and crs is None:
-        raise ValueError(
-            "Unable to determine `ds`'s coordinate "
-            "reference system (CRS). Please provide a "
-            "CRS using the `crs` parameter "
-            "(e.g. `crs='EPSG:3577'`)."
-        )
-        
-    return ds
-
-
-def xr_vectorize(
-    da,
-    attribute_col=None,
-    crs=None,
-    dtype="float32",
-    output_path=None,
-    verbose=True,
-    **rasterio_kwargs
-):
-    """
-    Vectorises a raster ``xarray.DataArray`` into a vector
-    ``geopandas.GeoDataFrame``.
-
     Parameters
     ----------
-    da : xarray.DataArray
-        The input ``xarray.DataArray`` data to vectorise.
+    da : xarray dataarray or a numpy ndarray  
     attribute_col : str, optional
-        Name of the attribute column in the resulting
-        ``geopandas.GeoDataFrame``. Values from ``da`` converted
-        to polygons will be assigned to this column. If None, 
-        the column name will default to 'attribute'.
+        Name of the attribute column in the resulting geodataframe. 
+        Values of the raster object converted to polygons will be 
+        assigned to this column. Defaults to 'attribute'.
+    transform : affine.Affine object, optional
+        An affine.Affine object (e.g. `from affine import Affine; 
+        Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "6886890.0) giving the 
+        affine transformation used to convert raster coordinates 
+        (e.g. [0, 0]) to geographic coordinates. If none is provided, 
+        the function will attempt to obtain an affine transformation 
+        from the xarray object (e.g. either at `da.transform` or
+        `da.geobox.transform`).
     crs : str or CRS object, optional
-        If ``da``'s coordinate reference system (CRS) cannot be
-        determined, provide a CRS using this parameter.
-        (e.g. 'EPSG:3577').
+        An EPSG string giving the coordinate system of the array 
+        (e.g. 'EPSG:3577'). If none is provided, the function will 
+        attempt to extract a CRS from the xarray object's `crs` 
+        attribute.
     dtype : str, optional
-         Data type  of  must be one of int16, int32, uint8, uint16,
+         Data type must be one of int16, int32, uint8, uint16, 
          or float32
-    output_path : string, optional
-        Provide an optional string file path to export the vectorised
-        data to file. Supports any vector file formats supported by
-        ``geopandas.GeoDataFrame.to_file()``.
+    export_shp : Boolean or string path, optional
+        To export the output vectorised features to a shapefile, supply
+        an output path (e.g. 'output_dir/output.shp'. The default is 
+        False, which will not write out a shapefile. 
     verbose : bool, optional
-        Print debugging messages. Default True.
-    **rasterio_kwargs :
-        A set of keyword arguments to ``rasterio.features.shapes``.
+        Print debugging messages. Default False.
+    **rasterio_kwargs : 
+        A set of keyword arguments to rasterio.features.shapes
         Can include `mask` and `connectivity`.
-
+    
     Returns
     -------
-    gdf : geopandas.GeoDataFrame
-
-    """
+    gdf : Geopandas GeoDataFrame
     
-    # Add GeoBox and odc.* accessor to array using `odc-geo`
-    da = add_geobox(da, crs)
-
-    # Run the vectorizing function
-    vectors = rasterio.features.shapes(
-        source=da.data.astype(dtype), transform=da.odc.transform, **rasterio_kwargs
-    )
+    """
 
+    
+    # Check for a crs object
+    try:
+        crs = da.crs
+    except:
+        if crs is None:
+            raise Exception("Please add a `crs` attribute to the "
+                            "xarray.DataArray, or provide a CRS using the "
+                            "function's `crs` parameter (e.g. 'EPSG:3577')")
+            
+    # Check if transform is provided as a xarray.DataArray method.
+    # If not, require supplied Affine
+    if transform is None:
+        try:
+            # First, try to take transform info from geobox
+            transform = da.geobox.transform
+        # If no geobox
+        except:
+            try:
+                # Try getting transform from 'transform' attribute
+                transform = da.transform
+            except:
+                # If neither of those options work, raise an exception telling the 
+                # user to provide a transform
+                raise TypeError("Please provide an Affine transform object using the "
+                                "`transform` parameter (e.g. `from affine import "
+                                "Affine; Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "
+                                "6886890.0)`")
+    
+    # Check to see if the input is a numpy array
+    if type(da) is np.ndarray:
+        vectors = rasterio.features.shapes(source=da.astype(dtype),
+                                           transform=transform,
+                                           **rasterio_kwargs)
+    
+    else:
+        # Run the vectorizing function
+        vectors = rasterio.features.shapes(source=da.data.astype(dtype),
+                                           transform=transform,
+                                           **rasterio_kwargs)
+    
     # Convert the generator into a list
     vectors = list(vectors)
-
+    
     # Extract the polygon coordinates and values from the list
     polygons = [polygon for polygon, value in vectors]
     values = [value for polygon, value in vectors]
-
+    
     # Convert polygon coordinates into polygon shapes
     polygons = [shape(polygon) for polygon in polygons]
-
+    
     # Create a geopandas dataframe populated with the polygon shapes
-    attribute_name = attribute_col if attribute_col is not None else 'attribute'
-    gdf = gpd.GeoDataFrame(data={attribute_name: values}, 
-                           geometry=polygons, 
-                           crs=da.odc.crs)
-
-    # If a file path is supplied, export to file
-    if output_path is not None:
-        if verbose: print(f"Exporting vector data to {output_path}")
-        gdf.to_file(output_path)
-
+    gdf = gpd.GeoDataFrame(data={attribute_col: values},
+                           geometry=polygons,
+                           crs=str(crs))
+    
+    # If a file path is supplied, export a shapefile
+    if export_shp:
+        gdf.to_file(export_shp) 
+        
     return gdf
 
 
 def xr_rasterize(gdf,
                  da,
-                 attribute_col=None,
+                 attribute_col=False,
                  crs=None,
+                 transform=None,
                  name=None,
-                 output_path=None,
-                 verbose=True,
+                 x_dim='x',
+                 y_dim='y',
+                 export_tiff=None,
+                 verbose=False,
                  **rasterio_kwargs):    
     """
-    Rasterizes a vector ``geopandas.GeoDataFrame`` into a 
-    raster ``xarray.DataArray``.
-  
+    Rasterizes a geopandas.GeoDataFrame into an xarray.DataArray.
+    
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
-        A ``geopandas.GeoDataFrame`` object containing the vector
+        A geopandas.GeoDataFrame object containing the vector/shapefile
         data you want to rasterise.
     da : xarray.DataArray or xarray.Dataset
         The shape, coordinates, dimensions, and transform of this object 
-        are used to define the array that ``gdf`` is rasterized into. 
-        It effectively provides a spatial template.
+        are used to build the rasterized shapefile. It effectively 
+        provides a template. The attributes of this object are also 
+        appended to the output xarray.DataArray.
     attribute_col : string, optional
-        Name of the attribute column in ``gdf`` containing values for
-        each vector feature that will be rasterized. If None, the 
-        output will be a boolean array of 1's and 0's.
-    crs : str or CRS object, optional
-        If ``da``'s coordinate reference system (CRS) cannot be
-        determined, provide a CRS using this parameter.
-        (e.g. 'EPSG:3577').
-    name : str, optional
-        An optional name used for the output ``xarray.DataArray`.
-    output_path : string, optional
-        Provide an optional string file path to export the rasterized
-        data as a GeoTIFF file.
+        Name of the attribute column in the geodataframe that the pixels 
+        in the raster will contain.  If set to False, output will be a 
+        boolean array of 1's and 0's.
+    crs : str, optional
+        CRS metadata to add to the output xarray. e.g. 'epsg:3577'.
+        The function will attempt get this info from the input 
+        GeoDataFrame first.
+    transform : affine.Affine object, optional
+        An affine.Affine object (e.g. `from affine import Affine; 
+        Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "6886890.0) giving the 
+        affine transformation used to convert raster coordinates 
+        (e.g. [0, 0]) to geographic coordinates. If none is provided, 
+        the function will attempt to obtain an affine transformation 
+        from the xarray object (e.g. either at `da.transform` or
+        `da.geobox.transform`).
+    x_dim : str, optional
+        An optional string allowing you to override the xarray dimension 
+        used for x coordinates. Defaults to 'x'. Useful, for example, 
+        if x and y dims instead called 'lat' and 'lon'.   
+    y_dim : str, optional
+        An optional string allowing you to override the xarray dimension 
+        used for y coordinates. Defaults to 'y'. Useful, for example, 
+        if x and y dims instead called 'lat' and 'lon'.
+    export_tiff: str, optional
+        If a filepath is provided (e.g 'output/output.tif'), will export a
+        geotiff file. A named array is required for this operation, if one
+        is not supplied by the user a default name, 'data', is used
     verbose : bool, optional
-        Print debugging messages. Default True.
+        Print debugging messages. Default False.
     **rasterio_kwargs : 
-        A set of keyword arguments to ``rasterio.features.rasterize``.
+        A set of keyword arguments to rasterio.features.rasterize
         Can include: 'all_touched', 'merge_alg', 'dtype'.
     
     Returns
     -------
-    da_rasterized : xarray.DataArray
-        The rasterized vector data.
+    xarr : xarray.DataArray
+    
     """
     
-    # Add GeoBox and odc.* accessor to array using `odc-geo`
-    da = add_geobox(da, crs)
-
-    # Reproject vector data to raster's CRS
-    gdf_reproj = gdf.to_crs(crs=da.odc.crs)
-
+    # Check for a crs object
+    try:
+        crs = da.geobox.crs
+    except:
+        try:
+            crs = da.crs
+        except:
+            if crs is None:
+                raise ValueError("Please add a `crs` attribute to the "
+                                 "xarray.DataArray, or provide a CRS using the "
+                                 "function's `crs` parameter (e.g. crs='EPSG:3577')")
+    
+    # Check if transform is provided as a xarray.DataArray method.
+    # If not, require supplied Affine
+    if transform is None:
+        try:
+            # First, try to take transform info from geobox
+            transform = da.geobox.transform
+        # If no geobox
+        except:
+            try:
+                # Try getting transform from 'transform' attribute
+                transform = da.transform
+            except:
+                # If neither of those options work, raise an exception telling the 
+                # user to provide a transform
+                raise TypeError("Please provide an Affine transform object using the "
+                                "`transform` parameter (e.g. `from affine import "
+                                "Affine; Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "
+                                "6886890.0)`")
+    
+    # Grab the 2D dims (not time)    
+    try:
+        dims = da.geobox.dims
+    except:
+        dims = y_dim, x_dim  
+    
+    # Coords
+    xy_coords = [da[dims[0]], da[dims[1]]]
+    
+    # Shape
+    try:
+        y, x = da.geobox.shape
+    except:
+        y, x = len(xy_coords[0]), len(xy_coords[1])
+    
+    # Reproject shapefile to match CRS of raster
+    if verbose:
+        print(f'Rasterizing to match xarray.DataArray dimensions ({y}, {x})')
+    
+    try:
+        gdf_reproj = gdf.to_crs(crs=crs)
+    except:
+        # Sometimes the crs can be a datacube utils CRS object
+        # so convert to string before reprojecting
+        gdf_reproj = gdf.to_crs(crs=str(crs))
+    
     # If an attribute column is specified, rasterise using vector 
     # attribute values. Otherwise, rasterise into a boolean array
-    if attribute_col is not None:        
+    if attribute_col:        
         # Use the geometry and attributes from `gdf` to create an iterable
         shapes = zip(gdf_reproj.geometry, gdf_reproj[attribute_col])
     else:
         # Use geometry directly (will produce a boolean numpy array)
         shapes = gdf_reproj.geometry
 
-    # Rasterise shapes into a numpy array
-    im = rasterio.features.rasterize(
-        shapes=shapes,
-        out_shape=da.odc.geobox.shape,
-        transform=da.odc.geobox.transform,
-        **rasterio_kwargs,
-    )
-
-    # Convert numpy array to a full xarray.DataArray
-    # and set array name if supplied
-    da_rasterized = odc.geo.xr.wrap_xr(im=im, 
-                                       gbox=da.odc.geobox)
-    da_rasterized.rename(name)
-    
-    # If a file path is supplied, export to file
-    if output_path is not None:
-        if verbose: print(f"Exporting raster data to {output_path}")
-        write_cog(da_rasterized, output_path, overwrite=True)
+    # Rasterise shapes into an array
+    arr = rasterio.features.rasterize(shapes=shapes,
+                                      out_shape=(y, x),
+                                      transform=transform,
+                                      **rasterio_kwargs)
+        
+    # Convert result to a xarray.DataArray
+    xarr = xr.DataArray(arr,
+                        coords=xy_coords,
+                        dims=dims,
+                        attrs=da.attrs,
+                        name=name if name else None)
+    
+    # Add back crs if xarr.attrs doesn't have it
+    if xarr.geobox is None:
+        xarr = assign_crs(xarr, str(crs))
     
-    return da_rasterized
+    if export_tiff: 
+        if verbose:
+            print(f"Exporting GeoTIFF to {export_tiff}")
+        write_cog(xarr,
+                  export_tiff,
+                  overwrite=True)
+                
+    return xarr
 
 
 def subpixel_contours(da,
                       z_values=[0.0],
                       crs=None,
+                      affine=None,
                       attribute_df=None,
                       output_path=None,
                       min_vertices=2,
                       dim='time',
                       errors='ignore',
-                      verbose=True):
+                      verbose=False):
     
     """
     Uses `skimage.measure.find_contours` to extract multiple z-value 
     contour lines from a two-dimensional array (e.g. multiple elevations
     from a single DEM), or one z-value for each array along a specified 
     dimension of a multi-dimensional array (e.g. to map waterlines 
     across time by extracting a 0 NDWI contour from each individual 
     timestep in an xarray timeseries).    
     
     Contours are returned as a geopandas.GeoDataFrame with one row per 
     z-value or one row per array along a specified dimension. The 
     `attribute_df` parameter can be used to pass custom attributes 
     to the output contour features.
     
-    Last modified: November 2022
+    Last modified: November 2020
     
     Parameters
     ----------  
     da : xarray DataArray
         A two-dimensional or multi-dimensional array from which 
         contours are extracted. If a two-dimensional array is provided, 
         the analysis will run in 'single array, multiple z-values' mode 
@@ -326,17 +361,26 @@
         extract contours for each array along the dimension specified 
         by the `dim` parameter.  
     z_values : int, float or list of ints, floats
         An individual z-value or list of multiple z-values to extract 
         from the array. If operating in 'single z-value, multiple 
         arrays' mode specify only a single z-value.
     crs : string or CRS object, optional
-        If ``da``'s coordinate reference system (CRS) cannot be
-        determined, provide a CRS using this parameter.
-        (e.g. 'EPSG:3577').
+        An EPSG string giving the coordinate system of the array 
+        (e.g. 'EPSG:3577'). If none is provided, the function will 
+        attempt to extract a CRS from the xarray object's `crs` 
+        attribute.
+    affine : affine.Affine object, optional
+        An affine.Affine object (e.g. `from affine import Affine; 
+        Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "6886890.0) giving the 
+        affine transformation used to convert raster coordinates 
+        (e.g. [0, 0]) to geographic coordinates. If none is provided, 
+        the function will attempt to obtain an affine transformation 
+        from the xarray object (e.g. either at `da.transform` or
+        `da.geobox.transform`).
     output_path : string, optional
         The path and filename for the output shapefile.
     attribute_df : pandas.Dataframe, optional
         A pandas.Dataframe containing attributes to pass to the output
         contour features. The dataframe must contain either the same 
         number of rows as supplied `z_values` (in 'multiple z-value, 
         single array' mode), or the same number of rows as the number 
@@ -355,86 +399,94 @@
         dimension.
     errors : string, optional
         If 'raise', then any failed contours will raise an exception.
         If 'ignore' (the default), a list of failed contours will be
         printed. If no contours are returned, an exception will always
         be raised.
     verbose : bool, optional
-        Print debugging messages. Default is True.
+        Print debugging messages. Default False.
         
     Returns
     -------
     output_gdf : geopandas geodataframe
         A geopandas geodataframe object with one feature per z-value 
         ('single array, multiple z-values' mode), or one row per array 
         along the dimension specified by the `dim` parameter ('single 
         z-value, multiple arrays' mode). If `attribute_df` was 
         provided, these values will be included in the shapefile's 
         attribute table.
     """
 
-    def _contours_to_multiline(da_i, z_value, min_vertices=2):
+    def contours_to_multiline(da_i, z_value, min_vertices=2):
         '''
         Helper function to apply marching squares contour extraction
         to an array and return a data as a shapely MultiLineString.
         The `min_vertices` parameter allows you to drop small contours 
         with less than X vertices.
         '''
         
         # Extracts contours from array, and converts each discrete
         # contour into a Shapely LineString feature. If the function 
         # returns a KeyError, this may be due to an unresolved issue in
         # scikit-image: https://github.com/scikit-image/scikit-image/issues/4830
-        try:            
-            line_features = [LineString(i[:,[1, 0]]) 
-                             for i in find_contours(da_i.data, z_value) 
-                             if i.shape[0] > min_vertices]
-        except KeyError:
-            line_features = [LineString(i[:,[1, 0]]) 
-                             for i in find_contours(da_i.data, z_value + 1e-12) 
-                             if i.shape[0] > min_vertices]
+        line_features = [LineString(i[:,[1, 0]]) 
+                         for i in find_contours(da_i.data, z_value) 
+                         if i.shape[0] > min_vertices]        
 
         # Output resulting lines into a single combined MultiLineString
         return MultiLineString(line_features)
 
+    # Check if CRS is provided as a xarray.DataArray attribute.
+    # If not, require supplied CRS
+    try:
+        crs = da.crs
+    except:
+        if crs is None:
+            raise ValueError("Please add a `crs` attribute to the "
+                             "xarray.DataArray, or provide a CRS using the "
+                             "function's `crs` parameter (e.g. 'EPSG:3577')")
 
-    # Add GeoBox and odc.* accessor to array using `odc-geo`
-    da = add_geobox(da, crs)
+    # Check if Affine transform is provided as a xarray.DataArray method.
+    # If not, require supplied Affine
+    try:
+        affine = da.geobox.transform
+    except KeyError:
+        affine = da.transform
+    except:
+        if affine is None:
+            raise TypeError("Please provide an Affine object using the "
+                            "`affine` parameter (e.g. `from affine import "
+                            "Affine; Affine(30.0, 0.0, 548040.0, 0.0, -30.0, "
+                            "6886890.0)`")
 
     # If z_values is supplied is not a list, convert to list:
     z_values = z_values if (isinstance(z_values, list) or 
                             isinstance(z_values, np.ndarray)) else [z_values]
-    
-    # If dask collection, load into memory
-    if dask.is_dask_collection(da):
-        if verbose:
-            print(f'Loading data into memory using Dask')
-        da = da.compute()
 
     # Test number of dimensions in supplied data array
     if len(da.shape) == 2:
         if verbose:
             print(f'Operating in multiple z-value, single array mode')
         dim = 'z_value'
         contour_arrays = {str(i)[0:10]: 
-                          _contours_to_multiline(da, i, min_vertices) 
+                          contours_to_multiline(da, i, min_vertices) 
                           for i in z_values}    
 
     else:
 
         # Test if only a single z-value is given when operating in 
         # single z-value, multiple arrays mode
         if verbose:
             print(f'Operating in single z-value, multiple arrays mode')
         if len(z_values) > 1:
             raise ValueError('Please provide a single z-value when operating '
                              'in single z-value, multiple arrays mode')
 
         contour_arrays = {str(i)[0:10]: 
-                          _contours_to_multiline(da_i, z_values[0], min_vertices) 
+                          contours_to_multiline(da_i, z_values[0], min_vertices) 
                           for i, da_i in da.groupby(dim)}
 
     # If attributes are provided, add the contour keys to that dataframe
     if attribute_df is not None:
 
         try:
             attribute_df.insert(0, dim, contour_arrays.keys())
@@ -451,20 +503,19 @@
     # Otherwise, use the contour keys as the only main attributes
     else:
         attribute_df = list(contour_arrays.keys())
 
     # Convert output contours to a geopandas.GeoDataFrame
     contours_gdf = gpd.GeoDataFrame(data=attribute_df, 
                                     geometry=list(contour_arrays.values()),
-                                    crs=da.odc.crs)   
+                                    crs=crs)   
 
     # Define affine and use to convert array coords to geographic coords.
     # We need to add 0.5 x pixel size to the x and y to obtain the centre 
     # point of our pixels, rather than the top-left corner
-    affine = da.odc.geobox.transform
     shapely_affine = [affine.a, affine.b, affine.d, affine.e, 
                       affine.xoff + affine.a / 2.0, 
                       affine.yoff + affine.e / 2.0]
     contours_gdf['geometry'] = contours_gdf.affine_transform(shapely_affine)
 
     # Rename the data column to match the dimension
     contours_gdf = contours_gdf.rename({0: dim}, axis=1)
@@ -491,15 +542,16 @@
         if verbose:
             print(f'Failed to generate contours: {failed}')
 
     # If asked to write out file, test if geojson or shapefile
     if output_path and output_path.endswith('.geojson'):
         if verbose:
             print(f'Writing contours to {output_path}')
-        contours_gdf.to_crs('EPSG:4326').to_file(filename=output_path)
+        contours_gdf.to_crs('EPSG:4326').to_file(filename=output_path, 
+                                                 driver='GeoJSON')
 
     if output_path and output_path.endswith('.shp'):
         if verbose:
             print(f'Writing contours to {output_path}')
         contours_gdf.to_file(filename=output_path)
         
     return contours_gdf
@@ -857,23 +909,23 @@
     
         'XX.XX S, XX.XX E'   
 
     """
 
     # Run reverse geocode using coordinates
     geocoder = Nominatim(user_agent='Digital Earth Australia')
+    out = geocoder.reverse(coords)
     
     # Create plain text-coords as fall-back
     lat = f'{-coords[0]:.2f} S' if coords[0] < 0 else f'{coords[0]:.2f} N'
     lon = f'{-coords[1]:.2f} W' if coords[1] < 0 else f'{coords[1]:.2f} E'
 
     try:
         
         # Get address from geocoded data
-        out = geocoder.reverse(coords)
         address = out.raw['address']
 
         # Use site and state classes if supplied; else use defaults
         default_site_classes = ['city', 'town', 'village', 'suburb', 'hamlet', 
                                 'county', 'municipality']
         default_state_classes = ['state', 'territory']
         site_classes = site_classes if site_classes else default_site_classes
@@ -892,15 +944,15 @@
         
         else:
             
             # If no geocoding result, return N/E/S/W coordinates
             print('No valid geocoded location; returning coordinates instead')
             return f'{lat}, {lon}'
               
-    except (KeyError, AttributeError, GeocoderUnavailable, GeocoderServiceError):
+    except (KeyError, AttributeError):
 
         # If no geocoding result, return N/E/S/W coordinates
         print('No valid geocoded location; returning coordinates instead')
         return f'{lat}, {lon}'
 
 
 def hillshade(dem, elevation, azimuth, vert_exag=1, dx=30, dy=30):
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/temporal.py` & `dea-tools-0.2.8.dev9/dea_tools/temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 ## dea_temporal.py
 '''
-Conducting temporal (time-domain) analyses on Digital Earth Australia.
+Description: This file contains a set of python functions for conducting
+temporal (time-domain) analyses on Digital Earth Australia.
 
 License: The code in this notebook is licensed under the Apache License,
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth
 Australia data is licensed under the Creative Commons by Attribution 4.0
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data
 Cube Slack channel (http://slack.opendatacube.org/) or on the GIS Stack
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube)
 using the `open-data-cube` tag (you can view previously asked questions
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube).
 
 If you would like to report an issue with this script, file one on
 Github: https://github.com/GeoscienceAustralia/dea-notebooks/issues/new
+
+Functions included:
+    allNaN_arg
+    fast_completion
+    smooth
+    phenology statistics
+    xr_phenology
+    temporal_statistics
+    time_buffer
+    calculate_vector_stat
+    calculate_sad
+    calculate_stsad
     
-Last modified: February 2023
+Last modified: September 2021    
 '''
 
 import sys
 import dask
 import numpy as np
 import xarray as xr
 import pandas as pd
@@ -108,27 +121,27 @@
     # select timesteps before peak of season (AKA greening)
     greenup = da.where(da.time < pos.time)
     # find the first order slopes
     green_deriv = greenup.differentiate("time")
     # find where the first order slope is postive
     pos_green_deriv = green_deriv.where(green_deriv > 0)
     # positive slopes on greening side
-    pos_greenup = greenup.where(~np.isnan(pos_green_deriv))
+    pos_greenup = greenup.where(~xr.ufuncs.isnan(pos_green_deriv))
     # find the median
     median = pos_greenup.median("time")
     # distance of values from median
     distance = pos_greenup - median
 
     if method_sos == "first":
         # find index (argmin) where distance is most negative
         idx = allNaN_arg(distance, "time", "min").astype("int16")
 
     if method_sos == "median":
         # find index (argmin) where distance is smallest absolute value
-        idx = allNaN_arg(np.fabs(distance), "time", "min").astype("int16")
+        idx = allNaN_arg(xr.ufuncs.fabs(distance), "time", "min").astype("int16")
 
     return pos_greenup.isel(time=idx)
 
 
 def _sos(vsos):
     """
     SOS = DOY for start of season
@@ -150,29 +163,29 @@
         side of the curve.
     """
     # select timesteps before peak of season (AKA greening)
     senesce = da.where(da.time > pos.time)
     # find the first order slopes
     senesce_deriv = senesce.differentiate("time")
     # find where the fst order slope is negative
-    neg_senesce_deriv = senesce_deriv.where(~np.isnan(senesce_deriv < 0))
+    neg_senesce_deriv = senesce_deriv.where(~xr.ufuncs.isnan(senesce_deriv < 0))
     # negative slopes on senescing side
     neg_senesce = senesce.where(neg_senesce_deriv)
     # find medians
     median = neg_senesce.median("time")
     # distance to the median
     distance = neg_senesce - median
 
     if method_eos == "last":
         # index where last negative slope occurs
         idx = allNaN_arg(distance, "time", "min").astype("int16")
 
     if method_eos == "median":
         # index where median occurs
-        idx = allNaN_arg(np.fabs(distance), "time", "min").astype("int16")
+        idx = allNaN_arg(xr.ufuncs.fabs(distance), "time", "min").astype("int16")
 
     return neg_senesce.isel(time=idx)
 
 
 def _eos(veos):
     """
     EOS = DOY for end of seasonn
@@ -229,38 +242,38 @@
     verbose=True
 ):
     """
     Obtain land surface phenology metrics from an
     xarray.DataArray containing a timeseries of a
     vegetation index like NDVI.
 
-    Last modified February 2023
+    last modified June 2020
 
     Parameters
     ----------
     da :  xarray.DataArray
         DataArray should contain a 2D or 3D time series of a
         vegetation index like NDVI, EVI
     stats : list
         list of phenological statistics to return. Regardless of
         the metrics returned, all statistics are calculated
         due to inter-dependencies between metrics.
         Options include:
 
-        * ``'SOS'``: DOY of start of season
-        * ``'POS'``: DOY of peak of season
-        * ``'EOS'``: DOY of end of season
-        * ``'vSOS'``: Value at start of season
-        * ``'vPOS'``: Value at peak of season
-        * ``'vEOS'``: Value at end of season
-        * ``'Trough'``: Minimum value of season
-        * ``'LOS'``: Length of season (DOY)
-        * ``'AOS'``: Amplitude of season (in value units)
-        * ``'ROG'``: Rate of greening
-        * ``'ROS'``: Rate of senescence
+        * `SOS` = DOY of start of season
+        * `POS` = DOY of peak of season
+        * `EOS` = DOY of end of season
+        * `vSOS` = Value at start of season
+        * `vPOS` = Value at peak of season
+        * `vEOS` = Value at end of season
+        * `Trough` = Minimum value of season
+        * `LOS` = Length of season (DOY)
+        * `AOS` = Amplitude of season (in value units)
+        * `ROG` = Rate of greening
+        * `ROS` = Rate of senescence
 
     method_sos : str
         If 'first' then vSOS is estimated as the first positive
         slope on the greening side of the curve. If 'median',
         then vSOS is estimated as the median value of the postive
         slopes on the greening side of the curve.
     method_eos : str
@@ -394,36 +407,37 @@
 def temporal_statistics(da, stats):
     """
     Calculate various generic summary statistics on any timeseries.
 
     This function uses the hdstats temporal library:
     https://github.com/daleroberts/hdstats/blob/master/hdstats/ts.pyx
 
-    Last modified June 2020
+    last modified June 2020
 
     Parameters
     ----------
     da :  xarray.DataArray
         DataArray should contain a 3D time series.
     stats : list
-        List of temporal statistics to calculate. Options include:
+        list of temporal statistics to calculate.
+        Options include:
 
-        * ``'discordance'``: TODO
-        * ``'f_std'``: std of discrete fourier transform coefficients, returns 
-        three layers: f_std_n1, f_std_n2, f_std_n3
-        * ``'f_mean'``: mean of discrete fourier transform coefficients, returns 
-        three layers: f_mean_n1, f_mean_n2, f_mean_n3
-        * ``'f_median'``: median of discrete fourier transform coefficients, returns 
-        three layers: f_median_n1, f_median_n2, f_median_n3
-        * ``'mean_change'``: mean of discrete difference along time dimension
-        * ``'median_change'``: median of discrete difference along time dimension
-        * ``'abs_change'``: mean of absolute discrete difference along time dimension
-        * ``'complexity'``: TODO
-        * ``'central_diff'``: TODO
-        * ``'num_peaks'``: The number of peaks in the timeseries, defined with a local
+        * 'discordance' =
+        * 'f_std' = std of discrete fourier transform coefficients, returns
+            three layers: f_std_n1, f_std_n2, f_std_n3
+        * 'f_mean' = mean of discrete fourier transform coefficients, returns
+            three layers: f_mean_n1, f_mean_n2, f_mean_n3
+        * 'f_median' = median of discrete fourier transform coefficients, returns
+            three layers: f_median_n1, f_median_n2, f_median_n3
+        * 'mean_change' = mean of discrete difference along time dimension
+        * 'median_change' = median of discrete difference along time dimension
+        * 'abs_change' = mean of absolute discrete difference along time dimension
+        * 'complexity' =
+        * 'central_diff' =
+        * 'num_peaks' : The number of peaks in the timeseries, defined with a local
             window of size 10.  NOTE: This statistic is very slow
 
     Returns
     -------
     xarray.Dataset
         Dataset containing variables for the selected
         temporal statistics
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools/waterbodies.py` & `dea-tools-0.2.8.dev9/dea_tools/waterbodies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ## dea_waterbodies.py
 """
-Loading and processing DEA Waterbodies data.
+Description: This file contains a set of python functions for loading
+and processing DEA Waterbodies.
 
 License: The code in this notebook is licensed under the Apache License, 
 Version 2.0 (https://www.apache.org/licenses/LICENSE-2.0). Digital Earth 
 Australia data is licensed under the Creative Commons by Attribution 4.0 
 license (https://creativecommons.org/licenses/by/4.0/).
 
 Contact: If you need assistance, please post a question on the Open Data 
@@ -12,14 +13,20 @@
 Exchange (https://gis.stackexchange.com/questions/ask?tags=open-data-cube) 
 using the `open-data-cube` tag (you can view previously asked questions 
 here: https://gis.stackexchange.com/questions/tagged/open-data-cube). 
 
 If you would like to report an issue with this script, file one on 
 Github: https://github.com/GeoscienceAustralia/dea-notebooks/issues/new
 
+Functions included:
+    get_waterbody
+    get_waterbodies
+    get_geohashes
+    get_time_series
+
 Last modified: September 2021
 """
 
 import geopandas as gpd
 from owslib.wfs import WebFeatureService
 from owslib.fes import PropertyIsEqualTo
 from owslib.etree import etree
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools.egg-info/PKG-INFO` & `dea-tools-0.2.8.dev9/dea_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dea-tools
-Version: 0.2.8.dev81
+Version: 0.2.8.dev9
 Summary: Functions and algorithms for analysing Digital Earth Australia data.
 Home-page: https://github.com/GeoscienceAustralia/dea-notebooks
 Author: Geoscience Australia
-Author-email: earth.observation@ga.gov.au
+Author-email: dea@ga.gov.au
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6.0
 Description-Content-Type: text/x-rst
 Provides-Extra: jupyter
-Provides-Extra: dask_gateway
-Provides-Extra: otps
+Provides-Extra: boto
 License-File: LICENSE
 
 
 dea-tools
 =========
 
 Python functions and algorithms developed to assist in analysing Digital Earth Australia (DEA) data (e.g. loading data, plotting, spatial analysis, machine learning). This includes the following modules:
@@ -39,45 +38,31 @@
 
 -  ``dea_tools.spatial``: Spatial analysis tools (e.g. rasterising, vectorising, contour extraction, image processing)
 -  ``dea_tools.temporal``: Temporal analysis tools (e.g. phenology, temporal statistics, multi-dimensional regression)
 
 **Classification and segmentation**
 
 -  ``dea_tools.classification.py``: Machine learning classification (e.g. training and applying machine learning models on satellite data)
--  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segmentation with RSGISLIB)
+-  ``dea_tools.segmentation.py``: Image segmentation tools (e.g. applying image segementation with RSGISLIB)
 
 **Parallel processing**
 
 -  ``dea_tools.dask``: Parallel processing with Dask (e.g. creating Dask clusters for scalable analysis)
 
 **Domain-specific analysis**
 
 -  ``dea_tools.land_cover``: Functions for plotting Digital Earth Australia Land Cover data.
 -  ``dea_tools.coastal``: Coastal and intertidal analysis tools (e.g. tidal tagging, coastal change timeseries)
--  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. gauge data, discharge data)
+-  ``dea_tools.bom``: Loading Bureau of Meteorology water data service data (e.g. guage data, discharge data)
 -  ``dea_tools.climate``: Retrieving and manipulating gridded climate data (e.g. ERA5)
 -  ``dea_tools.waterbodies``: Loading and processing DEA Waterbodies data (e.g. finding and loading waterbody timeseries data)
 
 Installation
 ------------
 
-With conda
-~~~~~~~~~~
-
-.. code-block:: bash
-
-    wget -O conda-environment.yml https://raw.githubusercontent.com/opendatacube/datacube-core/develop/conda-environment.yml
-
-    mamba env create -f conda-environment.yml
-    conda activate cubeenv
-
-
-Install dea-tools
-~~~~~~~~~~~~~~~~~
-
 Install the package from the source on any system with ``pip``:
 
 .. code-block:: bash
 
     pip install dea-tools
 
 To work with this module on the DEA Sandbox or National Computational Infrastructure environments without installing it, you can add the ``Tools`` directory to the system path from within the ``dea-notebooks`` repository:
@@ -125,7 +110,8 @@
 
 .. code-block:: bash
 
         cd Tools
         rm dea_tools/__version__.py  # if necessary
         pip install . --use-feature=in-tree-build
         python -m build
+
```

### Comparing `dea-tools-0.2.8.dev81/dea_tools.egg-info/SOURCES.txt` & `dea-tools-0.2.8.dev9/dea_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 MANIFEST.in
 README.rst
 index.rst
 pyproject.toml
 setup.py
 dea_tools/__init__.py
 dea_tools/__main__.py
+dea_tools/__version__.py
 dea_tools/bandindices.py
 dea_tools/bom.py
 dea_tools/classification.py
 dea_tools/climate.py
 dea_tools/coastal.py
 dea_tools/dask.py
 dea_tools/datahandling.py
 dea_tools/landcover.py
 dea_tools/plotting.py
 dea_tools/pyfes_model.py
+dea_tools/segmentation.py
 dea_tools/spatial.py
 dea_tools/temporal.py
-dea_tools/validation.py
 dea_tools/waterbodies.py
 dea_tools.egg-info/PKG-INFO
 dea_tools.egg-info/SOURCES.txt
 dea_tools.egg-info/dependency_links.txt
 dea_tools.egg-info/requires.txt
 dea_tools.egg-info/top_level.txt
 dea_tools/app/__init__.py
```

### Comparing `dea-tools-0.2.8.dev81/index.rst` & `dea-tools-0.2.8.dev9/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
    dea_tools.datahandling
    dea_tools.bandindices
    dea_tools.bom
    dea_tools.classification
    dea_tools.climate
    dea_tools.coastal
    dea_tools.dask
+   dea_tools.datahandling
    dea_tools.landcover
    dea_tools.plotting
    dea_tools.spatial
    dea_tools.temporal
    dea_tools.waterbodies
-   dea_tools.validation
    
 Apps and widgets
 -----------------
 
 ``dea_tools`` interactive app sub-packages can be accessed through ``dea_tools.app``.
 
 .. autosummary::
```

### Comparing `dea-tools-0.2.8.dev81/setup.py` & `dea-tools-0.2.8.dev9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,67 +12,60 @@
 from setuptools import find_packages, setup, Command
 import setuptools_scm
 
 # Package meta-data.
 NAME = 'dea-tools'
 DESCRIPTION = 'Functions and algorithms for analysing Digital Earth Australia data.'
 URL = 'https://github.com/GeoscienceAustralia/dea-notebooks'
-EMAIL = 'earth.observation@ga.gov.au'
+EMAIL = 'dea@ga.gov.au'
 AUTHOR = 'Geoscience Australia'
 REQUIRES_PYTHON = '>=3.6.0'
 
 # Where are we?
 IS_SANDBOX = os.getenv('JUPYTER_IMAGE', default='').startswith('geoscienceaustralia/sandbox')
 IS_NCI = 'dea-env' in os.getenv('LOADEDMODULES_modshare', default='')
 IS_DEA = IS_NCI or IS_SANDBOX
 
 # What packages are required for this module to be executed?
 # These are all on the Sandbox/NCI so shouldn't need installing on those platforms.
 REQUIRED = [
-    'aiohttp',
-    'boto3', 
-    'botocore',
-    'branca',
     'ciso8601',
-    'dask-ml',
-    'datacube',
-    'Fiona',
-    'folium',
-    'geopandas',
-    'geopy',
-    'hdstats',
-    'joblib',
+    'pytz',
+    'requests',
     'lxml',
-    'matplotlib',
     'numpy',
-    'odc-ui',
-    'OWSLib',
-    'packaging',
-    'pandas',
-    'pyproj',
-    'python_dateutil',
-    'pyTMD<2.0.0',    
-    'pytz',
+    'xarray',
+    'geopandas',
+    'datacube',
+    'tqdm',
+    'dask',
     'rasterio',
-    'rasterstats',
-    'requests',
-    'scikit-image',
     'scikit-learn',
+    'rasterstats',
+    'geopy',
+    'pandas',
     'scipy',
-    'setuptools',
-    'Shapely',
-    'tqdm',
-    'xarray',
+    # 'otps',  # Hard to install, but available on Sandbox and NCI
+    'GDAL',
+    'odc-ui',
+    'numexpr',
+    'matplotlib',
+    'folium',
+    'pyproj',
+    'branca',
+    'shapely',
+    'scikit-image',
+    'python-dateutil',
+    'OWSLib',
 ]
 
 # What packages are optional?
 EXTRAS = {
-    'jupyter': ['ipython', 'ipywidgets', 'ipyleaflet'],
-    'dask_gateway': ['dask_gateway'],
-    'otps': ['otps'],  # tidal model, hard to install; available on Sandbox/NCI
+    'jupyter': ['IPython', 'ipywidgets', 'ipyleaflet'],
+    'boto': ['boto3'],
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
@@ -119,34 +112,51 @@
 
         self.status('Pushing git tags…')
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
+
+# Versioning magic.
+VERSION_FILE_PATH = Path('dea_tools/__version__.py')
+about = {}
+try:
+    version = setuptools_scm.get_version(
+        root='..',
+        write_to='Tools' / VERSION_FILE_PATH,
+        relative_to=__file__,
+        local_scheme=lambda _: '')
+except (LookupError, FileNotFoundError):
+    # python -m build will trip the FNFError
+    try:
+        # no .git folder, so read from __version__.py
+        with open(VERSION_FILE_PATH) as f_version:
+            exec(f_version.read(), about)
+            version = about['version']
+    except FileNotFoundError:
+        # No __version__.py, yikes
+        raise RuntimeError('Build in-place with --use-feature=in-tree-build.')
+
 # Where the magic happens:
 setup(
     name=NAME,
+    version=version,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
-    use_scm_version = {
-        "root": '..',
-        "relative_to": __file__,
-        "local_scheme": "no-local-version",
-        },
     install_requires=REQUIRED if not IS_DEA else [],
     extras_require=EXTRAS if not IS_DEA else {k: [] for k in EXTRAS},
     include_package_data=True,
     license='Apache License 2.0',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

