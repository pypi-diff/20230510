# Comparing `tmp/fakemap-0.0.5.tar.gz` & `tmp/fakemap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakemap-0.0.5.tar", last modified: Fri Apr 28 00:47:50 2023, max compression
+gzip compressed data, was "fakemap-0.0.6.tar", last modified: Tue May  9 23:12:28 2023, max compression
```

## Comparing `fakemap-0.0.5.tar` & `fakemap-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 00:47:39.000000 fakemap-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 00:47:39.000000 fakemap-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-28 00:47:50.508988 fakemap-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-28 00:47:39.000000 fakemap-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/fakemap/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/fakemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-28 00:47:39.000000 fakemap-0.0.5/fakemap/foliummap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:50.508988 fakemap-0.0.5/fakemap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 00:47:50.000000 fakemap-0.0.5/fakemap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 00:47:39.000000 fakemap-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 00:47:50.508988 fakemap-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-28 00:47:39.000000 fakemap-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:12:28.666411 fakemap-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-09 23:12:17.000000 fakemap-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 23:12:17.000000 fakemap-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-09 23:12:28.666411 fakemap-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-09 23:12:17.000000 fakemap-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:12:28.666411 fakemap-0.0.6/fakemap/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 23:12:17.000000 fakemap-0.0.6/fakemap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-05-09 23:12:17.000000 fakemap-0.0.6/fakemap/fakemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-09 23:12:17.000000 fakemap-0.0.6/fakemap/foliummap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:12:28.666411 fakemap-0.0.6/fakemap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 23:12:28.000000 fakemap-0.0.6/fakemap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 23:12:17.000000 fakemap-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-09 23:12:28.670410 fakemap-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-09 23:12:17.000000 fakemap-0.0.6/setup.py
```

### Comparing `fakemap-0.0.5/LICENSE` & `fakemap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.5/fakemap/fakemap.py` & `fakemap-0.0.6/fakemap/fakemap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Main module."""
 
 import random
 import ipyleaflet
-
+import rasterio
+import matplotlib
 class Map(ipyleaflet.Map):
 
     def __init__(self, center=[20,0], **kwargs) -> None:
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
         
         super().__init__(center = center, **kwargs)
@@ -350,18 +351,119 @@
                 toolbar.children = [widgets.HBox([close_button, toolbar_button]), grid]
             else:
                 toolbar.children = [toolbar_button]
                 
         toolbar_button.observe(toolbar_click, "value")
         toolbar_ctrl = ipyleaflet.WidgetControl(widget=toolbar, position=position)
 
-        self.add_control(toolbar_ctrl)    
+        self.add_control(toolbar_ctrl)  
 
+import rasterio
+import matplotlib.pyplot as plt
 
-        
+def view_satellite_bands(filename):
+    """Display images of the satellite bands
+
+    Args:
+        filename (str): the path to the image
+    """
+    with rasterio.open(filename) as dataset:
+        # loop through each band and plot separately
+        for i in range(1, dataset.count+1):
+            band = dataset.read(i)
+            plt.imshow(band)
+            plt.title("Band {}".format(i))
+            plt.show()  
+
+
+
+
+import rasterio
+import geopandas as gpd
+import matplotlib.pyplot as plt
+
+def plot_pixel_spectral_profile(geotiff_path, pixel_x, pixel_y):
+    """_summary_
+
+    Args:
+        geotiff_path (str): path to the image
+        pixel_x (int): X location of pixel 
+        pixel_y (int): y location of pixel
+    """
+    # Open the geotiff file in read mode
+    src = rasterio.open(geotiff_path)
+
+    # Read the pixel values and geometry using the pixel's location
+    pixel_values = src.read()[:, pixel_y, pixel_x]
+    pixel_geometry = src.transform * (pixel_x, pixel_y)
+
+    # Plot the spectral profile
+    fig, ax = plt.subplots()
+    ax.plot(src.indexes, pixel_values)
+    ax.set_xlabel('Band Index')
+    ax.set_ylabel('Pixel Reflectance')
+    ax.set_title('Pixel Spectral Profile')
+    plt.show()
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+def read_band(src, band):
+    """Reads the data from a band in a rasterio dataset
+
+    Args:
+        src (rasterio DatasetReader): the rasterio dataset
+        band (int): the band number
+
+    Returns:
+        data (numpy array): the data from the selected band
+        band (int): the band number
+    """
+    data = src.read(band)
+    return data, band
+
+
+import rasterio
+
+def print_geotiff_metadata(filename):
+    """Displays available metadata for the image 
+
+    Args:
+        filename (str): path to the image
+    """
+    with rasterio.open(filename) as dataset:
+        print(f"Metadata for GeoTIFF file: {filename}")
+        print(f"Width: {dataset.width}")
+        print(f"Height: {dataset.height}")
+        print(f"Number of bands: {dataset.count}")
+        print(f"Data type: {dataset.dtypes[0]}")
+        print(f"Coordinate reference system: {dataset.crs}")
+        print(f"Transform: \n{dataset.transform}")
+        print(f"Bounds: {dataset.bounds}")
+        print(f"Metadata: {dataset.meta}")
+
+
+    
 
 
 
 
 # Generate random latitude and longitude coordinates
 def Generate_random_location():
     "Generates a Random Latitude and Longitude "
```

### Comparing `fakemap-0.0.5/fakemap/foliummap.py` & `fakemap-0.0.6/fakemap/foliummap.py`

 * *Files identical despite different names*

### Comparing `fakemap-0.0.5/setup.py` & `fakemap-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='fakemap',
     name='fakemap',
     packages=find_packages(include=['fakemap', 'fakemap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MattAGUT/fakemap',
-    version='0.0.5',
+    version='0.0.6',
     zip_safe=False,
 )
```

