# Comparing `tmp/pyaarlo-0.8.0b6.tar.gz` & `tmp/pyaarlo-0.8.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaarlo-0.8.0b6.tar", last modified: Tue Feb  7 02:40:47 2023, max compression
+gzip compressed data, was "pyaarlo-0.8.0b7.tar", last modified: Wed May 10 11:32:06 2023, max compression
```

## Comparing `pyaarlo-0.8.0b6.tar` & `pyaarlo-0.8.0b7.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-02-07 02:40:47.836598 pyaarlo-0.8.0b6/
--rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b6/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-02-07 02:40:47.836598 pyaarlo-0.8.0b6/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b6/README.md
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-02-07 02:40:47.836598 pyaarlo-0.8.0b6/pyaarlo/
--rw-rw-r--   0 steve     (1000) steve     (1000)    26802 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b6/pyaarlo/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    42200 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b6/pyaarlo/backend.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/background.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    21900 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b6/pyaarlo/base.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    49727 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/camera.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6318 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b6/pyaarlo/cfg.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9513 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b6/pyaarlo/constant.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b6/pyaarlo/device.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b6/pyaarlo/doorbell.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b6/pyaarlo/light.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6017 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b6/pyaarlo/location.py
--rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b6/pyaarlo/main.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/media.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/ratls.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b6/pyaarlo/security_utils.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b6/pyaarlo/sensor.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/sseclient.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b6/pyaarlo/storage.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5127 2023-02-06 22:06:46.000000 pyaarlo-0.8.0b6/pyaarlo/super.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b6/pyaarlo/tfa.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b6/pyaarlo/util.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-02-07 02:40:47.836598 pyaarlo-0.8.0b6/pyaarlo.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      601 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/entry_points.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-02-07 02:40:47.000000 pyaarlo-0.8.0b6/pyaarlo.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-02-07 02:40:47.836598 pyaarlo-0.8.0b6/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b6/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b7/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b7/README.md
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/pyaarlo/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    27069 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    42574 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/backend.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2023-05-10 01:20:55.000000 pyaarlo-0.8.0b7/pyaarlo/background.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    21900 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b7/pyaarlo/base.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    50293 2023-04-11 00:17:07.000000 pyaarlo-0.8.0b7/pyaarlo/camera.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6630 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/cfg.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     9513 2023-05-09 23:31:57.000000 pyaarlo-0.8.0b7/pyaarlo/constant.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b7/pyaarlo/device.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b7/pyaarlo/doorbell.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b7/pyaarlo/light.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6190 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b7/pyaarlo/location.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b7/pyaarlo/main.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/media.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/ratls.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b7/pyaarlo/security_utils.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b7/pyaarlo/sensor.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/sseclient.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/storage.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5183 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b7/pyaarlo/super.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b7/pyaarlo/tfa.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b7/pyaarlo/util.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/pyaarlo.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      623 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/entry_points.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/tests/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      269 2022-10-27 13:44:57.000000 pyaarlo-0.8.0b7/tests/test_backend.py
```

### Comparing `pyaarlo-0.8.0b6/LICENSE` & `pyaarlo-0.8.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/PKG-INFO` & `pyaarlo-0.8.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b6
+Version: 0.8.0b7
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b6/README.md` & `pyaarlo-0.8.0b7/README.md`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/__init__.py` & `pyaarlo-0.8.0b7/pyaarlo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .storage import ArloStorage
 from .location import ArloLocation
 from .sensor import ArloSensor
 from .util import time_to_arlotime
 
 _LOGGER = logging.getLogger("pyaarlo")
 
-__version__ = "0.8.0b6"
+__version__ = "0.8.0b7"
 
 
 class PyArlo(object):
     """Entry point for all Arlo operations.
 
     This is used to login to Arlo, open and maintain an evenstream with Arlo, find and store devices and device
     state, provide keep-alive services and make sure media sources are kept up to date.
@@ -122,14 +122,17 @@
       Normally not needed but some systems fail to push media uploads. Default 'False'.
     * **user_agent** - Set what 'user-agent' string is passed in request headers. It affects what video stream type is
       returned. Default is `arlo`.
     * **mode_api** - Which api to use to set the base station modes. Default is `auto` which choose an API
       based on camera model. Can also be `v1`, `v2` or `v3`. Use `v3` for the new location API.
     * **reconnect_every** - Time, in minutes, to close and relogin to Arlo.
     * **snapshot_timeout** - Time, in seconds, to stop the snapshot attempt and return the camera to the idle state.
+    * **mqtt_host** - specify the mqtt host to use, default mqtt-cluster.arloxcld.com
+    * **mqtt_hostname_check** - disable MQTT host SSL certificate checking, default True
+    * **mqtt_transport** - specify either `websockets` or `tcp`, default `tcp`
 
     **Attributes**
 
     Pyaarlo provides an asynchronous interface for receiving events from Arlo devices. To use it you register
     a callback for an attribute against a device. The following are a list of currently supported attributes:
 
     * **motionDetected** - called when motion start and stops
@@ -346,17 +349,17 @@
 
         url = LOCATIONS_PATH_FORMAT.format(self.be.user_id)
         location_data = self._be.get(url)
         if not location_data:
             self.warning("No locations returned from " + url)
         else:
             for user_location in location_data.get("userLocations", []):
-                self._locations.append(ArloLocation(self, user_location))
+                self._locations.append(ArloLocation(self, user_location, True))
             for shared_location in location_data.get("sharedLocations", []):
-                self._locations.append(ArloLocation(self, shared_location))
+                self._locations.append(ArloLocation(self, shared_location, False))
 
         self.vdebug("locations={}".format(pprint.pformat(self._locations)))
 
     def _refresh_camera_thumbnails(self, wait=False):
         """Request latest camera thumbnails, called at start up."""
         for camera in self._cameras:
             camera.update_last_image(wait)
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/backend.py` & `pyaarlo-0.8.0b7/pyaarlo/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,25 +497,30 @@
             self._event_client_id = f"user_{self._user_id}_" + "".join(
                 str(random.randint(0, 9)) for _ in range(10)
             )
             self.debug(f"mqtt: client_id={self._event_client_id}")
 
             # Create and set up the MQTT client.
             self._event_client = mqtt.Client(
-                client_id=self._event_client_id, transport="websockets"
+                client_id=self._event_client_id, transport=self._arlo.cfg.mqtt_transport
             )
             self._event_client.on_log = self._mqtt_on_log
             self._event_client.on_connect = self._mqtt_on_connect
             self._event_client.on_message = self._mqtt_on_message
-            self._event_client.tls_set_context(ssl.create_default_context())
+            ssl_context = ssl.create_default_context()
+            ssl_context.check_hostname = self._arlo.cfg.mqtt_hostname_check
+            self._event_client.tls_set_context(ssl_context)
             self._event_client.username_pw_set(f"{self._user_id}", self._token)
             self._event_client.ws_set_options(path=MQTT_PATH, headers=headers)
+            self.debug(f"mqtt: host={self._arlo.cfg.mqtt_host}, "
+                       f"check={self._arlo.cfg.mqtt_hostname_check}, "
+                       f"transport={self._arlo.cfg.mqtt_transport}")
 
             # Connect.
-            self._event_client.connect(MQTT_HOST, port=443, keepalive=60)
+            self._event_client.connect(self._arlo.cfg.mqtt_host, port=443, keepalive=60)
             self._event_client.loop_forever()
 
         except Exception as e:
             # self._arlo.warning('general exception ' + str(e))
             self._arlo.error(
                 "general-error={}\n{}".format(
                     type(e).__name__, traceback.format_exc()
@@ -667,15 +672,15 @@
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
             "Origin": ORIGIN_HOST,
             "Referer": REFERER_HOST,
             "Source": "arloCamWeb",
             "User-Agent": self._user_agent,
             "x-user-device-id": self._user_id,
-            "x-user-device-name": "QlJPV1NFUg==",
+            "x-user-device-automation-name": "QlJPV1NFUg==",
             "x-user-device-type": "BROWSER",
         }
 
         # Handle 1015 error
         attempt = 0
         body = None
         while attempt < 3:
@@ -818,15 +823,15 @@
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
             "Authorization": self._token64,
             "Origin": ORIGIN_HOST,
             "Referer": REFERER_HOST,
             "User-Agent": self._user_agent,
             "Source": "arloCamWeb",
             "x-user-device-id": self._user_id,
-            "x-user-device-name": "QlJPV1NFUg==",
+            "x-user-device-automation-name": "QlJPV1NFUg==",
             "x-user-device-type": "BROWSER",
         }
 
         # Validate it!
         validated = self.auth_get(
             AUTH_VALIDATE_PATH + "?data = {}".format(int(time.time())), {}, headers
         )
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/background.py` & `pyaarlo-0.8.0b7/pyaarlo/background.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/base.py` & `pyaarlo-0.8.0b7/pyaarlo/base.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/camera.py` & `pyaarlo-0.8.0b7/pyaarlo/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 pprint.pformat(self._user_requests),
                 pprint.pformat(self._local_users),
                 pprint.pformat(self._remote_users),
             )
         )
 
     # Media library has updated, reload today's events.
-    def _update_media(self):
+    def _update_from_media_library(self):
         self.debug("reloading cache for " + self._name)
         count, videos = self._arlo.ml.videos_for(self)
         if videos:
             captured_today = len([video for video in videos if video.created_today])
             last_captured = videos[0].created_at_pretty(self._arlo.cfg.last_format)
             last_image = videos[0].thumbnail_url
         else:
@@ -159,64 +159,69 @@
             last_image = None
 
         # update local copies
         with self._lock:
             self._cache_count = count
             self._cached_videos = videos
 
-        # update latest video details
+        # Update latest video details.
         if videos:
             if videos[0].created_at != self._load(LAST_VIDEO_CREATED_KEY):
                 self._save_and_do_callbacks(LAST_VIDEO_CREATED_KEY, videos[0].created_at)
                 self._save_and_do_callbacks(LAST_VIDEO_URL_KEY, videos[0].video_url)
                 self._save_and_do_callbacks(LAST_VIDEO_THUMBNAIL_URL_KEY, videos[0].thumbnail_url)
                 self._save_and_do_callbacks(LAST_VIDEO_OBJECT_TYPE, videos[0].object_type)
                 self._save_and_do_callbacks(LAST_VIDEO_OBJECT_REGION, videos[0].object_region)
 
-        # signal video up!
+        # Tell anyone listening about the new capture and how it affects things.
         self._save_and_do_callbacks(CAPTURED_TODAY_KEY, captured_today)
         if last_captured is not None:
             self._save_and_do_callbacks(LAST_CAPTURE_KEY, last_captured)
         self._do_callbacks(MEDIA_UPLOAD_KEY, True)
 
         # new snapshot?
         snapshot = self._arlo.ml.snapshot_for(self)
         if snapshot is not None:
-            self.debug("snapshot updated for media " + self.name)
-            self._save(SNAPSHOT_KEY, snapshot.image_url)
-            self._arlo.bg.run_low(self._update_snapshot)
+            if self._load(SNAPSHOT_KEY, None) != snapshot.image_url:
+                self.debug("snapshot updated for media " + self.name)
+                self._save(SNAPSHOT_KEY, snapshot.image_url)
+                self._arlo.bg.run_low(self._update_image_from_snapshot)
+            else:
+                self.debug("snapshot already done for " + self.name)
 
-        # new image?
+        # New image? Then fetch it an update image details.
         if last_image is not None:
-            self.debug("image updated for media " + self.name)
-            self._save(LAST_IMAGE_KEY, last_image)
-            self._arlo.bg.run_low(self._update_image)
+            if self._load(LAST_IMAGE_KEY, None) != last_image:
+                self.debug("image updated for media " + self.name)
+                self._save(LAST_IMAGE_KEY, last_image)
+                self._arlo.bg.run_low(self._update_image_from_capture)
+            else:
+                self.debug("image already done for " + self.name)
 
     # Update last captured image.
-    def _update_image(self):
+    def _update_image_from_capture(self):
         # Get image and date, if fails ignore
         img, date = http_get_img(self._load(LAST_IMAGE_KEY, None))
         if img is None:
             self.debug("failed to load image for " + self.name)
             return
 
         # Always make this the latest thumbnail image.
         if self._snapshot_time < date:
             self._snapshot_time = date
             date = date.strftime(self._arlo.cfg.last_format)
             self.debug(f"updating image for {self.name} ({date})")
             self._save_and_do_callbacks(LAST_IMAGE_SRC_KEY, "capture/" + date)
-            self._save_and_do_callbacks(LAST_CAPTURE_KEY, date)
             self._save_and_do_callbacks(LAST_IMAGE_DATA_KEY, img)
         else:
             date = date.strftime(self._arlo.cfg.last_format)
             self.vdebug(f"ignoring image for {self.name} ({date})")
 
     # Update the last snapshot
-    def _update_snapshot(self, ignore_date=False):
+    def _update_image_from_snapshot(self, ignore_date=False):
         # Get image and date, if fails ignore.
         img, date = http_get_img(self._load(SNAPSHOT_KEY, None), ignore_date)
         if img is None:
             self.debug("failed to load snapshot for " + self.name)
             return
 
         # Always make this the latest snapshot image.
@@ -266,15 +271,15 @@
             ACTIVITY_STATE_KEY, self._load(ACTIVITY_STATE_KEY, "unknown")
         )
 
     def _queue_media_updates(self):
         for retry in self._arlo.cfg.media_retry:
             self.debug("queueing update in {}".format(retry))
             self._arlo.bg.run_in(
-                self._arlo.ml.queue_update, retry, cb=self._update_media
+                self._arlo.ml.queue_update, retry, cb=self._update_from_media_library
             )
 
     def _mark_as_idle(self):
         """Camera has moved to idle.
         Either we did this or backend did this.
         """
         if self.has_any_local_users:
@@ -367,38 +372,38 @@
                     self._save_and_do_callbacks(key, value)
 
             # The last image thumbnail has changed. Queue an image or snapshot
             # update to download the image and process it.
             if LAST_IMAGE_KEY in event:
                 if not self.is_taking_snapshot:
                     self.debug("{} -> thumbnail changed".format(self.name))
-                    self._arlo.bg.run_low(self._update_image)
+                    self._arlo.bg.run_low(self._update_image_from_capture)
                 else:
                     self.debug(
                         "{} -> snapshot(thumbnail) ready".format(self.name)
                     )
                     self._save(SNAPSHOT_KEY, event.get(LAST_IMAGE_KEY, ""))
-                    self._arlo.bg.run_low(self._update_snapshot, ignore_date=True)
+                    self._arlo.bg.run_low(self._update_image_from_snapshot, ignore_date=True)
 
             # Recording has stopped so a new video is available. Queue an
             # media update, this could later trigger a snapshot or image
             # update.
             if event.get(RECORDING_STOPPED_KEY, False):
                 self.debug("{} -> recording stopped".format(self.name))
-                self._arlo.ml.queue_update(self._update_media)
+                self._arlo.ml.queue_update(self._update_from_media_library)
 
             # Examine the URL passed; snapshots contain `/snapshots/` and
             # recordings contain `recordings`. For snapshot, save URL and queue
             # up an event to download and process it. We do nothing with the
             # recording for now, it will come in via a media update.
             value = event.get(STREAM_SNAPSHOT_KEY, "")
             if "/snapshots/" in value:
                 self.debug("{} -> snapshot1 ready".format(self.name))
                 self._save(SNAPSHOT_KEY, value)
-                self._arlo.bg.run_low(self._update_snapshot)
+                self._arlo.bg.run_low(self._update_image_from_snapshot)
             if "/recordings/" in value:
                 self.debug("{} -> new recording ready".format(self.name))
 
             # Something just happened.
             self._set_recent(self._arlo.cfg.recent_time)
 
             return
@@ -439,23 +444,23 @@
         if event.get("action", "") == "fullFrameSnapshotAvailable":
             value = event.get("properties", {}).get(
                 "presignedFullFrameSnapshotUrl", None
             )
             if value is not None:
                 self.debug("{} -> snapshot2 ready".format(self.name))
                 self._save(SNAPSHOT_KEY, value)
-                self._arlo.bg.run_low(self._update_snapshot)
+                self._arlo.bg.run_low(self._update_image_from_snapshot)
 
         # Non subscription...
         if event.get("action", "") == "lastImageSnapshotAvailable":
             value = event.get("properties", {}).get("presignedLastImageUrl", None)
             if value is not None:
                 self.debug("{} -> snapshot3 ready".format(self.name))
                 self._save(SNAPSHOT_KEY, value)
-                self._arlo.bg.run_low(self._update_snapshot)
+                self._arlo.bg.run_low(self._update_image_from_snapshot)
 
         # Ambient sensors update, decode and push changes.
         if resource.endswith("/ambientSensors/history"):
             data = self._decode_sensor_data(event.get("properties", {}))
             if data is not None:
                 self._save_and_do_callbacks("temperature", data.get("temperature"))
                 self._save_and_do_callbacks("humidity", data.get("humidity"))
@@ -700,35 +705,35 @@
 
         Reloads the videos library from Arlo.
         """
         if wait is None:
             wait = self._arlo.cfg.synchronous_mode
         if wait:
             self.debug("doing media update")
-            self._update_media()
+            self._update_from_media_library()
         else:
             self.debug("queueing media update")
-            self._arlo.bg.run_low(self._update_media)
+            self._arlo.bg.run_low(self._update_from_media_library)
 
     def update_last_image(self, wait=None):
         """Requests last thumbnail from the backend server.
 
         :param wait if True then wait for completion, if False then don't wait,
         if None then use synchronous_mode setting.
 
         Updates the last image.
         """
         if wait is None:
             wait = self._arlo.cfg.synchronous_mode
         if wait:
             self.debug("doing image update")
-            self._update_image()
+            self._update_image_from_capture()
         else:
             self.debug("queueing image update")
-            self._arlo.bg.run_low(self._update_image)
+            self._arlo.bg.run_low(self._update_image_from_capture)
 
     def update_ambient_sensors(self):
         """Requests the latest temperature, humidity and air quality settings.
 
         Queues a job that requests the info from Arlo.
         """
         if self.model_id == MODEL_BABY:
@@ -808,15 +813,15 @@
             else:
                 self.debug("idle snapshot")
                 self._take_idle_snapshot()
 
         for check in self._arlo.cfg.snapshot_checks:
             self.debug("queueing snapshot check in {}".format(check))
             self._arlo.bg.run_in(
-                self._arlo.ml.queue_update, check, cb=self._update_media
+                self._arlo.ml.queue_update, check, cb=self._update_from_media_library
             )
 
         self.vdebug("handle dodgy cameras")
         self._arlo.bg.run_in(self._stop_snapshot, self._arlo.cfg.snapshot_timeout)
 
     def get_snapshot(self, timeout=60):
         """Gets a snapshot from the camera and returns it.
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/cfg.py` & `pyaarlo-0.8.0b7/pyaarlo/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import platform
 import tempfile
 from .constant import (
     DEFAULT_AUTH_HOST,
     DEFAULT_HOST,
+    MQTT_HOST,
     PRELOAD_DAYS,
     TFA_CONSOLE_SOURCE,
     TFA_DEFAULT_HOST,
     TFA_DELAY,
     TFA_EMAIL_TYPE,
     TFA_RETRIES,
 )
@@ -56,14 +57,26 @@
         return self._kw.get("host", DEFAULT_HOST)
 
     @property
     def auth_host(self):
         return self._kw.get("auth_host", DEFAULT_AUTH_HOST)
 
     @property
+    def mqtt_host(self):
+        return self._kw.get("mqtt_host", MQTT_HOST)
+
+    @property
+    def mqtt_hostname_check(self):
+        return self._kw.get("mqtt_hostname_check", True)
+
+    @property
+    def mqtt_transport(self):
+        return self._kw.get("mqtt_transport", "tcp")
+
+    @property
     def dump(self):
         return self._kw.get("dump", False)
 
     @property
     def max_days(self):
         return self._kw.get("max_days", 365)
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/constant.py` & `pyaarlo-0.8.0b7/pyaarlo/constant.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/device.py` & `pyaarlo-0.8.0b7/pyaarlo/device.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/doorbell.py` & `pyaarlo-0.8.0b7/pyaarlo/doorbell.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/light.py` & `pyaarlo-0.8.0b7/pyaarlo/light.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/location.py` & `pyaarlo-0.8.0b7/pyaarlo/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,28 @@
 DEFAULT_MODES = {
     "standby": "Stand By",
     "armAway": "Armed Away",
     "armHome": "Armed Home"
 }
 
 
+def location_name(name, user):
+    if user:
+        return f"user_location_{name}"
+    return f"location_{name}"
+
+
 class ArloLocation(ArloSuper):
     """ Represents a Location object.
 
     Each Arlo account can have multiple owned locations and multiple shared locations.
     """
-    def __init__(self, arlo, attrs):
-        super().__init__(attrs.get("locationName", "unknown"), arlo, attrs,
+    def __init__(self, arlo, attrs, user=False):
+        super().__init__(location_name(attrs.get("locationName", "unknown"), user),
+                         arlo, attrs,
                          id=attrs.get("locationId", "unknown"),
                          type="location")
 
         self._device_ids = attrs.get("gatewayDeviceIds", [])
 
     def _id_to_name(self, mode_id):
         return self._load([MODE_ID_TO_NAME_KEY, mode_id], None)
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/main.py` & `pyaarlo-0.8.0b7/pyaarlo/main.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/media.py` & `pyaarlo-0.8.0b7/pyaarlo/media.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/ratls.py` & `pyaarlo-0.8.0b7/pyaarlo/ratls.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/security_utils.py` & `pyaarlo-0.8.0b7/pyaarlo/security_utils.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/sensor.py` & `pyaarlo-0.8.0b7/pyaarlo/sensor.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/sseclient.py` & `pyaarlo-0.8.0b7/pyaarlo/sseclient.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/storage.py` & `pyaarlo-0.8.0b7/pyaarlo/storage.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/super.py` & `pyaarlo-0.8.0b7/pyaarlo/super.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,12 +155,16 @@
         :param attr: Attribute - eg `motionStarted` - to monitor.
         :type attr: str
         :param cb: Callback to run.
         """
         with self._lock:
             self._attr_cbs_.append((attr, cb))
 
+    @property
+    def state(self):
+        return "ok"
+
     def debug(self, msg):
         self._arlo.debug(f"{self._name}: {msg}")
 
     def vdebug(self, msg):
         self._arlo.vdebug(f"{self._name}: {msg}")
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo/tfa.py` & `pyaarlo-0.8.0b7/pyaarlo/tfa.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo/util.py` & `pyaarlo-0.8.0b7/pyaarlo/util.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b6/pyaarlo.egg-info/PKG-INFO` & `pyaarlo-0.8.0b7/pyaarlo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b6
+Version: 0.8.0b7
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b6/pyaarlo.egg-info/SOURCES.txt` & `pyaarlo-0.8.0b7/pyaarlo.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 pyaarlo/tfa.py
 pyaarlo/util.py
 pyaarlo.egg-info/PKG-INFO
 pyaarlo.egg-info/SOURCES.txt
 pyaarlo.egg-info/dependency_links.txt
 pyaarlo.egg-info/entry_points.txt
 pyaarlo.egg-info/requires.txt
-pyaarlo.egg-info/top_level.txt
+pyaarlo.egg-info/top_level.txt
+tests/test_backend.py
```

### Comparing `pyaarlo-0.8.0b6/setup.py` & `pyaarlo-0.8.0b7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,24 @@
     with open('README.md') as desc:
         return desc.read()
 
 
 setup(
 
     name='pyaarlo',
-    version='0.8.0b6',
+    version='0.8.0b7',
     packages=['pyaarlo'],
 
     python_requires='>=3.6',
     install_requires=[
         'requests',
         'click',
         'pycryptodome',
         'unidecode',
-        'cloudscraper>=1.2.64',
+        'cloudscraper>=1.2.71',
         'paho-mqtt',
         'cryptography'
     ],
 
     author='Steve Herrell',
     author_email='steve.herrell@gmail.com',
     description='PyAarlo is a library that provides asynchronous access to Arlo security cameras.',
```

