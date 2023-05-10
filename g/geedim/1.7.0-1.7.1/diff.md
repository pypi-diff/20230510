# Comparing `tmp/geedim-1.7.0.tar.gz` & `tmp/geedim-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geedim-1.7.0.tar", last modified: Sun Dec 11 15:30:16 2022, max compression
+gzip compressed data, was "geedim-1.7.1.tar", last modified: Wed May 10 13:45:37 2023, max compression
```

## Comparing `geedim-1.7.0.tar` & `geedim-1.7.1.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 15:30:16.684987 geedim-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-11 15:30:03.000000 geedim-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2022-12-11 15:30:16.684987 geedim-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2022-12-11 15:30:03.000000 geedim-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 15:30:16.680987 geedim-1.7.0/geedim/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36911 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    29111 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 15:30:16.684987 geedim-1.7.0/geedim/data/
--rw-r--r--   0 runner    (1001) docker     (123)   115185 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/data/ee_stac_urls.json
--rw-r--r--   0 runner    (1001) docker     (123)    45333 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23458 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/medoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13148 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-11 15:30:03.000000 geedim-1.7.0/geedim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-11 15:30:16.684987 geedim-1.7.0/geedim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-11 15:30:16.000000 geedim-1.7.0/geedim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-11 15:30:03.000000 geedim-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-11 15:30:16.684987 geedim-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2022-12-11 15:30:03.000000 geedim-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 13:45:21.000000 geedim-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-10 13:45:37.539969 geedim-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-10 13:45:21.000000 geedim-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.535969 geedim-1.7.1/geedim/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37237 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/geedim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   119884 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/data/ee_stac_urls.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 13:45:21.000000 geedim-1.7.1/geedim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.535969 geedim-1.7.1/geedim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 13:45:37.000000 geedim-1.7.1/geedim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 13:45:21.000000 geedim-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:45:37.539969 geedim-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-10 13:45:21.000000 geedim-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:45:37.539969 geedim-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26863 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29767 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 13:45:21.000000 geedim-1.7.1/tests/test_utils.py
```

### Comparing `geedim-1.7.0/LICENSE` & `geedim-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/PKG-INFO` & `geedim-1.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: geedim
-Version: 1.7.0
+Version: 1.7.1
 Summary: Search, composite and download Google Earth Engine imagery.
-Home-page: https://github.com/dugalh/geedim
+Home-page: https://github.com/leftfield-geospatial/geedim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://geedim.readthedocs.io
-Project-URL: Source, https://github.com/dugalh/geedim
+Project-URL: Source, https://github.com/leftfield-geospatial/geedim
 Keywords: earth engine,satellite imagery,search,download,composite,cloud,shadow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -275,18 +275,18 @@
    terms of the `MIT license <https://github.com/cordmaur/GEES2Downloader/blob/main/LICENSE>`__.
 -  Medoid compositing was adapted from `gee_tools <https://github.com/gee-community/gee_tools>`__ under the terms of the
    `MIT license <https://github.com/gee-community/gee_tools/blob/master/LICENSE>`__.
 -  Sentinel-2 cloud/shadow masking was adapted from `ee_extra <https://github.com/r-earthengine/ee_extra>`__ under
    terms of the `Apache-2.0 license <https://github.com/r-earthengine/ee_extra/blob/master/LICENSE>`__
 
 
-.. |Tests| image:: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
-   :target: https://codecov.io/gh/dugalh/geedim
+.. |Tests| image:: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
+   :target: https://codecov.io/gh/leftfield-geospatial/geedim
 .. |PyPI version| image:: https://img.shields.io/pypi/v/geedim.svg
    :target: https://pypi.org/project/geedim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/geedim.svg
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/geedim
 .. |docs| image:: https://readthedocs.org/projects/geedim/badge/?version=latest
    :target: https://geedim.readthedocs.io/en/latest/?badge=latest
```

### Comparing `geedim-1.7.0/README.rst` & `geedim-1.7.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -257,18 +257,18 @@
    terms of the `MIT license <https://github.com/cordmaur/GEES2Downloader/blob/main/LICENSE>`__.
 -  Medoid compositing was adapted from `gee_tools <https://github.com/gee-community/gee_tools>`__ under the terms of the
    `MIT license <https://github.com/gee-community/gee_tools/blob/master/LICENSE>`__.
 -  Sentinel-2 cloud/shadow masking was adapted from `ee_extra <https://github.com/r-earthengine/ee_extra>`__ under
    terms of the `Apache-2.0 license <https://github.com/r-earthengine/ee_extra/blob/master/LICENSE>`__
 
 
-.. |Tests| image:: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
-   :target: https://codecov.io/gh/dugalh/geedim
+.. |Tests| image:: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
+   :target: https://codecov.io/gh/leftfield-geospatial/geedim
 .. |PyPI version| image:: https://img.shields.io/pypi/v/geedim.svg
    :target: https://pypi.org/project/geedim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/geedim.svg
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/geedim
 .. |docs| image:: https://readthedocs.org/projects/geedim/badge/?version=latest
    :target: https://geedim.readthedocs.io/en/latest/?badge=latest
```

### Comparing `geedim-1.7.0/geedim/__init__.py` & `geedim-1.7.1/geedim/__init__.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/cli.py` & `geedim-1.7.1/geedim/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,14 +518,18 @@
 @bbox_option
 @region_option
 @scale_option
 @crs_transform_option
 @shape_option
 @like_option
 @dtype_option
+@click.option(
+    '-bn', '--band-name', 'bands', type=click.STRING, multiple=True, default=None, show_default='all bands',
+    help='Band name(s) to download.'
+)
 @mask_option
 @resampling_option
 @scale_offset_option
 @click.option(
     '-dd', '--download-dir', type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True), default=None,
     show_default='current working directory.', help='Directory to download image file(s) into.'
 )
@@ -624,14 +628,18 @@
 @bbox_option
 @region_option
 @scale_option
 @crs_transform_option
 @shape_option
 @like_option
 @dtype_option
+@click.option(
+    '-bn', '--band-name', 'bands', type=click.STRING, multiple=True, default=None, show_default='all bands',
+    help='Band name(s) to download.'
+)
 @mask_option
 @resampling_option
 @scale_offset_option
 @click.option(
     '-w/-nw', '--wait/--no-wait', default=True, show_default=True, help='Whether to wait for the export to complete.'
 )
 @click.pass_obj
```

### Comparing `geedim-1.7.0/geedim/collection.py` & `geedim-1.7.1/geedim/collection.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/data/ee_stac_urls.json` & `geedim-1.7.1/geedim/data/ee_stac_urls.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9087982832618026%*

 * *Differences: {"'ACA/reef_habitat/v2_0'": "'https://storage.googleapis.com/earthengine-stac/catalog/ACA/ACA_reef_habitat_v2_0.json'",*

 * * "'COPERNICUS/DEM/GLO30'": "'https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_DEM_GLO30.json'",*

 * * "'ECMWF/ERA5_LAND/DAILY_RAW'": "'https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_DAILY_RAW.json'",*

 * * "'ECMWF/ERA5_LAND/MONTHLY_AGGR'": "'https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY_AGGR.json'",*

 * *  […]*

```diff
@@ -1,10 +1,11 @@
 {
     "AAFC/ACI": "https://storage.googleapis.com/earthengine-stac/catalog/AAFC/AAFC_ACI.json",
     "ACA/reef_habitat/v1_0": "https://storage.googleapis.com/earthengine-stac/catalog/ACA/ACA_reef_habitat_v1_0.json",
+    "ACA/reef_habitat/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/ACA/ACA_reef_habitat_v2_0.json",
     "AHN/AHN2_05M_INT": "https://storage.googleapis.com/earthengine-stac/catalog/AHN/AHN_AHN2_05M_INT.json",
     "AHN/AHN2_05M_NON": "https://storage.googleapis.com/earthengine-stac/catalog/AHN/AHN_AHN2_05M_NON.json",
     "AHN/AHN2_05M_RUW": "https://storage.googleapis.com/earthengine-stac/catalog/AHN/AHN_AHN2_05M_RUW.json",
     "ASTER/AST_L1T_003": "https://storage.googleapis.com/earthengine-stac/catalog/ASTER/ASTER_AST_L1T_003.json",
     "AU/GA/AUSTRALIA_5M_DEM": "https://storage.googleapis.com/earthengine-stac/catalog/AU/AU_GA_AUSTRALIA_5M_DEM.json",
     "AU/GA/DEM_1SEC/v10/DEM-H": "https://storage.googleapis.com/earthengine-stac/catalog/AU/AU_GA_DEM_1SEC_v10_DEM-H.json",
     "AU/GA/DEM_1SEC/v10/DEM-S": "https://storage.googleapis.com/earthengine-stac/catalog/AU/AU_GA_DEM_1SEC_v10_DEM-S.json",
@@ -27,14 +28,15 @@
     "CIESIN/GPWv411/GPW_Population_Density": "https://storage.googleapis.com/earthengine-stac/catalog/CIESIN/CIESIN_GPWv411_GPW_Population_Density.json",
     "CIESIN/GPWv411/GPW_UNWPP-Adjusted_Population_Count": "https://storage.googleapis.com/earthengine-stac/catalog/CIESIN/CIESIN_GPWv411_GPW_UNWPP-Adjusted_Population_Count.json",
     "CIESIN/GPWv411/GPW_UNWPP-Adjusted_Population_Density": "https://storage.googleapis.com/earthengine-stac/catalog/CIESIN/CIESIN_GPWv411_GPW_UNWPP-Adjusted_Population_Density.json",
     "CIESIN/GPWv411/GPW_Water_Area": "https://storage.googleapis.com/earthengine-stac/catalog/CIESIN/CIESIN_GPWv411_GPW_Water_Area.json",
     "CIESIN/GPWv411/GPW_Water_Mask": "https://storage.googleapis.com/earthengine-stac/catalog/CIESIN/CIESIN_GPWv411_GPW_Water_Mask.json",
     "COPERNICUS/CORINE/V18_5_1/100m": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_CORINE_V18_5_1_100m.json",
     "COPERNICUS/CORINE/V20/100m": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_CORINE_V20_100m.json",
+    "COPERNICUS/DEM/GLO30": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_DEM_GLO30.json",
     "COPERNICUS/Landcover/100m/Proba-V-C3/Global": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_Landcover_100m_Proba-V-C3_Global.json",
     "COPERNICUS/Landcover/100m/Proba-V/Global": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_Landcover_100m_Proba-V_Global.json",
     "COPERNICUS/S1_GRD": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S1_GRD.json",
     "COPERNICUS/S2": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S2.json",
     "COPERNICUS/S2_CLOUD_PROBABILITY": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S2_CLOUD_PROBABILITY.json",
     "COPERNICUS/S2_HARMONIZED": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S2_HARMONIZED.json",
     "COPERNICUS/S2_SR": "https://storage.googleapis.com/earthengine-stac/catalog/COPERNICUS/COPERNICUS_S2_SR.json",
@@ -77,16 +79,18 @@
     "CSP/ERGo/1_0/US/topoDiversity": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_ERGo_1_0_US_topoDiversity.json",
     "CSP/HM/GlobalHumanModification": "https://storage.googleapis.com/earthengine-stac/catalog/CSP/CSP_HM_GlobalHumanModification.json",
     "DLR/WSF/WSF2015/v1": "https://storage.googleapis.com/earthengine-stac/catalog/DLR/DLR_WSF_WSF2015_v1.json",
     "DOE/ORNL/LandScan_HD/Ukraine_202201": "https://storage.googleapis.com/earthengine-stac/catalog/DOE/DOE_ORNL_LandScan_HD_Ukraine_202201.json",
     "ECMWF/CAMS/NRT": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_CAMS_NRT.json",
     "ECMWF/ERA5/DAILY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_DAILY.json",
     "ECMWF/ERA5/MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_MONTHLY.json",
+    "ECMWF/ERA5_LAND/DAILY_RAW": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_DAILY_RAW.json",
     "ECMWF/ERA5_LAND/HOURLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_HOURLY.json",
     "ECMWF/ERA5_LAND/MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY.json",
+    "ECMWF/ERA5_LAND/MONTHLY_AGGR": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY_AGGR.json",
     "ECMWF/ERA5_LAND/MONTHLY_BY_HOUR": "https://storage.googleapis.com/earthengine-stac/catalog/ECMWF/ECMWF_ERA5_LAND_MONTHLY_BY_HOUR.json",
     "EO1/HYPERION": "https://storage.googleapis.com/earthengine-stac/catalog/EO1/EO1_HYPERION.json",
     "ESA/CCI/FireCCI/5_1": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_CCI_FireCCI_5_1.json",
     "ESA/GLOBCOVER_L4_200901_200912_V2_3": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_GLOBCOVER_L4_200901_200912_V2_3.json",
     "ESA/WorldCover/v100": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_WorldCover_v100.json",
     "ESA/WorldCover/v200": "https://storage.googleapis.com/earthengine-stac/catalog/ESA/ESA_WorldCover_v200.json",
     "FAO/GHG/1/DROSA_A": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_GHG_1_DROSA_A.json",
@@ -98,21 +102,25 @@
     "FAO/WAPOR/2/L1_I_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_I_D.json",
     "FAO/WAPOR/2/L1_NPP_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_NPP_D.json",
     "FAO/WAPOR/2/L1_RET_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_RET_D.json",
     "FAO/WAPOR/2/L1_RET_E": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_RET_E.json",
     "FAO/WAPOR/2/L1_T_D": "https://storage.googleapis.com/earthengine-stac/catalog/FAO/FAO_WAPOR_2_L1_T_D.json",
     "FIRMS": "https://storage.googleapis.com/earthengine-stac/catalog/FIRMS/FIRMS.json",
     "FORMA/FORMA_500m": "https://storage.googleapis.com/earthengine-stac/catalog/FORMA/FORMA_FORMA_500m.json",
+    "Finland/MAVI/VV/50cm": "https://storage.googleapis.com/earthengine-stac/catalog/Finland/Finland_MAVI_VV_50cm.json",
+    "Finland/SMK/V/50cm": "https://storage.googleapis.com/earthengine-stac/catalog/Finland/Finland_SMK_V_50cm.json",
+    "Finland/SMK/VV/50cm": "https://storage.googleapis.com/earthengine-stac/catalog/Finland/Finland_SMK_VV_50cm.json",
     "GFW/GFF/V1/fishing_hours": "https://storage.googleapis.com/earthengine-stac/catalog/GFW/GFW_GFF_V1_fishing_hours.json",
     "GFW/GFF/V1/vessel_hours": "https://storage.googleapis.com/earthengine-stac/catalog/GFW/GFW_GFF_V1_vessel_hours.json",
     "GLCF/GLS_TCC": "https://storage.googleapis.com/earthengine-stac/catalog/GLCF/GLCF_GLS_TCC.json",
     "GLCF/GLS_WATER": "https://storage.googleapis.com/earthengine-stac/catalog/GLCF/GLCF_GLS_WATER.json",
     "GLOBAL_FLOOD_DB/MODIS_EVENTS/V1": "https://storage.googleapis.com/earthengine-stac/catalog/GLOBAL_FLOOD_DB/GLOBAL_FLOOD_DB_MODIS_EVENTS_V1.json",
     "GOOGLE/DYNAMICWORLD/V1": "https://storage.googleapis.com/earthengine-stac/catalog/GOOGLE/GOOGLE_DYNAMICWORLD_V1.json",
     "GRIDMET/DROUGHT": "https://storage.googleapis.com/earthengine-stac/catalog/GRIDMET/GRIDMET_DROUGHT.json",
+    "Germany/Brandenburg/orthos/20cm": "https://storage.googleapis.com/earthengine-stac/catalog/Germany/Germany_Brandenburg_orthos_20cm.json",
     "HYCOM/GLBu0_08/sea_surface_elevation": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_GLBu0_08_sea_surface_elevation.json",
     "HYCOM/GLBu0_08/sea_temp_salinity": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_GLBu0_08_sea_temp_salinity.json",
     "HYCOM/GLBu0_08/sea_water_velocity": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_GLBu0_08_sea_water_velocity.json",
     "HYCOM/sea_surface_elevation": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_sea_surface_elevation.json",
     "HYCOM/sea_temp_salinity": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_sea_temp_salinity.json",
     "HYCOM/sea_water_velocity": "https://storage.googleapis.com/earthengine-stac/catalog/HYCOM/HYCOM_sea_water_velocity.json",
     "IDAHO_EPSCOR/GRIDMET": "https://storage.googleapis.com/earthengine-stac/catalog/IDAHO_EPSCOR/IDAHO_EPSCOR_GRIDMET.json",
@@ -527,14 +535,15 @@
     "LANDSAT/LT5_L1T_ANNUAL_NDWI": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_ANNUAL_NDWI.json",
     "LANDSAT/LT5_L1T_ANNUAL_RAW": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_ANNUAL_RAW.json",
     "LANDSAT/LT5_L1T_ANNUAL_TOA": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_ANNUAL_TOA.json",
     "LANDSAT/LT5_L1T_TOA": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_LT5_L1T_TOA.json",
     "LANDSAT/MANGROVE_FORESTS": "https://storage.googleapis.com/earthengine-stac/catalog/LANDSAT/LANDSAT_MANGROVE_FORESTS.json",
     "LARSE/GEDI/GEDI02_A_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI02_A_002_MONTHLY.json",
     "LARSE/GEDI/GEDI02_B_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI02_B_002_MONTHLY.json",
+    "LARSE/GEDI/GEDI04_A_002_MONTHLY": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI04_A_002_MONTHLY.json",
     "LARSE/GEDI/GEDI04_B_002": "https://storage.googleapis.com/earthengine-stac/catalog/LARSE/LARSE_GEDI_GEDI04_B_002.json",
     "MERIT/DEM/v1_0_3": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_DEM_v1_0_3.json",
     "MERIT/Hydro/v1_0_1": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_Hydro_v1_0_1.json",
     "MERIT/Hydro_reduced/v1_0_1": "https://storage.googleapis.com/earthengine-stac/catalog/MERIT/MERIT_Hydro_reduced_v1_0_1.json",
     "MODIS/006/MCD12Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD12Q1.json",
     "MODIS/006/MCD12Q2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD12Q2.json",
     "MODIS/006/MCD15A3H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MCD15A3H.json",
@@ -581,43 +590,63 @@
     "MODIS/006/MYD14A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD14A2.json",
     "MODIS/006/MYD15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD15A2H.json",
     "MODIS/006/MYD17A2H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD17A2H.json",
     "MODIS/006/MYD17A3H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD17A3H.json",
     "MODIS/006/MYD17A3HGF": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYD17A3HGF.json",
     "MODIS/006/MYDOCGA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_006_MYDOCGA.json",
     "MODIS/055/MOD17A3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_055_MOD17A3.json",
+    "MODIS/061/MCD12Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD12Q1.json",
+    "MODIS/061/MCD12Q2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD12Q2.json",
     "MODIS/061/MCD15A3H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD15A3H.json",
+    "MODIS/061/MCD18C2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD18C2.json",
     "MODIS/061/MCD43A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A1.json",
+    "MODIS/061/MCD43A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A2.json",
+    "MODIS/061/MCD43A3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A3.json",
+    "MODIS/061/MCD43A4": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43A4.json",
+    "MODIS/061/MCD43C3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD43C3.json",
     "MODIS/061/MCD64A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MCD64A1.json",
     "MODIS/061/MOD08_M3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD08_M3.json",
     "MODIS/061/MOD09A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09A1.json",
+    "MODIS/061/MOD09CMG": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09CMG.json",
     "MODIS/061/MOD09GA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09GA.json",
     "MODIS/061/MOD09GQ": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09GQ.json",
     "MODIS/061/MOD09Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD09Q1.json",
     "MODIS/061/MOD11A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD11A1.json",
     "MODIS/061/MOD11A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD11A2.json",
     "MODIS/061/MOD13A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13A1.json",
     "MODIS/061/MOD13A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13A2.json",
     "MODIS/061/MOD13Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD13Q1.json",
     "MODIS/061/MOD14A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD14A1.json",
     "MODIS/061/MOD14A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD14A2.json",
     "MODIS/061/MOD15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD15A2H.json",
+    "MODIS/061/MOD17A3HGF": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD17A3HGF.json",
+    "MODIS/061/MOD21A1D": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21A1D.json",
+    "MODIS/061/MOD21A1N": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21A1N.json",
+    "MODIS/061/MOD21C1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C1.json",
+    "MODIS/061/MOD21C2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C2.json",
+    "MODIS/061/MOD21C3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MOD21C3.json",
     "MODIS/061/MYD08_M3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD08_M3.json",
     "MODIS/061/MYD09A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09A1.json",
     "MODIS/061/MYD09GA": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09GA.json",
     "MODIS/061/MYD09GQ": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09GQ.json",
     "MODIS/061/MYD09Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD09Q1.json",
     "MODIS/061/MYD11A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD11A1.json",
     "MODIS/061/MYD11A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD11A2.json",
     "MODIS/061/MYD13A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13A1.json",
     "MODIS/061/MYD13A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13A2.json",
     "MODIS/061/MYD13Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD13Q1.json",
     "MODIS/061/MYD14A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD14A1.json",
     "MODIS/061/MYD14A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD14A2.json",
     "MODIS/061/MYD15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD15A2H.json",
+    "MODIS/061/MYD17A3HGF": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD17A3HGF.json",
+    "MODIS/061/MYD21A1D": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD21A1D.json",
+    "MODIS/061/MYD21A1N": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD21A1N.json",
+    "MODIS/061/MYD21C1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD21C1.json",
+    "MODIS/061/MYD21C2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD21C2.json",
+    "MODIS/061/MYD21C3": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_061_MYD21C3.json",
     "MODIS/MCD43A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A1.json",
     "MODIS/MCD43A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A2.json",
     "MODIS/MCD43A4": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A4.json",
     "MODIS/MCD43A4_006_BAI": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A4_006_BAI.json",
     "MODIS/MCD43A4_006_EVI": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A4_006_EVI.json",
     "MODIS/MCD43A4_006_NDSI": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A4_006_NDSI.json",
     "MODIS/MCD43A4_006_NDVI": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MCD43A4_006_NDVI.json",
@@ -663,107 +692,119 @@
     "MODIS/MYD09Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD09Q1.json",
     "MODIS/MYD10A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD10A1.json",
     "MODIS/MYD11A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD11A1.json",
     "MODIS/MYD11A2": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD11A2.json",
     "MODIS/MYD13A1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD13A1.json",
     "MODIS/MYD13Q1": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_MYD13Q1.json",
     "MODIS/NTSG/MOD16A2/105": "https://storage.googleapis.com/earthengine-stac/catalog/MODIS/MODIS_NTSG_MOD16A2_105.json",
-    "NASA/ASTER_GED/AG100_003": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/ASTER_GED/NASA_ASTER_GED_AG100_003.json",
-    "NASA/FLDAS/NOAH01/C/GL/M/V001": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/FLDAS/NASA_FLDAS_NOAH01_C_GL_M_V001.json",
-    "NASA/GEOS-CF/v1/rpl/htf": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GEOS-CF/NASA_GEOS-CF_v1_rpl_htf.json",
-    "NASA/GEOS-CF/v1/rpl/tavg1hr": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GEOS-CF/NASA_GEOS-CF_v1_rpl_tavg1hr.json",
-    "NASA/GIMMS/3GV0": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GIMMS/NASA_GIMMS_3GV0.json",
-    "NASA/GLDAS/V021/NOAH/G025/T3H": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GLDAS/NASA_GLDAS_V021_NOAH_G025_T3H.json",
-    "NASA/GLDAS/V022/CLSM/G025/DA1D": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GLDAS/NASA_GLDAS_V022_CLSM_G025_DA1D.json",
-    "NASA/GLDAS/V20/NOAH/G025/T3H": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GLDAS/NASA_GLDAS_V20_NOAH_G025_T3H.json",
-    "NASA/GPM_L3/IMERG_MONTHLY_V06": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GPM_L3/NASA_GPM_L3_IMERG_MONTHLY_V06.json",
-    "NASA/GPM_L3/IMERG_V06": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GPM_L3/NASA_GPM_L3_IMERG_V06.json",
-    "NASA/GRACE/MASS_GRIDS/LAND": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GRACE/NASA_GRACE_MASS_GRIDS_LAND.json",
-    "NASA/GRACE/MASS_GRIDS/MASCON": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GRACE/NASA_GRACE_MASS_GRIDS_MASCON.json",
-    "NASA/GRACE/MASS_GRIDS/MASCON_CRI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GRACE/NASA_GRACE_MASS_GRIDS_MASCON_CRI.json",
-    "NASA/GRACE/MASS_GRIDS/OCEAN": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GRACE/NASA_GRACE_MASS_GRIDS_OCEAN.json",
-    "NASA/GRACE/MASS_GRIDS/OCEAN_EOFR": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GRACE/NASA_GRACE_MASS_GRIDS_OCEAN_EOFR.json",
-    "NASA/GSFC/MERRA/aer/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GSFC/NASA_GSFC_MERRA_aer_2.json",
-    "NASA/GSFC/MERRA/flx/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GSFC/NASA_GSFC_MERRA_flx_2.json",
-    "NASA/GSFC/MERRA/lnd/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GSFC/NASA_GSFC_MERRA_lnd_2.json",
-    "NASA/GSFC/MERRA/rad/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GSFC/NASA_GSFC_MERRA_rad_2.json",
-    "NASA/GSFC/MERRA/slv/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/GSFC/NASA_GSFC_MERRA_slv_2.json",
-    "NASA/JPL/global_forest_canopy_height_2005": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/JPL/NASA_JPL_global_forest_canopy_height_2005.json",
-    "NASA/MEASURES/GFCC/TC/v3": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/MEASURES/NASA_MEASURES_GFCC_TC_v3.json",
-    "NASA/NASADEM_HGT/001": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASADEM_HGT/NASA_NASADEM_HGT_001.json",
+    "NASA/ASTER_GED/AG100_003": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_ASTER_GED_AG100_003.json",
+    "NASA/FLDAS/NOAH01/C/GL/M/V001": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_FLDAS_NOAH01_C_GL_M_V001.json",
+    "NASA/GDDP-CMIP6": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GDDP-CMIP6.json",
+    "NASA/GEOS-CF/v1/fcst/htf": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GEOS-CF_v1_fcst_htf.json",
+    "NASA/GEOS-CF/v1/rpl/htf": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GEOS-CF_v1_rpl_htf.json",
+    "NASA/GEOS-CF/v1/rpl/tavg1hr": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GEOS-CF_v1_rpl_tavg1hr.json",
+    "NASA/GIMMS/3GV0": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GIMMS_3GV0.json",
+    "NASA/GLDAS/V021/NOAH/G025/T3H": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GLDAS_V021_NOAH_G025_T3H.json",
+    "NASA/GLDAS/V022/CLSM/G025/DA1D": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GLDAS_V022_CLSM_G025_DA1D.json",
+    "NASA/GLDAS/V20/NOAH/G025/T3H": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GLDAS_V20_NOAH_G025_T3H.json",
+    "NASA/GPM_L3/IMERG_MONTHLY_V06": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GPM_L3_IMERG_MONTHLY_V06.json",
+    "NASA/GPM_L3/IMERG_V06": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GPM_L3_IMERG_V06.json",
+    "NASA/GRACE/MASS_GRIDS/LAND": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GRACE_MASS_GRIDS_LAND.json",
+    "NASA/GRACE/MASS_GRIDS/MASCON": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GRACE_MASS_GRIDS_MASCON.json",
+    "NASA/GRACE/MASS_GRIDS/MASCON_CRI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GRACE_MASS_GRIDS_MASCON_CRI.json",
+    "NASA/GRACE/MASS_GRIDS/OCEAN": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GRACE_MASS_GRIDS_OCEAN.json",
+    "NASA/GRACE/MASS_GRIDS/OCEAN_EOFR": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GRACE_MASS_GRIDS_OCEAN_EOFR.json",
+    "NASA/GSFC/MERRA/aer/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GSFC_MERRA_aer_2.json",
+    "NASA/GSFC/MERRA/flx/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GSFC_MERRA_flx_2.json",
+    "NASA/GSFC/MERRA/lnd/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GSFC_MERRA_lnd_2.json",
+    "NASA/GSFC/MERRA/rad/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GSFC_MERRA_rad_2.json",
+    "NASA/GSFC/MERRA/slv/2": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_GSFC_MERRA_slv_2.json",
+    "NASA/JPL/global_forest_canopy_height_2005": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_JPL_global_forest_canopy_height_2005.json",
+    "NASA/MEASURES/GFCC/TC/v3": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_MEASURES_GFCC_TC_v3.json",
+    "NASA/NASADEM_HGT/001": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_NASADEM_HGT_001.json",
     "NASA/NEX-DCP30": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_NEX-DCP30.json",
     "NASA/NEX-DCP30_ENSEMBLE_STATS": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_NEX-DCP30_ENSEMBLE_STATS.json",
     "NASA/NEX-GDDP": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_NEX-GDDP.json",
-    "NASA/NLDAS/FORA0125_H002": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NLDAS/NASA_NLDAS_FORA0125_H002.json",
-    "NASA/OCEANDATA/MODIS-Aqua/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/OCEANDATA/NASA_OCEANDATA_MODIS-Aqua_L3SMI.json",
-    "NASA/OCEANDATA/MODIS-Terra/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/OCEANDATA/NASA_OCEANDATA_MODIS-Terra_L3SMI.json",
-    "NASA/OCEANDATA/SeaWiFS/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/OCEANDATA/NASA_OCEANDATA_SeaWiFS_L3SMI.json",
-    "NASA/ORNL/DAYMET_V3": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/ORNL/NASA_ORNL_DAYMET_V3.json",
-    "NASA/ORNL/DAYMET_V4": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/ORNL/NASA_ORNL_DAYMET_V4.json",
-    "NASA/ORNL/biomass_carbon_density/v1": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/ORNL/NASA_ORNL_biomass_carbon_density_v1.json",
+    "NASA/NLDAS/FORA0125_H002": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_NLDAS_FORA0125_H002.json",
+    "NASA/OCEANDATA/MODIS-Aqua/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_OCEANDATA_MODIS-Aqua_L3SMI.json",
+    "NASA/OCEANDATA/MODIS-Terra/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_OCEANDATA_MODIS-Terra_L3SMI.json",
+    "NASA/OCEANDATA/SeaWiFS/L3SMI": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_OCEANDATA_SeaWiFS_L3SMI.json",
+    "NASA/ORNL/DAYMET_V3": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_ORNL_DAYMET_V3.json",
+    "NASA/ORNL/DAYMET_V4": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_ORNL_DAYMET_V4.json",
+    "NASA/ORNL/biomass_carbon_density/v1": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_ORNL_biomass_carbon_density_v1.json",
+    "NASA/SMAP/SPL3SMP_E/005": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_SMAP_SPL3SMP_E_005.json",
+    "NASA/SMAP/SPL4SMGP/007": "https://storage.googleapis.com/earthengine-stac/catalog/NASA/NASA_SMAP_SPL4SMGP_007.json",
     "NASA_USDA/HSL/SMAP10KM_soil_moisture": "https://storage.googleapis.com/earthengine-stac/catalog/NASA_USDA/NASA_USDA_HSL_SMAP10KM_soil_moisture.json",
     "NASA_USDA/HSL/SMAP_soil_moisture": "https://storage.googleapis.com/earthengine-stac/catalog/NASA_USDA/NASA_USDA_HSL_SMAP_soil_moisture.json",
     "NASA_USDA/HSL/soil_moisture": "https://storage.googleapis.com/earthengine-stac/catalog/NASA_USDA/NASA_USDA_HSL_soil_moisture.json",
     "NCEP_RE/sea_level_pressure": "https://storage.googleapis.com/earthengine-stac/catalog/NCEP_RE/NCEP_RE_sea_level_pressure.json",
     "NCEP_RE/surface_temp": "https://storage.googleapis.com/earthengine-stac/catalog/NCEP_RE/NCEP_RE_surface_temp.json",
     "NCEP_RE/surface_wv": "https://storage.googleapis.com/earthengine-stac/catalog/NCEP_RE/NCEP_RE_surface_wv.json",
-    "NOAA/CDR/ATMOS_NEAR_SURFACE/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_ATMOS_NEAR_SURFACE_V2.json",
-    "NOAA/CDR/AVHRR/AOT/V3": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_AOT_V3.json",
-    "NOAA/CDR/AVHRR/LAI_FAPAR/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_LAI_FAPAR_V4.json",
-    "NOAA/CDR/AVHRR/LAI_FAPAR/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_LAI_FAPAR_V5.json",
-    "NOAA/CDR/AVHRR/NDVI/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_NDVI_V4.json",
-    "NOAA/CDR/AVHRR/NDVI/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_NDVI_V5.json",
-    "NOAA/CDR/AVHRR/SR/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_SR_V4.json",
-    "NOAA/CDR/AVHRR/SR/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_AVHRR_SR_V5.json",
-    "NOAA/CDR/GRIDSAT-B1/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_GRIDSAT-B1_V2.json",
-    "NOAA/CDR/HEAT_FLUXES/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_HEAT_FLUXES_V2.json",
-    "NOAA/CDR/OISST/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_OISST_V2.json",
-    "NOAA/CDR/OISST/V2_1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_OISST_V2_1.json",
-    "NOAA/CDR/PATMOSX/V53": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_PATMOSX_V53.json",
-    "NOAA/CDR/SST_PATHFINDER/V53": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_SST_PATHFINDER_V53.json",
-    "NOAA/CDR/SST_WHOI/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CDR/NOAA_CDR_SST_WHOI_V2.json",
+    "NOAA/CDR/ATMOS_NEAR_SURFACE/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_ATMOS_NEAR_SURFACE_V2.json",
+    "NOAA/CDR/AVHRR/AOT/V3": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_AOT_V3.json",
+    "NOAA/CDR/AVHRR/LAI_FAPAR/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_LAI_FAPAR_V4.json",
+    "NOAA/CDR/AVHRR/LAI_FAPAR/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_LAI_FAPAR_V5.json",
+    "NOAA/CDR/AVHRR/NDVI/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_NDVI_V4.json",
+    "NOAA/CDR/AVHRR/NDVI/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_NDVI_V5.json",
+    "NOAA/CDR/AVHRR/SR/V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_SR_V4.json",
+    "NOAA/CDR/AVHRR/SR/V5": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_AVHRR_SR_V5.json",
+    "NOAA/CDR/GRIDSAT-B1/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_GRIDSAT-B1_V2.json",
+    "NOAA/CDR/HEAT_FLUXES/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_HEAT_FLUXES_V2.json",
+    "NOAA/CDR/OISST/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_OISST_V2.json",
+    "NOAA/CDR/OISST/V2_1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_OISST_V2_1.json",
+    "NOAA/CDR/PATMOSX/V53": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_PATMOSX_V53.json",
+    "NOAA/CDR/SST_PATHFINDER/V53": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_SST_PATHFINDER_V53.json",
+    "NOAA/CDR/SST_WHOI/V2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CDR_SST_WHOI_V2.json",
     "NOAA/CFSR": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CFSR.json",
-    "NOAA/CFSV2/FOR6H": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/CFSV2/NOAA_CFSV2_FOR6H.json",
-    "NOAA/DMSP-OLS/CALIBRATED_LIGHTS_V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/DMSP-OLS/NOAA_DMSP-OLS_CALIBRATED_LIGHTS_V4.json",
-    "NOAA/DMSP-OLS/NIGHTTIME_LIGHTS": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/DMSP-OLS/NOAA_DMSP-OLS_NIGHTTIME_LIGHTS.json",
+    "NOAA/CFSV2/FOR6H": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_CFSV2_FOR6H.json",
+    "NOAA/DMSP-OLS/CALIBRATED_LIGHTS_V4": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_DMSP-OLS_CALIBRATED_LIGHTS_V4.json",
+    "NOAA/DMSP-OLS/NIGHTTIME_LIGHTS": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_DMSP-OLS_NIGHTTIME_LIGHTS.json",
     "NOAA/GFS0P25": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GFS0P25.json",
-    "NOAA/GOES/16/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_16_FDCC.json",
-    "NOAA/GOES/16/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_16_FDCF.json",
-    "NOAA/GOES/16/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_16_MCMIPC.json",
-    "NOAA/GOES/16/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_16_MCMIPF.json",
-    "NOAA/GOES/16/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_16_MCMIPM.json",
-    "NOAA/GOES/17/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_17_FDCC.json",
-    "NOAA/GOES/17/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_17_FDCF.json",
-    "NOAA/GOES/17/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_17_MCMIPC.json",
-    "NOAA/GOES/17/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_17_MCMIPF.json",
-    "NOAA/GOES/17/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_17_MCMIPM.json",
-    "NOAA/GOES/18/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_18_FDCC.json",
-    "NOAA/GOES/18/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_18_FDCF.json",
-    "NOAA/GOES/18/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_18_MCMIPC.json",
-    "NOAA/GOES/18/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_18_MCMIPF.json",
-    "NOAA/GOES/18/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/GOES/NOAA_GOES_18_MCMIPM.json",
-    "NOAA/NCEP_DOE_RE2/total_cloud_coverage": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NCEP_DOE_RE2/NOAA_NCEP_DOE_RE2_total_cloud_coverage.json",
-    "NOAA/NGDC/ETOPO1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NGDC/NOAA_NGDC_ETOPO1.json",
-    "NOAA/NWS/RTMA": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NWS/NOAA_NWS_RTMA.json",
+    "NOAA/GOES/16/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_16_FDCC.json",
+    "NOAA/GOES/16/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_16_FDCF.json",
+    "NOAA/GOES/16/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_16_MCMIPC.json",
+    "NOAA/GOES/16/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_16_MCMIPF.json",
+    "NOAA/GOES/16/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_16_MCMIPM.json",
+    "NOAA/GOES/17/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_17_FDCC.json",
+    "NOAA/GOES/17/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_17_FDCF.json",
+    "NOAA/GOES/17/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_17_MCMIPC.json",
+    "NOAA/GOES/17/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_17_MCMIPF.json",
+    "NOAA/GOES/17/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_17_MCMIPM.json",
+    "NOAA/GOES/18/FDCC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_18_FDCC.json",
+    "NOAA/GOES/18/FDCF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_18_FDCF.json",
+    "NOAA/GOES/18/MCMIPC": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_18_MCMIPC.json",
+    "NOAA/GOES/18/MCMIPF": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_18_MCMIPF.json",
+    "NOAA/GOES/18/MCMIPM": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_GOES_18_MCMIPM.json",
+    "NOAA/NCEP_DOE_RE2/total_cloud_coverage": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_NCEP_DOE_RE2_total_cloud_coverage.json",
+    "NOAA/NGDC/ETOPO1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_NGDC_ETOPO1.json",
+    "NOAA/NWS/RTMA": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_NWS_RTMA.json",
     "NOAA/PERSIANN-CDR": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_PERSIANN-CDR.json",
-    "NOAA/VIIRS/001/VNP09GA": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/VIIRS/NOAA_VIIRS_001_VNP09GA.json",
-    "NOAA/VIIRS/001/VNP13A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/VIIRS/NOAA_VIIRS_001_VNP13A1.json",
-    "NOAA/VIIRS/001/VNP22Q2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/VIIRS/NOAA_VIIRS_001_VNP22Q2.json",
-    "NOAA/VIIRS/DNB/MONTHLY_V1/VCMCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/VIIRS/NOAA_VIIRS_DNB_MONTHLY_V1_VCMCFG.json",
-    "NOAA/VIIRS/DNB/MONTHLY_V1/VCMSLCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/VIIRS/NOAA_VIIRS_DNB_MONTHLY_V1_VCMSLCFG.json",
+    "NOAA/VIIRS/001/VNP09GA": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP09GA.json",
+    "NOAA/VIIRS/001/VNP09H1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP09H1.json",
+    "NOAA/VIIRS/001/VNP13A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP13A1.json",
+    "NOAA/VIIRS/001/VNP14A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP14A1.json",
+    "NOAA/VIIRS/001/VNP15A2H": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP15A2H.json",
+    "NOAA/VIIRS/001/VNP21A1D": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP21A1D.json",
+    "NOAA/VIIRS/001/VNP21A1N": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP21A1N.json",
+    "NOAA/VIIRS/001/VNP22Q2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP22Q2.json",
+    "NOAA/VIIRS/001/VNP46A2": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP46A2.json",
+    "NOAA/VIIRS/001/VNP64A1": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_001_VNP64A1.json",
+    "NOAA/VIIRS/DNB/MONTHLY_V1/VCMCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_DNB_MONTHLY_V1_VCMCFG.json",
+    "NOAA/VIIRS/DNB/MONTHLY_V1/VCMSLCFG": "https://storage.googleapis.com/earthengine-stac/catalog/NOAA/NOAA_VIIRS_DNB_MONTHLY_V1_VCMSLCFG.json",
     "NRCan/CDEM": "https://storage.googleapis.com/earthengine-stac/catalog/NRCan/NRCan_CDEM.json",
     "OREGONSTATE/PRISM/AN81d": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_AN81d.json",
     "OREGONSTATE/PRISM/AN81m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_AN81m.json",
     "OREGONSTATE/PRISM/Norm81m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_Norm81m.json",
     "OREGONSTATE/PRISM/Norm91m": "https://storage.googleapis.com/earthengine-stac/catalog/OREGONSTATE/OREGONSTATE_PRISM_Norm91m.json",
     "ORTHO/Switzerland/SWISSIMAGE/10cm": "https://storage.googleapis.com/earthengine-stac/catalog/ORTHO/ORTHO_Switzerland_SWISSIMAGE_10cm.json",
     "OSU/GIMP/2000_ICE_OCEAN_MASK": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_2000_ICE_OCEAN_MASK.json",
     "OSU/GIMP/2000_IMAGERY_MOSAIC": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_2000_IMAGERY_MOSAIC.json",
     "OSU/GIMP/DEM": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_DEM.json",
     "OSU/GIMP/ICE_VELOCITY_OPT": "https://storage.googleapis.com/earthengine-stac/catalog/OSU/OSU_GIMP_ICE_VELOCITY_OPT.json",
+    "OpenET/ENSEMBLE/CONUS/GRIDMET/MONTHLY/v2_0": "https://storage.googleapis.com/earthengine-stac/catalog/OpenET/OpenET_ENSEMBLE_CONUS_GRIDMET_MONTHLY_v2_0.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAYNIGHT_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAYNIGHT_M_v01.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAY_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAY_M_v01.json",
     "OpenLandMap/CLM/CLM_LST_MOD11A2-DAY_SD/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_LST_MOD11A2-DAY_SD_v01.json",
     "OpenLandMap/CLM/CLM_PRECIPITATION_SM2RAIN_M/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_CLM_CLM_PRECIPITATION_SM2RAIN_M_v01.json",
     "OpenLandMap/PNV/PNV_BIOME-TYPE_BIOME00K_C/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_PNV_PNV_BIOME-TYPE_BIOME00K_C_v01.json",
     "OpenLandMap/PNV/PNV_FAPAR_PROBA-V_D/v01": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_PNV_PNV_FAPAR_PROBA-V_D_v01.json",
     "OpenLandMap/SOL/SOL_BULKDENS-FINEEARTH_USDA-4A1H_M/v02": "https://storage.googleapis.com/earthengine-stac/catalog/OpenLandMap/OpenLandMap_SOL_SOL_BULKDENS-FINEEARTH_USDA-4A1H_M_v02.json",
@@ -785,14 +826,15 @@
     "Oxford/MAP/accessibility_to_healthcare_2019": "https://storage.googleapis.com/earthengine-stac/catalog/Oxford/Oxford_MAP_accessibility_to_healthcare_2019.json",
     "Oxford/MAP/friction_surface_2015_v1_0": "https://storage.googleapis.com/earthengine-stac/catalog/Oxford/Oxford_MAP_friction_surface_2015_v1_0.json",
     "Oxford/MAP/friction_surface_2019": "https://storage.googleapis.com/earthengine-stac/catalog/Oxford/Oxford_MAP_friction_surface_2019.json",
     "RUB/RUBCLIM/LCZ/global_lcz_map/v1": "https://storage.googleapis.com/earthengine-stac/catalog/RUB/RUB_RUBCLIM_LCZ_global_lcz_map_v1.json",
     "SKYSAT/GEN-A/PUBLIC/ORTHO/MULTISPECTRAL": "https://storage.googleapis.com/earthengine-stac/catalog/SKYSAT/SKYSAT_GEN-A_PUBLIC_ORTHO_MULTISPECTRAL.json",
     "SKYSAT/GEN-A/PUBLIC/ORTHO/RGB": "https://storage.googleapis.com/earthengine-stac/catalog/SKYSAT/SKYSAT_GEN-A_PUBLIC_ORTHO_RGB.json",
     "SNU/ESL/BESS/Rad/v1": "https://storage.googleapis.com/earthengine-stac/catalog/SNU/SNU_ESL_BESS_Rad_v1.json",
+    "Spain/PNOA/PNOA10": "https://storage.googleapis.com/earthengine-stac/catalog/Spain/Spain_PNOA_PNOA10.json",
     "TERN/AET/CMRSET_LANDSAT_V2_1": "https://storage.googleapis.com/earthengine-stac/catalog/TERN/TERN_AET_CMRSET_LANDSAT_V2_1.json",
     "TERN/AET/CMRSET_LANDSAT_V2_2": "https://storage.googleapis.com/earthengine-stac/catalog/TERN/TERN_AET_CMRSET_LANDSAT_V2_2.json",
     "TOMS/MERGED": "https://storage.googleapis.com/earthengine-stac/catalog/TOMS/TOMS_MERGED.json",
     "TRMM/3B42": "https://storage.googleapis.com/earthengine-stac/catalog/TRMM/TRMM_3B42.json",
     "TRMM/3B43V7": "https://storage.googleapis.com/earthengine-stac/catalog/TRMM/TRMM_3B43V7.json",
     "TUBerlin/BigEarthNet/v1": "https://storage.googleapis.com/earthengine-stac/catalog/TUBerlin/TUBerlin_BigEarthNet_v1.json",
     "Tsinghua/DESS/ChinaTerraceMap/v1": "https://storage.googleapis.com/earthengine-stac/catalog/Tsinghua/Tsinghua_DESS_ChinaTerraceMap_v1.json",
@@ -827,31 +869,32 @@
     "UQ/murray/Intertidal/v1_1/qa_pixel_count": "https://storage.googleapis.com/earthengine-stac/catalog/UQ/UQ_murray_Intertidal_v1_1_qa_pixel_count.json",
     "USDA/NAIP/DOQQ": "https://storage.googleapis.com/earthengine-stac/catalog/USDA/USDA_NAIP_DOQQ.json",
     "USDA/NASS/CDL": "https://storage.googleapis.com/earthengine-stac/catalog/USDA/USDA_NASS_CDL.json",
     "USFS/GTAC/LCMS/v2020-5": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2020-5.json",
     "USFS/GTAC/LCMS/v2020-6": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2020-6.json",
     "USFS/GTAC/LCMS/v2021-7": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_LCMS_v2021-7.json",
     "USFS/GTAC/MTBS/annual_burn_severity_mosaics/v1": "https://storage.googleapis.com/earthengine-stac/catalog/USFS/USFS_GTAC_MTBS_annual_burn_severity_mosaics_v1.json",
-    "USGS/3DEP/10m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/3DEP/USGS_3DEP_10m.json",
-    "USGS/3DEP/1m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/3DEP/USGS_3DEP_1m.json",
-    "USGS/GAP/AK/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GAP/USGS_GAP_AK_2001.json",
-    "USGS/GAP/CONUS/2011": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GAP/USGS_GAP_CONUS_2011.json",
-    "USGS/GAP/HI/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GAP/USGS_GAP_HI_2001.json",
-    "USGS/GAP/PR/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GAP/USGS_GAP_PR_2001.json",
-    "USGS/GFSAD1000_V0": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GFSAD1000/USGS_GFSAD1000_V0.json",
-    "USGS/GFSAD1000_V1": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/GFSAD1000/USGS_GFSAD1000_V1.json",
+    "USGS/3DEP/10m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_3DEP_10m.json",
+    "USGS/3DEP/1m": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_3DEP_1m.json",
+    "USGS/GAP/AK/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_AK_2001.json",
+    "USGS/GAP/CONUS/2011": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_CONUS_2011.json",
+    "USGS/GAP/HI/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_HI_2001.json",
+    "USGS/GAP/PR/2001": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GAP_PR_2001.json",
+    "USGS/GFSAD1000_V0": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GFSAD1000_V0.json",
+    "USGS/GFSAD1000_V1": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GFSAD1000_V1.json",
     "USGS/GMTED2010": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GMTED2010.json",
     "USGS/GTOPO30": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_GTOPO30.json",
-    "USGS/LIMA/MOSAIC": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/LIMA/USGS_LIMA_MOSAIC.json",
-    "USGS/LIMA/SR": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/LIMA/USGS_LIMA_SR.json",
+    "USGS/LIMA/MOSAIC": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_LIMA_MOSAIC.json",
+    "USGS/LIMA/SR": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_LIMA_SR.json",
     "USGS/NED": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NED.json",
     "USGS/NLCD": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NLCD.json",
-    "USGS/NLCD_RELEASES/2016_REL": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/NLCD_RELEASES/USGS_NLCD_RELEASES_2016_REL.json",
-    "USGS/NLCD_RELEASES/2019_REL/NLCD": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/NLCD_RELEASES/USGS_NLCD_RELEASES_2019_REL_NLCD.json",
-    "USGS/NLCD_RELEASES/2019_REL/RCMAP/V4/COVER": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/NLCD_RELEASES/USGS_NLCD_RELEASES_2019_REL_RCMAP_V4_COVER.json",
+    "USGS/NLCD_RELEASES/2016_REL": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NLCD_RELEASES_2016_REL.json",
+    "USGS/NLCD_RELEASES/2019_REL/NLCD": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NLCD_RELEASES_2019_REL_NLCD.json",
+    "USGS/NLCD_RELEASES/2019_REL/RCMAP/V4/COVER": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NLCD_RELEASES_2019_REL_RCMAP_V4_COVER.json",
+    "USGS/NLCD_RELEASES/2019_REL/RCMAP/V5/COVER": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_NLCD_RELEASES_2019_REL_RCMAP_V5_COVER.json",
     "USGS/SRTMGL1_003": "https://storage.googleapis.com/earthengine-stac/catalog/USGS/USGS_SRTMGL1_003.json",
     "UTOKYO/WTLAB/KBDI/v1": "https://storage.googleapis.com/earthengine-stac/catalog/UTOKYO/UTOKYO_WTLAB_KBDI_v1.json",
     "VITO/PROBAV/C1/S1_TOC_100M": "https://storage.googleapis.com/earthengine-stac/catalog/VITO/VITO_PROBAV_C1_S1_TOC_100M.json",
     "VITO/PROBAV/C1/S1_TOC_333M": "https://storage.googleapis.com/earthengine-stac/catalog/VITO/VITO_PROBAV_C1_S1_TOC_333M.json",
     "VITO/PROBAV/S1_TOC_100M": "https://storage.googleapis.com/earthengine-stac/catalog/VITO/VITO_PROBAV_S1_TOC_100M.json",
     "VITO/PROBAV/S1_TOC_333M": "https://storage.googleapis.com/earthengine-stac/catalog/VITO/VITO_PROBAV_S1_TOC_333M.json",
     "WCMC/biomass_carbon_density/v1_0": "https://storage.googleapis.com/earthengine-stac/catalog/WCMC/WCMC_biomass_carbon_density_v1_0.json",
```

### Comparing `geedim-1.7.0/geedim/download.py` & `geedim-1.7.1/geedim/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         adj_im = adj_im.select(ee_image.bandNames())  # keep bands in original order
         # copy original ee_image properties and return
         return ee.Image(adj_im.copyProperties(ee_image, ee_image.propertyNames()))
 
     def _prepare_for_export(
         self, crs: str = None, crs_transform: Tuple[float] = None, shape: Tuple[int, int] = None, region: Dict =
         None, scale: float = None, resampling: ResamplingMethod = _default_resampling, dtype: str = None,
-        scale_offset: bool = False
+        scale_offset: bool = False, bands: List[str] = None,
     ) -> 'BaseImage':
         """
         Prepare the encapsulated image for export/download.  Will reproject, resample, clip and convert the image
         according to the provided parameters.
 
         Export bounds and resolution can be specified with ``region`` and ``scale`` / ``shape``, or ``crs_transform``
         and ``shape``.  If no bounds are specified (with either ``region``, or ``crs_transform`` & ``shape``), the
@@ -461,71 +461,82 @@
             # the default scale is in degrees.
             raise ValueError(f'This image is in EPSG:4326, you need to specify a scale (in meters); or a shape.')
 
         if scale and shape:
             # This error is raised in later calls to ee.Image.getInfo(), but is neater to raise here first
             raise ValueError('You can specify one of scale or shape, but not both.')
 
+        if bands:
+            band_diff = set(bands).difference([band_prop['name'] for band_prop in self.band_properties])
+            if len(band_diff) > 0:
+                # If one or more specified bands don't exist, raise an error
+                raise ValueError(f'The band(s) {list(band_diff)} don\'t exist.')
+
+        # Create a new BaseImage of band subset is specified.  This is done here so that crs, scale etc
+        # parameters used below will have the values specific to bands.
+        exp_image = BaseImage(self.ee_image.select(bands)) if bands else self
+
         # perform image scale/offset, dtype and resampling operations
-        ee_image = self.ee_image
+        ee_image = exp_image.ee_image
         if scale_offset:
-            ee_image = self._scale_offset(ee_image, self.band_properties)
+            ee_image = BaseImage._scale_offset(ee_image, exp_image.band_properties)
             im_dtype = 'float64'
         else:
-            im_dtype = self.dtype
+            im_dtype = exp_image.dtype
 
         resampling = ResamplingMethod(resampling)
-        if resampling != self._default_resampling:
-            if not self.has_fixed_projection:
+        if resampling != BaseImage._default_resampling:
+            if not exp_image.has_fixed_projection:
                 raise ValueError(
                     'This image has no fixed projection and cannot be resampled.  If this image is a composite, '
-                    'you can resample the compimages used to create the composite.'
+                    'you can resample the component images used to create the composite.'
                 )
             ee_image = utils.resample(ee_image, resampling)
         # TODO: only do this if there is a change?  Or do we need to standardise the bands?
-        ee_image = self._convert_dtype(ee_image, dtype=dtype or im_dtype)
+        ee_image = BaseImage._convert_dtype(ee_image, dtype=dtype or im_dtype)
 
         # configure the export parameter values
-        crs = crs or self.crs
+        crs = crs or exp_image.crs
         if not crs_transform and not shape:
             # if none of crs_transform, shape, region or scale are specified, then set region and scale to defaults
-            region = region or self.footprint
-            scale = scale or self.scale
+            region = region or exp_image.footprint
+            scale = scale or exp_image.scale
 
-            if (crs == self.crs) and (scale == self.scale):
+            if (crs == exp_image.crs) and (scale == exp_image.scale):
                 # if crs_transform & shape are not already specified, and crs & scale match this image's crs & scale,
-                # then set crs_transform and shape to export on this image's (self) pixel grid
-                if region == self.footprint:
-                    crs_transform = self.transform
-                    shape = self.shape
+                # then set crs_transform and shape to export on export image's pixel grid
+                if region == exp_image.footprint:
+                    crs_transform = exp_image.transform
+                    shape = exp_image.shape
                 else:
                     # find a crs_transform and shape that encompasses region
                     if isinstance(region, ee.Geometry):
                         region = region.getInfo()
                     region_crs = region['crs']['properties']['name'] if 'crs' in region else 'EPSG:4326'
                     region_bounds = warp.transform_bounds(region_crs, utils.rio_crs(crs), *features.bounds(region))
-                    region_win = windows.from_bounds(*region_bounds, transform=self.transform)
+                    region_win = windows.from_bounds(*region_bounds, transform=exp_image.transform)
                     region_win = utils.expand_window_to_grid(region_win)
-                    crs_transform = self.transform * rio.Affine.translation(region_win.col_off, region_win.row_off)
+                    crs_transform = exp_image.transform * rio.Affine.translation(region_win.col_off, region_win.row_off)
                     shape = (region_win.height, region_win.width)
 
                 # prevent exporting with region & scale now that crs_transform and shape are set
                 region = None
                 scale = None
 
         # create the export parameter dict
         crs_transform = crs_transform[:6] if crs_transform else None
         dimensions = shape[::-1] if shape else None
         export_kwargs = dict(
-            crs=crs, crs_transform=crs_transform, dimensions=dimensions, region=region, scale=scale,
+            crs=crs, crs_transform=crs_transform, dimensions=dimensions, region=region, scale=scale, bands=bands,
             fileFormat='GeoTIFF', filePerBand=False
         )
         # drop items with values==None
         export_kwargs = {k: v for k, v in export_kwargs.items() if v is not None}
         logger.debug(f'ee.Image.prepare_for_export() params: {export_kwargs}')
+        # TODO: prepare_for_export does not seem to be used in ee internals any more
         ee_image, _ = ee_image.prepare_for_export(export_kwargs)
         return BaseImage(ee_image)
 
     def _prepare_for_download(self, set_nodata: bool = True, **kwargs) -> Tuple['BaseImage', Dict]:
         """
         Prepare the encapsulated image for tiled GeoTIFF download. Will reproject, resample, clip and convert the image
         according to the provided parameters.
@@ -552,21 +563,20 @@
             compress='deflate', interleave='band', tiled=True, photometric='MINISBLACK',
         )
         # add BIGTIFF support if the uncompressed image is bigger than 4GB
         if exp_image.size >= 4e9:
             profile.update(bigtiff=True)
         return exp_image, profile
 
-    @staticmethod
     def _get_tile_shape(
-        exp_image: 'BaseImage', max_tile_size: Optional[float] = None, max_tile_dim: Optional[int] = None
+        self, max_tile_size: Optional[float] = None, max_tile_dim: Optional[int] = None
     ) -> Tuple[Tuple[int, int], int]:  # yapf: disable
         """
-        Return a tile shape and number of tiles for a given BaseImage, such that the tile shape satisfies GEE
-        download limits, and is 'square-ish'.
+        Return a tile shape and number of tiles, such that the tile shape satisfies GEE download limits, and is
+        'square-ish'.
         """
         # convert max_tile_size from MB to bytes & set to EE default if None
         if max_tile_size and (max_tile_size > BaseImage._ee_max_tile_size):
             raise ValueError(
                 f'`max_tile_size` must be less than or equal to the Earth Engine download size limit of '
                 f'{BaseImage._ee_max_tile_size} MB.'
             )
@@ -575,23 +585,23 @@
             raise ValueError(
                 f'`max_tile_dim` must be less than or equal to the Earth Engine download limit of '
                 f'{BaseImage._ee_max_tile_size} pixels.'
             )
         max_tile_dim = max_tile_dim or BaseImage._ee_max_tile_dim   # set max_tile_dim to EE default if None
 
         # find the total number of tiles the image must be divided into to satisfy max_tile_size
-        image_shape = np.array(exp_image.shape, dtype='int64')
-        dtype_size = np.dtype(exp_image.dtype).itemsize
-        image_size = exp_image.size
-        if exp_image.dtype.endswith('int8'):
+        image_shape = np.array(self.shape, dtype='int64')
+        dtype_size = np.dtype(self.dtype).itemsize
+        image_size = self.size
+        if self.dtype.endswith('int8'):
             # workaround for GEE overestimate of *int8 dtype download sizes
             dtype_size *= 2
             image_size *= 2
 
-        pixel_size = dtype_size * exp_image.count
+        pixel_size = dtype_size * self.count
 
         num_tile_shape = np.array([1, 1], dtype='int64')
         tile_size = image_size
         tile_shape = image_shape
         while tile_size >= max_tile_size:
             div_axis = np.argmax(tile_shape)
             num_tile_shape[div_axis] += 1  # increase the num tiles down the longest dimension of tile_shape
@@ -643,20 +653,19 @@
         # populate band metadata
         for band_i, band_dict in enumerate(self.band_properties):
             clean_band_dict = {k.replace(':', '-'): clean_text(v) for k, v in band_dict.items()}
             if 'name' in band_dict:
                 dataset.set_band_description(band_i + 1, clean_band_dict['name'])
             dataset.update_tags(band_i + 1, **clean_band_dict)
 
-    @staticmethod
-    def _tiles(exp_image: 'BaseImage', tile_shape: Tuple[int, int]) -> Iterator[Tile]:
+    def _tiles(self, tile_shape: Tuple[int, int]) -> Iterator[Tile]:
         """
         Iterator over downloadable image tiles.
 
-        Divides an image into adjoining tiles no bigger than `tile_shape`.
+        Divides the image into adjoining tiles no bigger than `tile_shape`.
 
         Parameters
         ----------
         exp_image: BaseImage
             Image to tile.
         tile_shape: Tuple[int, int]
             (row, column) tile shape to use (pixels). Use :meth:`BaseImage._get_tile_shape` to find a tile shape that
@@ -665,21 +674,21 @@
         Yields
         -------
         Tile
             An image tile that can be downloaded.
         """
 
         # split the image up into tiles of at most `tile_shape` dimension
-        image_shape = exp_image.shape
+        image_shape = self.shape
         start_range = product(range(0, image_shape[0], tile_shape[0]), range(0, image_shape[1], tile_shape[1]))
         for tile_start in start_range:
             tile_stop = np.clip(np.add(tile_start, tile_shape), a_min=None, a_max=image_shape)
             clip_tile_shape = (tile_stop - tile_start).tolist()  # tolist is just to convert to native int
             tile_window = windows.Window(tile_start[1], tile_start[0], clip_tile_shape[1], clip_tile_shape[0])
-            yield Tile(exp_image, tile_window)
+            yield Tile(self, tile_window)
 
     @staticmethod
     def monitor_export(task: ee.batch.Task, label: str = None):
         """
         Monitor and display the progress of an export task.
 
         Parameters
@@ -764,14 +773,16 @@
         resampling : ResamplingMethod, optional
             Resampling method - see :class:`~geedim.enums.ResamplingMethod` for available options.
         dtype: str, optional
            Convert to this data type (`uint8`, `int8`, `uint16`, `int16`, `uint32`, `int32`, `float32` or
            `float64`). Defaults to auto select a minimal type that can represent the range of pixel values.
         scale_offset: bool, optional
             Whether to apply any EE band scales and offsets to the image.
+        bands: list of str, optional
+            List of band names to export.
 
         Returns
         -------
         ee.batch.Task
             The Earth Engine export task, started if ``wait`` is False, or completed if ``wait`` is True.
         """
 
@@ -779,15 +790,15 @@
         if exp_image.crs == 'SR-ORG:6974':
             logger.warning(
                 'There is an earth engine bug exporting in SR-ORG:6974, you will need to edit the exported file to '
                 'replace the CRS with SR-ORG:6842. See: https://issuetracker.google.com/issues/194561313.'
             )
 
         if logger.getEffectiveLevel() <= logging.DEBUG:
-            logger.debug(f'Uncompressed size: {self._str_format_size(exp_image.size)}')
+            logger.debug(f'Uncompressed size: {BaseImage._str_format_size(exp_image.size)}')
 
         # create export task and start
         type = ExportType(type)
         if type == ExportType.drive:
             task = ee.batch.Export.image.toDrive(
                 image=exp_image.ee_image, description=filename[:100], folder=folder, fileNamePrefix=filename,
                 maxPixels=1e9, formatOptions=dict(cloudOptimized=True),
@@ -805,15 +816,15 @@
             task = ee.batch.Export.image.toCloudStorage(
                 image=exp_image.ee_image, description=filename[:100], bucket=folder, maxPixels=1e9,
                 formatOptions=dict(cloudOptimized=True),
             )
 
         task.start()
         if wait:  # wait for completion
-            self.monitor_export(task)
+            BaseImage.monitor_export(task)
         return task
 
     def download(
         self, filename: Union[pathlib.Path, str], overwrite: bool = False, num_threads: Optional[int] = None,
         max_tile_size: Optional[float] = None, max_tile_dim: Optional[int] = None, **kwargs
     ):
         """
@@ -861,14 +872,16 @@
         resampling : ResamplingMethod, optional
             Resampling method - see :class:`~geedim.enums.ResamplingMethod` for available options.
         dtype: str, optional
            Convert to this data type (`uint8`, `int8`, `uint16`, `int16`, `uint32`, `int32`, `float32` or
            `float64`). Defaults to auto select a minimal type that can represent the range of pixel values.
         scale_offset: bool, optional
             Whether to apply any EE band scales and offsets to the image.
+        bands: list of str, optional
+            List of band names to download.
         """
 
         max_threads = num_threads or min(32, (os.cpu_count() or 1) + 4)
         out_lock = threading.Lock()
         filename = pathlib.Path(filename)
         if filename.exists():
             if overwrite:
@@ -876,33 +889,33 @@
             else:
                 raise FileExistsError(f'{filename} exists')
 
         # prepare (resample, convert, reproject) the image for download
         exp_image, profile = self._prepare_for_download(**kwargs)
 
         # get the dimensions of an image tile that will satisfy GEE download limits
-        tile_shape, num_tiles = self._get_tile_shape(exp_image, max_tile_size=max_tile_size, max_tile_dim=max_tile_dim)
+        tile_shape, num_tiles = exp_image._get_tile_shape(max_tile_size=max_tile_size, max_tile_dim=max_tile_dim)
 
         # find raw size of the download data (less than the actual download size as the image data is zipped in a
         # compressed geotiff)
         raw_download_size = exp_image.size
         if logger.getEffectiveLevel() <= logging.DEBUG:
             dtype_size = np.dtype(exp_image.dtype).itemsize
             raw_tile_size = tile_shape[0] * tile_shape[1] * exp_image.count * dtype_size
             logger.debug(f'{filename.name}:')
-            logger.debug(f'Uncompressed size: {self._str_format_size(raw_download_size)}')
+            logger.debug(f'Uncompressed size: {BaseImage._str_format_size(raw_download_size)}')
             logger.debug(f'Num. tiles: {num_tiles}')
             logger.debug(f'Tile shape: {tile_shape}')
-            logger.debug(f'Tile size: {self._str_format_size(int(raw_tile_size))}')
+            logger.debug(f'Tile size: {BaseImage._str_format_size(int(raw_tile_size))}')
 
         if raw_download_size > 1e9:
             # warn if the download is large (>1GB)
             logger.warning(
                 f'Consider adjusting `region`, `scale` and/or `dtype` to reduce the {filename.name}'
-                f' download size (raw: {self._str_format_size(raw_download_size)}).'
+                f' download size (raw: {BaseImage._str_format_size(raw_download_size)}).'
             )
 
         # configure the progress bar to monitor raw/uncompressed download size
         desc = filename.name if (len(filename.name) < self._desc_width) else f'...{filename.name[-self._desc_width:]}'
         bar_format = (
             '{desc}: |{bar}| {n_fmt}/{total_fmt} (raw) [{percentage:5.1f}%] in {elapsed:>5s} (eta: {remaining:>5s})'
         )
@@ -921,21 +934,21 @@
                 """Download a tile and write into the destination GeoTIFF. """
                 tile_array = tile.download(session=session, bar=bar)
                 with out_lock:
                     out_ds.write(tile_array, window=tile.window)
 
             with ThreadPoolExecutor(max_workers=max_threads) as executor:
                 # Run the tile downloads in a thread pool
-                tiles = self._tiles(exp_image, tile_shape=tile_shape)
+                tiles = exp_image._tiles(tile_shape=tile_shape)
                 futures = [executor.submit(download_tile, tile) for tile in tiles]
                 try:
                     for future in as_completed(futures):
                         future.result()
                 except Exception as ex:
                     logger.info(f'Exception: {str(ex)}\nCancelling...')
                     executor.shutdown(wait=False)
                     raise ex
 
             bar.update(bar.total - bar.n)   # ensure the bar reaches 100%
             # populate GeoTIFF metadata and build overviews
-            self._write_metadata(out_ds)
-            self._build_overviews(out_ds)
+            exp_image._write_metadata(out_ds)
+            BaseImage._build_overviews(out_ds)
```

### Comparing `geedim-1.7.0/geedim/enums.py` & `geedim-1.7.1/geedim/enums.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/errors.py` & `geedim-1.7.1/geedim/errors.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/mask.py` & `geedim-1.7.1/geedim/mask.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/medoid.py` & `geedim-1.7.1/geedim/medoid.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/schema.py` & `geedim-1.7.1/geedim/schema.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/stac.py` & `geedim-1.7.1/geedim/stac.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/tile.py` & `geedim-1.7.1/geedim/tile.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim/utils.py` & `geedim-1.7.1/geedim/utils.py`

 * *Files identical despite different names*

### Comparing `geedim-1.7.0/geedim.egg-info/PKG-INFO` & `geedim-1.7.1/geedim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: geedim
-Version: 1.7.0
+Version: 1.7.1
 Summary: Search, composite and download Google Earth Engine imagery.
-Home-page: https://github.com/dugalh/geedim
+Home-page: https://github.com/leftfield-geospatial/geedim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://geedim.readthedocs.io
-Project-URL: Source, https://github.com/dugalh/geedim
+Project-URL: Source, https://github.com/leftfield-geospatial/geedim
 Keywords: earth engine,satellite imagery,search,download,composite,cloud,shadow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -275,18 +275,18 @@
    terms of the `MIT license <https://github.com/cordmaur/GEES2Downloader/blob/main/LICENSE>`__.
 -  Medoid compositing was adapted from `gee_tools <https://github.com/gee-community/gee_tools>`__ under the terms of the
    `MIT license <https://github.com/gee-community/gee_tools/blob/master/LICENSE>`__.
 -  Sentinel-2 cloud/shadow masking was adapted from `ee_extra <https://github.com/r-earthengine/ee_extra>`__ under
    terms of the `Apache-2.0 license <https://github.com/r-earthengine/ee_extra/blob/master/LICENSE>`__
 
 
-.. |Tests| image:: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/geedim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
-   :target: https://codecov.io/gh/dugalh/geedim
+.. |Tests| image:: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/geedim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/geedim/branch/main/graph/badge.svg?token=69GZNQ3TI3
+   :target: https://codecov.io/gh/leftfield-geospatial/geedim
 .. |PyPI version| image:: https://img.shields.io/pypi/v/geedim.svg
    :target: https://pypi.org/project/geedim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/geedim.svg
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/geedim
 .. |docs| image:: https://readthedocs.org/projects/geedim/badge/?version=latest
    :target: https://geedim.readthedocs.io/en/latest/?badge=latest
```

### Comparing `geedim-1.7.0/setup.py` & `geedim-1.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     name='geedim',
     version=__version__,
     description='Search, composite and download Google Earth Engine imagery.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Dugal Harris',
     author_email='dugalh@gmail.com',
-    url='https://github.com/dugalh/geedim',
+    url='https://github.com/leftfield-geospatial/geedim',
     license='Apache-2.0',
     packages=find_packages(include=['geedim']),
     package_data={'geedim': ['data/ee_stac_urls.json']},
     install_requires=[
         'numpy>=1.19',
         'rasterio>=1.1',
         'click>=8',
@@ -65,10 +65,10 @@
     ],
     keywords=[
         'earth engine', 'satellite imagery', 'search', 'download', 'composite', 'cloud', 'shadow',
     ],
     entry_points={'console_scripts': ['geedim=geedim.cli:cli']},
     project_urls={
         'Documentation': 'https://geedim.readthedocs.io',
-        'Source': 'https://github.com/dugalh/geedim',
+        'Source': 'https://github.com/leftfield-geospatial/geedim',
     },
 )  # yapf: disable
```

