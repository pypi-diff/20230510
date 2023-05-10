# Comparing `tmp/drift_mqtt-0.2.0-py3-none-any.whl.zip` & `tmp/drift_mqtt-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9398 bytes, number of entries: 8
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-28 11:37 drift_mqtt/VERSION
--rw-r--r--  2.0 unx      394 b- defN 23-Apr-28 11:37 drift_mqtt/__init__.py
--rw-r--r--  2.0 unx     4142 b- defN 23-Apr-28 11:37 drift_mqtt/client.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1802 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      629 b- defN 23-Apr-28 11:37 drift_mqtt-0.2.0.dist-info/RECORD
-8 files, 23801 bytes uncompressed, 8300 bytes compressed:  65.1%
+Zip file size: 9464 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        6 b- defN 23-May-10 13:56 drift_mqtt/VERSION
+-rw-r--r--  2.0 unx      394 b- defN 23-May-10 13:56 drift_mqtt/__init__.py
+-rw-r--r--  2.0 unx     4346 b- defN 23-May-10 13:56 drift_mqtt/client.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-May-10 13:56 drift_mqtt-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1802 b- defN 23-May-10 13:56 drift_mqtt-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 13:56 drift_mqtt-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-10 13:56 drift_mqtt-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      629 b- defN 23-May-10 13:56 drift_mqtt-0.2.1.dist-info/RECORD
+8 files, 24005 bytes uncompressed, 8366 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: drift_mqtt/__init__.py
 Comment: 
 
 Filename: drift_mqtt/client.py
 Comment: 
 
-Filename: drift_mqtt-0.2.0.dist-info/LICENSE
+Filename: drift_mqtt-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: drift_mqtt-0.2.0.dist-info/METADATA
+Filename: drift_mqtt-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: drift_mqtt-0.2.0.dist-info/WHEEL
+Filename: drift_mqtt-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: drift_mqtt-0.2.0.dist-info/top_level.txt
+Filename: drift_mqtt-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: drift_mqtt-0.2.0.dist-info/RECORD
+Filename: drift_mqtt-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drift_mqtt/VERSION

```diff
@@ -1 +1 @@
-0.2.0
+0.2.1
```

## drift_mqtt/client.py

```diff
@@ -50,14 +50,20 @@
 
     def on_message(self, _client, _userdata, message: MQTTMessage):
         """Message read callback"""
         for sub in self._subscriptions:
             try:
                 if re.match(sub.topic.replace("#", "(.*)"), message.topic):
                     sub.handler(message)
+                elif (
+                    re.search(r"\$share\/([a-zA-Z-_]*)\/(.*)", sub.topic).group(2)
+                    == message.topic
+                ):
+                    sub.handler(message)
+
             except Exception as err:  # pylint: disable=broad-except
                 logger.exception("Error in a message handler: %s", err)
 
     def __getattr__(self, item):
         """Forward unknown methods to MQTT client"""
         return getattr(self._client, item)
```

## Comparing `drift_mqtt-0.2.0.dist-info/LICENSE` & `drift_mqtt-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `drift_mqtt-0.2.0.dist-info/METADATA` & `drift_mqtt-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-mqtt
-Version: 0.2.0
+Version: 0.2.1
 Summary: A wrapper around Python Paho Mqtt library
 Home-page: https://gitlab.panda.technology/drift/sdk/drift-mqtt
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `drift_mqtt-0.2.0.dist-info/RECORD` & `drift_mqtt-0.2.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-drift_mqtt/VERSION,sha256=H5MN0fEzwfl6lP46y42zQ3LPTAH_2ys_9Mpy-UlBIek,6
+drift_mqtt/VERSION,sha256=cQFcl5zLD8igvnygroMEarBFzcLI-qCfsvD35ED5tKY,6
 drift_mqtt/__init__.py,sha256=9PNWAmjqAVpP_yJNdLDJNxKQ_jr82V7hw-MHc6Asxhw,394
-drift_mqtt/client.py,sha256=2TshRfMn8F8iS2MwgKhFXCHVsir3A6_lfiEFh462GQM,4142
-drift_mqtt-0.2.0.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-drift_mqtt-0.2.0.dist-info/METADATA,sha256=CVoQV8jBjX9hG7xdwD1Ve1mUucKrGVueeQtp9dRfR-c,1802
-drift_mqtt-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drift_mqtt-0.2.0.dist-info/top_level.txt,sha256=c85JmUaq2ByDg6uHWQ7xFK5FXJyBmuP_Vup3-1tdmfY,11
-drift_mqtt-0.2.0.dist-info/RECORD,,
+drift_mqtt/client.py,sha256=N_13H9m_dOdHQ3I_4zGl_4Polc2f8vVbcFzfyRMYgXU,4346
+drift_mqtt-0.2.1.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+drift_mqtt-0.2.1.dist-info/METADATA,sha256=D-grKu_dcNjqA8oFD6PJccyyJKcTg9WBKQhPLnAftYY,1802
+drift_mqtt-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drift_mqtt-0.2.1.dist-info/top_level.txt,sha256=c85JmUaq2ByDg6uHWQ7xFK5FXJyBmuP_Vup3-1tdmfY,11
+drift_mqtt-0.2.1.dist-info/RECORD,,
```

