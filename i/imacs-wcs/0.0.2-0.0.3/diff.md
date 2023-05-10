# Comparing `tmp/imacs_wcs-0.0.2.tar.gz` & `tmp/imacs_wcs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imacs_wcs-0.0.2.tar", last modified: Wed May 10 15:15:34 2023, max compression
+gzip compressed data, was "imacs_wcs-0.0.3.tar", last modified: Wed May 10 15:27:34 2023, max compression
```

## Comparing `imacs_wcs-0.0.2.tar` & `imacs_wcs-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/PKG-INFO
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:15:34.239697 imacs_wcs-0.0.2/imacs_wcs/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:12:38.761607 imacs_wcs-0.0.2/imacs_wcs/__init__.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.2/imacs_wcs/chip.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 15:11:54.666085 imacs_wcs-0.0.2/imacs_wcs/draggable_scatter.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     6543 2023-05-10 15:12:15.689857 imacs_wcs-0.0.2/imacs_wcs/header_reader.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      899 2023-05-10 15:12:34.793650 imacs_wcs-0.0.2/imacs_wcs/imacs_wcs.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-05-10 15:12:40.853585 imacs_wcs-0.0.2/imacs_wcs/instrument_constants.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10786 2023-05-10 15:12:51.721467 imacs_wcs-0.0.2/imacs_wcs/manual_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2211 2023-05-10 15:12:44.393546 imacs_wcs-0.0.2/imacs_wcs/semi_auto_astrometry.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 15:12:50.089484 imacs_wcs-0.0.2/setup.cfg
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-10 15:14:55.460120 imacs_wcs-0.0.2/setup.py
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:27:34.183416 imacs_wcs-0.0.3/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      779 2023-05-10 15:27:34.183416 imacs_wcs-0.0.3/PKG-INFO
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:27:34.183416 imacs_wcs-0.0.3/imacs_wcs/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-10 15:12:38.761607 imacs_wcs-0.0.3/imacs_wcs/__init__.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      843 2023-05-10 14:26:51.861324 imacs_wcs-0.0.3/imacs_wcs/chip.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2144 2023-05-10 15:11:54.666085 imacs_wcs-0.0.3/imacs_wcs/draggable_scatter.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     6512 2023-05-10 15:25:38.812742 imacs_wcs-0.0.3/imacs_wcs/header_reader.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      766 2023-05-10 15:25:20.188957 imacs_wcs-0.0.3/imacs_wcs/imacs_wcs.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      270 2023-05-10 15:12:40.853585 imacs_wcs-0.0.3/imacs_wcs/instrument_constants.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)    10787 2023-05-10 15:25:19.168969 imacs_wcs-0.0.3/imacs_wcs/manual_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     2179 2023-05-10 15:25:43.388690 imacs_wcs-0.0.3/imacs_wcs/semi_auto_astrometry.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-10 15:12:50.089484 imacs_wcs-0.0.3/setup.cfg
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1198 2023-05-10 15:25:40.972717 imacs_wcs-0.0.3/setup.py
```

### Comparing `imacs_wcs-0.0.2/PKG-INFO` & `imacs_wcs-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imacs_wcs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for determining and writing wcs information for IMACS images.
 Home-page: https://github.com/TrystanScottLambert
 Author: Trystan Scott Lambert
 Author-email: trystanscottlambert@gmail.com
 License: MIT
-Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.2.tar.gz
+Download-URL: https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.3.tar.gz
 Description: UNKNOWN
 Keywords: astronomy,wcs,imacs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imacs_wcs-0.0.2/imacs_wcs/chip.py` & `imacs_wcs-0.0.3/imacs_wcs/chip.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.2/imacs_wcs/draggable_scatter.py` & `imacs_wcs-0.0.3/imacs_wcs/draggable_scatter.py`

 * *Files identical despite different names*

### Comparing `imacs_wcs-0.0.2/imacs_wcs/header_reader.py` & `imacs_wcs-0.0.3/imacs_wcs/header_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 Module to read necessary information from the fits header and calculate correct values.
 """
 
-import sys
 import numpy as np
 from astropy.io import fits
 from astropy import wcs
 from astropy.coordinates import SkyCoord
 import astropy.units as u
 
-sys.path.append('./')
-from instrument_constants import Constants as c
-from chip import chips
+from .instrument_constants import Constants as c
+from .chip import chips
 
 def read_chip_number(fits_file_name: str) -> str:
     """Finds the chip number from the raw imacs file name."""
     chip_number = fits_file_name.split('.fits')[0].split('c')[-1]
     return f'c{chip_number}'
 
 def calculate_wcs_matrix(
```

### Comparing `imacs_wcs-0.0.2/imacs_wcs/imacs_wcs.py` & `imacs_wcs-0.0.3/imacs_wcs/imacs_wcs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """Module to update a raw IMACS fits file with wcs information."""
 
-import sys
 import glob
 from astropy.io import fits
 
-sys.path.append('./')
-import header_reader
+from .header_reader import HeaderInformation
 
 def add_wcs_to_fits(fits_file_name: str, outfile_name: str = ''):
     """Writes wcs information to the fits file."""
     hdu = fits.open(fits_file_name)
-    header_information = header_reader.HeaderInformation(fits_file_name)
+    header_information = HeaderInformation(fits_file_name)
     wcs = header_information.generate_wcs_object()
     header_wcs = wcs.to_header()
     hdu[0].header = hdu[0].header + header_wcs
 
     if outfile_name == '':
         outfile_name = fits_file_name.split('.fits')[0] + '.wcs.fits'
     hdu.writeto(outfile_name, overwrite=True)
 
 if __name__ == '__main__':
-    #files = glob.glob('/home/tlambert/Downloads/g_band/REDUCED/*science*.fits')
-    files = glob.glob('/home/tlambert/Downloads/g_band/SCIENCE/*.fits')
+    files = glob.glob('../SCIENCE/*.fits')
     for file in files:
         add_wcs_to_fits(file)
```

### Comparing `imacs_wcs-0.0.2/imacs_wcs/manual_astrometry.py` & `imacs_wcs-0.0.3/imacs_wcs/manual_astrometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from astropy.wcs import utils
 from photutils.detection import DAOStarFinder
 import astropy.units as u
 from scipy.optimize import curve_fit
 import matplotlib.pyplot as plt
 from astroquery.gaia import Gaia
 
-from draggable_scatter import DraggableScatter
+from .draggable_scatter import DraggableScatter
 
 
 def are_points_aligned(data: np.ndarray, x_array: np.array, y_array: np.ndarray) -> bool:
     """
     Tries to find a source in every cut out image. If less than 70% of the cutouts are determined to
     not have sources then the test is a fail.
     """
```

### Comparing `imacs_wcs-0.0.2/imacs_wcs/semi_auto_astrometry.py` & `imacs_wcs-0.0.3/imacs_wcs/semi_auto_astrometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 Semi-automated method for determining accurate WCS.
 This method will rely on manually correcting one chip and then 
 assume the correction is the same for the remaining chips. The remaining 
 chips will then be automatically matched with gaia stars. If at some point there isn't 
 a good match, manual correction will be required and the process continues.
 """
 
-import sys
 import glob
 import numpy as np
 
-sys.path.append('./')
-from manual_astrometry import ChipImage
+from .manual_astrometry import ChipImage
 
 
 def do_semi_automation_for_chip(directory: str, chip_number: int) -> None:
     """
     Runs the semi automation on a select chip.
     """
     if chip_number<1 or chip_number>8:
```

### Comparing `imacs_wcs-0.0.2/setup.py` & `imacs_wcs-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'imacs_wcs',
   packages = ['imacs_wcs'],
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Library for determining and writing wcs information for IMACS images.',
   author = 'Trystan Scott Lambert',
   author_email = 'trystanscottlambert@gmail.com',
   url = 'https://github.com/TrystanScottLambert',
-  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.2.tar.gz',
+  download_url = 'https://github.com/TrystanScottLambert/imacs_wcs/archive/refs/tags/v0.0.3.tar.gz',
   keywords = ['astronomy', 'wcs', 'imacs'],
   install_requires=[
     'numpy',
     'photutils',
     'astropy',
     'scipy',
     'matplotlib',
```

