# Comparing `tmp/stactools-sentinel1-0.5.3.tar.gz` & `tmp/stactools-sentinel1-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-sentinel1-0.5.3.tar", last modified: Fri Apr  7 13:56:33 2023, max compression
+gzip compressed data, was "stactools-sentinel1-0.6.0.tar", last modified: Tue May  9 17:26:12 2023, max compression
```

## Comparing `stactools-sentinel1-0.5.3.tar` & `stactools-sentinel1-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.530365 stactools-sentinel1-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.530365 stactools-sentinel1-0.5.3/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/src/stactools/sentinel1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/metadata_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/product_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/rtc_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-07 13:56:14.000000 stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:56:33.534365 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-04-07 13:56:33.000000 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-07 13:56:33.000000 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 13:56:33.000000 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-07 13:56:33.000000 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 13:56:33.000000 stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.138568 stactools-sentinel1-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-09 17:26:12.138568 stactools-sentinel1-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-09 17:26:12.138568 stactools-sentinel1-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.134568 stactools-sentinel1-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.134568 stactools-sentinel1-0.6.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.134568 stactools-sentinel1-0.6.0/src/stactools/sentinel1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.134568 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/metadata_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/product_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.138568 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/rtc_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-09 17:25:44.000000 stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:26:12.138568 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-09 17:26:12.000000 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-09 17:26:12.000000 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:26:12.000000 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 17:26:12.000000 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 17:26:12.000000 stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/top_level.txt
```

### Comparing `stactools-sentinel1-0.5.3/LICENSE` & `stactools-sentinel1-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/PKG-INFO` & `stactools-sentinel1-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel1
-Version: 0.5.3
+Version: 0.6.0
 Summary: stactools subpackage for creating sentinel1 STACs
 Home-page: https://github.com/stactools-packages/sentinel1
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://github.com/stactools-packages/sentinel1
 Project-URL: Issues, https://github.com/stactools-packages/sentinel1/issues
 Keywords: stactools,pystac,catalog,STAC,sentinel,GRD,radar
@@ -58,20 +58,26 @@
 
 The `stactools.sentinel1.grd` subpackage and `stac sentinel1 grd` commands deal
 with [Sentinel 1 Ground Range Detected (GRD)
 Level-1](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/resolutions/level-1-ground-range-detected)
 product. It is used to create STAC Items from the SAFE manifest format of the
 data hosted on Microsoft Azure.
 
-## Examples
+## Example Outputs
 
-### STAC objects
+### RTC
 
-- [Item (RTC)](examples/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
-- [Item (GRD)](examples/grd/item.json)
+- [Collection](examples/rtc/sentinel1-rtc-aws/collection.json)
+- [Item (S1B_20161121_12SYJ_ASC)](examples/rtc/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
+- [Item (S1A_20200103_17RMJ_ASC)](examples/rtc/sentinel1-rtc-aws/2020/S1A_20200103_17RMJ_ASC/S1A_20200103_17RMJ_ASC.json)
+
+### GRD
+
+- [Item (S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549)](examples/grd/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549.json)
+- [Item (S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13)](examples/grd/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13.json)
 
 ## How to use
 
 ### Install package
 
 ```shell
 pip install stactools-sentinel1
```

### Comparing `stactools-sentinel1-0.5.3/README.md` & `stactools-sentinel1-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -39,20 +39,26 @@
 
 The `stactools.sentinel1.grd` subpackage and `stac sentinel1 grd` commands deal
 with [Sentinel 1 Ground Range Detected (GRD)
 Level-1](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/resolutions/level-1-ground-range-detected)
 product. It is used to create STAC Items from the SAFE manifest format of the
 data hosted on Microsoft Azure.
 
-## Examples
+## Example Outputs
 
-### STAC objects
+### RTC
 
-- [Item (RTC)](examples/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
-- [Item (GRD)](examples/grd/item.json)
+- [Collection](examples/rtc/sentinel1-rtc-aws/collection.json)
+- [Item (S1B_20161121_12SYJ_ASC)](examples/rtc/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
+- [Item (S1A_20200103_17RMJ_ASC)](examples/rtc/sentinel1-rtc-aws/2020/S1A_20200103_17RMJ_ASC/S1A_20200103_17RMJ_ASC.json)
+
+### GRD
+
+- [Item (S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549)](examples/grd/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549.json)
+- [Item (S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13)](examples/grd/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13.json)
 
 ## How to use
 
 ### Install package
 
 ```shell
 pip install stactools-sentinel1
```

### Comparing `stactools-sentinel1-0.5.3/setup.cfg` & `stactools-sentinel1-0.6.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
-	stactools == 0.4.5
+	stactools >= 0.4.5
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/bands.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/bands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/commands.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/constants.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/metadata_links.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/metadata_links.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/product_metadata.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/product_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/properties.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/properties.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/grd/stac.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/grd/stac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import logging
 import os
 from typing import Any, Optional
 
 import pystac
+import shapely
 from pystac import Summaries
 from pystac.extensions.eo import EOExtension
 from pystac.extensions.item_assets import ItemAssetsExtension
+from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.sar import SarExtension
 from pystac.extensions.sat import SatExtension
 from stactools.core.io import ReadHrefModifier
+from stactools.core.projection import transform_from_bbox
 
 from stactools.sentinel1.grd import constants as c
 
 from . import Format
 from .bands import image_asset_from_href
 from .metadata_links import MetadataLinks
 from .product_metadata import ProductMetadata, get_shape
@@ -61,15 +64,15 @@
     sar.resolution_range = c.SENTINEL_GRD_SAR["resolution_range"]
     sar.resolution_azimuth = c.SENTINEL_GRD_SAR["resolution_azimuth"]
     sar.pixel_spacing_range = c.SENTINEL_GRD_SAR["pixel_spacing_range"]
     sar.observation_direction = c.SENTINEL_GRD_SAR["observation_direction"]
     sar.pixel_spacing_azimuth = c.SENTINEL_GRD_SAR["pixel_spacing_azimuth"]
     sar.looks_equivalent_number = c.SENTINEL_GRD_SAR["looks_equivalent_number"]
 
-    # SAT Extension
+    # Satellite Extension
     sat = SatExtension.summaries(collection, add_if_missing=True)
     sat.orbit_state = c.SENTINEL_GRD_SAT["orbit_state"]
 
     # Item Asset Extension
     assets = ItemAssetsExtension.ext(collection, add_if_missing=True)
     assets.item_assets = c.SENTINEL_GRD_ASSETS
 
@@ -108,43 +111,66 @@
     product_metadata = ProductMetadata(
         metalinks.product_metadata_href,
         metalinks.grouped_hrefs,
         metalinks.map_filename,
         metalinks.manifest,
     )
 
+    scene_id = product_metadata.scene_id
+
+    # Remove the last segment of the scene id so the same scene reprocessed
+    # at different times will have the same Item ID
+    item_id = scene_id[:-5]
+
     item = pystac.Item(
-        id=product_metadata.scene_id,
+        id=item_id,
         geometry=product_metadata.geometry,
         bbox=product_metadata.bbox,
         datetime=product_metadata.get_datetime,
         properties={},
         stac_extensions=[],
     )
 
     # ---- Add Extensions ----
-    # sar
+    # SAR Extension
     sar = SarExtension.ext(item, add_if_missing=True)
     fill_sar_properties(sar, metalinks.manifest, product_metadata.resolution)
 
-    # sat
+    # Satellite Extension
     sat = SatExtension.ext(item, add_if_missing=True)
     fill_sat_properties(sat, metalinks.manifest)
 
     # eo
     EOExtension.ext(item, add_if_missing=True)
 
+    # Projection Extension
+    projection = ProjectionExtension.ext(item, add_if_missing=True)
+    projection.epsg = 4326
+    projection.bbox = product_metadata.bbox
+    shape = get_shape(metalinks, read_href_modifier, **kwargs)
+    projection.shape = shape
+    projection.transform = transform_from_bbox(projection.bbox, shape)
+    centroid = shapely.geometry.shape(item.geometry).centroid
+    projection.centroid = {"lat": round(centroid.y, 5), "lon": round(centroid.x, 5)}
+
     # --Common metadata--
     item.common_metadata.providers = [c.SENTINEL_PROVIDER]
     item.common_metadata.platform = product_metadata.platform
     item.common_metadata.constellation = c.SENTINEL_CONSTELLATION
 
-    # s1 properties
-    shape = get_shape(metalinks, read_href_modifier, **kwargs)
-    item.properties.update({**product_metadata.metadata_dict, "s1:shape": shape})
+    # Add s1 properties
+    item.properties.update(product_metadata.metadata_dict)
+
+    item.properties["s1:shape"] = shape
+    item.properties["s1:product_identifier"] = scene_id
+
+    if pdt := metalinks.manifest.find_attr(
+        "stop", ".//safe:processing[@name='GRD Post Processing']"
+    ):
+        item.properties["s1:processing_datetime"] = f"{pdt}Z"
 
     # Add assets to item
     item.add_asset(*metalinks.create_manifest_asset())
 
     # Annotations for bands
     for asset_obj in metalinks.create_product_asset():
         item.add_asset(asset_obj[0], asset_obj[1])
```

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/commands.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/constants.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/rtc_metadata.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/rtc_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools/sentinel1/rtc/stac.py` & `stactools-sentinel1-0.6.0/src/stactools/sentinel1/rtc/stac.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/PKG-INFO` & `stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel1
-Version: 0.5.3
+Version: 0.6.0
 Summary: stactools subpackage for creating sentinel1 STACs
 Home-page: https://github.com/stactools-packages/sentinel1
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Documentation, https://github.com/stactools-packages/sentinel1
 Project-URL: Issues, https://github.com/stactools-packages/sentinel1/issues
 Keywords: stactools,pystac,catalog,STAC,sentinel,GRD,radar
@@ -58,20 +58,26 @@
 
 The `stactools.sentinel1.grd` subpackage and `stac sentinel1 grd` commands deal
 with [Sentinel 1 Ground Range Detected (GRD)
 Level-1](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-1-sar/resolutions/level-1-ground-range-detected)
 product. It is used to create STAC Items from the SAFE manifest format of the
 data hosted on Microsoft Azure.
 
-## Examples
+## Example Outputs
 
-### STAC objects
+### RTC
 
-- [Item (RTC)](examples/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
-- [Item (GRD)](examples/grd/item.json)
+- [Collection](examples/rtc/sentinel1-rtc-aws/collection.json)
+- [Item (S1B_20161121_12SYJ_ASC)](examples/rtc/sentinel1-rtc-aws/2016/S1B_20161121_12SYJ_ASC/S1B_20161121_12SYJ_ASC.json)
+- [Item (S1A_20200103_17RMJ_ASC)](examples/rtc/sentinel1-rtc-aws/2020/S1A_20200103_17RMJ_ASC/S1A_20200103_17RMJ_ASC.json)
+
+### GRD
+
+- [Item (S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549)](examples/grd/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549/S1A_EW_GRDM_1SDH_20221130T014342_20221130T014446_046117_058549.json)
+- [Item (S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13)](examples/grd/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13/S1A_IW_GRDH_1SDV_20210809T173953_20210809T174018_039156_049F13.json)
 
 ## How to use
 
 ### Install package
 
 ```shell
 pip install stactools-sentinel1
```

### Comparing `stactools-sentinel1-0.5.3/src/stactools_sentinel1.egg-info/SOURCES.txt` & `stactools-sentinel1-0.6.0/src/stactools_sentinel1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

