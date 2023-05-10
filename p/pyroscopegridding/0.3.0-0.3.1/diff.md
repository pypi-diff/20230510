# Comparing `tmp/pyroscopegridding-0.3.0.tar.gz` & `tmp/pyroscopegridding-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.3.0.tar", last modified: Wed May 10 01:01:10 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.3.1.tar", last modified: Wed May 10 01:02:58 2023, max compression
```

## Comparing `pyroscopegridding-0.3.0.tar` & `pyroscopegridding-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:01:10.064669 pyroscopegridding-0.3.0/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 01:01:10.059667 pyroscopegridding-0.3.0/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.0/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:01:09.920668 pyroscopegridding-0.3.0/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.0/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.0/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.0/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.0/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.3.0/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.0/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.3.0/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:00:07.000000 pyroscopegridding-0.3.0/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-05-10 00:44:59.000000 pyroscopegridding-0.3.0/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.0/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:01:10.038669 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 01:01:09.000000 pyroscopegridding-0.3.0/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 01:01:10.065666 pyroscopegridding-0.3.0/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 01:01:06.000000 pyroscopegridding-0.3.0/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:02:58.353948 pyroscopegridding-0.3.1/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 01:02:58.348947 pyroscopegridding-0.3.1/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:02:58.202944 pyroscopegridding-0.3.1/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.3.1/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.3.1/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-05-10 00:44:59.000000 pyroscopegridding-0.3.1/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 01:02:58.327943 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 01:02:57.000000 pyroscopegridding-0.3.1/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 01:02:58.354946 pyroscopegridding-0.3.1/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 01:02:48.000000 pyroscopegridding-0.3.1/setup.py
```

### Comparing `pyroscopegridding-0.3.0/PKG-INFO` & `pyroscopegridding-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.0/README.md` & `pyroscopegridding-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.3.1/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.3.1/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.3.1/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/gridding.py` & `pyroscopegridding-0.3.1/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/gtools.py` & `pyroscopegridding-0.3.1/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.3.1/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.3.1/pyroscopegridding/sat_data_input.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 def open_file(L2FileName):
    if not os.path.isfile(L2FileName):
       err = "Error: file not exis {} ... ".format(L2FileName)
       print(err)
 
       return(False)
    
+   ftype = os.path.splitext(L2FileName)[1]
    """
    try: # netcdf
       #print("OPENED AS NETCDF")
       L2FID = netCDF4.Dataset(L2FileName,'r',format='NETCDF4')
    except:
       L2FID = SD.SD(L2FileName)
       print("HDF:", L2FileName)
       #L2FID = netCDF4.Dataset(L2FileName,'r')#,format='HDF') 
    """
    if ftype != '.hdf':
       L2FID = netCDF4.Dataset(L2FileName,'r',format='NETCDF4')
    else:
       L2FID = SD.SD(L2FileName)
    
-   ftype = os.path.splitext(L2FileName)[1]
    GeoGroupID = L2FID
    PhyGroupID = L2FID
     
    if ftype != '.hdf':
       GeoGroupID =  L2FID.groups['geolocation_data']
       PhyGroupID =  L2FID.groups['geophysical_data']
```

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.3.1/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.3.1/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.3.1/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.0/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.3.1/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.0/setup.py` & `pyroscopegridding-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.3.0',      # Initial version
+    version = '0.3.1',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

