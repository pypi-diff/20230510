# Comparing `tmp/SeanFunctions-0.4.7.tar.gz` & `tmp/SeanFunctions-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.4.7.tar", last modified: Tue Apr 18 20:12:09 2023, max compression
+gzip compressed data, was "SeanFunctions-0.5.0.tar", last modified: Tue May  9 21:50:05 2023, max compression
```

## Comparing `SeanFunctions-0.4.7.tar` & `SeanFunctions-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-18 20:12:09.216758 SeanFunctions-0.4.7/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/.gitignore
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.4.7/LICENSE
--rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/MANIFEST.in
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-18 20:12:09.216454 SeanFunctions-0.4.7/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.4.7/README.md
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-04-18 16:28:59.000000 SeanFunctions-0.4.7/pyproject.toml
--rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-04-18 20:12:09.216814 SeanFunctions-0.4.7/setup.cfg
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-18 20:12:09.211755 SeanFunctions-0.4.7/src/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-18 20:12:09.214536 SeanFunctions-0.4.7/src/SeanFunctions/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-18 20:12:09.216088 SeanFunctions-0.4.7/src/SeanFunctions/Data/
--rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/src/SeanFunctions/__init__.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     4719 2023-04-18 20:11:26.000000 SeanFunctions-0.4.7/src/SeanFunctions/fitting.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     9393 2023-04-14 16:08:58.000000 SeanFunctions-0.4.7/src/SeanFunctions/math.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     4166 2023-01-14 21:57:03.000000 SeanFunctions-0.4.7/src/SeanFunctions/scattering.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-04-18 20:12:09.000000 SeanFunctions-0.4.7/src/SeanFunctions/version.py
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-04-18 20:12:09.215118 SeanFunctions-0.4.7/src/SeanFunctions.egg-info/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-04-18 20:12:09.000000 SeanFunctions-0.4.7/src/SeanFunctions.egg-info/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-04-18 20:12:09.000000 SeanFunctions-0.4.7/src/SeanFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-04-18 20:12:09.000000 SeanFunctions-0.4.7/src/SeanFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-04-18 20:12:09.000000 SeanFunctions-0.4.7/src/SeanFunctions.egg-info/top_level.txt
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.133871 SeanFunctions-0.5.0/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/.gitignore
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.5.0/LICENSE
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/MANIFEST.in
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-09 21:50:05.133551 SeanFunctions-0.5.0/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.5.0/README.md
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-05-09 21:38:49.000000 SeanFunctions-0.5.0/pyproject.toml
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-05-09 21:50:05.133926 SeanFunctions-0.5.0/setup.cfg
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.128271 SeanFunctions-0.5.0/src/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.131547 SeanFunctions-0.5.0/src/SeanFunctions/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.133200 SeanFunctions-0.5.0/src/SeanFunctions/Data/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/__init__.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     4717 2023-04-19 13:48:50.000000 SeanFunctions-0.5.0/src/SeanFunctions/fitting.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     9393 2023-04-14 16:08:58.000000 SeanFunctions-0.5.0/src/SeanFunctions/math.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    12866 2023-05-09 21:48:13.000000 SeanFunctions-0.5.0/src/SeanFunctions/scattering.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions/version.py
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.132357 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.4.7/LICENSE` & `SeanFunctions-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.7/PKG-INFO` & `SeanFunctions-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.7
+Version: 0.5.0
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.7/pyproject.toml` & `SeanFunctions-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SeanFunctions"
-version = "0.4.7"
+version = "0.5.0"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.5.0/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions/fitting.py` & `SeanFunctions-0.5.0/src/SeanFunctions/fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         params['gamma'].set(**gammaParams)
     
     fitResult = modCombined.fit(fity,params,x=fitx)
     
     return fitResult
 
 
-def find_max(fitfunction,bounds,min=False,evalUnc=True,params=params):
+def find_max(fitfunction,bounds,min=False,evalUnc=True,params=None):
     '''
     Finds the maximum value of a Gaussian shaped function determined through a fit
 
     Parameters
     ---------
     fitfunction : lmfit fitted class
         Fitting result from lmfit
```

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions/math.py` & `SeanFunctions-0.5.0/src/SeanFunctions/math.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions.egg-info/PKG-INFO` & `SeanFunctions-0.5.0/src/SeanFunctions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.4.7
+Version: 0.5.0
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.4.7/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.5.0/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

