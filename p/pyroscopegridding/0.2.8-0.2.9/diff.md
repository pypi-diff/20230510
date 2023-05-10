# Comparing `tmp/pyroscopegridding-0.2.8.tar.gz` & `tmp/pyroscopegridding-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegridding-0.2.8.tar", last modified: Wed May 10 00:24:00 2023, max compression
+gzip compressed data, was "pyroscopegridding-0.2.9.tar", last modified: Wed May 10 00:45:23 2023, max compression
```

## Comparing `pyroscopegridding-0.2.8.tar` & `pyroscopegridding-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:24:00.372280 pyroscopegridding-0.2.8/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:24:00.369273 pyroscopegridding-0.2.8/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.8/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:24:00.219272 pyroscopegridding-0.2.8/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.8/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.8/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10348 2023-04-14 22:25:02.000000 pyroscopegridding-0.2.8/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33842 2023-04-15 01:27:44.000000 pyroscopegridding-0.2.8/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.8/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29719 2023-05-10 00:23:04.000000 pyroscopegridding-0.2.8/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9304 2023-04-14 22:28:16.000000 pyroscopegridding-0.2.8/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.2.8/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-04-15 01:56:21.000000 pyroscopegridding-0.2.8/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.8/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:24:00.346273 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 00:23:59.000000 pyroscopegridding-0.2.8/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 00:24:00.376284 pyroscopegridding-0.2.8/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 00:23:57.000000 pyroscopegridding-0.2.8/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:45:23.630134 pyroscopegridding-0.2.9/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:45:23.623132 pyroscopegridding-0.2.9/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.2.9/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:45:23.476137 pyroscopegridding-0.2.9/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.2.9/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3851 2023-04-15 01:27:45.000000 pyroscopegridding-0.2.9/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10187 2023-05-10 00:45:01.000000 pyroscopegridding-0.2.9/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33125 2023-05-10 00:42:37.000000 pyroscopegridding-0.2.9/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10530 2023-04-14 22:28:03.000000 pyroscopegridding-0.2.9/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    29222 2023-05-10 00:41:12.000000 pyroscopegridding-0.2.9/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9123 2023-05-10 00:43:58.000000 pyroscopegridding-0.2.9/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14020 2023-05-10 00:43:38.000000 pyroscopegridding-0.2.9/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10669 2023-05-10 00:44:59.000000 pyroscopegridding-0.2.9/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5159 2023-04-15 01:01:16.000000 pyroscopegridding-0.2.9/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-05-10 00:45:23.602133 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    12160 2023-05-10 00:45:22.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-05-10 00:45:23.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-05-10 00:45:22.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-05-10 00:45:22.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       56 2023-05-10 00:45:22.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-05-10 00:45:22.000000 pyroscopegridding-0.2.9/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-05-10 00:45:23.632136 pyroscopegridding-0.2.9/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1777 2023-05-10 00:45:07.000000 pyroscopegridding-0.2.9/setup.py
```

### Comparing `pyroscopegridding-0.2.8/PKG-INFO` & `pyroscopegridding-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.8
+Version: 0.2.9
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.8/README.md` & `pyroscopegridding-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.2.9/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.2.9/pyroscopegridding/filter_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,14 @@
             #we try to map it to where data exists for lat and long
             #lat1 = lat1[np.logical_not(np.isnan(phy_vars1))]
             #lon1 = lon1[np.logical_not(np.isnan(phy_vars1))]
             lat1=[]
             lon1=[]
             
         #print("valid range: ", phy['valid_range'][p][0])
-        print("VARIABLE:", phy_list[p])
-        print("VALID RANGE: ",phy['valid_range'][p][0], " to ", phy['valid_range'][p][1])
         phy_vars1 = phy_vars1[np.logical_and(phy_vars1>=phy['valid_range'][p][0],phy_vars1<=phy['valid_range'][p][1])]
         
         #print("AFTER FILTER MAX: ", phy_vars1.max())
         #print("AFTER FILTER MIN: ", phy_vars1.min())
         
         lat1 = np.array(lat1) * float(geo['scale_factor'][0]) + float(geo['add_offset'][0])
         lat.append(lat1)
@@ -174,15 +172,15 @@
     # scale factors
     phy_vars = np.array(phy_vars) * float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
     for p in phy_vars:
         pass
         #print("FINAL MAXES HDF:", p.max())
     #print("latitude:", len(lat))
     #print("Physical:", len(phy_vars))
-    print("Metadata: ", metadata)
+    
 
     # probably should put in a check that lat lon phys has same length
     # sometimes phys var may differ between aerosol optical depth and angle
     # ALL variables must pass the filter test otherwise get rid of them
 
     return lat,lon,phy_vars, metadata
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.2.9/pyroscopegridding/grid_ncf.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,14 @@
     maxlat=float(limit[1])
     minlon=float(limit[2])
     maxlon=float(limit[3])
     
     # pixel dimensions
     lat_dim = int(1+round(((maxlat-minlat)/gsize))) #int(1+round(((maxlat-minlat)/gsize)))
     lon_dim = int(1+round(((maxlon-minlon)/gsize))) #int(1+round(((maxlon-minlon)/gsize)))
-    print("LAT:" ,lat_dim)
-    print("LON:" ,lon_dim)
     
     #set target netcdf file
     ds = netCDF4.Dataset(filename, 'w',format='NETCDF4')
     
     #start_timer = time.time()
     time_date = time_start.strftime('%Y-%m-%d')
     time_time = time_start.strftime('%H:%M:%S.%f')[:-4]
@@ -108,15 +106,14 @@
     ds.RangeBeginningDate = time_date
     ds.RangeBeginningTime = time_time
     ds.RangeEndingDate = time_end_date
     ds.RangeEndingTime = time_end_time
     ds.ProcessingLevel = "Level 3"
     ds.ShortName = "AERDT_L3_MEASURES_QD_HH"
     
-    print("FILENAME:", filename)
     filename = convert_path_to_linux(filename) #convert to linux pwd
     cut_index = filename.rindex("/")
     filename_without_path = filename[cut_index+1 :]
     ds.GranuleID = filename_without_path
     
     production_yyyymmdd = filename_without_path[-11:-3]
     currtime = datetime.datetime.now()
@@ -200,15 +197,14 @@
         for name, dimension in src.dimensions.items():
             ds.createDimension(
                 name, (len(dimension) if not dimension.isunlimited() else None))
         """
         # copy all file data in the specified variables
         for name, variable in src.variables.items():
             if name in static_vars:
-                print(name)
                 dimensions = ('time', 'lat', 'lon',)
                 x = ds.createVariable(name, variable.datatype, dimensions) #variable.dimensions)
                 #ds[name][:] = src[name][:]
                 ds[name][0, :, :] = src[name][:]
                 #print(ds[name][:])
                 # copy variable attributes all at once via dictionary
                 ds[name].setncatts(src[name].__dict__)
@@ -297,15 +293,14 @@
         start_timer = time.time()
 
         for s in filelist.get(s_name):
             print("WORK SENSOR: ", s_name)
             print("FILE ORIGINAL: ", str(s))
             if not os.path.exists(s):
                 s = convert_to_other_system(s)
-            print("FILE INPUT: ", str(s))
             
             L2FID,GeoID,PhyID = open_file(s)
 
             # check for hdf files 
             if (str(s).split(".")[-1] == "hdf"):
                 geo_list = ['Latitude', 'Longitude']
                 lat,lon,phy_vars, meta = filter_data_hdf(GeoID, PhyID, geo_list, phy_list, phy_hdf)
@@ -424,37 +419,31 @@
                     else:
                         rotated = list(zip(*avgtau))[::-1]
                         
                         leogeo_stats_arr[p_vars]["Mean"].append(np.flipud(rotated))
                         #leogeo_stats["Mean"].append(np.flipud(rotated)) #for leogeo calculation later
                         print("STATISTIC ERROR")
                     
-                    print("ROTATED AOD for", aod_stat)
                     #print(np.flipud(rotated))
                     
                     #manually set to fill_value
                     rotated = np.array(rotated)
-                    print("VALID RANGE:", meta[j]["valid_range"][0], " TO ", meta[j]["valid_range"][1])
                     rotated[rotated > meta[j]["valid_range"][1]+1] = -800#meta[j]["_FillValue"]
                     rotated[rotated < meta[j]["valid_range"][0]-1] = -800 #meta[j]["_FillValue"]
                     
                     final_input = np.flipud(rotated)#.astype(np.short)
                     final_input = final_input #/meta[j]["scale_factor"]
-                    print(final_input)
                     #curr_sensor_value = values[index]
                     #values[index][0, :, :] = values[index][0, :, :].astype(np.short)
                     values[index][0, :, :] = final_input 
                     values[index][0, :, :] = values[index][0, :, :].astype("f4")
                     #values[index][0, :, :] = (values[index][0, :, :]*meta[j]["scale_factor"]).astype(np.short)
 
                     # AOD print
-                    print("AFTER ASSIGNMENT: ",final_input)
-                    print("TYPE: ", values[index][0, :, :].dtype)
-                    print("AOD nc check: ", np.array(values[index][0, :, :] ))
-                    
+                   
                     sensors[p_vars].append(np.flipud(rotated)) #add it to complete dataset for LEOGEO calculations
                     
                 #time
                 end_timer = time.time()
                 print("Sensor: ",s_name ," time: ", end_timer - start_timer)
                 
             else:  #phy_var is NOT AOD
@@ -483,15 +472,14 @@
                 
                 rotated = list(zip(*avgtau))[::-1]
                 #print("ROTATED NON AOD")
                 #print(np.flipud(rotated)) # print what is input into the variable
                 
                 #manually set to fill_value
                 rotated = np.array(rotated)
-                print("VALID RANGE:", meta[j]["valid_range"][0], " TO ", meta[j]["valid_range"][1])
                 rotated[rotated > meta[j]["valid_range"][1]+1] = meta[j]["_FillValue"]
                 rotated[rotated < meta[j]["valid_range"][0]-1] = meta[j]["_FillValue"]
                 
                 
                 values[index][0, :, :] = np.flipud(rotated) # put into variable
                 #sensors[p_vars].append(np.flipud(rotated)) #add it to complete dataset for LEOGEO calculations
 
@@ -669,19 +657,17 @@
             print(sensors.get(p_vars))
     """
 
     # print modis mean again
     #print(values)
     #print(values[0])
     #print(values[0].long_name)
-    print("CHECK 1")
     #close file
     #ds.close()
     #grid_close(ds)s
-    print("CHECK 2")
     
     
     return ds
     # output = 1 netcdf with six variables (one for each sensor) 
     # merge = run two loops (lat lon) (xdim, ydim from grid) 
     # merge aod equal to average of six sensors making sure no nan
     # identify which sensors are availabe - sensor ID variable 0 or 1 (unavailable vs available)
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/gridding.py` & `pyroscopegridding-0.2.9/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/gtools.py` & `pyroscopegridding-0.2.9/pyroscopegridding/gtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,49 +138,38 @@
     print("Results at: " + output)
 
     grid_ncf.gridNC_single(limit, gsize, indata, inlat, inlon, output)
 """
 #gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, sat_files[:10], fpath + "viirs_time_compv1.nc")
 def netCDF_multi(filelist, geo_list, phy_list, output):
     geo_list = geo_list.split(" ")
-    print(geo_list)
+
     phy_list = phy_list.split(" ")
-    print(phy_list)
     filelist = read_file_sat_data(filelist)
 
-    print(filelist)
-
     lat,lon,phy_vars = multi_sensor_grid_data(filelist, phy_list, geo_list)
 
-    print(lat)
-    print(lon)
-    print(phy_vars)
-
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = 0.25
     indata = phy_vars
     inlat=lat
     inlon = lon
 
-    print("Results at: " + output)
-
     #grid_ncf.gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, filelist, output)
     
     #grid_ncf.gridNC_time(limit, gsize, indata, inlat, inlon, output)
 
 
     
 def netCDF_multi_time(filelist, gsize, geo_list, phy_list, output, time_interval, time_start, time_end):
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
     filelist = read_file_sat_data(filelist)
 
     start = to_datetime(time_start)
     end = to_datetime(time_end)
 
     split_files = split_filetimes(filelist, start, end, int(time_interval))
 
@@ -198,17 +187,15 @@
     print("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_sensor_statistics(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
     start_timer = time.time()
     
     geo_list = geo_list.split(" ")
-    print(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = read_file_sat_data(filelist)
 
     start = to_datetime(time_start)
     end = to_datetime(time_end)
 
     split_files = split_filetimes(filelist, start, end, int(time_interval))
@@ -228,17 +215,15 @@
 
 # output - folder location
 def netCDF_sensor_statistics_split(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
 
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = read_file_sat_data(filelist)
 
     start = to_datetime(time_start)
     end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -264,17 +249,15 @@
 
 # output - folder location
 def netCDF_sensor_statistics_id(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
 
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = read_file_sat_data(filelist)
 
     start = to_datetime(time_start)
     end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -323,15 +306,14 @@
             filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
         filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
         
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
-    print("static file:", static_file)
 
     time_start = grid_settings["time_start"]
     time_end = grid_settings["time_end"]
     start = to_datetime(time_start)
     end = to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -397,18 +379,16 @@
         if file_io["file_location_folder"] == "NA":
             filelist = read_file_sat_data(file_io["file_location_file"])
         else:
             filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
         filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
-    print("FILELIST: ", filelist)
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
-    print("static file:", static_file)
 
     #time_start = grid_settings["time_start"]
     #time_end = grid_settings["time_end"]
     start = to_datetime(time_start)
     end = to_datetime(time_end)
     
 
@@ -432,21 +412,19 @@
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = sys_time()
         
         if not os.path.exists(outputfolder):
-            print("/n/nCONVERT/n/n")
             outputfolder = convert_to_other_system(outputfolder)
             
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
         
-        print("USED NAME: ", name)
         ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
     print("Full execution time: ", end_timer - start_timer)
 
@@ -470,18 +448,18 @@
         if file_io["file_location_folder"] == "NA":
             filelist = read_file_sat_data(file_io["file_location_file"])
         else:
             filelist = read_folder_sat_data(file_io["file_location_folder"])
     else:
         filelist = read_directory_sat_data(file_io["file_directory_folder"])
         
-    print("FILELIST: ", filelist)
+    #print("FILELIST: ", filelist)
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
-    print("static file:", static_file)
+    #print("static file:", static_file)
 
     time_start = grid_settings["time_start"]
     time_end = grid_settings["time_end"]
     start = to_datetime(time_start)
     end = to_datetime(time_end)
     
 
@@ -504,14 +482,15 @@
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = sys_time()
         if not os.path.exists(outputfolder):
             outputfolder = convert_to_other_system(outputfolder)
+            
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
         
         ds = grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.2.9/pyroscopegridding/naming_conventions.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,17 +143,15 @@
         #print("ORIGINAL DATA2:", data)
         
         #avgtau = np.nanmean(np.array(data), axis=0 )
         avgtau = avgtau/scale_factor
         
         avgtau[avgtau > 5001] = -9999
         avgtau[avgtau < -101] = -9999
-        
-        print("AVGTAU LEOGEO TYPE: ", avgtau.dtype)
-    
+           
         return avgtau
     
     # https://stats.stackexchange.com/questions/55999/is-it-possible-to-find-the-combined-standard-deviation
     if statistic == "STD":
         
         # [[std g16], [ g17], []]
         """
@@ -200,11 +198,8 @@
     #data = np.array([[[0,1],[2,3]], [[1,2], [3, 4]]])
     #print(np.nanmean(np.array(data), axis=0 ))
     
     #path = "/mnt/c/Users/bobgr/Desktop/NASA Spring 2023/Gridtools Package (Code, README, inputs, outputs, examples, verification)/SampleOutputs 0000-0059 01-01-2020/"
     #filename = "XAERDT_L3_MEASURES_QD_HH.20200101.0000.V0.20230130.nc"
     #L2FID = netCDF4.Dataset(path+filename,'r',format='NETCDF4')
     #L2FID.close()
-    
-    print(data)
-    print("MEAN:", calculate_statistic("Mean", data))
-    print("STD:", calculate_statistic("STD", data))
+
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.2.9/pyroscopegridding/sat_data_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
          #L2FID = SD.SD(L2FileName)
          L2FID = netCDF4.Dataset(L2FileName,'r',format='HDF') 
       except:
          #print("touching")
          os.touch(L2FileName)
       """
       L2FID = SD.SD(L2FileName)
-      print("HDF\n:", L2FID)
+      print("HDF:", L2FileName)
       #L2FID = netCDF4.Dataset(L2FileName,'r')#,format='HDF') 
       
    ftype = os.path.splitext(L2FileName)[1]
    GeoGroupID = L2FID
    PhyGroupID = L2FID
     
    if ftype != '.hdf':
@@ -308,24 +308,20 @@
          phy['long_name'].append(metadata["long_name"])
          phy['units'].append(metadata["units"])
          phy['scale_factor'].append(metadata["scale_factor"])
          phy['add_offset'].append(metadata["add_offset"])
          phy['Parameter_Type'].append(metadata["Parameter_Type"])
          
          #display data
-         print("DATA")
          data2 = np.array(data).flatten()
-         print(data2[data2!=-9999])
-         
          
          
       except: # varaible not found
          raise AttributeError("No such variable", var_list[i])      
      
-   print("HDF:", phy)    
    return(phy)
 
 # nc
 # Parses the geophysical group after file is read
 # Variables are aod by default only
 def read_phy_data_hdf_vnew(L2PhyGroup, L2GeoGroup, var_list=None, var_hdf=None):
    if var_list is None:
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.2.9/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.2.9/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.2.9/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegridding
-Version: 0.2.8
+Version: 0.2.9
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: # README
```

### Comparing `pyroscopegridding-0.2.8/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.2.9/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.2.8/setup.py` & `pyroscopegridding-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.2.8',      # Initial version
+    version = '0.2.9',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

