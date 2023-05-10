# Comparing `tmp/pyroscopegridding-0.3.1.1.tar.gz` & `tmp/pyroscopegridding-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.3.1.1.tar", last modified: Wed May 10 18:19:00 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.3.1.2.tar", last modified: Wed May 10 20:36:55 2023, max compression
```

## Comparing `pyroscopegridding-0.3.1.1.tar` & `pyroscopegridding-0.3.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 18:19:00.897650 pyroscopegridding-0.3.1.1/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 18:19:00.889551 pyroscopegridding-0.3.1.1/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.1/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 18:19:00.136534 pyroscopegridding-0.3.1.1/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10710 2023-05-10 18:17:51.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1.1/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 18:19:00.849326 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 18:18:59.000000 pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 18:19:00.899652 pyroscopegridding-0.3.1.1/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-10 18:18:02.000000 pyroscopegridding-0.3.1.1/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:36:55.266845 pyroscopegridding-0.3.1.2/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 20:36:55.262846 pyroscopegridding-0.3.1.2/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.3.1.2/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:36:55.099843 pyroscopegridding-0.3.1.2/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6684 2023-05-10 20:36:03.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13920 2023-05-10 01:02:30.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10710 2023-05-10 18:17:51.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.3.1.2/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 20:36:55.235846 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12162 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 20:36:54.000000 pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 20:36:55.268843 pyroscopegridding-0.3.1.2/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1779 2023-05-10 20:36:10.000000 pyroscopegridding-0.3.1.2/setup.py
```

### Comparing `pyroscopegridding-0.3.1.1/PKG-INFO` & `pyroscopegridding-0.3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.1/README.md` & `pyroscopegridding-0.3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/gtools.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.3.1.2/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.3.1.1/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.3.1.2/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.3.1.1/setup.py` & `pyroscopegridding-0.3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.3.1.1',      # Initial version
+    version = '0.3.1.2',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

