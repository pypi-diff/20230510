# Comparing `tmp/pyduke-energy-1.0.5.tar.gz` & `tmp/pyduke-energy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyduke-energy-1.0.5.tar", last modified: Fri Jan  6 20:31:34 2023, max compression
+gzip compressed data, was "pyduke-energy-1.0.6.tar", last modified: Wed May 10 15:36:58 2023, max compression
```

## Comparing `pyduke-energy-1.0.5.tar` & `pyduke-energy-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-06 20:31:34.589900 pyduke-energy-1.0.5/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1069 2021-08-20 20:56:35.000000 pyduke-energy-1.0.5/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6837 2023-01-06 20:31:34.590987 pyduke-energy-1.0.5/PKG-INFO
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6197 2023-01-06 18:57:44.000000 pyduke-energy-1.0.5/README.md
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      103 2021-08-20 21:06:40.000000 pyduke-energy-1.0.5/pyproject.toml
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1023 2023-01-06 20:31:34.595816 pyduke-energy-1.0.5/setup.cfg
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)       69 2021-08-25 12:55:50.000000 pyduke-energy-1.0.5/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-06 20:31:34.257475 pyduke-energy-1.0.5/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-06 20:31:34.454583 pyduke-energy-1.0.5/src/pyduke_energy/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)       46 2021-08-25 14:50:56.000000 pyduke-energy-1.0.5/src/pyduke_energy/__init__.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    16559 2022-09-07 19:38:41.000000 pyduke-energy-1.0.5/src/pyduke_energy/client.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1805 2023-01-06 20:30:51.000000 pyduke-energy-1.0.5/src/pyduke_energy/const.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1075 2021-12-18 14:02:31.000000 pyduke-energy-1.0.5/src/pyduke_energy/errors.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    17752 2023-01-06 19:29:00.000000 pyduke-energy-1.0.5/src/pyduke_energy/realtime.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4698 2022-09-07 19:38:41.000000 pyduke-energy-1.0.5/src/pyduke_energy/types.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      834 2021-08-25 14:54:59.000000 pyduke-energy-1.0.5/src/pyduke_energy/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-06 20:31:34.566876 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6837 2023-01-06 20:31:34.000000 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      452 2023-01-06 20:31:34.000000 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-01-06 20:31:34.000000 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      275 2023-01-06 20:31:34.000000 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-01-06 20:31:34.000000 pyduke-energy-1.0.5/src/pyduke_energy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 15:36:58.452775 pyduke-energy-1.0.6/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1069 2021-08-20 20:56:35.000000 pyduke-energy-1.0.6/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7012 2023-05-10 15:36:58.453775 pyduke-energy-1.0.6/PKG-INFO
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6372 2023-05-10 15:23:21.000000 pyduke-energy-1.0.6/README.md
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      103 2021-08-20 21:06:40.000000 pyduke-energy-1.0.6/pyproject.toml
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1023 2023-05-10 15:36:58.458775 pyduke-energy-1.0.6/setup.cfg
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)       69 2021-08-25 12:55:50.000000 pyduke-energy-1.0.6/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 15:36:57.965256 pyduke-energy-1.0.6/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 15:36:58.262155 pyduke-energy-1.0.6/src/pyduke_energy/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)       46 2021-08-25 14:50:56.000000 pyduke-energy-1.0.6/src/pyduke_energy/__init__.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    16559 2022-09-07 19:38:41.000000 pyduke-energy-1.0.6/src/pyduke_energy/client.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1805 2023-05-10 15:19:11.000000 pyduke-energy-1.0.6/src/pyduke_energy/const.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1075 2021-12-18 14:02:31.000000 pyduke-energy-1.0.6/src/pyduke_energy/errors.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    17752 2023-01-06 19:29:00.000000 pyduke-energy-1.0.6/src/pyduke_energy/realtime.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4698 2022-09-07 19:38:41.000000 pyduke-energy-1.0.6/src/pyduke_energy/types.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      834 2021-08-25 14:54:59.000000 pyduke-energy-1.0.6/src/pyduke_energy/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 15:36:58.401269 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7012 2023-05-10 15:36:57.000000 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      485 2023-05-10 15:36:57.000000 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-10 15:36:57.000000 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      275 2023-05-10 15:36:57.000000 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-05-10 15:36:57.000000 pyduke-energy-1.0.6/src/pyduke_energy.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 15:36:58.429592 pyduke-energy-1.0.6/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      350 2021-08-25 15:44:38.000000 pyduke-energy-1.0.6/tests/test_duke_energy_client.py
```

### Comparing `pyduke-energy-1.0.5/LICENSE` & `pyduke-energy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/PKG-INFO` & `pyduke-energy-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyduke-energy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Wrapper for unofficial Duke Energy REST API
 Home-page: https://github.com/mjmeli/pyduke-energy
 Author: Michael Meli
 Author-email: mjmeli94@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjmeli/pyduke-energy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,18 @@
 
 Python3 wrapper for the unofficial Duke Energy API.
 
 Designed to work with Home Assistant. Unlikely to ever be fully implemented. The primary goal is to expose Duke Energy Gateway usage information.
 
 The library supports access to the real-time power usage implemented via an MQTT over websockets connection, or a more traditional REST API to poll near-real-time data.
 
+## IMPORTANT - Deprecation Warning
+
+**Duke Energy is shutting down the Gateway pilot program at the end of June. This library will stop functioning and will be deprecated.**
+
 ## Before You Begin
 
 ### Disclaimer
 
 The API is unofficial, not documented, and probably not supposed to be used by third-parties. It is only accessible as it powers the Duke Energy phone app and we can mimic the app requests.
 
 In addition, the Gateway functionality is part of a pilot program. There is no guarantee on availability going forward.
```

### Comparing `pyduke-energy-1.0.5/README.md` & `pyduke-energy-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 Python3 wrapper for the unofficial Duke Energy API.
 
 Designed to work with Home Assistant. Unlikely to ever be fully implemented. The primary goal is to expose Duke Energy Gateway usage information.
 
 The library supports access to the real-time power usage implemented via an MQTT over websockets connection, or a more traditional REST API to poll near-real-time data.
 
+## IMPORTANT - Deprecation Warning
+
+**Duke Energy is shutting down the Gateway pilot program at the end of June. This library will stop functioning and will be deprecated.**
+
 ## Before You Begin
 
 ### Disclaimer
 
 The API is unofficial, not documented, and probably not supposed to be used by third-parties. It is only accessible as it powers the Duke Energy phone app and we can mimic the app requests.
 
 In addition, the Gateway functionality is part of a pilot program. There is no guarantee on availability going forward.
```

### Comparing `pyduke-energy-1.0.5/setup.cfg` & `pyduke-energy-1.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyduke-energy
-version = 1.0.5
+version = 1.0.6
 author = Michael Meli
 author_email = mjmeli94@gmail.com
 description = Python Wrapper for unofficial Duke Energy REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mjmeli/pyduke-energy
 project_urls =
```

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/client.py` & `pyduke-energy-1.0.6/src/pyduke_energy/client.py`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/const.py` & `pyduke-energy-1.0.6/src/pyduke_energy/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ACCT_ENDPOINT = "auth/account-list"
 ACCT_DET_ENDPOINT = "auth/account-details"
 GW_STATUS_ENDPOINT = "gw/gateways/status"
 GW_USAGE_ENDPOINT = "smartmeter/usageByHour"
 
 # hard-coded from Android app
 BASIC_AUTH = (
-    "Basic NEdtR3J1M085TEFIV3BMNjVjbWpyZDhtQ1VKZU5XTVo6OWFyZVZoZlM3R2N4UmgzWA=="
+    "Basic ZEJEMnl0TE1IYm9UMjBNNDRkQVRqM29JelNoUG15NGQ6ODZ0QW1zVXFZcmV3R3N2WA=="
 )
 
 DEFAULT_TIMEOUT = 10  # seconds
 
 MQTT_HOST = "app-core1.de-iot.io"
 MQTT_PORT = 443
 MQTT_ENDPOINT = "/app-mqtt"
```

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/errors.py` & `pyduke-energy-1.0.6/src/pyduke_energy/errors.py`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/realtime.py` & `pyduke-energy-1.0.6/src/pyduke_energy/realtime.py`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/types.py` & `pyduke-energy-1.0.6/src/pyduke_energy/types.py`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy/utils.py` & `pyduke-energy-1.0.6/src/pyduke_energy/utils.py`

 * *Files identical despite different names*

### Comparing `pyduke-energy-1.0.5/src/pyduke_energy.egg-info/PKG-INFO` & `pyduke-energy-1.0.6/src/pyduke_energy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyduke-energy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Wrapper for unofficial Duke Energy REST API
 Home-page: https://github.com/mjmeli/pyduke-energy
 Author: Michael Meli
 Author-email: mjmeli94@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjmeli/pyduke-energy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,18 @@
 
 Python3 wrapper for the unofficial Duke Energy API.
 
 Designed to work with Home Assistant. Unlikely to ever be fully implemented. The primary goal is to expose Duke Energy Gateway usage information.
 
 The library supports access to the real-time power usage implemented via an MQTT over websockets connection, or a more traditional REST API to poll near-real-time data.
 
+## IMPORTANT - Deprecation Warning
+
+**Duke Energy is shutting down the Gateway pilot program at the end of June. This library will stop functioning and will be deprecated.**
+
 ## Before You Begin
 
 ### Disclaimer
 
 The API is unofficial, not documented, and probably not supposed to be used by third-parties. It is only accessible as it powers the Duke Energy phone app and we can mimic the app requests.
 
 In addition, the Gateway functionality is part of a pilot program. There is no guarantee on availability going forward.
```

