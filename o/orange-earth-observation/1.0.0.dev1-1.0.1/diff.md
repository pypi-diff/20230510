# Comparing `tmp/orange-earth-observation-1.0.0.dev1.tar.gz` & `tmp/orange-earth-observation-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-earth-observation-1.0.0.dev1.tar", last modified: Fri Mar 24 14:29:03 2023, max compression
+gzip compressed data, was "orange-earth-observation-1.0.1.tar", last modified: Wed May 10 16:14:38 2023, max compression
```

## Comparing `orange-earth-observation-1.0.0.dev1.tar` & `orange-earth-observation-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.045200 orange-earth-observation-1.0.0.dev1/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5513 2023-03-24 14:29:03.045200 orange-earth-observation-1.0.0.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5001 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.013200 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5513 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1729 2023-03-24 14:29:03.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-24 14:29:02.000000 orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.009200 orange-earth-observation-1.0.0.dev1/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.045200 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-03-24 14:29:03.045200 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.029200 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19663 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/cloud_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/crop_image.py
--rw-rw-rw-   0 root         (0) root         (0)    10887 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/histogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 14:29:03.041200 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/catalog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/cloud.svg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/crop.svg
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/histogram.svg
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/load.svg
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/mosaic.svg
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/nuts.svg
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/projection.svg
--rw-rw-rw-   0 root         (0) root         (0)     2492 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/view.svg
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/load_image.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/mosaic_image.py
--rw-rw-rw-   0 root         (0) root         (0)     7523 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/nuts_shape.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/reproject_image.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4255 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/view_image.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-03-24 14:10:52.000000 orange-earth-observation-1.0.0.dev1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-03-24 14:29:03.045200 orange-earth-observation-1.0.0.dev1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-03-24 13:41:55.000000 orange-earth-observation-1.0.0.dev1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5739 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.562636 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-10 16:14:38.000000 orange-earth-observation-1.0.1/orange_earth_observation.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.558636 orange-earth-observation-1.0.1/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/orangecontrib/earth_observation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/orangecontrib/earth_observation/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19663 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/cloud_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/crop_image.py
+-rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/histogram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/catalog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/cloud.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/crop.svg
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/histogram.svg
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/load.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/mosaic.svg
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/nuts.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/projection.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/view.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/load_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/mosaic_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/nuts_shape.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/reproject_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4255 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/view_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-05-10 16:14:38.566636 orange-earth-observation-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.1/versioneer.py
```

### Comparing `orange-earth-observation-1.0.0.dev1/PKG-INFO` & `orange-earth-observation-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,40 @@
-Metadata-Version: 2.1
-Name: orange-earth-observation
-Version: 1.0.0.dev1
-Summary: Add-on containing widgets for earth observation data operations
-Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
-Author: GAEL Systems
-Author-email: drb-python@gael.fr
-License: LGPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 Orange3 Earth Observation Add-on
 ======================
 
 This is an add-on for [Orange3](https://orangedatamining.com/). Add-on can extend Orange either 
 in scripting or GUI part, or in both. Register it with Orange and add a new workflow with some 
 of these widget to example tutorials.
 
-Installation
-------------
-
-To install the add-on from source run
-
-    pip install .
-
-Usage
------
-
-After the installation, widgets from this add-on are registered with Orange. To run Orange from the terminal,
-use
-
-    orange-canvas
-
+## Installation
+_Orange3_ and the _EO_ Addon must be installed in the same
+_Python_ environment.
+
+### Orange 3
+```shell
+pip install pyQt5 PyQtWebEngine
+pip install orange3
+```
+
+### Earth Observation Addon
+```shell
+pip install orange-earth-observation
+```
+
+## Usage
+Orange3 can be run using the following command:
+```shell
+orange-canvas
+```
 or
-
-    python -m Orange.canvas
-
-New widgets appears in the toolbox bar under the section Earth Observation.
-
-![screenshot](screenshots/category_EO.png)
+```shell
+python -m orange.canvas
+```
+New widgets should appear in the toolbox bar under the __Earth Observation__
+section.
 
 Widgets Description
 -----
 
 **ODM** (_Orange Data Mining_) is an open source machine learning and data visualization tool.
 It allows to build data analysis workflows visually, with a large, diverse toolbox.
 
@@ -68,75 +58,75 @@
 EODataCatalog Widget has a list of multi-option boxes to filter for products by **Mission**, **Platform**, **Type**, 
 **Sensor**, and a slider to define the **Cloud Cover** maximum value, the filter is passed through `ODataQueryPredicate`. 
 
 A `DrbNode` is retrieved, and can be passed through the output to be used by other ODM widgets, the product corresponding 
 can also be downloaded to local file.
 
 
-![](screenshots/Catalog.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Catalog.png)
 
 ## EONutsShape Widget
 
 EONutsShape Widget is used to crop Sentinel 2 TCI (True Color Image), remove parts not part of NUTS shape. 
 It takes a `DrbNode` as input, needs a file in .shp format containing polygons shapes corresponding to NUTS Region. 
 The output is a `DrbImageBaseNode` of the TC Image in selected NUTS Region. 
 
 
-![](screenshots/Nuts.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Nuts.png)
 
 ## EOMosaicImage Widget
 
 EOMosaicImage Widget is used to assemble image parts when possible, creating a mosaic image, corresponding to a predefined NUTS Region. 
 It takes a list of `DrbImageBaseNode` as input, all inputs need to be in same CRS and NUTS region. 
 The output is a `DrbImageBaseNode` of the assembled TC Image. 
 
-![](screenshots/Mosaic.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Mosaic.png)
 
 ## EOReprojectImage Widget
 
 EOReprojectImage Widget is used to reproject an image from one CRS to another. 
 It takes a `DrbImageBaseNode` as input and outputs the same.
 
-![](screenshots/Projection.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Projection.png)
 
 ## EOCloudMask Widget
 
 EOCloudMask Widget is used to mask Sentinel 2 TCI (True Color Image), remove pixels representing clouds, 
 shadows, water, snow or ice.
 It takes a `DrbNode` as input, needs the SCL band containing the mask information which can be found 
 in the same S2 product. The output is a `DrbImageBaseNode` of the TC Image with selected mask applied on.  
 
-![](screenshots/Cloud.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Cloud.png)
 
 ## EOHistogram Widget
 
 EOHistogram Widget is used for histogram visualisation, basic and adaptive histogram equalization.
 It takes a `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` after histogram equalization are done. 
 It might need to specify the **Clip Limit** which is used by the algorithm to apply adaptive equalization.
 EOHistogram Widget can also take a list of `DrbImageBaseNode` as input, in order to perform a histogram matching 
 after specifying the reference image. 
 
-![](screenshots/Histogram.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Histogram.png)
 
 ## EOCropImage Widget
 
 EOCropImage Widget is used to crop an image in a selected rectangle ROI, defined visually on the widget's GUI
 with a red rectangle, sliders can be used to variate **Crop Size**, **Vertical Range X** and the
 **Horizontal Range Y** that modify visually the red rectangle's size and position.
 It takes a `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the cropped image. 
 
-![](screenshots/Crop.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Crop.png)
 
 ## EOLoadImage Widget
 
 EOLoadImage Widget is used to load images from the directory structure.
 The output is a `DrbImageBaseNode` of the selected image. 
 
-![](screenshots/Load.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Load.png)
 
 ## EOViewImage Widget
 
 EOViewImage Widget is used to visualize images inside Orange Data Mining.
 A slider is used to variate **Image Size** that modify visually the size of the image.
 It takes a list of `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the selected image. 
 
-![](screenshots/View.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/View.png)
```

### Comparing `orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/PKG-INFO` & `orange-earth-observation-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-earth-observation
-Version: 1.0.0.dev1
+Version: 1.0.1
 Summary: Add-on containing widgets for earth observation data operations
 Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
@@ -15,36 +15,40 @@
 Orange3 Earth Observation Add-on
 ======================
 
 This is an add-on for [Orange3](https://orangedatamining.com/). Add-on can extend Orange either 
 in scripting or GUI part, or in both. Register it with Orange and add a new workflow with some 
 of these widget to example tutorials.
 
-Installation
-------------
-
-To install the add-on from source run
-
-    pip install .
-
-Usage
------
-
-After the installation, widgets from this add-on are registered with Orange. To run Orange from the terminal,
-use
-
-    orange-canvas
-
+## Installation
+_Orange3_ and the _EO_ Addon must be installed in the same
+_Python_ environment.
+
+### Orange 3
+```shell
+pip install pyQt5 PyQtWebEngine
+pip install orange3
+```
+
+### Earth Observation Addon
+```shell
+pip install orange-earth-observation
+```
+
+## Usage
+Orange3 can be run using the following command:
+```shell
+orange-canvas
+```
 or
-
-    python -m Orange.canvas
-
-New widgets appears in the toolbox bar under the section Earth Observation.
-
-![screenshot](screenshots/category_EO.png)
+```shell
+python -m orange.canvas
+```
+New widgets should appear in the toolbox bar under the __Earth Observation__
+section.
 
 Widgets Description
 -----
 
 **ODM** (_Orange Data Mining_) is an open source machine learning and data visualization tool.
 It allows to build data analysis workflows visually, with a large, diverse toolbox.
 
@@ -68,75 +72,75 @@
 EODataCatalog Widget has a list of multi-option boxes to filter for products by **Mission**, **Platform**, **Type**, 
 **Sensor**, and a slider to define the **Cloud Cover** maximum value, the filter is passed through `ODataQueryPredicate`. 
 
 A `DrbNode` is retrieved, and can be passed through the output to be used by other ODM widgets, the product corresponding 
 can also be downloaded to local file.
 
 
-![](screenshots/Catalog.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Catalog.png)
 
 ## EONutsShape Widget
 
 EONutsShape Widget is used to crop Sentinel 2 TCI (True Color Image), remove parts not part of NUTS shape. 
 It takes a `DrbNode` as input, needs a file in .shp format containing polygons shapes corresponding to NUTS Region. 
 The output is a `DrbImageBaseNode` of the TC Image in selected NUTS Region. 
 
 
-![](screenshots/Nuts.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Nuts.png)
 
 ## EOMosaicImage Widget
 
 EOMosaicImage Widget is used to assemble image parts when possible, creating a mosaic image, corresponding to a predefined NUTS Region. 
 It takes a list of `DrbImageBaseNode` as input, all inputs need to be in same CRS and NUTS region. 
 The output is a `DrbImageBaseNode` of the assembled TC Image. 
 
-![](screenshots/Mosaic.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Mosaic.png)
 
 ## EOReprojectImage Widget
 
 EOReprojectImage Widget is used to reproject an image from one CRS to another. 
 It takes a `DrbImageBaseNode` as input and outputs the same.
 
-![](screenshots/Projection.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Projection.png)
 
 ## EOCloudMask Widget
 
 EOCloudMask Widget is used to mask Sentinel 2 TCI (True Color Image), remove pixels representing clouds, 
 shadows, water, snow or ice.
 It takes a `DrbNode` as input, needs the SCL band containing the mask information which can be found 
 in the same S2 product. The output is a `DrbImageBaseNode` of the TC Image with selected mask applied on.  
 
-![](screenshots/Cloud.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Cloud.png)
 
 ## EOHistogram Widget
 
 EOHistogram Widget is used for histogram visualisation, basic and adaptive histogram equalization.
 It takes a `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` after histogram equalization are done. 
 It might need to specify the **Clip Limit** which is used by the algorithm to apply adaptive equalization.
 EOHistogram Widget can also take a list of `DrbImageBaseNode` as input, in order to perform a histogram matching 
 after specifying the reference image. 
 
-![](screenshots/Histogram.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Histogram.png)
 
 ## EOCropImage Widget
 
 EOCropImage Widget is used to crop an image in a selected rectangle ROI, defined visually on the widget's GUI
 with a red rectangle, sliders can be used to variate **Crop Size**, **Vertical Range X** and the
 **Horizontal Range Y** that modify visually the red rectangle's size and position.
 It takes a `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the cropped image. 
 
-![](screenshots/Crop.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Crop.png)
 
 ## EOLoadImage Widget
 
 EOLoadImage Widget is used to load images from the directory structure.
 The output is a `DrbImageBaseNode` of the selected image. 
 
-![](screenshots/Load.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/Load.png)
 
 ## EOViewImage Widget
 
 EOViewImage Widget is used to visualize images inside Orange Data Mining.
 A slider is used to variate **Image Size** that modify visually the size of the image.
 It takes a list of `DrbImageBaseNode` as input, the output is a `DrbImageBaseNode` of the selected image. 
 
-![](screenshots/View.png)
+![Screenshot](https://gitlab.com/drb-python/samples/odm/eo_addon/-/blob/main/screenshots/View.png)
```

### Comparing `orange-earth-observation-1.0.0.dev1/orange_earth_observation.egg-info/SOURCES.txt` & `orange-earth-observation-1.0.1/orange_earth_observation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/catalog.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/catalog.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/cloud_mask.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/crop_image.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/crop_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/histogram.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/catalog.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/catalog.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/category.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/cloud.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/cloud.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/crop.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/crop.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/load.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/load.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/mosaic.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/mosaic.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/projection.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/projection.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/icons/view.svg` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/icons/view.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/load_image.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/load_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/mosaic_image.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/mosaic_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/nuts_shape.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/nuts_shape.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/reproject_image.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/reproject_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/orangecontrib/earth_observation/widgets/view_image.py` & `orange-earth-observation-1.0.1/orangecontrib/earth_observation/widgets/view_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/setup.cfg` & `orange-earth-observation-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.0.dev1/versioneer.py` & `orange-earth-observation-1.0.1/versioneer.py`

 * *Files identical despite different names*

