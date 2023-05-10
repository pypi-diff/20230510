# Comparing `tmp/terrainman-0.0.13.tar.gz` & `tmp/terrainman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrainman-0.0.13.tar", max compression
+gzip compressed data, was "terrainman-0.0.9.tar", max compression
```

## Comparing `terrainman-0.0.13.tar` & `terrainman-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.13/LICENSE
--rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.13/README.md
--rw-r--r--   0        0        0      946 2023-05-10 18:37:51.371815 terrainman-0.0.13/pyproject.toml
--rw-r--r--   0        0        0      546 2023-05-10 18:34:44.739467 terrainman-0.0.13/src/terrainman/__init__.py
--rw-r--r--   0        0        0     9600 2023-05-10 18:34:18.488944 terrainman-0.0.13/src/terrainman/tile_io.py
--rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 terrainman-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.9/LICENSE
+-rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.9/README.md
+-rw-r--r--   0        0        0      969 2023-05-10 17:54:37.102852 terrainman-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-08 00:34:50.893087 terrainman-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     9650 2023-05-09 02:23:25.027650 terrainman-0.0.9/src/tile_io.py
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 terrainman-0.0.9/PKG-INFO
```

### Comparing `terrainman-0.0.13/LICENSE` & `terrainman-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terrainman-0.0.13/pyproject.toml` & `terrainman-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "terrainman"
-version = "0.0.13"
+version = "0.0.9"
 description = "A package for downloading and managing high-fidelity terrain files"
 authors = ["Liam Robinson <robin502@purdue.edu>"]
 readme = "README.md"
-packages = [{include = "terrainman", from = "src"}]
+packages = [{include = "src"}]
+include = [{path = "src", format = "sdist"}]
 documentation = "https://python-poetry.org/docs/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS",
 ]
```

### Comparing `terrainman-0.0.13/src/terrainman/tile_io.py` & `terrainman-0.0.9/src/tile_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 import pickle
 from typing import Tuple
 from abc import ABC
 from netCDF4 import Dataset
 import datetime
 
 
+_SRC_DIR = os.path.dirname(
+    os.path.abspath(inspect.getsourcefile(lambda: 0))
+)
+_DATA_DIRECTORY = os.path.join(_SRC_DIR, 'data')
 
 def strip_tuple(t: tuple) -> tuple:
     """Returns a copy of a tuple-of-tuples with no extra layers such that `t[0][0]` is not a tuple
 
     :param t: Input tuple
     :type t: tuple
     :return: Same tuple, stripped of outer layers past the first
@@ -128,15 +132,15 @@
             if self._before_request(*input_set):
                 self._make_request(*input_set)
                 self._after_request()
 
 
 class TerrainDataHandler(DataProduct):
     def __init__(self) -> None:
-        self._storage_dir = os.path.join(os.environ['TERRAIN_DATA'], 'terrain')
+        self._storage_dir = os.path.join(_DATA_DIRECTORY, 'terrain')
         self.url_base = 'https://e4ftl01.cr.usgs.gov/DP133/SRTM/SRTMGL1.003/2000.02.11/'
         self.download_format = "zip"
         self.save_format = "hgt"
         self.HTTP_ERR_MSG = "HTTP error occured, likely because tile is ocean, aborting..."
         self.DNE_MSG = "Tile does not exist, likely because it's ocean, skipping"
         self.EXISTS_MSG = "Tile already downloaded, skipping"
 
@@ -187,26 +191,25 @@
         unique_lat_lons = np.array(unique_lat_lons, np.int32)
         return tuple(map(tuple, unique_lat_lons))
 
         
 class AerosolDataHandler(DataProduct):
     def __init__(self) -> None:
         # Signature (dates, cadence)
-        self._storage_dir = os.path.join(os.environ['TERRAIN_DATA'], 'aerosol')
+        self._storage_dir = os.path.join(_DATA_DIRECTORY, 'aerosol')
         self.url_base = 'https://ladsweb.modaps.eosdis.nasa.gov'
         self.download_format = "nc"
         self.save_format = "nc"
         self._VIIRS_AEROSOL_CADENCES = ["daily", "monthly"]
 
         self._after_init()
     
     def _set_fnames(self, date: datetime.datetime, cadence: str) -> str:
         assert cadence in self._VIIRS_AEROSOL_CADENCES, f"Cadence must be in {self._VIIRS_AEROSOL_CADENCES}!"
-        csv_path = os.path.join(os.environ['TERRAIN_DATA'], f'viirs_aerosol_{cadence}.csv')
-        with open(csv_path, 'r') as f:
+        with open(f'src/data/viirs_aerosol_{cadence}.csv', 'r') as f:
             csv_els = f.read().split(',')
             if cadence == "daily":
                 fnames = [c for c in csv_els if f'/{date.year}/{date.strftime("%j")}/' in c][-1]
             elif cadence == "monthly":
                 month_first = datetime.datetime(year=date.year, month=date.month, day=1)
                 month_first_doy = int(month_first.strftime("%j"))
                 possible_date_strs = [f'/{date.year}/{d}/' for d in range(month_first_doy, month_first_doy+32)]
```

### Comparing `terrainman-0.0.13/PKG-INFO` & `terrainman-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrainman
-Version: 0.0.13
+Version: 0.0.9
 Summary: A package for downloading and managing high-fidelity terrain files
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
```

