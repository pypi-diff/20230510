# Comparing `tmp/hhnk_research_tools-0.8.tar.gz` & `tmp/hhnk_research_tools-2023.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk_research_tools-0.8.tar", last modified: Wed Aug 17 15:08:12 2022, max compression
+gzip compressed data, was "hhnk_research_tools-2023.1.tar", last modified: Mon Jan 23 10:03:10 2023, max compression
```

## Comparing `hhnk_research_tools-0.8.tar` & `hhnk_research_tools-2023.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:11.924820 hhnk_research_tools-0.8/
--rw-rw-rw-   0        0        0      534 2022-08-17 15:08:12.521299 hhnk_research_tools-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:12.001821 hhnk_research_tools-0.8/hhnk_research_tools/
--rw-rw-rw-   0        0        0     1291 2022-08-17 15:08:00.000000 hhnk_research_tools-0.8/hhnk_research_tools/__init__.py
--rw-rw-rw-   0        0        0     5861 2022-05-04 08:10:39.000000 hhnk_research_tools-0.8/hhnk_research_tools/dataframe_functions.py
--rw-rw-rw-   0        0        0      327 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/general_functions.py
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:12.243825 hhnk_research_tools-0.8/hhnk_research_tools/gis/
--rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/gis/__init__.py
--rw-rw-rw-   0        0        0     9613 2022-07-20 14:26:46.000000 hhnk_research_tools-0.8/hhnk_research_tools/gis/raster.py
--rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-0.8/hhnk_research_tools/gis/vector.py
--rw-rw-rw-   0        0        0    16987 2022-08-01 14:54:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/raster_functions.py
--rw-rw-rw-   0        0        0    11535 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/sql_functions.py
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:12.400827 hhnk_research_tools-0.8/hhnk_research_tools/threedi/
--rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/__init__.py
--rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/construct_rain_scenario.py
--rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
--rw-rw-rw-   0        0        0     1981 2022-07-04 12:38:36.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/geometry_functions.py
--rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/grid.py
--rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/gridedit.py
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:12.496829 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/
--rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/__init__.py
--rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/gridadmin.py
--rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/rain_dataframe.py
--rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/results_mapping.py
--rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/threedi/variables/variables_container.py
--rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-0.8/hhnk_research_tools/variables.py
-drwxrwxrwx   0        0        0        0 2022-08-17 15:08:12.139823 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/
--rw-rw-rw-   0        0        0      534 2022-08-17 15:08:11.000000 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1113 2022-08-17 15:08:11.000000 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-17 15:08:11.000000 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2022-08-17 15:08:11.000000 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-08-17 15:08:11.000000 hhnk_research_tools-0.8/hhnk_research_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-17 15:08:12.540351 hhnk_research_tools-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1639 2022-05-04 07:44:27.000000 hhnk_research_tools-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:09.437515 hhnk_research_tools-2023.1/
+-rw-rw-rw-   0        0        0      537 2023-01-23 10:03:10.102142 hhnk_research_tools-2023.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:09.558517 hhnk_research_tools-2023.1/hhnk_research_tools/
+-rw-rw-rw-   0        0        0     1311 2023-01-23 09:57:31.000000 hhnk_research_tools-2023.1/hhnk_research_tools/__init__.py
+-rw-rw-rw-   0        0        0     5861 2022-05-04 08:10:39.000000 hhnk_research_tools-2023.1/hhnk_research_tools/dataframe_functions.py
+-rw-rw-rw-   0        0        0      327 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/general_functions.py
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:09.766520 hhnk_research_tools-2023.1/hhnk_research_tools/gis/
+-rw-rw-rw-   0        0        0     1092 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/gis/__init__.py
+-rw-rw-rw-   0        0        0    16611 2023-01-20 11:08:55.000000 hhnk_research_tools-2023.1/hhnk_research_tools/gis/raster.py
+-rw-rw-rw-   0        0        0     1427 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.1/hhnk_research_tools/gis/vector.py
+-rw-rw-rw-   0        0        0    15545 2023-01-17 13:55:17.000000 hhnk_research_tools-2023.1/hhnk_research_tools/raster_functions.py
+-rw-rw-rw-   0        0        0    11535 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/sql_functions.py
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:09.949523 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/
+-rw-rw-rw-   0        0        0      149 2022-07-04 12:41:36.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/__init__.py
+-rw-rw-rw-   0        0        0     3603 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/construct_rain_scenario.py
+-rw-rw-rw-   0        0        0     2260 2022-08-17 15:04:24.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py
+-rw-rw-rw-   0        0        0     1981 2022-07-04 12:38:36.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/geometry_functions.py
+-rw-rw-rw-   0        0        0    12463 2022-07-04 14:10:34.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/grid.py
+-rw-rw-rw-   0        0        0     1722 2022-05-04 07:44:27.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/gridedit.py
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:10.073525 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/
+-rw-rw-rw-   0        0        0        0 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/__init__.py
+-rw-rw-rw-   0        0        0       66 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/gridadmin.py
+-rw-rw-rw-   0        0        0      182 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/rain_dataframe.py
+-rw-rw-rw-   0        0        0       33 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/results_mapping.py
+-rw-rw-rw-   0        0        0      415 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/threedi/variables/variables_container.py
+-rw-rw-rw-   0        0        0     1870 2021-10-25 11:51:58.000000 hhnk_research_tools-2023.1/hhnk_research_tools/variables.py
+drwxrwxrwx   0        0        0        0 2023-01-23 10:03:09.696519 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/
+-rw-rw-rw-   0        0        0      537 2023-01-23 10:03:08.000000 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1113 2023-01-23 10:03:09.000000 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-23 10:03:08.000000 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-01-23 10:03:08.000000 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-01-23 10:03:08.000000 hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-23 10:03:10.119925 hhnk_research_tools-2023.1/setup.cfg
+-rw-rw-rw-   0        0        0     1671 2022-09-09 15:01:24.000000 hhnk_research_tools-2023.1/setup.py
```

### Comparing `hhnk_research_tools-0.8/PKG-INFO` & `hhnk_research_tools-2023.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hhnk_research_tools
-Version: 0.8
+Version: 2023.1
 Summary: HHNK tools for working with 3di
 Home-page: https://github.com/HHNK/hhnk-research-tools
 Author: Wietse van Gerwen
 Author-email: w.vangerwen@hhnk.nl
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/HHNK/hhnk-research-tools/issues
 Description: UNKNOWN
```

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/__init__.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/gis/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import hhnk_research_tools.variables as variables
 
-from hhnk_research_tools.gis.raster import Raster
-
-import hhnk_research_tools.threedi as threedi
-
-
 from hhnk_research_tools.sql_functions import (
     sql_create_update_case_statement,
     sql_construct_select_query,
     create_sqlite_connection,
     sql_table_exists,
     execute_sql_selection,
     execute_sql_changes,
@@ -27,21 +22,17 @@
 from hhnk_research_tools.general_functions import ensure_file_path
 
 from hhnk_research_tools.raster_functions import (
     load_gdal_raster,
     gdf_to_raster,
     create_new_raster_file,
     save_raster_array_to_tiff,
-    build_vrt,
-    create_meta_from_gdf,
-    dx_dy_between_rasters,
-    Raster_calculator,
 )
 
 # TODO how does this versioning work?
 # Threedigrid version number is automatic updated with zest.releaser. Geopandas uses versioneer.py.
 # the version number in setup.py is updated using the find_version()
-__version__ = '0.8'
+__version__ = '0.3'
 
 __doc__ = """
 General toolbox for loading, converting and saving serval datatypes.
 """
```

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/dataframe_functions.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/dataframe_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/gis/__init__.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import hhnk_research_tools.variables as variables
 
+from hhnk_research_tools.gis.raster import Raster, RasterMetadata
+
+import hhnk_research_tools.threedi as threedi
+
+
 from hhnk_research_tools.sql_functions import (
     sql_create_update_case_statement,
     sql_construct_select_query,
     create_sqlite_connection,
     sql_table_exists,
     execute_sql_selection,
     execute_sql_changes,
@@ -22,17 +27,21 @@
 from hhnk_research_tools.general_functions import ensure_file_path
 
 from hhnk_research_tools.raster_functions import (
     load_gdal_raster,
     gdf_to_raster,
     create_new_raster_file,
     save_raster_array_to_tiff,
+    build_vrt,
+    create_meta_from_gdf,
+    dx_dy_between_rasters,
+    Raster_calculator,
 )
 
 # TODO how does this versioning work?
 # Threedigrid version number is automatic updated with zest.releaser. Geopandas uses versioneer.py.
 # the version number in setup.py is updated using the find_version()
-__version__ = '0.3'
+__version__ = '2023.01'
 
 __doc__ = """
 General toolbox for loading, converting and saving serval datatypes.
 """
```

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/gis/vector.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/gis/vector.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/raster_functions.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/raster_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from osgeo import gdal
+# %%
+from osgeo import gdal, ogr
 import numpy as np
 import json
-from osgeo import ogr
-from shapely.geometry import LineString
 from hhnk_research_tools.variables import DEF_TRGT_CRS
 from hhnk_research_tools.variables import GDAL_DATATYPE, GEOTIFF
 from hhnk_research_tools.variables import GEOTIFF, GDAL_DATATYPE
 from hhnk_research_tools.general_functions import ensure_file_path
+from hhnk_research_tools.gis.raster import Raster, RasterMetadata
+from pathlib import Path
 import os
 
+
 # Loading
 def _get_array_from_bands(gdal_file, band_count, window, raster_source):
     try:
         if band_count == 1:
             band = gdal_file.GetRasterBand(1)
             if window is not None:
                 raster_array = band.ReadAsArray(
@@ -54,60 +56,34 @@
             raise ValueError(
                 f"Unexpected number of bands in raster {raster_source} (expect 1 or 3)"
             )
     except Exception as e:
         raise e
 
 
-def _get_gdal_metadata(gdal_file) -> dict:
-    try:
-        meta = {}
-        meta["proj"] = gdal_file.GetProjection()
-        meta["georef"] = gdal_file.GetGeoTransform()
-        meta["pixel_width"] = meta["georef"][1]
-        meta["x_min"] = meta["georef"][0]
-        meta["y_max"] = meta["georef"][3]
-        meta["x_max"] = meta["x_min"] + meta["georef"][1] * gdal_file.RasterXSize
-        meta["y_min"] = meta["y_max"] + meta["georef"][5] * gdal_file.RasterYSize
-        meta["bounds"] = [meta["x_min"], meta["x_max"], meta["y_min"], meta["y_max"]]
-        # for use in threedi_scenario_downloader
-        meta["bounds_dl"] = {
-            "west": meta["x_min"],
-            "south": meta["y_min"],
-            "east": meta["x_max"],
-            "north": meta["y_max"],
-        }
-        meta["x_res"] = gdal_file.RasterXSize
-        meta["y_res"] = gdal_file.RasterYSize
-        meta["shape"] = [meta["y_res"], meta["x_res"]]
-        return meta
-    except Exception as e:
-        raise e
-
-
 def load_gdal_raster(raster_source, window=None, return_array=True, band_count=None):
     """
     Loads a raster (tif) and returns an array of its values, its no_data value and
     dict containing associated metadata
     returns raster_array, no_data, metadata
     """
     try:
-        gdal_file = gdal.Open(raster_source)
-        if gdal_file:
+        gdal_src = gdal.Open(raster_source)
+        if gdal_src:
             if return_array:
                 if band_count==None:
-                    band_count = gdal_file.RasterCount
+                    band_count = gdal_src.RasterCount
                 raster_array = _get_array_from_bands(
-                    gdal_file, band_count, window, raster_source
+                    gdal_src, band_count, window, raster_source
                 )
             else:
                 raster_array = None
             # are they always same even if more bands?
-            no_data = gdal_file.GetRasterBand(1).GetNoDataValue()
-            metadata = _get_gdal_metadata(gdal_file)
+            no_data = gdal_src.GetRasterBand(1).GetNoDataValue()
+            metadata = RasterMetadata(gdal_src=gdal_src)
             return raster_array, no_data, metadata
     except Exception as e:
         raise e
 
 
 # Conversion
 def _gdf_to_json(gdf, epsg=DEF_TRGT_CRS):
@@ -214,24 +190,24 @@
     Compression:
     LZW - highest compression ratio, highest processing power
     DEFLATE
     PACKBITS - lowest compression ratio, lowest processing power
     """
     try:
         target_ds = gdal.GetDriverByName(driver).Create(
-            file_name,
-            meta["x_res"],
-            meta["y_res"],
+            str(file_name),
+            meta.x_res,
+            meta.y_res,
             num_bands,
             datatype,
             options=[f"COMPRESS={compression}", f"TILED={tiled}"],
         )
-        target_ds.SetGeoTransform(meta["georef"])
+        target_ds.SetGeoTransform(meta.georef)
         _set_band_data(target_ds, num_bands, nodata)
-        target_ds.SetProjection(meta["proj"])
+        target_ds.SetProjection(meta.proj)
         return target_ds
     except Exception as e:
         raise e
 
 
 def save_raster_array_to_tiff(
     output_file,
@@ -266,103 +242,90 @@
             target_ds.GetRasterBand(i).WriteArray(raster_array)  # fill file with data
         target_ds = None
     except Exception as e:
         raise e
 
         
 def build_vrt(raster_folder, vrt_name='combined_rasters', bandlist=[1], bounds=None, overwrite=False):
+    #TODO check resolution of all rasters in folder. if not equal then no vrt.
     """create vrt from all rasters in a folder.
     bounds=(xmin, ymin, xmax, ymax)
     bandList doesnt work as expected."""
     output_path = os.path.join(raster_folder, f'{vrt_name}.vrt')
     
     if os.path.exists(output_path) and not overwrite:
         print(f'vrt already exists: {output_path}')
         return
 
     tifs_list = [os.path.join(raster_folder, i) for i in os.listdir(raster_folder) if i.endswith('.tif') or i.endswith('.tiff')]
 
 
+    for r in tifs_list:
+        if Raster(r).metadata.pixel_width==1:
+            print(Path(r.source_path).stem)
+
+
     vrt_options = gdal.BuildVRTOptions(resolution='highest',
                                        separate=False,
                                        resampleAlg='nearest',
                                        addAlpha=False,
                                        outputBounds=bounds,
                                        bandList=bandlist,)
     ds = gdal.BuildVRT(output_path, tifs_list, options=vrt_options)
     ds.FlushCache()
+    del tifs_list
+
     if not os.path.exists(output_path):
         print('Something went wrong, vrt not created.')
 
 
-
-def create_meta(minx, maxx, miny, maxy, res, proj='epsg:28992') -> dict:
-    """
-    only works for epsg:28992. 
-    example input:
-    minx=113891
-    maxy=535912
-    maxx=120760
-    miny=534177
-    res=0.5
-    """
-    projections = {'epsg:28992':'PROJCS["Amersfoort / RD New",GEOGCS["Amersfoort",DATUM["Amersfoort",SPHEROID["Bessel 1841",6377397.155,299.1528128,AUTHORITY["EPSG","7004"]],TOWGS84[565.2369,50.0087,465.658,-0.406857,0.350733,-1.87035,4.0812],AUTHORITY["EPSG","6289"]],PRIMEM["Greenwich",0,AUTHORITY["EPSG","8901"]],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4289"]],PROJECTION["Oblique_Stereographic"],PARAMETER["latitude_of_origin",52.15616055555555],PARAMETER["central_meridian",5.38763888888889],PARAMETER["scale_factor",0.9999079],PARAMETER["false_easting",155000],PARAMETER["false_northing",463000],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["X",EAST],AXIS["Y",NORTH],AUTHORITY["EPSG","28992"]]'}
-    
-    meta = {'proj': projections[proj],
-         'georef': (int(np.floor(minx)), res, 0.0, int(np.ceil(maxy)), 0.0, -res),
-         'pixel_width': res,
-         'x_min': int(np.floor(minx)),
-         'y_max': int(np.ceil(maxy)),
-         'x_max': int(np.ceil(maxx)),
-         'y_min': int(np.floor(miny))}
-    meta = {**meta, 
-          'x_res': int((meta['x_max']-meta['x_min'])/res),
-         'y_res': int((meta['y_max']-meta['y_min'])/res)} 
-    return meta
-    
-
 def create_meta_from_gdf(gdf, res) -> dict:
     """Create metadata that can be used in raster creation based on gdf bounds. 
     Projection is 28992 default, only option.""" 
     gdf_local=gdf.copy()
     gdf_local['temp'] = 0
-    bounds = gdf_local.dissolve('temp').bounds.iloc[0]
-
-    return create_meta(**bounds, res=res)
+    bounds_dict = gdf_local.dissolve('temp').bounds.iloc[0]
+    return RasterMetadata(res=res, bounds_dict=bounds_dict)
 
 
 def dx_dy_between_rasters(meta_big, meta_small):
     """create window to subset a large 2-d array with a smaller rectangle. Usage:
     shapes_array[dy_min:dy_max, dx_min:dx_max]
     window=create_array_window_from_meta(meta_big, meta_small)
     shapes_array[window]"""
-    if meta_small['pixel_width'] != meta_big['pixel_width']:
+    if meta_small.pixel_width != meta_big.pixel_width:
         raise Exception(f"""Input rasters dont have same resolution. 
-                meta_big   = {meta_big['pixel_width']}m
-                meta_small = {meta_small['pixel_width']}m""")
+                meta_big   = {meta_big.pixel_width}m
+                meta_small = {meta_small.pixel_width}m""")
 
-    dx_min = max(0, int((meta_small['x_min']-meta_big['x_min'])/meta_big['pixel_width']))
-    dy_min = max(0, int((meta_big['y_max']-meta_small['y_max'])/meta_big['pixel_width']))
-    dx_max = int(min(dx_min + meta_small['x_res'], meta_big['x_res']))
-    dy_max = int(min(dy_min + meta_small['y_res'], meta_big['y_res']))
-    return dx_min, dy_min
+    dx_min = max(0, int((meta_small.x_min-meta_big.x_min)/meta_big.pixel_width))
+    dy_min = int((meta_big.y_max-meta_small.y_max)/meta_big.pixel_width)
+
+    if dx_min < 0:
+        raise Exception(f"dx_min smaller than 0 ({dx_min})")
+    if dy_min < 0:
+        raise Exception(f"dy_min smaller than 0 ({dy_min})")
+
+    dx_max = int(min(dx_min + meta_small.x_res, meta_big.x_res))
+    dy_max = int(min(dy_min + meta_small.y_res, meta_big.y_res))
+    return dx_min, dy_min, dx_max, dy_max
 
 
 class Raster_calculator():
     """Make a custom calculation between two rasters by 
     reading the blocks and applying a calculation
     input raster should be of type hhnk_research_tools.gis.raster.Raster
 
     raster1: hrt.Raster -> big raster
     raster2: hrt.Raster -> smaller raster with full extent within big raster. Raster numbering is interchangeable as the scripts checks the bounds.
     raster_out: hrt.Raster -> output, doesnt need to exists. self.create also creates it.
     custom_run_window_function: function that takes window of small and big raster as input and does calculation with these arrays.
     customize below function for this, can take more inputs.
 
-    def custom_run_window_function(self, window_small, window_big, band_out):
+    def custom_run_window_function(self, window_small, window_big, band_out, **kwargs):
         #Customize this function with a calculation
         #Load windows
         block_big = self.raster_big._read_array(window=window_big)
         block_small = self.raster_small._read_array(window=window_small)
 
         #Calculate output
         block_out = None #replace with a calculation.
@@ -383,21 +346,21 @@
         self.blocks_df = self.raster_small.generate_blocks()
         self.blocks_total = len(self.blocks_df)
         self.custom_run_window_function = custom_run_window_function
         self.verbose = verbose
 
 
     def _checkbounds(self, raster1, raster2):
-        x1, x2, y1, y2=raster1.metadata['bounds']
-        xx1, xx2, yy1, yy2=raster1.metadata['bounds']
+        x1, x2, y1, y2=raster1.metadata.bounds
+        xx1, xx2, yy1, yy2=raster2.metadata.bounds
         bounds_diff = x1 - xx1, y1 - yy1, xx2-x2, yy2 - y2 #subtract bounds
         check_arr = np.array([i<=0 for i in bounds_diff]) #check if values <=0
 
         #If all are true (or all false) we know that the rasters fully overlap. 
-        if raster1.metadata['pixel_width'] != raster2.metadata['pixel_width']:
+        if raster1.metadata.pixel_width != raster2.metadata.pixel_width:
             raise Exception("""Rasters do not have equal resolution""")
 
         if np.all(check_arr):
             #In this case raster1 is the bigger raster.
             return raster1, raster2
         elif np.all(~check_arr):
             #In this case raster2 is the bigger raster
@@ -442,8 +405,28 @@
                 self.custom_run_window_function(self=self, window_small=window_small, window_big=window_big, band_out=band_out, **kwargs)
                 if self.verbose:
                     print(f"{idx} / {self.blocks_total}", end= '\r')
                 # break
                 
         band_out.FlushCache()  # close file after writing
         band_out = None
-        target_ds = None
+        target_ds = None
+
+
+def reproject(src:Raster, target_res:float, output_path:str):
+        """
+        src : hrt.Raster
+        output_path : str
+        meta_new : hrt.core"""
+        #https://svn.osgeo.org/gdal/trunk/autotest/alg/reproject.py
+        # drv = gdal.GetDriverByName( 'GTiff' )
+        # drv.Delete(output_path)
+
+        src.metadata.update_resolution(target_res)
+
+        src_ds = src.source
+        dst_ds = create_new_raster_file(file_name=output_path,
+                    nodata=src.nodata,
+                    meta=src.metadata)
+
+        gdal.ReprojectImage(src_ds, dst_ds, src_wkt='EPSG:28992')
+
```

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/sql_functions.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/sql_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/threedi/construct_rain_scenario.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/threedi/construct_rain_scenario.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/threedi/construct_rain_scenario_dataframe.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/threedi/geometry_functions.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/threedi/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/threedi/grid.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/threedi/grid.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/threedi/gridedit.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/threedi/gridedit.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools/variables.py` & `hhnk_research_tools-2023.1/hhnk_research_tools/variables.py`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/hhnk_research_tools.egg-info/SOURCES.txt` & `hhnk_research_tools-2023.1/hhnk_research_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hhnk_research_tools-0.8/setup.py` & `hhnk_research_tools-2023.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,9 +46,10 @@
         "numpy>=1.17.0",  # Was 1.19.1
         "Shapely>=1.6.4",  # Was 1.7.0
         "gdal>=2.4.0",  # Was 3.1.4
         "pandas>=0.25.3",  # Was 1.0.1
         "geopandas>=0.6.0",  # Was 0.7.0
         "threedigrid>=1.0.16",  # Was 1.0.25
         "xarray",
+        "threedigrid_builder",
     ],
 )
```

