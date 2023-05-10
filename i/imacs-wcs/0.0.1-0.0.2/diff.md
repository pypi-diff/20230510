# Comparing `tmp/imacs_wcs-0.0.1.tar.gz` & `tmp/imacs_wcs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imacs_wcs-0.0.1.tar", last modified: Wed May 10 14:49:58 2023, max compression
+gzip compressed data, was "imacs_wcs-0.0.2.tar", last modified: Wed May 10 15:15:34 2023, max compression
```

## Comparing `imacs_wcs-0.0.1.tar` & `imacs_wcs-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 14:49:58.166875 imacs_wcs-0.0.1/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-10 14:49:58.166875 imacs_wcs-0.0.1/PKG-INFO
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 14:49:58.166875 imacs_wcs-0.0.1/imacs_wcs/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 14:27:39.364752 imacs_wcs-0.0.1/imacs_wcs/__init__.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.1/imacs_wcs/chip.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 14:20:13.402107 imacs_wcs-0.0.1/imacs_wcs/draggable_scatter.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     6510 2023-05-10 14:24:46.050837 imacs_wcs-0.0.1/imacs_wcs/header_reader.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      865 2023-05-10 14:24:44.626854 imacs_wcs-0.0.1/imacs_wcs/imacs_wcs.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-04-26 17:21:24.509436 imacs_wcs-0.0.1/imacs_wcs/instrument_constants.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10786 2023-05-10 14:20:48.633685 imacs_wcs-0.0.1/imacs_wcs/manual_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2177 2023-05-10 14:26:41.829445 imacs_wcs-0.0.1/imacs_wcs/semi_auto_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 14:48:30.195479 imacs_wcs-0.0.1/setup.cfg
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-10 14:47:34.723823 imacs_wcs-0.0.1/setup.py
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/PKG-INFO
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/imacs_wcs/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:12:38.761607 imacs_wcs-0.0.2/imacs_wcs/__init__.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.2/imacs_wcs/chip.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 15:11:54.666085 imacs_wcs-0.0.2/imacs_wcs/draggable_scatter.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     6543 2023-05-10 15:12:15.689857 imacs_wcs-0.0.2/imacs_wcs/header_reader.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      899 2023-05-10 15:12:34.793650 imacs_wcs-0.0.2/imacs_wcs/imacs_wcs.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-05-10 15:12:40.853585 imacs_wcs-0.0.2/imacs_wcs/instrument_constants.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10786 2023-05-10 15:12:51.721467 imacs_wcs-0.0.2/imacs_wcs/manual_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2211 2023-05-10 15:12:44.393546 imacs_wcs-0.0.2/imacs_wcs/semi_auto_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 15:12:50.089484 imacs_wcs-0.0.2/setup.cfg
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-10 15:14:55.460120 imacs_wcs-0.0.2/setup.py
```

### Comparing `imacs_wcs-0.0.1/PKG-INFO` & `imacs_wcs-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imacs_wcs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for determining and writing wcs information for IMACS images.
 Home-page: https://github.com/TrystanScottLambert
 Author: Trystan Scott Lambert
 Author-email: trystanscottlambert@gmail.com
 License: MIT
-Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.2.tar.gz
 Description: UNKNOWN
 Keywords: astronomy,wcs,imacs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imacs_wcs-0.0.1/imacs_wcs/chip.py` & `imacs_wcs-0.0.2/imacs_wcs/chip.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.1/imacs_wcs/draggable_scatter.py` & `imacs_wcs-0.0.2/imacs_wcs/draggable_scatter.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.1/imacs_wcs/header_reader.py` & `imacs_wcs-0.0.2/imacs_wcs/header_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Module to read necessary information from the fits header and calculate correct values.
 """
 
+import sys
 import numpy as np
 from astropy.io import fits
 from astropy import wcs
 from astropy.coordinates import SkyCoord
 import astropy.units as u
 
+sys.path.append('./')
 from instrument_constants import Constants as c
 from chip import chips
 
 def read_chip_number(fits_file_name: str) -> str:
     """Finds the chip number from the raw imacs file name."""
     chip_number = fits_file_name.split('.fits')[0].split('c')[-1]
     return f'c{chip_number}'
```

### Comparing `imacs_wcs-0.0.1/imacs_wcs/imacs_wcs.py` & `imacs_wcs-0.0.2/imacs_wcs/imacs_wcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Module to update a raw IMACS fits file with wcs information."""
 
+import sys
 import glob
 from astropy.io import fits
+
+sys.path.append('./')
 import header_reader
 
 def add_wcs_to_fits(fits_file_name: str, outfile_name: str = ''):
     """Writes wcs information to the fits file."""
     hdu = fits.open(fits_file_name)
     header_information = header_reader.HeaderInformation(fits_file_name)
     wcs = header_information.generate_wcs_object()
```

### Comparing `imacs_wcs-0.0.1/imacs_wcs/manual_astrometry.py` & `imacs_wcs-0.0.2/imacs_wcs/manual_astrometry.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.1/imacs_wcs/semi_auto_astrometry.py` & `imacs_wcs-0.0.2/imacs_wcs/semi_auto_astrometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 Semi-automated method for determining accurate WCS.
 This method will rely on manually correcting one chip and then 
 assume the correction is the same for the remaining chips. The remaining 
 chips will then be automatically matched with gaia stars. If at some point there isn't 
 a good match, manual correction will be required and the process continues.
 """
 
+import sys
 import glob
 import numpy as np
+
+sys.path.append('./')
 from manual_astrometry import ChipImage
 
 
 def do_semi_automation_for_chip(directory: str, chip_number: int) -> None:
     """
     Runs the semi automation on a select chip.
     """
```

### Comparing `imacs_wcs-0.0.1/setup.py` & `imacs_wcs-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'imacs_wcs',
   packages = ['imacs_wcs'],
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Library for determining and writing wcs information for IMACS images.',
   author = 'Trystan Scott Lambert',
   author_email = 'trystanscottlambert@gmail.com',
   url = 'https://github.com/TrystanScottLambert',
-  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.1.tar.gz',
+  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.2.tar.gz',
   keywords = ['astronomy', 'wcs', 'imacs'],
   install_requires=[
     'numpy',
     'photutils',
     'astropy',
     'scipy',
     'matplotlib',
```

