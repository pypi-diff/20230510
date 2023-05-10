# Comparing `tmp/iosense_connect-2.1.1.tar.gz` & `tmp/iosense_connect-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.1.tar", last modified: Thu May  4 07:23:40 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.2.tar", last modified: Wed May 10 12:01:34 2023, max compression
```

## Comparing `iosense_connect-2.1.1.tar` & `iosense_connect-2.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.009220 iosense_connect-2.1.1/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.1/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    19576 2023-05-04 07:23:32.000000 iosense_connect-2.1.1/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-04 07:23:31.000000 iosense_connect-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.912703 iosense_connect-2.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-10 12:01:34.909015 iosense_connect-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.621196 iosense_connect-2.1.2/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.2/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    22027 2023-05-10 12:00:03.000000 iosense_connect-2.1.2/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:01:34.900920 iosense_connect-2.1.2/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 12:01:33.000000 iosense_connect-2.1.2/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:01:34.913701 iosense_connect-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-10 11:59:25.000000 iosense_connect-2.1.2/setup.py
```

### Comparing `iosense_connect-2.1.1/LICENSE.txt` & `iosense_connect-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.1/PKG-INFO` & `iosense_connect-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.1
+Version: 2.1.2
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.1/README.md` & `iosense_connect-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.1/iosense_connect/data_access.py` & `iosense_connect-2.1.2/iosense_connect/data_access.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,47 @@
-# import libraries
 import json
+import os
+import re
 import sys
 import time
-from datetime import datetime, timedelta
 import numpy as np
 import pandas as pd
 import requests
 import urllib3
+from azure.storage.blob import BlobServiceClient
+from concurrent.futures import ThreadPoolExecutor
+from datetime import datetime, timezone
+from datetime import timedelta
 
 pd.options.mode.chained_assignment = None
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class DataAccess:
-
-    def __init__(self, userID, url):
-        self.userID = userID
+    def __init__(self, userid, url, connection_string, container_name):
+        self.userid = userid
         self.url = url
+        self.connection_string = connection_string
+        self.container_name = container_name
 
-    def get_device_metadata(self, device_id):
-        """
-
-        :param device_id: string
-        :return: Json
-
-         Every detail related to a particular device like device added date, m,c,min,max values, sensor id, sensor alias and so on
-
-        """
-        try:
-            url = "https://" + self.url + "/api/metaData/device/" + device_id
-            header = {'userID': self.userID}
-            payload = {}
-            response = requests.request('GET', url, headers=header, data=payload, verify=False)
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
-
-        except Exception as e:
-            print('Failed to fetch device Metadata')
-            print(e)
-
-    def get_sensor_alias(self, device_id, df, raw_metadata):
+    def get_caliberation(self, device_id, metadata, df,onpremise=False):
         """
-
-        :param raw_metadata: json of device metadata
-        :param device_id: string
+        :param metadata:
         :param df: Dataframe
-        :return: dataframe with columns having sensor alias
-
-        Maps sensor_alias/ sensor name with corresponding sensor ID
-        replaces column names with sensor_alias_sensor_id
-
-        """
-
-        list1 = list(df['sensor'].unique())
-
-        if len(raw_metadata) == 0:
-            raw_metadata = DataAccess.get_device_metadata(self, device_id)
-
-        sensor_spec = 'sensors'
-        sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
-
-        for i in list1:
-            sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == i]
-            if len(sensor_param_df1) != 0:
-                sensor_name = sensor_param_df1.iloc[0]['sensorName']
-                sensor_name = sensor_name + " (" + i + ")"
-                df['sensor'] = df['sensor'].replace(i, sensor_name)
-        return df, raw_metadata
-
-    def get_caliberation(self, device_id, metadata, df):
-        """
-
-        :param df_raw: Dataframe
         :param device_id: string
         :return: Calibrated dataframe
 
         Perform cal on original data
              y = mx + c
              if y is greater than max value replace y with max value
              if y is less than min value replace y with min value
 
         """
         sensor_name_list = list(df.columns)
         sensor_name_list.remove('time')
-
         if "(" not in sensor_name_list[0]:
             sensor_id_list = sensor_name_list
         else:
             sensor_id_list = [s[s.rfind("(") + 1:s.rfind(")")] for s in sensor_name_list]
 
         if len(metadata) == 0:
             metadata = DataAccess.get_device_metadata(self, device_id)
@@ -113,15 +63,70 @@
                     df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
                 if 'max' in df_meta.columns:
                     max = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
                         '1000000000000000000000000000', '99999').replace('100000000000', '99999'))
                     df[str(value2)] = np.where(df[str(value2)] >= max, max, df[str(value2)])
         return df
 
-    def time_grouping(self, df, bands):
+    def get_device_metadata(self, device_id,onpremise=False):
+        """
+
+        :param device_id: string
+        :return: Json
+
+         Every detail related to a particular device like device added date, calibration values, sensor details etc
+
+        """
+        try:
+            if str(onpremise).lower() == 'true':
+                url = "http://" + self.url + "/api/metaData/device/" + device_id
+            else:
+                url = "https://" + self.url + "/api/metaData/device/" + device_id
+            header = {'userID': self.userid}
+            payload = {}
+            response = requests.request('GET', url, headers=header, data=payload, verify=False)
+
+            if response.status_code != 200:
+                raw = json.loads(response.text)
+                raise ValueError(raw['error'])
+            else:
+                raw_data = json.loads(response.text)['data']
+                return raw_data
+
+        except Exception as e:
+            print('Failed to fetch device Metadata')
+            print(e)
+
+    def get_sensor_alias(self, device_id, df, raw_metadata,onpremise=False):
+        """
+
+        :param raw_metadata: json of device metadata
+        :param device_id: string
+        :param df: Dataframe
+        :return: dataframe with columns having sensor alias
+
+        Maps sensor_alias/ sensor name with corresponding sensor ID
+        replaces column names with sensor_alias_sensor_id
+
+        """
+        sensors = list(df.columns)
+        sensors.remove('time')
+        if len(raw_metadata) == 0:
+            raw_metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+        sensor_spec = 'sensors'
+        sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
+        for sensor in sensors:
+            sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == sensor]
+            if len(sensor_param_df1) != 0:
+                sensor_name = sensor_param_df1.iloc[0]['sensorName']
+                sensor_name = sensor_name + " (" + sensor + ")"
+                df.rename(columns={sensor:sensor_name},inplace=True)
+        return df, raw_metadata
+
+    def time_grouping(self, df, bands,compute=None):
         """
 
         :param df: DataFrame
         :param bands: 05,1W,1D
         :return: Dataframe
 
         Group time series DataFrame
@@ -130,15 +135,18 @@
         """
 
         df['Time'] = pd.to_datetime(df['time'])
         df.sort_values("Time", inplace=True)
         df = df.drop(['time'], axis=1)
         df = df.set_index(['Time'])
         df.index = pd.to_datetime(df.index)
-        df = df.groupby(pd.Grouper(freq=str(bands) + "Min", label='right')).mean()
+        if compute is None:
+            df = df.groupby(pd.Grouper(freq=str(bands) + "Min")).mean()
+        else:
+            df = df.groupby(pd.Grouper(freq=str(bands) + "Min")).apply(compute)
         df.reset_index(drop=False, inplace=True)
         return df
 
     def get_cleaned_table(self, df):
         """
 
         :param df: Raw Dataframe
@@ -151,25 +159,28 @@
 
         df = df.sort_values('time')
         df.reset_index(drop=True, inplace=True)
         results = df.pivot(index='time', columns='sensor', values='value')
         results.reset_index(drop=False, inplace=True)
         return results
 
-    def get_device_details(self):
+    def get_device_details(self,onpremise=False):
         """
 
         :return: Details Device id and Device Name of a particular account
 
-        Dataframe with list of device ids and device names.
+        Dataframe with columne device ids and device names.
 
         """
         try:
-            url = "https://" + self.url + "/api/metaData/allDevices"
-            header = {'userID': self.userID}
+            if str(onpremise).lower() == 'true':
+                url = "http://" + self.url + "/api/metaData/allDevices"
+            else:
+                url = "https://" + self.url + "/api/metaData/allDevices"
+            header = {'userID': self.userid}
             payload = {}
             response = requests.request('GET', url, headers=header, data=payload, verify=False)
 
             if response.status_code != 200:
                 raw = json.loads(response.text)
                 raise ValueError(raw['error'])
             else:
@@ -177,60 +188,44 @@
                 df_raw = pd.DataFrame(raw_data)
                 return df_raw
 
         except Exception as e:
             print('Failed to fetch device Details')
             print(e)
 
-    def get_userinfo(self):
-        """
-        :return: Json
-
-        Details like phone,name,gender,emailed etc are fetched
-        """
-        try:
-            url = "https://" + self.url + "/api/metaData/user"
-            header = {'userID': self.userID}
-            payload = {}
-            response = requests.request('GET', url, headers=header, data=payload, verify=False)
-
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
-
-        except Exception as e:
-            print('Failed to fetch user Information')
-            print(e)
-
-    def get_dp(self, device_id, sensors, n=1, cal=True, alias=True, end_time=datetime.now(), IST=True):
+    def get_dp(self, device_id, sensors=None, n=1, cal=True, end_time=datetime.now(),alias=True, IST=True,onpremise=False):
         """
 
         :param device_id: string
-        :param sensors: list of sensors
+        :param sensors: IST of sensors
         :param n: number of data points (default: 1)
         :param cal: bool (default: True)
         :param end_time: 'YYYY:MM:DD HH:MM:SS'
-        :param IST: bool (default: True)
+        :param IST: bool (default: True) Indian Standard Timezone
         :return: Dataframe with values
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
-            df_devices = DataAccess.get_device_details(self)
-            device_list = df_devices['devID'].tolist()
-            if device_id not in device_list:
-                raise Exception('Message: Device not added')
+
             metadata = {}
+            if sensors == None:
+                metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
+                data_sensor = metadata['sensors']
+                df_sensor = pd.DataFrame(data_sensor)
+                sensor_id_list = list(df_sensor['sensorId'])
+                sensors = sensor_id_list
+
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
+            else:
+                if end_time == datetime.now:
+                    end_time=datetime.now(timezone.utc)
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
                 if len_sensors == 0:
                     raise Exception('Message: No sensors provided')
                 if n < 1:
                     raise ValueError('Incorrect number of data points')
@@ -245,59 +240,59 @@
             df = pd.DataFrame()
             counter = 0
             while True:
                 for record in range(counter):
                     sys.stdout.write('\r')
                     sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
                     sys.stdout.flush()
-                url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
+                if str(onpremise).lower() == "true":
+                    url = "http://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
+                        cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
+                else:
+                    url = "https://" + self.url + "/api/apiLayer/getLimitedDataMultipleSensors/?device=" + device_id + "&sensor=" + sensor_values + "&eTime=" + str(
                     cursor['end']) + "&lim=" + str(cursor['limit']) + "&cursor=true"
                 response = requests.request("GET", url, headers=header, data=payload)
                 raw = json.loads(response.text)
                 if response.status_code != 200:
                     raise ValueError(response.status_code)
                 if 'success' in raw:
                     raise ValueError(raw)
                 else:
                     raw_data = json.loads(response.text)['data']
                     cursor = json.loads(response.text)['cursor']
                     if len(raw_data) != 0:
                         df = pd.concat([df, pd.DataFrame(raw_data)])
                     counter = counter + 1
-                if cursor['end'] == None:
+                if cursor['end'] is None:
                     break
             if len(df) != 0:
                 if IST:
                     df['time'] = pd.to_datetime(df['time'], utc=False)
                     df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
                 if str(alias).lower() == "true":
-                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
-                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
+                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
                 df = DataAccess.get_cleaned_table(self, df)
                 if str(cal).lower() == 'true':
-                    df = DataAccess.get_caliberation(self, device_id, metadata, df)
+                    df = DataAccess.get_caliberation(self, device_id, metadata, df,onpremise=onpremise)
             return df
         except Exception as e:
             print(e)
 
-    def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, alias=True, cal=True, bands=None,
-                   IST=True,
-                   echo=True):
-        # df = pd.DataFrame()
-        df_devices = DataAccess.get_device_details(self)
-        device_list = df_devices['devID'].tolist()
-        if device_id not in device_list:
-            raise Exception('Message: Device not added')
+    def fetch_data(self, device_id,start_time, end_time=datetime.now(), alias=True,sensors=None, echo=True,onpremise=False,IST=True):
+        """
+        Fetch data from influxdb using apis in given timeslot
+        """
         metadata = {}
-        if sensors == None:
-            metadata = DataAccess.get_device_metadata(self, device_id)
+        if sensors is None:
+            metadata = DataAccess.get_device_metadata(self, device_id,onpremise=onpremise)
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
+
         rawdata_res = []
         temp = ''
         try:
             end_time = datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S')
         except Exception:
             if type(end_time) == str:
                 end_time = str(end_time) + " 23:59:59"
@@ -315,24 +310,19 @@
         cursor = {'start': st_time, 'end': en_time}
         while True:
             if echo:
                 for record in range(counter):
                     sys.stdout.write('\r')
                     sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
                     sys.stdout.flush()
-            if sensors is None:
-                url_api = "https://" + self.url + "/api/apiLayer/getDataByStEt?device="
-                if counter == 0:
-                    temp = url_api + device_id + "&sTime=" + str(st_time) + "&eTime=" + str(
-                        en_time) + "&cursor=true&limit=50000"
-                else:
-                    temp = url_api + device_id + "&sTime=" + str(cursor['start']) + "&eTime=" + str(
-                        cursor['end']) + "&cursor=true&limit=50000"
             if sensors is not None:
-                url_api = "https://" + self.url + "/api/apiLayer/getAllData?device="
+                if str(onpremise).lower() == 'true':
+                    url_api = "http://" + self.url + "/api/apiLayer/getAllData?device="
+                else:
+                    url_api = "https://" + self.url + "/api/apiLayer/getAllData?device="
                 if counter == 0:
                     str1 = ","
                     sensor_values = str1.join(sensors)
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         st_time) + "&eTime=" + str(
                         en_time) + "&cursor=true&limit=50000"
                 else:
@@ -340,166 +330,168 @@
                     sensor_values = str1.join(sensors)
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         cursor['start']) + "&eTime=" + str(cursor['end']) + "&cursor=true&limit=50000"
 
             response = requests.request("GET", temp, headers=header, data=payload)
             raw = json.loads(response.text)
             if response.status_code != 200:
-                raise ValueError(raw)
+                raise ValueError(raw['error'])
             if 'success' in raw:
-                raise ValueError(raw)
+                raise ValueError(raw['error'])
 
             else:
                 raw_data = json.loads(response.text)['data']
                 cursor = json.loads(response.text)['cursor']
                 if len(raw_data) != 0:
                     rawdata_res = rawdata_res + raw_data
                 counter = counter + 1
             if cursor['start'] is None or cursor['end'] is None:
                 break
-        df_raw = pd.DataFrame(rawdata_res)
 
-        if len(df_raw) != 0:
+        df = pd.DataFrame(rawdata_res)
+        if len(df) != 0:
             if IST:
-                df_raw['time'] = pd.to_datetime(df_raw['time'], utc=False)
-                df_raw['time'] = df_raw['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
-            if len(df_raw.columns) == 2:
-                df_raw['sensor'] = sensors[0]
+                df['time'] = pd.to_datetime(df['time'], utc=False)
+                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
+            if len(df.columns) == 2:
+                df['sensor'] = sensors[0]
             if str(alias).lower() == "true":
-                df_raw, metadata = DataAccess.get_sensor_alias(self, device_id, df_raw, metadata)
-            df = DataAccess.get_cleaned_table(self, df_raw)
-            if str(cal).lower() == 'true':
-                df = DataAccess.get_caliberation(self, device_id, metadata, df)
-            if bands is not None:
-                df = DataAccess.time_grouping(self, df, bands)
-        else:
-            df = df_raw
+                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata,onpremise=onpremise)
+            df = DataAccess.get_cleaned_table(self, df)
         return df
 
-    def publish_event(self, title, message, meta_data, hover_data, event_tags, created_on):
-        """
-
-        :param title: string
-        :param message: string
-        :param meta_data: string
-        :param hover_data: string
-        :param event_tags: string
-        :param created_on: date string
-        :return: json
-
-        Fetches Data of published events based on input parameters
-
-        """
-        raw_data = []
-        try:
-            url = "https://" + self.url + "/api/eventTag/publishEvent"
-            header = {'userID': self.userID}
-            payload = {
-                "title": title,
-                "message": message,
-                "metaData": meta_data,
-                "eventTags": [event_tags],
-                "hoverData": "",
-                "createdOn": created_on
-            }
-            response = requests.request('POST', url, headers=header, json=payload, verify=True)
-
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
-
-        except Exception as e:
-            print('Failed to fetch event Details')
-            print(e)
-        return raw_data
-
-    def get_events_in_timeslot(self, start_time, end_time):
+    def data_query(self, device_id, sensors,start_time, end_time=str(datetime.now()), alias=True,cal=True, bands=None,onpremise=False,compute=None,IST=True):
         """
 
-        :param start_time: date string
-        :param end_time: date string
-        :return: Json
-
-        Fetches events data in given timeslot
-
-        """
-        raw_data = []
-        try:
-            url = "https://" + self.url + "/api/eventTag/fetchEvents/timeslot"
-            header = {'userID': self.userID}
-            payload = {
-                "startTime": start_time,
-                "endTime": end_time
-            }
-            response = requests.request('PUT', url, headers=header, data=payload, verify=False)
-
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
-
-        except Exception as e:
-            print('Failed to fetch event Details')
-            print(e)
-
-        return raw_data
-
-    def get_event_data_count(self, end_time=time.time(), count=None):
-        """
-
-        :param end_time: date string
-        :param count: integer
-        :return: Json
-        """
-        raw_data = []
-        try:
-            url = "https://" + self.url + "/api/eventTag/fetchEvents/count"
-            header = {'userID': self.userID}
-            payload = {
-                "endTime": end_time,
-                "count": count
-            }
-            response = requests.request('PUT', url, headers=header, json=payload, verify=False)
-
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
-            else:
-                raw_data = json.loads(response.text)
-                return raw_data
-
-        except Exception as e:
-            print('Failed to fetch event Count')
-            print(e)
-
-        return raw_data
+        :param device_id: string
+        :param start_time: yyyy-MM-dd HH:MM:SS
+        :param end_time: yyyy-MM-dd HH:MM:SS
+        :param cal: bool
+        :param bands: None
+        :param IST: bool Indian Time Zone
+        :return: df
 
-    def get_event_categories(self):
-        """
+        If requested data exists in feature store fetch data from the container.
+        IF data is not available the data is fetched from influxdb
 
-        :return: Event Categories Details
         """
-        raw_data = []
         try:
-            url = "https://" + self.url + "/api/eventTag"
-            header = {'userID': self.userID}
-            payload = {}
-            response = requests.request('GET', url, headers=header, data=payload, verify=False)
+            df = pd.DataFrame()
+            metadata = {}
+            connection_string = self.connection_string
+            blob_svc = BlobServiceClient.from_connection_string(conn_str=connection_string)
 
-            if response.status_code != 200:
-                raw = json.loads(response.text)
-                raise ValueError(raw['error'])
+            def check_device(device_id):
+                flag = False
+                container_client = blob_svc.get_container_client(self.container_name)
+                blob_list = container_client.list_blobs()
+                for blob in blob_list:
+                    split_text = blob.name.split('/')
+                    if device_id == split_text[0]:
+                        flag = True
+                return flag
+            def get_dates():
+                temp_list = []
+                match_start_str = re.search(r'\d{4}-\d{2}-\d{2}', start_time)
+                match_end_str = re.search(r'\d{4}-\d{2}-\d{2}', end_time)
+
+                start_t = (datetime.strptime(match_start_str.group(), '%Y-%m-%d').date())
+                end_t = (datetime.strptime(match_end_str.group(), '%Y-%m-%d').date())
+                curr_date = start_t
+                date_list = []
+                while curr_date <= end_t:
+                    date_list.append(curr_date)
+                    curr_date += timedelta(days=1)
+
+                for date_value in date_list:
+                    month_value = date_value.month
+                    year_value = date_value.year
+                    str_format = str(month_value) + '-' + str(year_value)
+                    temp_list.append(str_format)
+
+                def sort_dates(dates):
+                    def date_key(date_string):
+                        return datetime.strptime(date_string, '%m-%Y')
+
+                    return sorted(dates, key=date_key)
+
+                filtered_list = [*set(temp_list)]
+                list_of_dates_in_azure = sort_dates(filtered_list)
+                return list_of_dates_in_azure
+
+            def read_one(blobfile):
+                blob = blob_svc.get_blob_client(self.container_name, device_id + '/' + blobfile + '.parquet')
+
+                with open(blobfile + '.parquet', "wb") as my_blob:
+                    blob_data = blob.download_blob()
+                    blob_data.readinto(my_blob)
+                df = pd.read_parquet(blobfile + '.parquet')
+                os.remove(blobfile + '.parquet')
+                return df
+
+            def thread_read():
+                results = []
+                blob_list = get_dates()
+                with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
+                    for record in range(len(blob_list)):
+                        sys.stdout.write('\r')
+                        sys.stdout.write("Please Wait .. ")
+                        sys.stdout.flush()
+                    results = executor.map(read_one, blob_list)
+                final_df = pd.concat(results, axis=0)
+                return final_df
+            flag = check_device(device_id)
+            if flag:
+                df = thread_read()
+                try:
+                    end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
+                except Exception:
+                    if type(end_time) == str:
+                        end_time = str(end_time) + " 23:59:59"
+                    pass
+                try:
+                    start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
+                    end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
+                    df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                except ValueError:
+                    df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                    pass
+                except Exception as e:
+                    print('Message: \t',e)
+                if sensors != None:
+                    sensors.insert(0,'time')
+                    df =  df[sensors]
+                df.reset_index(drop=True, inplace=True)
+                last_date = df['time'].iloc[len(df) - 1]
+                start_date = last_date.date() + timedelta(days=1)
+                end_time = pd.to_datetime(end_time)
+                if last_date.date() != end_time.date():
+                    df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                    df = pd.concat([df, df1])
+                else:
+                    df1 = DataAccess.fetch_data(self, device_id,start_time=str(last_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
+                    df = pd.concat([df, df1])
+                df.reset_index(drop=True, inplace=True)
             else:
-                raw_data = json.loads(response.text)['data']
-                return raw_data
+                df_devices = DataAccess.get_device_details(self)
+                device_list = df_devices['devID'].tolist()
+                if device_id in device_list:
+                    df = DataAccess.fetch_data(self, device_id, start_time,end_time, alias,sensors=sensors,echo=True,onpremise=onpremise,IST=IST)
+                else:
+                    raise Exception('Message: Device not added in account')
+            if len(df) != 0:
+                if str(alias).lower() == "true":
+                    df,metadata = DataAccess.get_sensor_alias(self,device_id,df,metadata,onpremise=onpremise)
 
+                if str(cal).lower() == 'true':
+                    df = DataAccess.get_caliberation(self, device_id, metadata, df,onpremise=onpremise)
+                if bands is not None:
+                    df = DataAccess.time_grouping(self, df, bands,compute)
+                df = df.set_index(['time'])
+                df = df.fillna(value=np.nan)
+                df.dropna(axis=0, how='all', inplace=True)
+                df.reset_index(drop=False, inplace=True)
+                if IST == False:
+                    df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5,minutes=30)
+            return df
         except Exception as e:
-            print('Failed to fetch event Count')
-            print(e)
-
-        return raw_data
-
+            print(e)
```

### Comparing `iosense_connect-2.1.1/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.2/iosense_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.1
+Version: 2.1.2
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.1/setup.py` & `iosense_connect-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.1",
+    version = "2.1.2",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

