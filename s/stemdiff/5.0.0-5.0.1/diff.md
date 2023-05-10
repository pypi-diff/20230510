# Comparing `tmp/stemdiff-5.0.0.tar.gz` & `tmp/stemdiff-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemdiff-5.0.0.tar", last modified: Tue May  2 21:45:28 2023, max compression
+gzip compressed data, was "stemdiff-5.0.1.tar", last modified: Wed May 10 12:11:34 2023, max compression
```

## Comparing `stemdiff-5.0.0.tar` & `stemdiff-5.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.920915 stemdiff-5.0.0/
--rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-5.0.0/CITATION
--rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-5.0.0/LICENCE
--rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3053 2023-05-02 21:45:28.920915 stemdiff-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2496 2023-05-02 21:44:30.000000 stemdiff-5.0.0/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 21:45:28.920915 stemdiff-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1373 2022-08-26 14:48:12.000000 stemdiff-5.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.872384 stemdiff-5.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.904949 stemdiff-5.0.0/src/stemdiff/
--rw-rw-rw-   0        0        0      794 2023-04-30 14:47:13.000000 stemdiff-5.0.0/src/stemdiff/__init__.py
--rw-rw-rw-   0        0        0     5224 2023-05-02 21:01:54.000000 stemdiff-5.0.0/src/stemdiff/dbase.py
--rw-rw-rw-   0        0        0     5058 2023-05-02 21:03:20.000000 stemdiff-5.0.0/src/stemdiff/detectors.py
--rw-rw-rw-   0        0        0     4437 2023-04-30 15:34:56.000000 stemdiff-5.0.0/src/stemdiff/gvars.py
--rw-rw-rw-   0        0        0    27995 2023-05-02 20:50:16.000000 stemdiff-5.0.0/src/stemdiff/io.py
--rw-rw-rw-   0        0        0    11432 2023-05-02 18:17:46.000000 stemdiff-5.0.0/src/stemdiff/psf.py
--rw-rw-rw-   0        0        0    12382 2023-05-02 21:20:53.000000 stemdiff-5.0.0/src/stemdiff/sum.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:45:28.916274 stemdiff-5.0.0/src/stemdiff.egg-info/
--rw-rw-rw-   0        0        0     3053 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 21:45:28.000000 stemdiff-5.0.0/src/stemdiff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:11:34.179527 stemdiff-5.0.1/
+-rw-rw-rw-   0        0        0      243 2021-12-11 16:39:22.000000 stemdiff-5.0.1/CITATION
+-rw-rw-rw-   0        0        0     1340 2021-12-11 16:39:46.000000 stemdiff-5.0.1/LICENCE
+-rw-rw-rw-   0        0        0      139 2021-12-12 12:41:28.000000 stemdiff-5.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3488 2023-05-10 12:11:34.179527 stemdiff-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-05-10 11:17:57.000000 stemdiff-5.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 stemdiff-5.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:11:34.195153 stemdiff-5.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2022-08-26 14:48:12.000000 stemdiff-5.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:11:34.116573 stemdiff-5.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:11:34.179527 stemdiff-5.0.1/src/stemdiff/
+-rw-rw-rw-   0        0        0      794 2023-05-08 14:19:09.000000 stemdiff-5.0.1/src/stemdiff/__init__.py
+-rw-rw-rw-   0        0        0     5224 2023-05-02 21:01:54.000000 stemdiff-5.0.1/src/stemdiff/dbase.py
+-rw-rw-rw-   0        0        0     5441 2023-05-08 14:22:33.000000 stemdiff-5.0.1/src/stemdiff/detectors.py
+-rw-rw-rw-   0        0        0     4437 2023-04-30 15:34:56.000000 stemdiff-5.0.1/src/stemdiff/gvars.py
+-rw-rw-rw-   0        0        0    27878 2023-05-06 23:36:48.000000 stemdiff-5.0.1/src/stemdiff/io.py
+-rw-rw-rw-   0        0        0    14357 2023-05-07 11:24:49.000000 stemdiff-5.0.1/src/stemdiff/psf.py
+-rw-rw-rw-   0        0        0    15600 2023-05-07 10:59:16.000000 stemdiff-5.0.1/src/stemdiff/sum.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:11:34.179527 stemdiff-5.0.1/src/stemdiff.egg-info/
+-rw-rw-rw-   0        0        0     3488 2023-05-10 12:11:34.000000 stemdiff-5.0.1/src/stemdiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-10 12:11:34.000000 stemdiff-5.0.1/src/stemdiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:11:34.000000 stemdiff-5.0.1/src/stemdiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-10 12:11:34.000000 stemdiff-5.0.1/src/stemdiff.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 12:11:34.000000 stemdiff-5.0.1/src/stemdiff.egg-info/top_level.txt
```

### Comparing `stemdiff-5.0.0/LICENCE` & `stemdiff-5.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.0/PKG-INFO` & `stemdiff-5.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: stemdiff
-Version: 5.0.0
-Summary: Convert 4D-STEM data to a single powder diffraction pattern.
-Home-page: https://github.com/mirekslouf/stemdiff/
-Author: Mirek Slouf
-Author-email: mirek.slouf@gmail.com
-License: MIT
-Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 STEMDIFF :: Simple processing of 4D-STEM data
 ---------------------------------------------
 
 * The **STEMDIFF package** converts... <br>
   ... a 4D-STEM dataset from a SEM microscope (huge and complex) <br>
-  ... to a single powder diffraction pattern (simple and easy to work with).
+  ... to a 2D-powder diffraction pattern (simple and easy to work with).
 * The STEMDIFF package is a key part of our **4D-STEM/PNBD** method, <br>
   which was described (together with the package) in open-access publications:
 	1. *Nanomaterials* 11 (2021) 962.
 	   [https://doi.org/10.3390/nano11040962](https://doi.org/10.3390/nano11040962)
 	2. *Materials* 14 (2021) 7550.
        [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
 * If you use STEMDIFF package, **please cite** the 2nd publication (or both :-).
@@ -32,40 +16,46 @@
 ---------
 
 <img src="https://mirekslouf.github.io/stemdiff/images/principle2.png" alt="STEMDIFF principle" width="500"/>
 
 Quick start
 -----------
 
-* Install stemdiff: `pip install stemdiff`
-* TODO
+* See how it works:
+	- Look at [worked example](https://mirekslouf.github.io/stemdiff/docs/examples/ex1_stemdiff.nb.html)
+      in Jupyter.
+* Try it yourself:
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/321rnw7ywyiym0gsv68r1/h?dl=0&rlkey=ucr4kmaxqmgewsx20soo4rjsm).
+	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
-More detailed help, demo and source code including documentation are in
-[GitHub](https://mirekslouf.github.io/stemdiff).
+* [PyPI](https://pypi.org/project/stemdiff) repository.
+* [GitHub](https://github.com/mirekslouf/stemdiff) repository.
+* [GitHub Pages](https://mirekslouf.github.io/stemdiff)
+  with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
 * Version 2.0 = like v1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
-	* deconvolution = reduce the effect of primary beam spread
+	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
 * Version 4.2 = like v4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
 * Version 5.0 = complete rewrite of v4.2
-	* all features of v4.2 (summation, filtering, deconvolution)
+	* all key features of v4.2 (summation, filtering, deconvolution)
 	* plus several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
-		- better filtering (which can employ number of diffractions)
-		- possibility to define more types of deconvolution
+		- better filtering (including estimated number of diffractions)
+		- more types of deconvolution algorithms
 	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to sister package EDIFF
+		- this was improved and moved to a sister package EDIFF
```

### Comparing `stemdiff-5.0.0/README.md` & `stemdiff-5.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,29 @@
+Metadata-Version: 2.1
+Name: stemdiff
+Version: 5.0.1
+Summary: Convert 4D-STEM data to a single powder diffraction pattern.
+Home-page: https://github.com/mirekslouf/stemdiff/
+Author: Mirek Slouf
+Author-email: mirek.slouf@gmail.com
+License: MIT
+Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 STEMDIFF :: Simple processing of 4D-STEM data
 ---------------------------------------------
 
 * The **STEMDIFF package** converts... <br>
   ... a 4D-STEM dataset from a SEM microscope (huge and complex) <br>
-  ... to a single powder diffraction pattern (simple and easy to work with).
+  ... to a 2D-powder diffraction pattern (simple and easy to work with).
 * The STEMDIFF package is a key part of our **4D-STEM/PNBD** method, <br>
   which was described (together with the package) in open-access publications:
 	1. *Nanomaterials* 11 (2021) 962.
 	   [https://doi.org/10.3390/nano11040962](https://doi.org/10.3390/nano11040962)
 	2. *Materials* 14 (2021) 7550.
        [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
 * If you use STEMDIFF package, **please cite** the 2nd publication (or both :-).
@@ -16,40 +32,46 @@
 ---------
 
 <img src="https://mirekslouf.github.io/stemdiff/images/principle2.png" alt="STEMDIFF principle" width="500"/>
 
 Quick start
 -----------
 
-* Install stemdiff: `pip install stemdiff`
-* TODO
+* See how it works:
+	- Look at [worked example](https://mirekslouf.github.io/stemdiff/docs/examples/ex1_stemdiff.nb.html)
+      in Jupyter.
+* Try it yourself:
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/321rnw7ywyiym0gsv68r1/h?dl=0&rlkey=ucr4kmaxqmgewsx20soo4rjsm).
+	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
-More detailed help, demo and source code including documentation are in
-[GitHub](https://mirekslouf.github.io/stemdiff).
+* [PyPI](https://pypi.org/project/stemdiff) repository.
+* [GitHub](https://github.com/mirekslouf/stemdiff) repository.
+* [GitHub Pages](https://mirekslouf.github.io/stemdiff)
+  with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
 * Version 2.0 = like v1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
-	* deconvolution = reduce the effect of primary beam spread
+	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
 * Version 4.2 = like v4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
 * Version 5.0 = complete rewrite of v4.2
-	* all features of v4.2 (summation, filtering, deconvolution)
+	* all key features of v4.2 (summation, filtering, deconvolution)
 	* plus several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
-		- better filtering (which can employ number of diffractions)
-		- possibility to define more types of deconvolution
+		- better filtering (including estimated number of diffractions)
+		- more types of deconvolution algorithms
 	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to sister package EDIFF
+		- this was improved and moved to a sister package EDIFF
```

### Comparing `stemdiff-5.0.0/setup.py` & `stemdiff-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.0/src/stemdiff/__init__.py` & `stemdiff-5.0.1/src/stemdiff/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     - 2D-NBD's = monocrystalline-like nanobeam diffraction patterns.
 * Output = 2D-powder diffraction pattern
     - A 2D-powder diffraction pattern is calculated from a 4D-STEM dataset.
     - The calculation is basically a specific summation of 2D-NBD patterns.
     - In other words, a 4D-STEM dataset is reduced to a 2D-diffraction pattern.
     - The whole method (and final pattern) is called 4D-STEM/PNBD (powder NBD).
 '''
-__version__ = "5.0.0"
+__version__ = "5.0.1"
```

### Comparing `stemdiff-5.0.0/src/stemdiff/dbase.py` & `stemdiff-5.0.1/src/stemdiff/dbase.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.0/src/stemdiff/detectors.py` & `stemdiff-5.0.1/src/stemdiff/detectors.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 Known detectors for package stemdiff.
 
 This module is basically a container of classes.
 Each class describes a pixelated STEM detector, from which we get datafiles.
 The description is not difficult - all we need to define is
 detector name, detector size, data type, upscaling coefficient,
 and how to read/save datafiles in given detector format.
-All these parameters are described below in TimePix detector class.
+
+All detector parameters are described below in TimePix detector class.
 Therefore, the new classes = new detectors can be added quite easily:
 
-* Copy class describing detector TimePix
-* Rename the class as needed, for example: My_new_STEM_detector
-* Re-define all properties and methods of the new class as necessary
-* When you are done, the new detector can be used within STEMDIFF package
+* Copy class describing detector TimePix.
+* Rename the class as needed, for example: My_new_STEM_detector.
+* Re-define all properties and methods of the new class as necessary.
+* When you are done, the new detector can be used within STEMDIFF package.
 '''
 
 import sys
 import inspect
 import numpy as np
     
 def list_of_known_detectors():
@@ -110,29 +111,39 @@
         -------
         arr : 2D-numpy array
             2D-array containing image from TimePix detector.
             Each element of the array = the intensity detected at given pixel.
         '''
         # Read binary datafile (to 1D-array)
         arr = np.fromfile(filename, dtype=self.data_type)
-        # Reshape the 1D-array to 2D-square array
-        if arr_size:
-            # If arr_size was given,
-            # the datafile must have been saved with cut edges
-            # and, as a result, we read a smaller array with array_size.
-            arr = arr.reshape(self.detector_size, self.detector_size)
-        else:
-            # If arr_size was not given,
-            # the datafile must be in its original format
-            # and, as a result, we read it with default detector.size.
-            arr = arr.reshape(self.detector_size, self.detector_size)
-        # Return the final square array
+        # Determine edge of the file - we work only with square files
+        edge = int(np.sqrt(arr.size))
+        # Reshape the array and return
+        arr = arr.reshape(edge, edge)
         return(arr)
-    
-    def save_datafile(self, filename):
-        '''
-        Save datafile in TimePix detector format.
-        '''
-        # TODO
-        # Save the datafile to a binary file
-        # Flatten array to 1D, save as binary file with given format.
-        pass
+        
+        # # Reshape the 1D-array to 2D-square array
+        # if arr_size:
+        #     # If arr_size was given,
+        #     # the datafile must have been saved with cut edges
+        #     # and, as a result, we read a smaller array with array_size.
+        #     arr = arr.reshape(self.arr_size, self.arr_size)
+        # else:
+        #     # If arr_size was not given,
+        #     # the datafile must be in its original format
+        #     # and, as a result, we read it with default detector.size.
+        #     arr = arr.reshape(self.detector_size, self.detector_size)
+        # # Return the final square array
+        # return(arr)
+    
+    def save_datafile(self, arr, filename):
+        '''
+        Save 2D-array as a datafile in the TimePix detector format.
+        '''
+        # Slightly modified according to
+        # https://stackoverflow.com/q/43211616
+        fh = open(filename,'wb')
+        arr = arr.flatten()
+        BlockArray = np.array(arr).astype(np.uint16)
+        BlockArray.tofile(fh)
+        fh.close()
+
```

### Comparing `stemdiff-5.0.0/src/stemdiff/gvars.py` & `stemdiff-5.0.1/src/stemdiff/gvars.py`

 * *Files identical despite different names*

### Comparing `stemdiff-5.0.0/src/stemdiff/io.py` & `stemdiff-5.0.1/src/stemdiff/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,16 @@
         # Initialization
         file_counter = 0
         # Iterate through the files
         for datafile in SDATA.filenames:
             # Read datafile from disk to array
             arr = Datafiles.read(SDATA, datafile)
             # Print datafile name
-            print('Datafile:', datafile.name)
+            datafile_name = datafile.relative_to(SDATA.data_dir)
+            print('Datafile:', datafile_name)
             # Describe the datafile/array
             Arrays.describe(arr,
                 central_square, cintensity, peak_height, peak_distance)
             # Show the datafile/array
             Arrays.show(arr,
                 icut, itype, R, cmap,
                 center, central_square, cintensity)
@@ -551,18 +552,15 @@
         else:
             img = Image.fromarray(arr)
         # Save image
         img.save(output_image)
         
 
     def save_as_datafile(SDATA, arr, filename):
-        # TODO - Mirek
-        # (1) Datafile format should correspond to format of selected detector
-        #     so that it was possbile to re-read the datafile!
-        # (2) Therefore, this function should be just a wrapper of 
+        SDATA.detector.save_datafile(arr, filename) 
         pass
 
 
     def prepare_for_show_or_save(arr, icut=None, itype=None, R=None):
         '''
         Prepare 2D numpy array (which contains a 2D-STEM datafile)
         for showing/saving as grayscale image.
```

### Comparing `stemdiff-5.0.0/src/stemdiff/psf.py` & `stemdiff-5.0.1/src/stemdiff/psf.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 PSF = Point Spread Function = XY-spread of the primary beam
 '''
 
 import numpy as np
 import matplotlib.pyplot as plt
 import stemdiff.io, stemdiff.dbase
+import scipy
 
 def save_psf_to_disk(arr, output_file):
     """
     Save PSF function;
     the function is saved as a file in NumPy format = NPY-file.
 
     Parameters
@@ -195,19 +196,19 @@
         '''
         # (0) Prepare variables
         file_counter = 0
         R = SDATA.detector.upscale
         det_size = SDATA.detector.detector_size
         psf_size = DIFFIMAGES.psfsize
         # (1) Prepare empty array for PSF calculation
-        psf = np.zeros((det_size*R, det_size*R), dtype=np.float)
+        psf = np.zeros((det_size*R, det_size*R), dtype=np.float32)
         if psf_size:
-            psf =  np.zeros((psf_size*R, psf_size*R), dtype=np.float)
+            psf =  np.zeros((psf_size*R, psf_size*R), dtype=np.float32)
         else:
-            psf =  np.zeros((det_size*R, det_size*R), dtype=np.float)
+            psf =  np.zeros((det_size*R, det_size*R), dtype=np.float32)
         # (2) Go through the files and calculate average PSF out of them
         for index,datafile in df.iterrows():
             # (a) Read datafile to array and increase file_counter
             file_to_read = SDATA.data_dir.joinpath(datafile.DatafileName)
             arr = stemdiff.io.Datafiles.read(SDATA, file_to_read)
             file_counter += 1
             # (b) Rescale array
@@ -261,35 +262,100 @@
         # (just geometrical center as explained in the docstring
         xc = yc = arr.shape[0]//2
         # Remove edges
         # (leave only central square with psf_size 
         psf = stemdiff.io.Arrays.remove_edges(arr, psf_size, xc,yc)
         # Remove background
         # (PSF is from the center, it "sits" on some background intensity
+        # !!! Convert PSF from uint to float - uint fails for negative values!
+        psf = psf.astype(np.float32)
         psf = psf - np.min(psf)
         # Convert square PSF to circular PSF if requested
         if circular:
             # Apply mask
             psf = psf * circular_mask(psf_size, psf_size)
             # Remove the remnants of background
             # (after removing edges, array values may be slightly above zero!
             # (1) We subtract the 2nd lowest value - the lowest are the zeros
             the_second_lowest_value = np.min(psf[psf != np.min(psf)])
             psf = psf - the_second_lowest_value
-            # (2) All negative values shoud go back above zero!
-            psf = np.where(psf < 0, 0, psf)
+        # All negative values shoud go back above zero!
+        # (the negative values may occur due to various recalcs and roundings
+        # (they are very dangerous, leading to unwanted side-effects and errors
+        psf = np.where(psf < 0, 0, psf)
         # Return final PSF
         return(psf)
 
 class PSFtype3:
+        
+    def get_psf(arr, psf_size, cake, subtract = False):
+        '''
+        Get PSF of type3 = individual PSF based on cake-method.
+
+        Parameters
+        ----------
+        arr : 2D-numpy array
+            The array/datafile, from which the PSF is to be determined.
+            The array is a square with geometrical center = intensity center.
+            See *Technical notes* below for more details and consequences.
+        psf_size : int
+            The size/diameter of PSF function to be determined.
+        cake : int
+            Size of cake-piece in degrees.
+        subtract : bool, optional, default is False
+            If True, prepare PSF with the same size as scattering pattern.
+            
+        Returns
+        -------
+        psf : 2D-numpy array
+            The array represents estimate of experimental PSF.
+
+        Technical notes
+        --------------
+        In our algorithm, we send a square centered array to this function.
+        This means that intensity center = geometric center of the array.
+        Consequence: we do not have to determine intensity center
+        and waste time - it is enough to calculate geometrical center.
+        '''
+           
+        if subtract == True:     
+            # PSF in the same size as image, converted to circular PSF
+            arr  = arr * circular_mask(arr.shape[0], arr.shape[1])     
+        else:   
+            # Picking the PSF from center of image
+            od = int(arr.shape[0]/2)-psf_size//2
+            do = int(arr.shape[0]/2)+psf_size//2
+            arr = arr[od:do,od:do]
+            # Convert to circular PSF
+            arr = arr * circular_mask(psf_size, psf_size)  
+
+        # Initial rotation angle
+        angle = 0
+        psf_multilevel = np.zeros((arr.shape[0], arr.shape[1], cake)) 
+        # Perform roation - PSF smooting
+        for j in range(0,cake):
+            # Storing all rotated diffraction patterns
+            psf_multilevel[:,:,j] = scipy.ndimage.rotate(
+                arr, angle=angle, reshape = False) 
+            angle += 1
     
-    def get_psf():
-        # TODO - Radim
-        # Individual PSF from whole datafile, cake-method.
-        pass
+        psf = np.zeros((arr.shape[0],arr.shape[1]))
+        # Pixels selection without peak 
+        for i in range(arr.shape[0]):
+            for ii in range(arr.shape[1]):
+                sig_sorted = np.sort(psf_multilevel[i,ii,:], axis=None)
+                # Prepared for np.mean and interval [0:x]
+                psf[i,ii] = np.median(sig_sorted[:]) 
+        
+        # XXX: Important safety insertion
+        # (due to various recalcs and roundings, psf may go below 0
+        # (negative psf values result in many unwanted side effects and errors!
+        psf = np.where(psf < 0, 0, psf)
+        
+        return(psf)
 
 class PSFtype4:
     
     def get_psf():
         # TODO - Radim
         # 1) Individual PSF from whole datafile (like PSFtype3).)
         # 2) Subtract the PSF from whole datafile (background removal).
```

### Comparing `stemdiff-5.0.0/src/stemdiff/sum.py` & `stemdiff-5.0.1/src/stemdiff/sum.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 '''
 
 import numpy as np
 import stemdiff.io
 import stemdiff.dbase
 from skimage import restoration
 
+
 def sum_datafiles(
         SDATA, DIFFIMAGES,
-        df, deconv=0, iterate=10, psf=None):
+        df, deconv=0, iterate=10, psf=None, cake=None, subtract=None):
     '''
     Sum datafiles from a 4D-STEM dataset.
     
     Parameters
     ----------
     SDATA : stemdiff.gvars.SourceData object
         The object describes source data (detector, data_dir, filenames).
@@ -64,15 +65,15 @@
         arr = sum_with_deconvolution_type1( 
             SDATA, DIFFIMAGES, df, psf, iterate)
     elif deconv == 2:
         arr = sum_with_deconvolution_type2(
             SDATA, DIFFIMAGES, df, iterate)
     elif deconv == 3:
         arr = sum_with_deconvolution_type3(
-            SDATA, DIFFIMAGES, df, iterate)
+            SDATA, DIFFIMAGES, df, iterate, cake, subtract)
     else:
         print(f'Unknown deconvolution type: deconv={deconv}')
         print('Nothing to do.')
         return(None)
     return(arr)
 
 def sum_without_deconvolution(SDATA, DIFFIMAGES, df):
@@ -87,15 +88,15 @@
     n = 0  # number of summed datafiles
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     # Prepare array for summation
     # (for summation without deconvolution array size = detector size
     # (we will sum original datafiles, just without the borders/edges  
     # (rescaling to higher resolution can be done AFTER the summation
-    sum_arr   = np.zeros((img_size,img_size), dtype=np.float)
+    sum_arr   = np.zeros((img_size,img_size), dtype=np.float32)
     # Sum datafiles
     for index,datafile in df.iterrows():
         # Read datafile to array
         datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
         arr = stemdiff.io.Datafiles.read(SDATA, datafile_name)
         # Reduce array size = cut borders, keep just central region
         # (some border region is ALWAYS cut, due to detector edge artifacts
@@ -130,15 +131,15 @@
     '''
     # Prepare variables .......................................................
     n = 0
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     # Prepare array for summation
     # (arr size = detector size * R => deconvolution on rescaled/upscaled array
-    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float)
+    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     # (we sum datafiles cut, rescaled, and deconvoluted
     # (rescaling DURING the summation => smoother deconvolution function
     # Sum with deconvolution, external PSF from low-diffracting files .........
     for index,datafile in df.iterrows():
         # (0) Simple progress indicator
         print('.', end='')
@@ -199,15 +200,15 @@
     # Prepare variables .......................................................
     n = 0
     R = SDATA.detector.upscale
     img_size = DIFFIMAGES.imgsize
     psf_size = DIFFIMAGES.psfsize
     # Prepare array for summation
     # (arr size = detector size * R => deconvolution on rescaled/upscaled array
-    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float)
+    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
     # Sum datafiles
     # (we sum datafiles cut, rescaled, and deconvoluted
     # (rescaling DURING the summation => smoother deconvolution function
     # Sum with deconvolution, PSF from center of image ........................
     for index,datafile in df.iterrows():
         # (0) Simple progress indicator
         print('.', end='')
@@ -249,27 +250,90 @@
     # (c) convert to final array with integer values
     # (why integer values? => arr with int's can be plotted as image and saved
     final_arr = np.round(sum_arr).astype(np.uint16)
     # (d) return the finalized array
     return(final_arr)
 
 def sum_with_deconvolution_type3(
-        DETECTOR, DATAFILES, DIFFIMAGES, df, iterate):
+        SDATA, DIFFIMAGES, df, iterate, cake, subtract):
     '''
     Sum datafiles with 2D-PSF deconvolution of type3.
     
     * What deconvolution type3:
         - Richardson-Lucy deconvolution.
         - The 2D-PSF function is estimated from each (whole) datafile.
         - The diffractions in 2D-PSF are removed by means of "cake method".
     * Parameters of the function:
         - This function is usually called from stemdiff.sum.sum_files.
         - The parameters are transferred from the sum_files function
     '''
-    pass
+    
+    # Prepare variables .......................................................
+    n = 0
+    R = SDATA.detector.upscale
+    # !!! img_size and psf_size must by multiplied by R wherever relevant
+    img_size = DIFFIMAGES.imgsize 
+    psf_size = DIFFIMAGES.psfsize
+    # Prepare array for summation
+    # (arr size = detector size * R => deconvolution on rescaled/upscaled array
+    sum_arr = np.zeros((img_size*R,img_size*R), dtype=np.float32)
+    # Sum datafiles
+    # (we sum datafiles cut, rescaled, and deconvoluted
+    # (rescaling DURING the summation => smoother deconvolution function
+    # Sum with deconvolution, PSF from center of image ........................
+    for index,datafile in df.iterrows():
+        # (0) Simple progress indicator
+        print('.', end='')
+        # (1) Read datafile
+        datafile_name = SDATA.data_dir.joinpath(datafile.DatafileName)
+        arr = stemdiff.io.Datafiles.read(SDATA, datafile_name) 
+        # (2) Remove edges
+        # (reason: edges usually contain weak or neglibible difractions
+        xc,yc = (round(datafile.Xcenter),round(datafile.Ycenter))
+        arr = stemdiff.io.Arrays.remove_edges(arr,img_size,xc,yc)
+        # (3) Upscale array
+        # (reason: deconvolution should be performed at higher resolution
+        # ( -logically, more pixels means smoother PSF => better deconvolution
+        # ( -surprisingly, upscaling increases real final resolution
+        arr = stemdiff.io.Arrays.rescale(arr, R, order=3)
+        # (4) Prepare PSF from the center of given array
+        # !!! psf_size must by multiplied by R
+        psf = stemdiff.psf.PSFtype3.get_psf(arr, psf_size*R, cake, subtract)   
+        if subtract:    
+            # Individual background (PSF) subtraction
+            arr = arr - psf
+            # All negative values shoud go to zero!
+            # (the negative values have result in many side effects and errors!
+            arr = np.where(arr < 0, 0, arr)
+        # (5) Deconvolute
+        # (a) save np.max, normalize
+        # (reason: deconvolution algorithm requires normalized arrays...
+        # (...and we save original max.intensity to re-normalize the result
+        norm_const = np.max(arr)
+        arr_norm = arr/np.max(arr)
+        psf_norm = psf/np.max(psf)
+        # (b) perform the deconvolution
+        arr_deconv = restoration.richardson_lucy(
+            arr_norm, psf_norm, num_iter=iterate)
+        # (c) restore original range of intensities = re-normalize
+        arr = arr_deconv * norm_const
+        # (6) Add rescaled and deconvoluted array to summation
+        sum_arr += arr
+        # (7) Updated n = number of summed arrays
+        n += 1
+    # Finalize and return result ..............................................
+    # (a) terminate simple progress indicator
+    print('End')
+    # (b) normalize the final array
+    sum_arr = sum_arr/n
+    # (c) convert to final array with integer values
+    # (why integer values? => arr with int's can be plotted as image and saved
+    final_arr = np.round(sum_arr).astype(np.uint16)
+    # (d) return the finalized array
+    return(final_arr)
 
 def sum_with_deconvolution_type4(
         DETECTOR, DATAFILES, DIFFIMAGES, df, iterate):
     '''
     Sum datafiles with 2D-PSF deconvolution of type4.
     
     * What is deconvolution type4:
```

### Comparing `stemdiff-5.0.0/src/stemdiff.egg-info/PKG-INFO` & `stemdiff-5.0.1/src/stemdiff.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemdiff
-Version: 5.0.0
+Version: 5.0.1
 Summary: Convert 4D-STEM data to a single powder diffraction pattern.
 Home-page: https://github.com/mirekslouf/stemdiff/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/stemdiff/
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 License-File: LICENCE
 
 STEMDIFF :: Simple processing of 4D-STEM data
 ---------------------------------------------
 
 * The **STEMDIFF package** converts... <br>
   ... a 4D-STEM dataset from a SEM microscope (huge and complex) <br>
-  ... to a single powder diffraction pattern (simple and easy to work with).
+  ... to a 2D-powder diffraction pattern (simple and easy to work with).
 * The STEMDIFF package is a key part of our **4D-STEM/PNBD** method, <br>
   which was described (together with the package) in open-access publications:
 	1. *Nanomaterials* 11 (2021) 962.
 	   [https://doi.org/10.3390/nano11040962](https://doi.org/10.3390/nano11040962)
 	2. *Materials* 14 (2021) 7550.
        [https://doi.org/10.3390/ma14247550](https://doi.org/10.3390/ma14247550)
 * If you use STEMDIFF package, **please cite** the 2nd publication (or both :-).
@@ -32,40 +32,46 @@
 ---------
 
 <img src="https://mirekslouf.github.io/stemdiff/images/principle2.png" alt="STEMDIFF principle" width="500"/>
 
 Quick start
 -----------
 
-* Install stemdiff: `pip install stemdiff`
-* TODO
+* See how it works:
+	- Look at [worked example](https://mirekslouf.github.io/stemdiff/docs/examples/ex1_stemdiff.nb.html)
+      in Jupyter.
+* Try it yourself:
+	- Download and unzip the [complete example with data](https://www.dropbox.com/scl/fo/321rnw7ywyiym0gsv68r1/h?dl=0&rlkey=ucr4kmaxqmgewsx20soo4rjsm).
+	- Look at `00readme.txt` and run the example in Jupyter.
 
 Documentation, help and examples
 --------------------------------
 
-More detailed help, demo and source code including documentation are in
-[GitHub](https://mirekslouf.github.io/stemdiff).
+* [PyPI](https://pypi.org/project/stemdiff) repository.
+* [GitHub](https://github.com/mirekslouf/stemdiff) repository.
+* [GitHub Pages](https://mirekslouf.github.io/stemdiff)
+  with [documentation](https://mirekslouf.github.io/stemdiff/docs).
 
 ## Versions of STEMDIFF
 
 * Version 1.0 = Matlab: just simple summation of 4D-dataset
 * Version 2.0 = like v1.0 + post-processing in Jupyter
 * Version 3.0 = Python scripts: summation + S-filtering
 * Version 4.0 = Python package: summation + S-filtering + deconvolution
 	* summation = summation of all 2D-diffractograms
 	* S-filtering = sum only diffractograms with strong diffractions = high S
-	* deconvolution = reduce the effect of primary beam spread
+	* deconvolution = reduce the primary beam spread effect
 	  &rArr; better resolution 
 * Version 4.2 = like v4.0 + a few important improvements, such as:
 	* sum just the central region with the strongest diffractions
 	  &rArr; higher speed
 	* 3 centering types: (0) geometry, (1) weight of 1st, (2) individual weights 
 	* better definition of summation and centering parameters
 	* better documentation strings + demo data + improved *master script*
 * Version 5.0 = complete rewrite of v4.2
-	* all features of v4.2 (summation, filtering, deconvolution)
+	* all key features of v4.2 (summation, filtering, deconvolution)
 	* plus several generalizations and improvements, namely:
 		- possibility to define and use more detectors/datafile formats
-		- better filtering (which can employ number of diffractions)
-		- possibility to define more types of deconvolution
+		- better filtering (including estimated number of diffractions)
+		- more types of deconvolution algorithms
 	* no conversion of 2D-diffractograms to 1D-profiles
-		- this was improved and moved to sister package EDIFF
+		- this was improved and moved to a sister package EDIFF
```

