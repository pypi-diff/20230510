# Comparing `tmp/segment-geospatial-0.4.0.tar.gz` & `tmp/segment-geospatial-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.4.0.tar", last modified: Sat May  6 04:53:40 2023, max compression
+gzip compressed data, was "segment-geospatial-0.5.0.tar", last modified: Wed May 10 20:59:47 2023, max compression
```

## Comparing `segment-geospatial-0.4.0.tar` & `segment-geospatial-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39601 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 04:53:40.000000 segment-geospatial-0.4.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-06 04:53:40.882409 segment-geospatial-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-06 04:53:30.000000 segment-geospatial-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.078302 segment-geospatial-0.5.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26344 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 20:59:47.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 20:59:46.000000 segment-geospatial-0.5.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 20:59:47.082303 segment-geospatial-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 20:59:33.000000 segment-geospatial-0.5.0/setup.py
```

### Comparing `segment-geospatial-0.4.0/LICENSE` & `segment-geospatial-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.4.0/PKG-INFO` & `segment-geospatial-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.4.0
+Version: 0.5.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
 License-File: LICENSE
 
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
@@ -41,21 +42,32 @@
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+-   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
+-   Interactive segmentation with input prompts
+
+![](https://i.imgur.com/GV7Rzxt.gif)
+
+## Tutorials
+
+Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
+
+[![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.4.0/README.md` & `segment-geospatial-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,21 +20,32 @@
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+-   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
+-   Interactive segmentation with input prompts
+
+![](https://i.imgur.com/GV7Rzxt.gif)
+
+## Tutorials
+
+Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
+
+[![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

### Comparing `segment-geospatial-0.4.0/samgeo/common.py` & `segment-geospatial-0.5.0/samgeo/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 The source code is adapted from https://github.com/aliaksandr960/segment-anything-eo. Credit to the author Aliaksandr Hancharenka.
 """
 
 import os
 import tempfile
 import cv2
 import numpy as np
-import rasterio
 from tqdm import tqdm
 
 import shapely
-import geopandas as gpd
-from pyproj import Transformer, transform
+import pyproj
 import rasterio
-from rasterio import features
+import geopandas as gpd
+import matplotlib.pyplot as plt
 
 
 def check_file_path(file_path, make_dirs=True):
     """Gets the absolute file path.
 
     Args:
         file_path (str): The path to the file.
@@ -588,16 +587,17 @@
 
 def get_crs(src_fp):
     with rasterio.open(src_fp) as src:
         return src.crs
 
 
 def get_features(src_fp, bidx=1):
+    from rasterio import features
     with rasterio.open(src_fp) as src:
-        features = rasterio.features.dataset_features(
+        features = features.dataset_features(
             src,
             bidx=bidx,
             sampling=1,
             band=True,
             as_mask=False,
             with_nodata=False,
             geographic=True,
@@ -608,19 +608,158 @@
         return gdf
 
 
 def set_transform(geo_box, width, height):
     return rasterio.transform.from_bounds(*geo_box, width, height)
 
 
-def transform_coords(x, y, src_crs, dst_crs):
-    transformer = Transformer.from_crs(src_crs, dst_crs, always_xy=True)
+def transform_coords(x, y, src_crs, dst_crs, **kwargs):
+    """Transform coordinates from one CRS to another.
+
+    Args:
+        x (float): The x coordinate.
+        y (float): The y coordinate.
+        src_crs (str): The source CRS, e.g., "EPSG:4326".
+        dst_crs (str): The destination CRS, e.g., "EPSG:3857".
+
+    Returns:
+        dict: The transformed coordinates in the format of (x, y)
+    """
+    transformer = pyproj.Transformer.from_crs(
+        src_crs, dst_crs, always_xy=True, **kwargs
+    )
     return transformer.transform(x, y)
 
 
+def vector_to_geojson(filename, output=None, **kwargs):
+    """Converts a vector file to a geojson file.
+
+    Args:
+        filename (str): The vector file path.
+        output (str, optional): The output geojson file path. Defaults to None.
+
+    Returns:
+        dict: The geojson dictionary.
+    """
+    gdf = gpd.read_file(filename, **kwargs)
+    if output is None:
+        return gdf.__geo_interface__
+    else:
+        gdf.to_file(output, driver="GeoJSON")
+
+
+def get_vector_crs(filename, **kwargs):
+    """Gets the CRS of a vector file.
+
+    Args:
+        filename (str): The vector file path.
+
+    Returns:
+        str: The CRS of the vector file.
+    """
+    gdf = gpd.read_file(filename, **kwargs)
+    epsg = gdf.crs.to_epsg()
+    if epsg is None:
+        return gdf.crs
+    else:
+        return f"EPSG:{epsg}"
+
+
+def geojson_to_coords(
+    geojson: str, src_crs: str = "epsg:4326", dst_crs: str = "epsg:4326"
+) -> list:
+    """Converts a geojson file or a dictionary of feature collection to a list of centroid coordinates.
+
+    Args:
+        geojson (str | dict): The geojson file path or a dictionary of feature collection.
+        src_crs (str, optional): The source CRS. Defaults to "epsg:4326".
+        dst_crs (str, optional): The destination CRS. Defaults to "epsg:4326".
+
+    Returns:
+        list: A list of centroid coordinates in the format of [[x1, y1], [x2, y2], ...]
+    """
+
+    import json
+    import warnings
+
+    warnings.filterwarnings("ignore")
+
+    if isinstance(geojson, dict):
+        geojson = json.dumps(geojson)
+    gdf = gpd.read_file(geojson, driver="GeoJSON")
+    centroids = gdf.geometry.centroid
+    centroid_list = [[point.x, point.y] for point in centroids]
+    if src_crs != dst_crs:
+        centroid_list = transform_coords(
+            [x[0] for x in centroid_list],
+            [x[1] for x in centroid_list],
+            src_crs,
+            dst_crs,
+        )
+        centroid_list = [[x, y] for x, y in zip(centroid_list[0], centroid_list[1])]
+    return centroid_list
+
+
+def coords_to_xy(
+    src_fp: str, coords: list, coord_crs: str = "epsg:4326", **kwargs
+) -> list:
+    """Converts a list of coordinates to pixel coordinates, i.e., (col, row) coordinates.
+
+    Args:
+        src_fp: The source raster file path.
+        coords: A list of coordinates in the format of [[x1, y1], [x2, y2], ...]
+        coord_crs: The coordinate CRS of the input coordinates. Defaults to "epsg:4326".
+        **kwargs: Additional keyword arguments to pass to rasterio.transform.rowcol.
+
+    Returns:
+        A list of pixel coordinates in the format of [[x1, y1], [x2, y2], ...]
+    """
+    if isinstance(coords, np.ndarray):
+        coords = coords.tolist()
+
+    xs, ys = zip(*coords)
+    with rasterio.open(src_fp) as src:
+        width = src.width
+        height = src.height
+        if coord_crs != src.crs:
+            xs, ys = transform_coords(xs, ys, coord_crs, src.crs, **kwargs)
+        rows, cols = rasterio.transform.rowcol(src.transform, xs, ys, **kwargs)
+    result = [[col, row] for col, row in zip(cols, rows)]
+
+    result = [
+        [x, y] for x, y in result if x >= 0 and y >= 0 and x < width and y < height
+    ]
+    if len(result) == 0:
+        print("No valid pixel coordinates found.")
+    elif len(result) < len(coords):
+        print("Some coordinates are out of the image boundary.")
+
+    return result
+
+
+def geojson_to_xy(
+    src_fp: str, geojson: str, coord_crs: str = "epsg:4326", **kwargs
+) -> list:
+    """Converts a geojson file or a dictionary of feature collection to a list of pixel coordinates.
+
+    Args:
+        src_fp: The source raster file path.
+        geojson: The geojson file path or a dictionary of feature collection.
+        coord_crs: The coordinate CRS of the input coordinates. Defaults to "epsg:4326".
+        **kwargs: Additional keyword arguments to pass to rasterio.transform.rowcol.
+
+    Returns:
+        A list of pixel coordinates in the format of [[x1, y1], [x2, y2], ...]
+    """
+    with rasterio.open(src_fp) as src:
+        src_crs = src.crs
+    coords = geojson_to_coords(geojson, coord_crs, src_crs)
+    return coords_to_xy(src_fp, coords, src_crs, **kwargs)
+
+
 def get_pixel_coords(src_fp, xs, ys):
     with rasterio.open(src_fp) as src:
         rows, cols = rasterio.transform.rowcol(src.transform, xs, ys)
         box = np.array([min(cols), min(rows), max(cols), max(rows)])
     return box
 
 
@@ -697,14 +836,18 @@
     src_fp,
     dst_fp,
     func,
     data_to_rgb=chw_to_hwc,
     sample_size=(512, 512),
     sample_resize=None,
     bound=128,
+    foreground=True,
+    erosion_kernel=(3, 3),
+    mask_multiplier=255,
+    **kwargs,
 ):
     with rasterio.open(src_fp) as src:
         profile = src.profile
 
         # Computer blocks
         rh, rw = profile["height"], profile["width"]
         sh, sw = sample_size
@@ -716,28 +859,37 @@
         sample_grid = calculate_sample_grid(
             raster_h=rh, raster_w=rw, sample_h=sh, sample_w=sw, bound=bound
         )
         # set 1 channel uint8 output
         profile["count"] = 1
         profile["dtype"] = "uint8"
 
+        if erosion_kernel is not None:
+            erosion_kernel = np.ones(erosion_kernel, np.uint8)
+
         with rasterio.open(dst_fp, "w", **profile) as dst:
             for b in tqdm(sample_grid):
                 # Read each tile from the source
                 r = read_block(src, **b)
                 # Extract the first 3 channels as RGB
                 uint8_rgb_in = data_to_rgb(r)
                 orig_size = uint8_rgb_in.shape[:2]
                 if resize_hw is not None:
                     uint8_rgb_in = cv2.resize(
                         uint8_rgb_in, resize_hw, interpolation=cv2.INTER_LINEAR
                     )
 
                 # Run the model, call the __call__ method of SamGeo class
-                uin8_out = func(uint8_rgb_in)
+                uin8_out = func(
+                    uint8_rgb_in,
+                    foreground=foreground,
+                    erosion_kernel=erosion_kernel,
+                    mask_multiplier=mask_multiplier,
+                    **kwargs,
+                )
 
                 if resize_hw is not None:
                     uin8_out = cv2.resize(
                         uin8_out, orig_size, interpolation=cv2.INTER_NEAREST
                     )
                 # Write the output to the destination
                 write_block(dst, uin8_out, **b)
@@ -785,14 +937,16 @@
         )
 
         result = cv2.imread(dst_fp)
     return result[..., 0]
 
 
 def tiff_to_shapes(tiff_path, simplify_tolerance=None):
+    from rasterio import features
+
     with rasterio.open(tiff_path) as src:
         band = src.read()
 
         mask = band != 0
         shapes = features.shapes(band, mask=mask, transform=src.transform)
     result = [shapely.geometry.shape(shape) for shape, _ in shapes]
     if simplify_tolerance is not None:
@@ -812,25 +966,26 @@
         return_image=True,
         quiet=False,
         **kwargs,
     )
     return image
 
 
-def tiff_to_vector(tiff_path, output, simplify_tolerance=None, **kwargs):
-    """Convert a tiff file to a gpkg file.
+def raster_to_vector(source, output, simplify_tolerance=None, **kwargs):
+    """Vectorize a raster dataset.
 
     Args:
-        tiff_path (str): The path to the tiff file.
+        source (str): The path to the tiff file.
         output (str): The path to the vector file.
         simplify_tolerance (float, optional): The maximum allowed geometry displacement.
             The higher this value, the smaller the number of vertices in the resulting geometry.
     """
+    from rasterio import features
 
-    with rasterio.open(tiff_path) as src:
+    with rasterio.open(source) as src:
         band = src.read()
 
         mask = band != 0
         shapes = features.shapes(band, mask=mask, transform=src.transform)
 
     fc = [
         {"geometry": shapely.geometry.shape(shape), "properties": {"value": value}}
@@ -842,60 +997,60 @@
 
     gdf = gpd.GeoDataFrame.from_features(fc)
     if src.crs is not None:
         gdf.set_crs(crs=src.crs, inplace=True)
     gdf.to_file(output, **kwargs)
 
 
-def tiff_to_gpkg(tiff_path, output, simplify_tolerance=None, **kwargs):
+def raster_to_gpkg(tiff_path, output, simplify_tolerance=None, **kwargs):
     """Convert a tiff file to a gpkg file.
 
     Args:
         tiff_path (str): The path to the tiff file.
         output (str): The path to the gpkg file.
         simplify_tolerance (float, optional): The maximum allowed geometry displacement.
             The higher this value, the smaller the number of vertices in the resulting geometry.
     """
 
     if not output.endswith(".gpkg"):
         output += ".gpkg"
 
-    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+    raster_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
 
 
-def tiff_to_shp(tiff_path, output, simplify_tolerance=None, **kwargs):
+def raster_to_shp(tiff_path, output, simplify_tolerance=None, **kwargs):
     """Convert a tiff file to a shapefile.
 
     Args:
         tiff_path (str): The path to the tiff file.
         output (str): The path to the shapefile.
         simplify_tolerance (float, optional): The maximum allowed geometry displacement.
             The higher this value, the smaller the number of vertices in the resulting geometry.
     """
 
     if not output.endswith(".shp"):
         output += ".shp"
 
-    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+    raster_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
 
 
-def tiff_to_geojson(tiff_path, output, simplify_tolerance=None, **kwargs):
+def raster_to_geojson(tiff_path, output, simplify_tolerance=None, **kwargs):
     """Convert a tiff file to a GeoJSON file.
 
     Args:
         tiff_path (str): The path to the tiff file.
         output (str): The path to the GeoJSON file.
         simplify_tolerance (float, optional): The maximum allowed geometry displacement.
             The higher this value, the smaller the number of vertices in the resulting geometry.
     """
 
     if not output.endswith(".geojson"):
         output += ".geojson"
 
-    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+    raster_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
 
 
 def get_xyz_dict(free_only=True):
     """Returns a dictionary of xyz services.
 
     Args:
         free_only (bool, optional): Whether to return only free xyz tile services that do not require an access token. Defaults to True.
@@ -1046,18 +1201,16 @@
 
     else:
         img = Image.fromarray(array)
         img.save(output, **kwargs)
 
 
 def show_image(
-    source, figsize=(20, 20), cmap=None, axis="off", fig_args={}, show_args={}, **kwargs
+    source, figsize=(12, 10), cmap=None, axis="off", fig_args={}, show_args={}, **kwargs
 ):
-    import matplotlib.pyplot as plt
-
     if isinstance(source, str):
         if source.startswith("http"):
             source = download_file(source)
 
         if not os.path.exists(source):
             raise ValueError(f"Input path {source} does not exist.")
 
@@ -1066,27 +1219,96 @@
 
     plt.figure(figsize=figsize, **fig_args)
     plt.imshow(source, cmap=cmap, **show_args)
     plt.axis(axis)
     plt.show(**kwargs)
 
 
+def show_mask(mask, random_color=False):
+    ax = plt.gca()
+    if random_color:
+        color = np.concatenate([np.random.random(3), np.array([0.6])], axis=0)
+    else:
+        color = np.array([30 / 255, 144 / 255, 255 / 255, 0.6])
+    h, w = mask.shape[-2:]
+    mask_image = mask.reshape(h, w, 1) * color.reshape(1, 1, -1)
+    ax.imshow(mask_image)
+
+
+def show_points(
+    image,
+    coords,
+    labels,
+    marker_size=375,
+    figsize=(12, 10),
+    axis="on",
+    title=None,
+    mask=None,
+    **kwargs,
+):
+    if isinstance(image, str):
+        if image.startswith("http"):
+            image = download_file(image)
+
+        if not os.path.exists(image):
+            raise ValueError(f"Input path {image} does not exist.")
+
+        image = cv2.imread(image)
+        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+
+    plt.figure(figsize=figsize)
+    plt.imshow(image)
+    ax = plt.gca()
+    pos_points = coords[labels == 1]
+    neg_points = coords[labels == 0]
+    ax.scatter(
+        pos_points[:, 0],
+        pos_points[:, 1],
+        color="green",
+        marker="*",
+        s=marker_size,
+        edgecolor="white",
+        linewidth=1.25,
+    )
+    ax.scatter(
+        neg_points[:, 0],
+        neg_points[:, 1],
+        color="red",
+        marker="*",
+        s=marker_size,
+        edgecolor="white",
+        linewidth=1.25,
+    )
+    if title is not None:
+        plt.title(title)
+    plt.axis(axis)
+    plt.show()
+
+
+def show_box(image, box, ax):
+    ax = plt.gca()
+    x0, y0 = box[0], box[1]
+    w, h = box[2] - box[0], box[3] - box[1]
+    ax.add_patch(
+        plt.Rectangle((x0, y0), w, h, edgecolor="green", facecolor=(0, 0, 0, 0), lw=2)
+    )
+
+
 def overlay_images(
     image1,
     image2,
     opacity=0.5,
     backend="TkAgg",
     height_ratios=[10, 1],
     show_args1={},
     show_args2={},
 ):
     import sys
     import matplotlib
     import matplotlib.widgets as mpwidgets
-    import matplotlib.pyplot as plt
 
     if "google.colab" in sys.modules:
         backend = "inline"
         print(
             "The TkAgg backend is not supported in Google Colab. The overlay_images function will not work on Colab."
         )
         return
@@ -1154,16 +1376,14 @@
         axis (str, optional): The axis of the figure. Defaults to "off".
         **kwargs: Additional keyword arguments to pass to the cv2.addWeighted() function.
 
     Returns:
         numpy.ndarray: The blended image as a NumPy array.
     """
     # Resize the images to have the same dimensions
-    import matplotlib.pyplot as plt
-
     if isinstance(img1, str):
         if img1.startswith("http"):
             img1 = download_file(img1)
 
         if not os.path.exists(img1):
             raise ValueError(f"Input path {img1} does not exist.")
 
@@ -1241,7 +1461,176 @@
             shutil.rmtree(pkg_dir)
             os.remove(filename)
 
         print("Package updated successfully.")
 
     except Exception as e:
         raise Exception(e)
+
+
+def sam_map_gui(sam, basemap="SATELLITE", repeat_mode=True, **kwargs):
+    try:
+        import leafmap
+        import ipyleaflet
+        import ipyevents
+        import ipywidgets as widgets
+    except ImportError:
+        raise ImportError(
+            "The sam_map function requires the leafmap package. Please install it first."
+        )
+
+    m = leafmap.Map(repeat_mode=repeat_mode, **kwargs)
+    m.add_basemap(basemap, show=False)
+    m.add_raster(sam.image, layer_name="Image")
+
+    widget_width = "100px"
+    padding = "0px 0px 0px 5px"  # upper, right, bottom, left
+    style = {"description_width": "initial"}
+
+    toolbar_button = widgets.ToggleButton(
+        value=True,
+        tooltip="Toolbar",
+        icon="gear",
+        layout=widgets.Layout(width="28px", height="28px", padding="0px 0px 0px 4px"),
+    )
+
+    close_button = widgets.ToggleButton(
+        value=False,
+        tooltip="Close the tool",
+        icon="times",
+        button_style="primary",
+        layout=widgets.Layout(height="28px", width="28px", padding="0px 0px 0px 4px"),
+    )
+
+    segment_button = widgets.ToggleButton(
+        description="Segment", value=False, button_style="primary"
+    )
+    reset_button = widgets.ToggleButton(
+        description="Reset", value=False, button_style="primary"
+    )
+    segment_button.layout.width = widget_width
+    reset_button.layout.width = widget_width
+
+    buttons = widgets.VBox([segment_button, reset_button])
+
+    opacity_slider = widgets.FloatSlider(
+        min=0,
+        max=1,
+        value=0.5,
+        readout=False,
+        continuous_update=True,
+        layout=widgets.Layout(width="95px"),
+        style=style,
+    )
+
+    def opacity_changed(change):
+        if change["new"]:
+            mask_layer = m.find_layer("Masks")
+            if mask_layer is not None:
+                mask_layer.interact(opacity=opacity_slider.value)
+
+    opacity_slider.observe(opacity_changed, "value")
+
+    output = widgets.Output(layout=widgets.Layout(width=widget_width, padding=padding))
+
+    toolbar_header = widgets.HBox()
+    toolbar_header.children = [close_button, toolbar_button]
+    toolbar_footer = widgets.VBox()
+    toolbar_footer.children = [
+        buttons,
+        opacity_slider,
+        output,
+    ]
+    toolbar_widget = widgets.VBox()
+    toolbar_widget.children = [toolbar_header, toolbar_footer]
+
+    toolbar_event = ipyevents.Event(
+        source=toolbar_widget, watched_events=["mouseenter", "mouseleave"]
+    )
+
+    def handle_toolbar_event(event):
+        if event["type"] == "mouseenter":
+            toolbar_widget.children = [toolbar_header, toolbar_footer]
+        elif event["type"] == "mouseleave":
+            if not toolbar_button.value:
+                toolbar_widget.children = [toolbar_button]
+                toolbar_button.value = False
+                close_button.value = False
+
+    toolbar_event.on_dom_event(handle_toolbar_event)
+
+    def toolbar_btn_click(change):
+        if change["new"]:
+            close_button.value = False
+            toolbar_widget.children = [toolbar_header, toolbar_footer]
+        else:
+            if not close_button.value:
+                toolbar_widget.children = [toolbar_button]
+
+    toolbar_button.observe(toolbar_btn_click, "value")
+
+    def close_btn_click(change):
+        if change["new"]:
+            toolbar_button.value = False
+            if m.toolbar_control in m.controls:
+                m.remove_control(m.toolbar_control)
+            toolbar_widget.close()
+
+    close_button.observe(close_btn_click, "value")
+
+    def segment_button_click(change):
+        if change["new"]:
+            reset_button.value = False
+            with output:
+                output.clear_output()
+                print("Segmenting...")
+                try:
+                    if m.user_rois is not None:
+                        filename = f"masks_{random_string()}.tif"
+                        sam.predict(point_coords=m.user_rois,  point_crs='EPSG:4326', output=filename)
+                        if m.find_layer("Masks") is not None:
+                            m.remove_layer(m.find_layer("Masks"))
+                        m.add_raster(filename, nodata=0, cmap='Blues', opacity=opacity_slider.value, layer_name="Masks", zoom_to_layer=False)
+                    output.clear_output()
+                    segment_button.value = False
+                    sam.prediction_fp = filename
+                except Exception as e:
+                    print(e)
+
+    segment_button.observe(segment_button_click, "value")
+
+    def reset_button_click(change):
+        if change["new"]:
+            segment_button.value = False
+            reset_button.value = False
+            opacity_slider.value = 0.5
+            output.clear_output()
+            m.remove_layer(m.find_layer("Masks"))
+            m.clear_drawings()
+            os.remove(sam.prediction_fp)
+
+    reset_button.observe(reset_button_click, "value")
+
+    toolbar_control = ipyleaflet.WidgetControl(
+        widget=toolbar_widget, position="topright"
+    )
+    m.add_control(toolbar_control)
+    m.toolbar_control = toolbar_control
+
+    return m
+
+
+def random_string(string_length=6):
+    """Generates a random string of fixed length.
+
+    Args:
+        string_length (int, optional): Fixed length. Defaults to 3.
+
+    Returns:
+        str: A random string
+    """
+    import random
+    import string
+
+    # random.seed(1001)
+    letters = string.ascii_lowercase
+    return "".join(random.choice(letters) for i in range(string_length))
```

### Comparing `segment-geospatial-0.4.0/samgeo/samgeo.py` & `segment-geospatial-0.5.0/samgeo/samgeo.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,50 +3,43 @@
 """
 
 import os
 import cv2
 import torch
 import numpy as np
 from segment_anything import sam_model_registry, SamAutomaticMaskGenerator, SamPredictor
-from segment_anything.utils.transforms import ResizeLongestSide
 
 from .common import *
 
 
 class SamGeo:
     """The main class for segmenting geospatial data with the Segment Anything Model (SAM). See
-    https://github.com/facebookresearch/segment-anything
+    https://github.com/facebookresearch/segment-anything for details.
     """
 
     def __init__(
         self,
         model_type="vit_h",
         checkpoint="sam_vit_h_4b8939.pth",
         automatic=True,
         device=None,
-        erosion_kernel=None,
-        mask_multiplier=255,
         sam_kwargs=None,
     ):
         """Initialize the class.
 
         Args:
             model_type (str, optional): The model type. It can be one of the following: vit_h, vit_l, vit_b.
                 Defaults to 'vit_h'. See https://bit.ly/3VrpxUh for more details.
-            checkpoint (str, optional): The path to the checkpoint. It can be one of the following:
+            checkpoint (str, optional): The path to the model checkpoint. It can be one of the following:
                 sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
                 Defaults to "sam_vit_h_4b8939.pth". See https://bit.ly/3VrpxUh for more details.
             automatic (bool, optional): Whether to use the automatic mask generator or input prompts. Defaults to True.
                 The automatic mask generator will segment the entire image, while the input prompts will segment selected objects.
             device (str, optional): The device to use. It can be one of the following: cpu, cuda.
                 Defaults to None, which will use cuda if available.
-            erosion_kernel (tuple, optional): The erosion kernel for filtering object masks and extract borders.
-                Set to None to disable it. Defaults to (3, 3).
-            mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
-                You can use this parameter to scale the mask to a larger range, for example [0, 255]. Defaults to 255.
             sam_kwargs (dict, optional): Optional arguments for fine-tuning the SAM model. Defaults to None.
                 The available arguments with default values are listed below. See https://bit.ly/410RV0v for more details.
 
                 points_per_side: Optional[int] = 32,
                 points_per_batch: int = 64,
                 pred_iou_thresh: float = 0.88,
                 stability_score_thresh: float = 0.95,
@@ -65,73 +58,91 @@
         if not os.path.exists(checkpoint):
             print(f"Checkpoint {checkpoint} does not exist.")
             download_checkpoint(output=checkpoint)
 
         # Use cuda if available
         if device is None:
             device = "cuda" if torch.cuda.is_available() else "cpu"
+            if device == "cuda":
+                torch.cuda.empty_cache()
 
         self.checkpoint = checkpoint
         self.model_type = model_type
         self.device = device
         self.sam_kwargs = sam_kwargs  # Optional arguments for fine-tuning the SAM model
         self.source = None  # Store the input image path
         self.image = None  # Store the input image as a numpy array
         # Store the masks as a list of dictionaries. Each mask is a dictionary
         # containing segmentation, area, bbox, predicted_iou, point_coords, stability_score, and crop_box
         self.masks = None
         self.objects = None  # Store the mask objects as a numpy array
         # Store the annotations (objects with random color) as a numpy array.
         self.annotations = None
 
+        # Store the predicted masks, iou_predictions, and low_res_masks
+        self.prediction = None
+        self.scores = None
+        self.logits = None
+
         # Build the SAM model
         self.sam = sam_model_registry[self.model_type](checkpoint=self.checkpoint)
         self.sam.to(device=self.device)
         # Use optional arguments for fine-tuning the SAM model
         sam_kwargs = self.sam_kwargs if self.sam_kwargs is not None else {}
 
         if automatic:
             # Segment the entire image using the automatic mask generator
             self.mask_generator = SamAutomaticMaskGenerator(self.sam, **sam_kwargs)
         else:
             # Segment selected objects using input prompts
             self.predictor = SamPredictor(self.sam, **sam_kwargs)
 
-        # Apply the erosion filter to the mask to extract borders
-        self.erosion_kernel = erosion_kernel
-        if self.erosion_kernel is not None:
-            self.erosion_kernel = np.ones(erosion_kernel, np.uint8)
-
-        # Rescale the binary mask to a larger range, for example, from [0, 1] to [0, 255].
-        self.mask_multiplier = mask_multiplier
+    def __call__(
+        self,
+        image,
+        foreground=True,
+        erosion_kernel=(3, 3),
+        mask_multiplier=255,
+        **kwargs,
+    ):
+        """Generate masks for the input tile. This function originates from the segment-anything-eo repository.
+            See https://bit.ly/41pwiHw
 
-    def __call__(self, image):
-        # Segment each image tile
+        Args:
+            image (np.ndarray): The input image as a numpy array.
+            foreground (bool, optional): Whether to generate the foreground mask. Defaults to True.
+            erosion_kernel (tuple, optional): The erosion kernel for filtering object masks and extract borders. Defaults to (3, 3).
+            mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
+                You can use this parameter to scale the mask to a larger range, for example [0, 255]. Defaults to 255.
+        """
         h, w, _ = image.shape
 
         masks = self.mask_generator.generate(image)
 
-        resulting_mask = np.ones((h, w), dtype=np.uint8)
+        if foreground:  # Extract foreground objects only
+            resulting_mask = np.zeros((h, w), dtype=np.uint8)
+        else:
+            resulting_mask = np.ones((h, w), dtype=np.uint8)
         resulting_borders = np.zeros((h, w), dtype=np.uint8)
 
         for m in masks:
             mask = (m["segmentation"] > 0).astype(np.uint8)
             resulting_mask += mask
 
             # Apply erosion to the mask
-            if self.erosion_kernel is not None:
-                mask_erode = cv2.erode(mask, self.erosion_kernel, iterations=1)
+            if erosion_kernel is not None:
+                mask_erode = cv2.erode(mask, erosion_kernel, iterations=1)
                 mask_erode = (mask_erode > 0).astype(np.uint8)
                 edge_mask = mask - mask_erode
                 resulting_borders += edge_mask
 
         resulting_mask = (resulting_mask > 0).astype(np.uint8)
         resulting_borders = (resulting_borders > 0).astype(np.uint8)
         resulting_mask_with_borders = resulting_mask - resulting_borders
-        return resulting_mask_with_borders * self.mask_multiplier
+        return resulting_mask_with_borders * mask_multiplier
 
     def generate(
         self,
         source,
         output=None,
         foreground=True,
         batch=False,
@@ -161,15 +172,23 @@
             if source.startswith("http"):
                 source = download_file(source)
 
             if not os.path.exists(source):
                 raise ValueError(f"Input path {source} does not exist.")
 
             if batch:  # Subdivide the image into tiles and segment each tile
-                return tiff_to_tiff(source, output, self, **kwargs)
+                return tiff_to_tiff(
+                    source,
+                    output,
+                    self,
+                    foreground=foreground,
+                    erosion_kernel=erosion_kernel,
+                    mask_multiplier=mask_multiplier,
+                    **kwargs,
+                )
 
             image = cv2.imread(source)
         elif isinstance(source, np.ndarray):
             image = source
         else:
             raise ValueError("Input source must be either a path or a numpy array.")
 
@@ -274,14 +293,15 @@
         """Show the binary mask or the mask of objects with unique values.
 
         Args:
             figsize (tuple, optional): The figure size. Defaults to (12, 10).
             cmap (str, optional): The colormap. Defaults to "binary_r".
             axis (str, optional): Whether to show the axis. Defaults to "off".
             foreground (bool, optional): Whether to show the foreground mask only. Defaults to True.
+            **kwargs: Other arguments for save_masks().
         """
 
         import matplotlib.pyplot as plt
 
         if self.objects is None:
             self.save_masks(foreground=foreground, **kwargs)
 
@@ -345,26 +365,165 @@
 
         self.annotations = (img[:, :, 0:3] * 255).astype(np.uint8)
 
         if output is not None:
             array = blend_images(self.annotations, self.image, alpha=alpha, show=False)
             array_to_image(array, output, self.source)
 
-    def predict(self, in_path, out_path, prompts, image_format="RGB", **kwargs):
-        """Segment the input image and save the result to the output path.
+    def set_image(self, image, image_format="RGB"):
+        """Set the input image as a numpy array.
+
+        Args:
+            image (np.ndarray): The input image as a numpy array.
+            image_format (str, optional): The image format, can be RGB or BGR. Defaults to "RGB".
+        """
+        if isinstance(image, str):
+            if image.startswith("http"):
+                image = download_file(image)
+
+            if not os.path.exists(image):
+                raise ValueError(f"Input path {image} does not exist.")
+
+            self.image = image
+
+            image = cv2.imread(image)
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        elif isinstance(image, np.ndarray):
+            pass
+        else:
+            raise ValueError("Input image must be either a path or a numpy array.")
+
+        self.predictor.set_image(image, image_format=image_format)
+
+    def save_prediction(
+        self,
+        output,
+        index=None,
+        mask_multiplier=255,
+        dtype=np.float32,
+        vector=None,
+        simplify_tolerance=None,
+        **kwargs,
+    ):
+        """Save the predicted mask to the output path.
 
         Args:
-            in_path (str): The path to the input image.
-            out_path (str): The path to the output image.
-            prompts (list): The prompts to use.
+            output (str): The path to the output image.
+            index (int, optional): The index of the mask to save. Defaults to None,
+                which will save the mask with the highest score.
+            mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
+            vector (str, optional): The path to the output vector file. Defaults to None.
+            dtype (np.dtype, optional): The data type of the output image. Defaults to np.float32.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
+
         """
+        if self.scores is None:
+            raise ValueError("No predictions found. Please run predict() first.")
+
+        if index is None:
+            index = self.scores.argmax(axis=0)
+
+        array = self.masks[index] * mask_multiplier
+        self.prediction = array
+        array_to_image(array, output, self.image, dtype=dtype, **kwargs)
+
+        if vector is not None:
+            raster_to_vector(output, vector, simplify_tolerance=simplify_tolerance)
+
+    def predict(
+        self,
+        point_coords=None,
+        point_labels=None,
+        box=None,
+        point_crs=None,
+        mask_input=None,
+        multimask_output=True,
+        return_logits=False,
+        output=None,
+        index=None,
+        mask_multiplier=255,
+        dtype=np.float32,
+        return_results=False,
+        **kwargs,
+    ):
+        """Predict masks for the given input prompts, using the currently set image.
+
+        Args:
+            point_coords (str | dict | list | np.ndarray, optional): A Nx2 array of point prompts to the
+                model. Each point is in (X,Y) in pixels. It can be a path to a vector file, a GeoJSON
+                dictionary, a list of coordinates [lon, lat], or a numpy array. Defaults to None.
+            point_labels (list | int | np.ndarray, optional): A length N array of labels for the
+                point prompts. 1 indicates a foreground point and 0 indicates a background point.
+            point_crs (str, optional): The coordinate reference system (CRS) of the point prompts.
+            box (list | np.ndarray, optional): A length 4 array given a box prompt to the
+                model, in XYXY format.
+            mask_input (np.ndarray, optional): A low resolution mask input to the model, typically
+                coming from a previous prediction iteration. Has form 1xHxW, where for SAM, H=W=256.
+                multimask_output (bool, optional): If true, the model will return three masks.
+                For ambiguous input prompts (such as a single click), this will often
+                produce better masks than a single prediction. If only a single
+                mask is needed, the model's predicted quality score can be used
+                to select the best mask. For non-ambiguous prompts, such as multiple
+                input prompts, multimask_output=False can give better results.
+            return_logits (bool, optional): If true, returns un-thresholded masks logits
+                instead of a binary mask.
+            output (str, optional): The path to the output image. Defaults to None.
+            index (index, optional): The index of the mask to save. Defaults to None,
+                which will save the mask with the highest score.
+            mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
+            dtype (np.dtype, optional): The data type of the output image. Defaults to np.float32.
+            return_results (bool, optional): Whether to return the predicted masks, scores, and logits. Defaults to False.
+
+        """
+
+        if isinstance(point_coords, str):
+            point_coords = vector_to_geojson(point_coords)
+
+        if isinstance(point_coords, dict):
+            point_coords = geojson_to_coords(point_coords)
+
+        if point_crs is not None:
+            point_coords = coords_to_xy(self.image, point_coords, point_crs)
+
+        if isinstance(point_coords, list):
+            point_coords = np.array(point_coords)
+
+        if point_labels is None:
+            point_labels = [1] * len(point_coords)
+        elif isinstance(point_labels, int):
+            point_labels = [point_labels] * len(point_coords)
+
+        if isinstance(point_labels, list):
+            if len(point_labels) != len(point_coords):
+                if len(point_labels) == 1:
+                    point_labels = point_labels * len(point_coords)
+                else:
+                    raise ValueError(
+                        "The length of point_labels must be equal to the length of point_coords."
+                    )
+            point_labels = np.array(point_labels)
+
         predictor = self.predictor
-        predictor.set_image(in_path, image_format=image_format)
-        masks, _, _ = predictor.predict(prompts, **kwargs)
-        return masks
+        masks, scores, logits = predictor.predict(
+            point_coords, point_labels, box, mask_input, multimask_output, return_logits
+        )
+        self.masks = masks
+        self.scores = scores
+        self.logits = logits
+
+        if output is not None:
+            self.save_prediction(output, index, mask_multiplier, dtype, **kwargs)
+
+        if return_results:
+            return masks, scores, logits
+
+    def show_map(self, **kwargs):
+
+        return sam_map_gui(self, **kwargs)
 
     def image_to_image(self, image, **kwargs):
         return image_to_image(image, self, **kwargs)
 
     def download_tms_as_tiff(self, source, pt1, pt2, zoom, dist):
         image = draw_tile(source, pt1[0], pt1[1], pt2[0], pt2[1], zoom, dist)
         return image
@@ -375,62 +534,68 @@
         Args:
             tiff_path (str): The path to the tiff file.
             output (str): The path to the vector file.
             simplify_tolerance (float, optional): The maximum allowed geometry displacement.
                 The higher this value, the smaller the number of vertices in the resulting geometry.
         """
 
-        tiff_to_vector(
+        raster_to_vector(
             tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs
         )
 
     def tiff_to_gpkg(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a gpkg file.
 
         Args:
             tiff_path (str): The path to the tiff file.
             output (str): The path to the gpkg file.
             simplify_tolerance (float, optional): The maximum allowed geometry displacement.
                 The higher this value, the smaller the number of vertices in the resulting geometry.
         """
 
-        tiff_to_gpkg(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+        raster_to_gpkg(
+            tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs
+        )
 
     def tiff_to_shp(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a shapefile.
 
         Args:
             tiff_path (str): The path to the tiff file.
             output (str): The path to the shapefile.
             simplify_tolerance (float, optional): The maximum allowed geometry displacement.
                 The higher this value, the smaller the number of vertices in the resulting geometry.
         """
 
-        tiff_to_shp(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+        raster_to_shp(
+            tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs
+        )
 
     def tiff_to_geojson(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a GeoJSON file.
 
         Args:
             tiff_path (str): The path to the tiff file.
             output (str): The path to the GeoJSON file.
             simplify_tolerance (float, optional): The maximum allowed geometry displacement.
                 The higher this value, the smaller the number of vertices in the resulting geometry.
         """
 
-        tiff_to_geojson(
+        raster_to_geojson(
             tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs
         )
 
 
 class SamGeoPredictor(SamPredictor):
     def __init__(
         self,
         sam_model,
     ):
+        from segment_anything.utils.transforms import ResizeLongestSide
+
         self.model = sam_model
         self.transform = ResizeLongestSide(sam_model.image_encoder.img_size)
 
     def set_image(self, image):
         super(SamGeoPredictor, self).set_image(image)
 
     def predict(
```

### Comparing `segment-geospatial-0.4.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.5.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.4.0
+Version: 0.5.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: all
 License-File: LICENSE
 
 # segment-geospatial
 
 [![image](https://studiolab.sagemaker.aws/studiolab.svg)](https://studiolab.sagemaker.aws/import/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
 [![image](https://img.shields.io/badge/Open-Planetary%20Computer-black?style=flat&logo=microsoft)](https://pccompute.westeurope.cloudapp.azure.com/compute/hub/user-redirect/git-pull?repo=https://github.com/opengeos/segment-geospatial&urlpath=lab/tree/segment-geospatial/docs/examples/satellite.ipynb&branch=main)
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/segment-geospatial/blob/main/docs/examples/satellite.ipynb)
@@ -41,21 +42,32 @@
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
+-   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
 
+-   Interactive segmentation with input prompts
+
+![](https://i.imgur.com/GV7Rzxt.gif)
+
+## Tutorials
+
+Video tutorials are available on my [YouTube Channel](https://youtube.com/@giswqs).
+
+[![Alt text](https://img.youtube.com/vi/YHA_-QMB8_U/0.jpg)](https://www.youtube.com/playlist?list=PLAxJ4-o7ZoPcrg5RnZjkB_KY6tv96WO2h)
+
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
```

