# Comparing `tmp/pyroscopegridding-0.2.6.tar.gz` & `tmp/pyroscopegridding-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.2.6.tar", last modified: Wed May 10 00:11:35 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.2.7.tar", last modified: Wed May 10 00:17:33 2023, max compression
```

## Comparing `pyroscopegridding-0.2.6.tar` & `pyroscopegridding-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:11:35.130601 pyroscopegridding-0.2.6/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:11:35.127597 pyroscopegridding-0.2.6/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.6/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:11:34.979597 pyroscopegridding-0.2.6/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.6/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.6/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.6/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.6/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.6/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29627 2023-05-10 00:08:03.000000 pyroscopegridding-0.2.6/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.6/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.6/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.6/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.6/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:11:35.105597 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 00:11:34.000000 pyroscopegridding-0.2.6/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 00:11:35.132595 pyroscopegridding-0.2.6/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 00:10:25.000000 pyroscopegridding-0.2.6/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:17:33.559726 pyroscopegridding-0.2.7/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:17:33.555729 pyroscopegridding-0.2.7/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.7/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:17:33.423726 pyroscopegridding-0.2.7/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.7/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.7/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.7/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.7/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.7/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29685 2023-05-10 00:17:09.000000 pyroscopegridding-0.2.7/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.7/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.7/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.7/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.7/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:17:33.535725 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 00:17:33.000000 pyroscopegridding-0.2.7/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 00:17:33.561726 pyroscopegridding-0.2.7/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 00:17:30.000000 pyroscopegridding-0.2.7/setup.py
```

### Comparing `pyroscopegridding-0.2.6/PKG-INFO` & `pyroscopegridding-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.6/README.md` & `pyroscopegridding-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.7/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.7/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.7/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.7/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.7/pyroscopegridding/gtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,18 +430,21 @@
     count= 0
     for f in split_files:
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = sys_time()
-        name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
-        if not os.path.exists(name):
+        
+        if not os.path.exists(outputfolder):
             print("/n/nCONVERT/n/n")
-            name = convert_to_other_system(name)
+            outputfolder = convert_to_other_system(outputfolder)
+            
+        name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
+        
         
         print("USED NAME: ", name)
         ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
```

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.7/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.7/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.7/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.7/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.2.7/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.6/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.7/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.6/setup.py` & `pyroscopegridding-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.2.6',      # Initial version
+    version = '0.2.7',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

