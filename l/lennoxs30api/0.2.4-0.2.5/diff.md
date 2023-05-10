# Comparing `tmp/lennoxs30api-0.2.4.tar.gz` & `tmp/lennoxs30api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennoxs30api-0.2.4.tar", last modified: Thu May  4 15:42:42 2023, max compression
+gzip compressed data, was "lennoxs30api-0.2.5.tar", last modified: Wed May 10 12:02:30 2023, max compression
```

## Comparing `lennoxs30api-0.2.4.tar` & `lennoxs30api-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.388599 lennoxs30api-0.2.4/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.4/LICENSE
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-04 15:42:42.385604 lennoxs30api-0.2.4/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.4/README.md
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.305001 lennoxs30api-0.2.4/lennoxs30api/
--rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-05-04 15:39:18.000000 lennoxs30api-0.2.4/lennoxs30api/__init__.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_ble.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_equipment.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_errors.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_home.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_period.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.4/lennoxs30api/lennox_schedule.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.4/lennoxs30api/message_logger.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/metrics.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)   129341 2023-05-04 15:33:30.000000 lennoxs30api-0.2.4/lennoxs30api/s30api_async.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.4/lennoxs30api/s30exception.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.4/lennoxs30api/subscriber_base.py
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-04 15:42:42.368599 lennoxs30api-0.2.4/lennoxs30api.egg-info/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/SOURCES.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/dependency_links.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/requires.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-05-04 15:42:42.000000 lennoxs30api-0.2.4/lennoxs30api.egg-info/top_level.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-05-04 15:42:42.389602 lennoxs30api-0.2.4/setup.cfg
--rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-05-04 15:39:24.000000 lennoxs30api-0.2.4/setup.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-10 12:02:30.274798 lennoxs30api-0.2.5/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.5/LICENSE
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-10 12:02:30.271797 lennoxs30api-0.2.5/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.5/README.md
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-10 12:02:30.188796 lennoxs30api-0.2.5/lennoxs30api/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-05-10 12:00:03.000000 lennoxs30api-0.2.5/lennoxs30api/__init__.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_ble.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_equipment.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_errors.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_home.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_period.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.5/lennoxs30api/lennox_schedule.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.5/lennoxs30api/message_logger.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.5/lennoxs30api/metrics.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)   131031 2023-05-10 12:00:03.000000 lennoxs30api-0.2.5/lennoxs30api/s30api_async.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.5/lennoxs30api/s30exception.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.5/lennoxs30api/subscriber_base.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-05-10 12:02:30.255797 lennoxs30api-0.2.5/lennoxs30api.egg-info/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-05-10 12:02:29.000000 lennoxs30api-0.2.5/lennoxs30api.egg-info/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-05-10 12:02:29.000000 lennoxs30api-0.2.5/lennoxs30api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-05-10 12:02:29.000000 lennoxs30api-0.2.5/lennoxs30api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-05-10 12:02:29.000000 lennoxs30api-0.2.5/lennoxs30api.egg-info/requires.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-05-10 12:02:29.000000 lennoxs30api-0.2.5/lennoxs30api.egg-info/top_level.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-05-10 12:02:30.275796 lennoxs30api-0.2.5/setup.cfg
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-05-10 12:00:03.000000 lennoxs30api-0.2.5/setup.py
```

### Comparing `lennoxs30api-0.2.4/LICENSE` & `lennoxs30api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/PKG-INFO` & `lennoxs30api-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.4
+Version: 0.2.5
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.4/README.md` & `lennoxs30api-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_ble.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_ble.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_equipment.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_equipment.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_errors.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_errors.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_home.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_home.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_period.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_period.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/lennox_schedule.py` & `lennoxs30api-0.2.5/lennoxs30api/lennox_schedule.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/message_logger.py` & `lennoxs30api-0.2.5/lennoxs30api/message_logger.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/metrics.py` & `lennoxs30api-0.2.5/lennoxs30api/metrics.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/s30api_async.py` & `lennoxs30api-0.2.5/lennoxs30api/s30api_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1071,28 +1071,52 @@
         self.humidificationMode: str = None
         # Internet status
         self.relayServerConnected: bool = None
         self.internetStatus: bool = None
         # Cloud Connected  "online" or "offline"
         self.cloud_status: str = None
 
+        # Indoor Air Quality
+        self.iaq_mitigation_action = None
+        self.iaq_mitigation_state = None
+        self.iaq_overall_index = None
+
+        self.iaq_pm25_sta = None
+        self.iaq_pm25_sta_valid = None
+        self.iaq_pm25_lta = None
+        self.iaq_pm25_lta_valid = None
+        self.iaq_pm25_component_score = None
+
+        self.iaq_voc_sta = None
+        self.iaq_voc_sta_valid = None
+        self.iaq_voc_lta = None
+        self.iaq_voc_lta_valid = None
+        self.iaq_voc_component_score = None
+
+        self.iaq_co2_sta = None
+        self.iaq_co2_sta_valid = None
+        self.iaq_co2_lta = None
+        self.iaq_co2_lta_valid = None
+        self.iaq_co2_component_score = None
+
         self._dirty = False
         self._dirtyList = []
         self.message_processing_list = {
             "system": self._processSystemMessage,
             "zones": self._processZonesMessage,
             "schedules": self._processSchedules,
             "occupancy": self._processOccupancy,
             "devices": self._processDevices,
             "equipments": self._processEquipments,
             "systemControl": self._processSystemControl,
             "siblings": self._processSiblings,
             "rgw": self._process_rgw,
             "alerts": self._process_alerts,
             "ble": self._process_ble,
+            "indoorAirQuality": self._process_indoor_air_quality,
         }
 
         self.equipment: dict[int, lennox_equipment] = {}
         self.ble_devices: dict[int, LennoxBle] = {}
         _LOGGER.info(f"Creating lennox_system sysId [{self.sysId}]")
 
     async def update_system_online_cloud(self):
@@ -1282,14 +1306,28 @@
             if "device" in devices:
                 device = devices["device"]
                 if "wdn" in device and device["wdn"] != 0:
                     ble_device = self.get_or_create_ble_device(device["wdn"])
                     ble_device.update_from_json(device)
                     ble_device.execute_on_update_callbacks()
 
+    def _process_indoor_air_quality(self, iaq):
+        self.attr_updater(iaq, "mitigation_action", "iaq_mitigation_action")
+        self.attr_updater(iaq, "mitigation_state", "iaq_mitigation_state")
+        self.attr_updater(iaq, "overall_index", "iaq_overall_index")
+        if "sensor" in iaq:
+            for sensor in iaq["sensor"]:
+                if sensor["name"] in ("PM25", "VOC", "CO2"):
+                    name = str(sensor["name"]).lower()
+                    self.attr_updater(sensor, "sta", f"iaq_{name}_sta")
+                    self.attr_updater(sensor, "sta_validNumber", f"iaq_{name}_sta_valid")
+                    self.attr_updater(sensor, "lta", f"iaq_{name}_lta")
+                    self.attr_updater(sensor, "lta_validNumber", f"iaq_{name}_lta_valid")
+                    self.attr_updater(sensor, "component_score", f"iaq_{name}_component_score")
+
     def _processSchedules(self, schedules):
         """Processes the schedule messages, throws base exceptions if a problem is encoutered"""
         for schedule in schedules:
             self._dirty = True
             if "schedules" in self._dirtyList is False:
                 self._dirtyList.append("schedules")
             schedule_id = schedule["id"]
```

### Comparing `lennoxs30api-0.2.4/lennoxs30api/s30exception.py` & `lennoxs30api-0.2.5/lennoxs30api/s30exception.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api/subscriber_base.py` & `lennoxs30api-0.2.5/lennoxs30api/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/lennoxs30api.egg-info/PKG-INFO` & `lennoxs30api-0.2.5/lennoxs30api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.4
+Version: 0.2.5
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.4/lennoxs30api.egg-info/SOURCES.txt` & `lennoxs30api-0.2.5/lennoxs30api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.4/setup.py` & `lennoxs30api-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lennoxs30api",
-    version="0.2.4",
+    version="0.2.5",
     description="API Wrapper for Lennox S30 Cloud and LAN API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PeteRager/lennoxs30api",
     author="Pete Rage",
     author_email="pete.rager@x.com",
     license="MIT",
```

