# Comparing `tmp/relative_dose_1d-0.1.2.tar.gz` & `tmp/relative_dose_1d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.1.2.tar", last modified: Thu May  4 03:48:53 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.3.tar", last modified: Tue May  9 23:47:06 2023, max compression
```

## Comparing `relative_dose_1d-0.1.2.tar` & `relative_dose_1d-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 03:48:53.747720 relative_dose_1d-0.1.2/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3422 2023-05-04 03:48:53.740773 relative_dose_1d-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-05-04 03:45:45.000000 relative_dose_1d-0.1.2/README.md
--rw-rw-rw-   0        0        0     1395 2023-05-04 03:46:00.000000 relative_dose_1d-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 03:48:53.747720 relative_dose_1d-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 03:48:53.620147 relative_dose_1d-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 03:48:53.670005 relative_dose_1d-0.1.2/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     9352 2023-05-03 01:27:57.000000 relative_dose_1d-0.1.2/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.2/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0     9217 2023-05-04 03:27:26.000000 relative_dose_1d-0.1.2/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-04 03:48:53.728064 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     3422 2023-05-04 03:48:53.000000 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-04 03:48:53.000000 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 03:48:53.000000 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-04 03:48:53.000000 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 03:48:53.000000 relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/
+-rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4105 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-09 23:44:23.000000 relative_dose_1d-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1414 2023-05-08 22:29:08.000000 relative_dose_1d-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:47:06.916575 relative_dose_1d-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.813105 relative_dose_1d-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.864545 relative_dose_1d-0.1.3/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     9352 2023-05-03 01:27:57.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/__init__.py
+-rw-rw-rw-   0        0        0     9133 2023-05-08 22:22:38.000000 relative_dose_1d-0.1.3/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:47:06.904500 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     4105 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 23:47:06.000000 relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.1.2/LICENSE` & `relative_dose_1d-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.2/PKG-INFO` & `relative_dose_1d-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: relative_dose_1d
-Version: 0.1.2
-Summary: Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison.
+Version: 0.1.3
+Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
-Project-URL: homepage, https://github.com/LuisOlivaresJ/relative_dose_1d
+Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
-Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d
+Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
@@ -17,43 +17,40 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # relative_dose_1d
 
-Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison.
+Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
+## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
+
 ## Format specifications
 The data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
-* File in w2CAD format (format used by the TPS Eclipse 16.1, from the Varian(R) company).
+* File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
 
-* File in mcc format (format used by Verisoft 7.1.0.199 software, from PTW(R) company).
+* File in mcc format (used by Verisoft 7.1.0.199 software, from PTW(R) company).
   In the algorithm, the beginning of the data is identified by the word: 'BEGIN_DATA'
   Physical unit assumed to be in mm.
 
 * File in text format
   The data must be distributed in M ​​rows by 2 columns and separated
   for a blank space.
   The script ask for a word to identify the beginning of the data in the text file, 
   a number to add to the positions, and a factor for distance dimension conversion.
 
-For proper operation, the text file must meet the following characteristics:
-
-1. Contain a single profile
-2. The data should be in M ​​rows and two columns, (M, 2).
-
 ## Installation
 **Linux**<br/>
 The easiest method of installation is by typing in a terminal:
 ```bash
 pip install relative_dose_1d
 ```
 **Windows**<br/>
@@ -70,15 +67,28 @@
 ```
 Finally, write:
 
 ```python
 import relative_dose_1d.GUI
 ```
 
-## Versions
+## Contributing
+
+### Submitting bugs
+The easiest way to contribute is to report bugs. Submit bugs via a Github issue [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+### 
+Suggesting ideas
+Ideas are always welcome (though they might not get implemented). You can submit new ideas [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+## Changelog
 April-2023  Versión 0.0.3
   * *relative_dose_1d* is added to [PyPi](https://pypi.org/)
 
 May-2023 Version 0.1.0
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
+May-2023 Version 0.1.2
+  * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
+May-2023 Version 0.1.3
+  * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
```

### Comparing `relative_dose_1d-0.1.2/README.md` & `relative_dose_1d-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # relative_dose_1d
 
-Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison.
+Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
+## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
+
 ## Format specifications
 The data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
-* File in w2CAD format (format used by the TPS Eclipse 16.1, from the Varian(R) company).
+* File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
 
-* File in mcc format (format used by Verisoft 7.1.0.199 software, from PTW(R) company).
+* File in mcc format (used by Verisoft 7.1.0.199 software, from PTW(R) company).
   In the algorithm, the beginning of the data is identified by the word: 'BEGIN_DATA'
   Physical unit assumed to be in mm.
 
 * File in text format
   The data must be distributed in M ​​rows by 2 columns and separated
   for a blank space.
   The script ask for a word to identify the beginning of the data in the text file, 
   a number to add to the positions, and a factor for distance dimension conversion.
 
-For proper operation, the text file must meet the following characteristics:
-
-1. Contain a single profile
-2. The data should be in M ​​rows and two columns, (M, 2).
-
 ## Installation
 **Linux**<br/>
 The easiest method of installation is by typing in a terminal:
 ```bash
 pip install relative_dose_1d
 ```
 **Windows**<br/>
@@ -49,15 +46,28 @@
 ```
 Finally, write:
 
 ```python
 import relative_dose_1d.GUI
 ```
 
-## Versions
+## Contributing
+
+### Submitting bugs
+The easiest way to contribute is to report bugs. Submit bugs via a Github issue [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+### 
+Suggesting ideas
+Ideas are always welcome (though they might not get implemented). You can submit new ideas [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+## Changelog
 April-2023  Versión 0.0.3
   * *relative_dose_1d* is added to [PyPi](https://pypi.org/)
 
 May-2023 Version 0.1.0
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
+May-2023 Version 0.1.2
+  * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
+May-2023 Version 0.1.3
+  * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
```

### Comparing `relative_dose_1d-0.1.2/pyproject.toml` & `relative_dose_1d-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
-description = "Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison."
+description = "Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
@@ -28,16 +28,16 @@
 keywords = ["Radiotherapy", "Relative dose distribution", "gamma index", "python", "w2CAD", "mcc"]
 dependencies = [
   "numpy >= 1.23.4",
   "matplotlib >= 3.6.1",
   "PyQt6 >= 6.4.2",
 ]
 [project.urls]
-homepage = "https://github.com/LuisOlivaresJ/relative_dose_1d"
+homepage = "https://relative-dose-1d.readthedocs.io/en/latest/intro.html"
 repository = "https://github.com/LuisOlivaresJ/relative_dose_1d"
-Bug-Tracker = "https://github.com/LuisOlivaresJ/relative_dose_1d"
+Bug-Tracker = "https://github.com/LuisOlivaresJ/relative_dose_1d/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 dp_dep = ["*.csv", "*.png"]
```

### Comparing `relative_dose_1d-0.1.2/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.3/src/relative_dose_1d/GUI.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.1.2/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.3/src/relative_dose_1d/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,36 +38,38 @@
     ----------
 
     file_name : string
         Text file name
     
     Returns
     -------
-    out : list
+
+    list
         Loaded data as a list.
     
     """
     with open(file_name, encoding='UTF-8', mode = 'r') as file:
         data_list = [line.strip() for line in file]    
     return data_list
 
+
 def identify_format(data_list):
     """
     Identify text format.
 
     Parameters
     ----------
 
     data_list : list
         Each element of the list represents a line from the text file.
 
     Returns
     -------
 
-    out : string
+    string
         'varian' for w2CAD format, identified by the '$' character at the beginning of the file.
 
         'ptw' for mcc fromat, identified by the word 'BEGIN_SCAN_DATA'.
 
         'just_numbers' for data without headers.
         
         'text_file' for other formats. 
@@ -115,22 +117,17 @@
     delta : float 
         Displacement in mm to define the started point
     
         
     Returns
     -------
 
-    out : ndarray
+    ndarray
         Data as a Numpy object
     
-        
-    Examples
-    --------
-    (Todo) Add some exaples
-    
     """
 
     all_list = text_to_list(file_name)
     file_format = identify_format(all_list)
     
 
     #   w2CAD format (Varian)
@@ -147,15 +144,15 @@
         data_list = all_list[start_index: end_index]
         # Extraer datos de las lineas que comienzan con el caracter '<'
         data_list = [idx[1:-1].split() for idx in data_list if idx[0] == "<"]
         data_array = np.array(data_list).astype(float)
         data_array[:,1] = 100*data_array[:,1]/np.amax(data_array[:,1])
         
 
-    #   MCC format (PTW)     
+    #   mcc format (PTW)     
 
     elif file_format == 'ptw':
 
         start_index = all_list.index('BEGIN_DATA') + 1  
         end_index = all_list.index('END_DATA')          #Find the beginning and end of the data
         
         data_list = all_list[start_index: end_index]
@@ -193,15 +190,14 @@
         data_array[:,0] = data_array[:,0] + float(delta)
         
     
     return data_array
 
 
 def gamma_1D(ref, eval, dose_t = 3, dist_t = 2, dose_tresh = 0, interpol = 1):
-
     '''
     1-dimensional gamma index calculation.
     Dose profiles have to be normalized (0-100%).
 
     Parameters
     ----------
 
@@ -224,23 +220,24 @@
     
     interpol : float, default = 1
         Number of interpolated points to generate between each two consecutive points in "eval" data.
 
     Returns
     -------
 
-    out : ndarray, float
+    ndarray, float
         gamma distribution and gamma percent
+        
     '''
 
     # min_position and max_position to analize.
     min_position = np.max( (np.min(ref[:,0]), np.min([eval[:,0]])) )
     max_position = np.min( (np.max(ref[:,0]), np.max([eval[:,0]])) ) 
 
-    num_of_points = ref.shape[0]
+    num_of_points = eval.shape[0]
     interp_positions = np.linspace(ref[0,0], ref[-1,0], (interpol + 1)*(num_of_points - 1) + 1, endpoint=True)
     eval_from_interp_positions = np.interp(interp_positions, eval[:,0], eval[:,1], left = np.nan, right = np.nan) 
     add_positions = np.array((interp_positions, eval_from_interp_positions))
     eval_from_interp_positions = np.transpose(add_positions)
 
     #   A variable to storage gamma calculations.
     gamma = np.zeros( (num_of_points, 2) )
```

### Comparing `relative_dose_1d-0.1.2/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.3/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: relative-dose-1d
-Version: 0.1.2
-Summary: Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison.
+Version: 0.1.3
+Summary: Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
-Project-URL: homepage, https://github.com/LuisOlivaresJ/relative_dose_1d
+Project-URL: homepage, https://relative-dose-1d.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
-Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d
+Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d/issues
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
@@ -17,43 +17,40 @@
 Classifier: Natural Language :: Spanish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # relative_dose_1d
 
-Python package to read 1-dimensional dose profiles from text files and perform subtraction and gamma index comparison.
+Python package to read an 1-dimensional dose profile from text file and perform subtraction and gamma index comparison.
 
 ![image_gui](/docs/assets/GUI_v011.PNG)
 
+## [Documentation](https://relative-dose-1d.readthedocs.io/en/latest/intro.html)
+
 ## Format specifications
 The data should be in M ​​rows by 2 columns, corresponding to positions and
 dose values, respectively.
 
 The package has been tested with the following examples:
 
-* File in w2CAD format (format used by the TPS Eclipse 16.1, from the Varian(R) company).
+* File in w2CAD format (used by the TPS Eclipse 16.1, from the Varian(R) company).
   In the algorithm, the start of the data is identified by the words: 'STOM' or 'STOD'
   Physical unit assumed to be in mm.
 
-* File in mcc format (format used by Verisoft 7.1.0.199 software, from PTW(R) company).
+* File in mcc format (used by Verisoft 7.1.0.199 software, from PTW(R) company).
   In the algorithm, the beginning of the data is identified by the word: 'BEGIN_DATA'
   Physical unit assumed to be in mm.
 
 * File in text format
   The data must be distributed in M ​​rows by 2 columns and separated
   for a blank space.
   The script ask for a word to identify the beginning of the data in the text file, 
   a number to add to the positions, and a factor for distance dimension conversion.
 
-For proper operation, the text file must meet the following characteristics:
-
-1. Contain a single profile
-2. The data should be in M ​​rows and two columns, (M, 2).
-
 ## Installation
 **Linux**<br/>
 The easiest method of installation is by typing in a terminal:
 ```bash
 pip install relative_dose_1d
 ```
 **Windows**<br/>
@@ -70,15 +67,28 @@
 ```
 Finally, write:
 
 ```python
 import relative_dose_1d.GUI
 ```
 
-## Versions
+## Contributing
+
+### Submitting bugs
+The easiest way to contribute is to report bugs. Submit bugs via a Github issue [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+### 
+Suggesting ideas
+Ideas are always welcome (though they might not get implemented). You can submit new ideas [here](https://github.com/LuisOlivaresJ/relative_dose_1d/issues).
+
+## Changelog
 April-2023  Versión 0.0.3
   * *relative_dose_1d* is added to [PyPi](https://pypi.org/)
 
 May-2023 Version 0.1.0
   * It is now possible to perform unit transformation for distance using a multiplication factor, and move the origin of the coordinate system.
 
+May-2023 Version 0.1.2
+  * New web page for documentation, following [PEP 287 – reStructuredText Docstring Format](https://peps.python.org/pep-0287/) and [napoleon extension](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html#module-sphinx.ext.napoleon)
 
+May-2023 Version 0.1.3
+  * [Interpolation error](https://github.com/LuisOlivaresJ/relative_dose_1d/issues/1) solved.
```

