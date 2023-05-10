# Comparing `tmp/dv-1.0.8.tar.gz` & `tmp/dv-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dv-1.0.8.tar", last modified: Tue Apr 21 00:31:40 2020, max compression
+gzip compressed data, was "dist/dv-1.0.9.tar", last modified: Wed Aug 12 17:21:13 2020, max compression
```

## Comparing `dv-1.0.8.tar` & `dv-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-21 00:31:40.000000 dv-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       19 2020-04-21 00:31:29.000000 dv-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      295 2020-04-21 00:31:40.000000 dv-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6282 2020-04-21 00:31:29.000000 dv-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2020-04-21 00:31:40.000000 dv-1.0.8/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-21 00:31:40.000000 dv-1.0.8/dv/
--rw-rw-rw-   0 root         (0) root         (0)    10642 2020-04-21 00:31:29.000000 dv-1.0.8/dv/AedatFile.py
--rw-rw-rw-   0 root         (0) root         (0)     3100 2020-04-21 00:31:29.000000 dv-1.0.8/dv/Control.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2020-04-21 00:31:29.000000 dv-1.0.8/dv/Event.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2020-04-21 00:31:29.000000 dv-1.0.8/dv/EventFrameIterator.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2020-04-21 00:31:29.000000 dv-1.0.8/dv/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2020-04-21 00:31:29.000000 dv-1.0.8/dv/IMU.py
--rw-rw-rw-   0 root         (0) root         (0)     6482 2020-04-21 00:31:29.000000 dv-1.0.8/dv/LegacyAedatFile.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2020-04-21 00:31:29.000000 dv-1.0.8/dv/NetworkInput.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2020-04-21 00:31:29.000000 dv-1.0.8/dv/Trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2020-04-21 00:31:29.000000 dv-1.0.8/dv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-21 00:31:40.000000 dv-1.0.8/dv/fb/
--rw-rw-rw-   0 root         (0) root         (0)      192 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/Constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/Event.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/EventPacket.py
--rw-rw-rw-   0 root         (0) root         (0)     2597 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/FileDataDefinition.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/FileDataTable.py
--rw-rw-rw-   0 root         (0) root         (0)     5448 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/FrameFormat.py
--rw-rw-rw-   0 root         (0) root         (0)     4914 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/IMU.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/IMUPacket.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/IOHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/PacketHeader.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/Trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/TriggerPacket.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/TriggerType.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2020-04-21 00:31:29.000000 dv-1.0.8/dv/fb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/
--rw-r--r--   0 root         (0) root         (0)      295 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2020-04-21 00:31:40.000000 dv-1.0.8/dv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-04-21 00:31:40.000000 dv-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      639 2020-04-21 00:31:29.000000 dv-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-12 17:21:13.000000 dv-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2020-08-12 17:21:05.000000 dv-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      295 2020-08-12 17:21:13.000000 dv-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6255 2020-08-12 17:21:05.000000 dv-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2020-08-12 17:21:13.000000 dv-1.0.9/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-12 17:21:13.000000 dv-1.0.9/dv/
+-rw-rw-rw-   0 root         (0) root         (0)    10672 2020-08-12 17:21:05.000000 dv-1.0.9/dv/AedatFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2020-08-12 17:21:05.000000 dv-1.0.9/dv/Control.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2020-08-12 17:21:05.000000 dv-1.0.9/dv/Event.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2020-08-12 17:21:05.000000 dv-1.0.9/dv/EventFrameIterator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2020-08-12 17:21:05.000000 dv-1.0.9/dv/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2020-08-12 17:21:05.000000 dv-1.0.9/dv/IMU.py
+-rw-rw-rw-   0 root         (0) root         (0)     6493 2020-08-12 17:21:05.000000 dv-1.0.9/dv/LegacyAedatFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2020-08-12 17:21:05.000000 dv-1.0.9/dv/NetworkInput.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2020-08-12 17:21:05.000000 dv-1.0.9/dv/Trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2020-08-12 17:21:05.000000 dv-1.0.9/dv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-12 17:21:13.000000 dv-1.0.9/dv/fb/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/Constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/Event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/EventPacket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/FileDataDefinition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/FileDataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5533 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/FrameFormat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4960 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/IMU.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/IMUPacket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/IOHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/PacketHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/Trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/TriggerPacket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/TriggerType.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2020-08-12 17:21:05.000000 dv-1.0.9/dv/fb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      295 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        3 2020-08-12 17:21:13.000000 dv-1.0.9/dv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-08-12 17:21:13.000000 dv-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      592 2020-08-12 17:21:05.000000 dv-1.0.9/setup.py
```

### Comparing `dv-1.0.8/README.md` & `dv-1.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <center>![logo](img/head.png)</center>
 
 # DV-Python
 
 *A library that to connect a python script to outputs from the dynamic vision system DV. This is used in conjunction with the Dynamic Vision Sensor (DVS).*
 
 ## Features
-[DV (Dynamic Vision System)](https://inivation.gitlab.io/dv/dv-docs/) is a platform to develop high-performance, embedded, deployable C++ applications. However, for rapid prototyping and experimenting, many developers prefer to use python. 
+[DV (Dynamic Vision System)](https://inivation.gitlab.io/dv/dv-docs/) is a platform to develop high-performance, embedded, deployable C++ applications. However, for rapid prototyping and experimenting, many developers prefer to use python.
 
 **DV-Python** DV python is a library that helps you:
 
 * Get live (raw or processed) data from DV into your python application
 * Open files you recorded with DV
 * Open older files, recorded with now obsolete software (such as jaer)
 
@@ -34,29 +34,29 @@
    ![add module screenshot](img/1.png)
 
 4. Name the module as you wish, for example "event_server"
 5. Connect `events` output of your camera with the input of the added module
 
    ![connection screenshot](img/2.png)
 
-6. The module assumes port `7777` by default. If you are happy with that, you can start the module by pressing the play button. If not, click on the plus button next to the modules name in the configuration list in the right sidebar. 
+6. The module assumes port `7777` by default. If you are happy with that, you can start the module by pressing the play button. If not, click on the plus button next to the modules name in the configuration list in the right sidebar.
 7. To change the port, change the setting in the window that popped up
 
    ![connection screenshot](img/3.png)
 
 8. In that same window, you can change the 'Max Data Backlog' configuration if needed. By default the TCP server module discards data if the Python client cannot keep up. To avoid this, change the value to '-1'.
 
 #### Connect in your python program
 
 A sample program that loops over the events in the input:
 
 ```python
 from dv import NetworkEventInput
 
-with NetworkEventInput(address='localhost', port=7777) as i:
+with NetworkEventInput(address='127.0.0.1', port=7777) as i:
     for event in i:
         print(event.timestamp)
 ```
 
 An event has properties `x`, `y`, `polarity` and timestamp. The timestamp is in microseconds.
 
 ## Get live frame data from the camera
@@ -67,15 +67,15 @@
 
 A sample program that loops over the events in the input:
 
 ```python
 from dv import NetworkFrameInput
 import cv2
 
-with NetworkFrameInput(address='localhost', port=7777) as i:
+with NetworkFrameInput(address='127.0.0.1', port=7777) as i:
     for frame in i:
         print(frame)
         cv2.imshow('out', frame.image)
         cv2.waitKey(1)
 ```
 
 `frame.image` is a *numpy* matrix that can directly be used to perform openCV operations on it.
@@ -90,57 +90,57 @@
 
 ```python
 from dv import AedatFile
 
 with AedatFile(<Path to aedat file>) as f:
     # list all the names of streams in the file
     print(f.names)
-    
+
     # Access dimensions of the event stream
-    height, width = f['events'].size    
+    height, width = f['events'].size
 
     # loop through the "events" stream
     for e in f['events']:
         print(e.timestamp)
-        
+
     # loop through the "frames" stream
     for frame in f['frames']:
         print(frame.timestamp)
         cv2.imshow('out', frame.image)
         cv2.waitKey(1)
 ```
 
 ### Direct numpy access
 
 Iterating over all events in a python loop is pretty slow. In order to improve performance, *dv-python* offers direct *numpy* access.
 With numpy access the underlying data is directly interpreted by numpy and no data has to be copied.
-Events are accessed in packets of varying size. 
+Events are accessed in packets of varying size.
 
 ```python
 from dv import AedatFile
 
 with AedatFile(<Path to aedat file>) as f:
     # list all the names of streams in the file
     print(f.names)
-    
+
     # loop through the "events" stream as numpy packets
     for e in f['events'].numpy():
         print(e.shape)
 ```
 
 **Example** Extract all events from a file into a numpy array
 
 ```python
 from dv import AedatFile
 import numpy as np
 
 with AedatFile(<Path to aedat file>) as f:
     # events will be a named numpy array
     events = np.hstack([packet for packet in f['events'].numpy()])
-    
+
     # Access information of all events by type
     timestamps, x, y, polarities = events['timestamp'], events['x'], events['y'], events['polarity']
     # Access individual events information
     event_123_x = events[123]['x']
     # Slice events
     first_100_events = events[:100]
 ```
@@ -164,15 +164,15 @@
 The configuration of DV at runtime is stored in a tree structure accesible over the network. The config tree is what is altered making changes in the dv gui. *dv-python* offers experimental wrappers for the `dv-control` command line utility to read and change config options at runtime from python.
 
 #### Example
 
 ```python
 from dv import Control
 
-ctrl = Control(address='localhost', port=4040)
+ctrl = Control(address='127.0.0.1', port=4040)
 print(ctrl.get('/mainloop/output_file/', 'file', 'string'))
 ctrl.put('/mainloop/accumulator/', 'running', 'bool', True)
 ```
 
 #### Available functions
 
 * `put(path, attribute, type, value)`
```

### Comparing `dv-1.0.8/dv/AedatFile.py` & `dv-1.0.9/dv/AedatFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,31 @@
 
     def source(self):
         if 'source' in self._stream_info:
             return self._stream_info['source']
         raise NameError('Source attribute not present for stream')
 
     def _read_next_packet(self):
-        if self._aedat_file._data_table_position > 0 and self._file.tell() >= self._aedat_file._data_table_position:
-            raise StopIteration
-
         packet_header = dv.fb.PacketHeader.PacketHeader()
-        packet_header_data = self._file.read(8)
-        # we reached end of file, there is no next package
-        if len(packet_header_data) < 8:
-            raise StopIteration
-
-        packet_header.Init(packet_header_data, 0)
-        # skip packet if not on our stream
-        if not packet_header.StreamID() == self._stream_id:
+
+        while True:
+            if self._aedat_file._data_table_position > 0 and self._file.tell() >= self._aedat_file._data_table_position:
+                raise StopIteration
+
+            packet_header_data = self._file.read(8)
+            # we reached end of file, there is no next package
+            if len(packet_header_data) < 8:
+                raise StopIteration
+
+            packet_header.Init(packet_header_data, 0)
+            # use packet if part of our stream (same ID)
+            if packet_header.StreamID() == self._stream_id:
+                break
+
             self._file.seek(packet_header.Size(), 1)
-            self._read_next_packet()
-            return
 
         packet_data_compressed = self._file.read(packet_header.Size())
         packet_data = None
         if self._aedat_file._compression == dv.fb.CompressionType.CompressionType.NONE:
             packet_data = packet_data_compressed
         elif self._aedat_file._compression == dv.fb.CompressionType.CompressionType.LZ4 or self._aedat_file._compression == dv.fb.CompressionType.CompressionType.LZ4_HIGH:
             packet_data = lz4.frame.decompress(packet_data_compressed)
```

### Comparing `dv-1.0.8/dv/Control.py` & `dv-1.0.9/dv/Control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import subprocess
 import warnings
 from subprocess import PIPE
 import platform
+import os
 
 
 class Control:
-    def __init__(self, address='localhost', port=4040):
-        if (platform.system().find("MINGW") != -1) or (platform.system() == "Windows"):
-            self._control_name = "dv-control.exe"
+    def __init__(self, address='127.0.0.1', port=4040):
+        if 'DV_CONTROL_PATH' in os.environ:
+            self._control_name = os.environ['DV_CONTROL_PATH']
         else:
-            self._control_name = "dv-control"
+            if (platform.system().upper().find("MINGW") != -1) or (platform.system() == "Windows"):
+                self._control_name = "dv-control.exe"
+            else:
+                self._control_name = "dv-control"
 
         self._address = address
         self._port = str(port)
 
     def _communicate(self, command):
-        proc = subprocess.Popen([self._control_name, '-i', self._address, '-p', self._port, '-s'] + command.split(' '), stdout=PIPE, stderr=PIPE)
+        proc = subprocess.Popen([self._control_name, '-i', self._address, '-p', self._port, '-s'] + command.split(' '),
+                                stdout=PIPE,
+                                stderr=PIPE)
         stdout, stderr = proc.communicate()
         error = stderr.decode('utf-8').strip() if stderr is not None else ''
         out = stdout.decode('utf-8').strip() if stdout is not None else ''
         exit_code = proc.returncode
 
         if exit_code != 0:
             raise RuntimeError('Could not perform action. exit code %d' % exit_code)
@@ -63,15 +69,16 @@
 
     def node_exists(self, path):
         output = self._communicate('node_exists %s' % path)
         return output == 'true'
 
     def attribute_exists(self, path, parameter, value_type=None):
         if value_type is not None:
-            warnings.warn("attribute_exists with value_type is deprecated. Use attribute_exists(path, parameter) instead", DeprecationWarning)
+            warnings.warn(
+                "attribute_exists with value_type is deprecated. Use attribute_exists(path, parameter) instead",
+                DeprecationWarning)
         output = self._communicate('attr_exists %s %s' % (path, parameter))
         return output == 'true'
 
     def get_children(self, path):
         output = self._communicate('get_children %s' % path)
         return [] if output == '' else output.strip().split('|')
-
```

### Comparing `dv-1.0.8/dv/Event.py` & `dv-1.0.9/dv/Event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import dv.fb.Event
 
-class Event(dv.fb.Event.Event):
 
+class Event(dv.fb.Event.Event):
     def __init__(self, fb_event):
         self._fb_event = fb_event
 
     @property
     def x(self):
         return self._fb_event.X()
 
@@ -18,16 +18,14 @@
         return self._fb_event.Polarity()
 
     @property
     def timestamp(self):
         return self._fb_event.Timestamp()
 
     def __str__(self):
-        return '{} ({:3d} {:3d}) | {:8d}'.format('+'
-                                                 if self._fb_event.polarity else '-',
-                                                 self._fb_event.x, self._fb_event.y, self._fb_event.timestamp)
+        return '{} ({:3d} {:3d}) | {:8d}'.format('+' if self._fb_event.Polarity() else '-', self._fb_event.X(),
+                                                 self._fb_event.Y(), self._fb_event.Timestamp())
 
     @classmethod
     def from_fb(cls, obj):
         obj.__class__ = Event
         return obj
-
```

### Comparing `dv-1.0.8/dv/EventFrameIterator.py` & `dv-1.0.9/dv/EventFrameIterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 class EventFrameIterator:
     def __init__(self, file, frameTime, shape):
         self.file = file
         self.frameTime = frameTime
         self.shape = shape
         self._iterator = iter(file)
 
@@ -12,14 +13,14 @@
 
     def __next__(self):
         frame = np.zeros(self.shape)
         first_event_time = -1
         for event in self._iterator:
             if first_event_time < 0:
                 first_event_time = event.timestamp
-            frame[self.shape[0]-event.y-1, event.x] += 1 if event.polarity else -1
+            frame[self.shape[0] - event.y - 1, event.x] += 1 if event.polarity else -1
             if event.timestamp - first_event_time >= self.frameTime * 1000:
                 break
 
         if first_event_time < 0:
             raise StopIteration
         return frame
```

### Comparing `dv-1.0.8/dv/Frame.py` & `dv-1.0.9/dv/Frame.py`

 * *Files identical despite different names*

### Comparing `dv-1.0.8/dv/IMU.py` & `dv-1.0.9/dv/IMU.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import dv.fb.IMU
 
 
 class IMUSample(dv.fb.IMU.IMU):
-
     def __init__(self, fb_sample):
         self._fb_sample = fb_sample
 
     @property
     def timestamp(self):
         return self._fb_sample.Timestamp()
 
@@ -25,8 +24,8 @@
     @property
     def magnetometer(self):
         return self._fb_sample.MagnetometerX(), self._fb_sample.MagnetometerY(), self._fb_sample.MagnetometerZ()
 
     @classmethod
     def from_fb(cls, obj):
         obj.__class__ = IMUSample
-        return obj
+        return obj
```

### Comparing `dv-1.0.8/dv/LegacyAedatFile.py` & `dv-1.0.9/dv/LegacyAedatFile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import struct
 import re
 import sys
 import numpy as np
 from enum import Enum
 
+
 class Type(Enum):
     Event = 0
     Frame = 1
 
+
 class LegacyEvent:
     def __init__(self, x, y, polarity, timestamp):
         self.x = x
         self.y = y
         self.polarity = polarity
         self.timestamp = timestamp
         self.type = Type.Event
 
     def __str__(self):
         return '{} ({:3d} {:3d}) | {:8d}'.format('+' if self.polarity else '-', self.x, self.y, self.timestamp)
 
+
 class LegacyFrame:
     def __init__(self, width, height):
         self.image = np.zeros((height, width), dtype='uint8')
         self.start_of_frame = -1
         self.end_of_frame = -1
         self.start_of_exposure = -1
         self.end_of_exposure = -1
@@ -116,32 +119,31 @@
             x = (address & 0x3FF000) >> 12
             if timestamp32 < last_timestamp32:
                 tsoverflow += 1
 
             last_timestamp32 = timestamp32
             timestamp = timestamp32 | tsoverflow << 31
 
-
             if (address >> 31) & 0x1 > 0:  # non polarity data
                 if not self.enable_frames:
                     continue
 
                 type_info = (address & 0xC00) >> 10
                 adc_value = (address & 0x3FF) >> 2
-                if type_info == 0: # aps reset read
+                if type_info == 0:  # aps reset read
                     if current_frame.reset_count == 0:
                         current_frame.start_of_frame = timestamp
                     current_frame.start_of_exposure = timestamp
-                    current_frame.image[self.frame_height-y-1, x] = adc_value
+                    current_frame.image[self.frame_height - y - 1, x] = adc_value
                     current_frame.reset_count += 1
-                elif type_info == 1: # aps signal read
+                elif type_info == 1:  # aps signal read
                     if current_frame.signal_count == 0:
                         current_frame.end_of_exposure = timestamp
                     current_frame.end_of_frame = timestamp
-                    current_frame.image[self.frame_height-y-1, x] -= adc_value
+                    current_frame.image[self.frame_height - y - 1, x] -= adc_value
                     current_frame.signal_count += 1
 
                 if current_frame.signal_count >= self.frame_height * self.frame_width:
                     yield current_frame
                     current_frame = LegacyFrame(self.frame_width, self.frame_height)
 
             else:  #polarity data
@@ -178,8 +180,7 @@
                     y = (aer_data >> 2) & 0x00007FFF
                     pol = (aer_data >> 1) & 0x00000001
                     counter = counter + size
                     yield LegacyEvent(x, y, pol, timestamp)
             else:
                 # non-polarity event packet, not implemented
                 pass
-
```

### Comparing `dv-1.0.8/dv/NetworkInput.py` & `dv-1.0.9/dv/NetworkInput.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,26 +36,26 @@
 
     def __next__(self):
         if self._packet is None:
             self._receive_next_packet()
 
     def _receive_next_packet(self):
         io_header = self._socket.recv(8, socket.MSG_WAITALL)
-        length = int.from_bytes(io_header[4:],  byteorder='little')
+        length = int.from_bytes(io_header[4:], byteorder='little')
         packet_data = self._socket.recv(length, socket.MSG_WAITALL)
         packet_data = packet_data[4:]
         self._packetIteratorPosition = 0
         self._parse_packet(packet_data)
 
     def _parse_packet(self, packet_data):
         pass
 
 
 class NetworkEventInput(_NetworkInput):
-    def __init__(self, address='localhost', port=7777):
+    def __init__(self, address='127.0.0.1', port=7777):
         super().__init__(address, port)
 
     def _parse_packet(self, packet_data):
         self._packet = dv.fb.EventPacket.EventPacket.GetRootAsEventPacket(packet_data, 0)
 
     def __next__(self):
         super().__next__()
@@ -63,43 +63,43 @@
         self._packetIteratorPosition += 1
         if self._packetIteratorPosition >= self._packet.EventsLength():
             self._packet = None
         return event
 
 
 class NetworkNumpyEventPacketInput(_NetworkInput):
-    def __init__(self, address='localhost', port=7777):
+    def __init__(self, address='127.0.0.1', port=7777):
         super().__init__(address, port)
 
     def _parse_packet(self, packet_data):
         self._packet = dv.fb.EventPacket.EventPacket.GetRootAsEventPacket(packet_data, 0)
 
     def __next__(self):
         super().__next__()
         buff = self._packet.EventsBufferAsNumpy()
         self._packet = None
         return buff
 
 
 class NetworkFrameInput(_NetworkInput):
-    def __init__(self, address='localhost', port=7777):
+    def __init__(self, address='127.0.0.1', port=7777):
         super().__init__(address, port)
 
     def _parse_packet(self, packet_data):
         self._packet = dv.fb.Frame.Frame.GetRootAsFrame(packet_data, 0)
 
     def __next__(self):
         super().__next__()
         frame = Frame.Frame(self._packet)
         self._packet = None
         return frame
 
 
 class NetworkIMUInput(_NetworkInput):
-    def __init__(self, address='localhost', port=7777):
+    def __init__(self, address='127.0.0.1', port=7777):
         super().__init__(address, port)
 
     def _parse_packet(self, packet_data):
         self._packet = dv.fb.IMUPacket.IMUPacket.GetRootAsIMUPacket(packet_data, 0)
 
     def __next__(self):
         super().__next__()
@@ -107,22 +107,20 @@
         self._packetIteratorPosition += 1
         if self._packetIteratorPosition >= self._packet.SamplesLength():
             self._packet = None
         return sample
 
 
 class NetworkTriggerInput(_NetworkInput):
-    def __init__(self, address='localhost', port=7777):
+    def __init__(self, address='127.0.0.1', port=7777):
         super().__init__(address, port)
 
     def _parse_packet(self, packet_data):
         self._packet = dv.fb.TriggerPacket.TriggerPacket.GetRootAsTriggerPacket(packet_data, 0)
 
     def __next__(self):
         super().__next__()
         trigger = Trigger.Trigger(self._packet.Triggers(self._packetIteratorPosition))
         self._packetIteratorPosition += 1
         if self._packetIteratorPosition >= self._packet.TriggersLength():
             self._packet = None
         return trigger
-
-
```

### Comparing `dv-1.0.8/dv/fb/Event.py` & `dv-1.0.9/dv/fb/Event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class Event(object):
     __slots__ = ['_tab']
 
     # Event
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
+
 # /// Timestamp (µs).
+# Event
+
+    def Timestamp(self):
+        return self._tab.Get(flatbuffers.number_types.Int64Flags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(0))
+
     # Event
-    def Timestamp(self): return self._tab.Get(flatbuffers.number_types.Int64Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(0))
-    # Event
-    def X(self): return self._tab.Get(flatbuffers.number_types.Int16Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(8))
+    def X(self):
+        return self._tab.Get(flatbuffers.number_types.Int16Flags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(8))
+
     # Event
-    def Y(self): return self._tab.Get(flatbuffers.number_types.Int16Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(10))
+    def Y(self):
+        return self._tab.Get(flatbuffers.number_types.Int16Flags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(10))
+
     # Event
-    def Polarity(self): return self._tab.Get(flatbuffers.number_types.BoolFlags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(12))
+    def Polarity(self):
+        return self._tab.Get(flatbuffers.number_types.BoolFlags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(12))
+
 
 def CreateEvent(builder, timestamp, x, y, polarity):
     builder.Prep(8, 16)
     builder.Pad(3)
     builder.PrependBool(polarity)
     builder.PrependInt16(y)
     builder.PrependInt16(x)
```

### Comparing `dv-1.0.8/dv/fb/EventPacket.py` & `dv-1.0.9/dv/fb/EventPacket.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # namespace: dv
 
 import flatbuffers
 from .util import import_numpy
 
 np = import_numpy()
 
+
 class EventPacket(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsEventPacket(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = EventPacket()
@@ -49,11 +50,22 @@
 
         np_dtype = np.dtype({
             'names': ['timestamp', 'x', 'y', 'polarity', '_p1', '_p2'],
             'formats': ['<i8', '<i2', '<i2', '<i1', '<i2', '<i1']
         })
         return np.frombuffer(self._tab.Bytes, dtype=np_dtype, count=count, offset=offset)
 
-def EventPacketStart(builder): builder.StartObject(1)
-def EventPacketAddEvents(builder, events): builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(events), 0)
-def EventPacketStartEventsVector(builder, numElems): return builder.StartVector(16, numElems, 8)
-def EventPacketEnd(builder): return builder.EndObject()
+
+def EventPacketStart(builder):
+    builder.StartObject(1)
+
+
+def EventPacketAddEvents(builder, events):
+    builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(events), 0)
+
+
+def EventPacketStartEventsVector(builder, numElems):
+    return builder.StartVector(16, numElems, 8)
+
+
+def EventPacketEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/FileDataDefinition.py` & `dv-1.0.9/dv/fb/FileDataDefinition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class FileDataDefinition(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsFileDataDefinition(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = FileDataDefinition()
@@ -53,14 +54,34 @@
     # FileDataDefinition
     def TimestampEnd(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
-def FileDataDefinitionStart(builder): builder.StartObject(5)
-def FileDataDefinitionAddByteOffset(builder, ByteOffset): builder.PrependInt64Slot(0, ByteOffset, 0)
-def FileDataDefinitionAddPacketInfo(builder, PacketInfo): builder.PrependStructSlot(1, flatbuffers.number_types.UOffsetTFlags.py_type(PacketInfo), 0)
-def FileDataDefinitionAddNumElements(builder, NumElements): builder.PrependInt64Slot(2, NumElements, 0)
-def FileDataDefinitionAddTimestampStart(builder, TimestampStart): builder.PrependInt64Slot(3, TimestampStart, 0)
-def FileDataDefinitionAddTimestampEnd(builder, TimestampEnd): builder.PrependInt64Slot(4, TimestampEnd, 0)
-def FileDataDefinitionEnd(builder): return builder.EndObject()
+
+def FileDataDefinitionStart(builder):
+    builder.StartObject(5)
+
+
+def FileDataDefinitionAddByteOffset(builder, ByteOffset):
+    builder.PrependInt64Slot(0, ByteOffset, 0)
+
+
+def FileDataDefinitionAddPacketInfo(builder, PacketInfo):
+    builder.PrependStructSlot(1, flatbuffers.number_types.UOffsetTFlags.py_type(PacketInfo), 0)
+
+
+def FileDataDefinitionAddNumElements(builder, NumElements):
+    builder.PrependInt64Slot(2, NumElements, 0)
+
+
+def FileDataDefinitionAddTimestampStart(builder, TimestampStart):
+    builder.PrependInt64Slot(3, TimestampStart, 0)
+
+
+def FileDataDefinitionAddTimestampEnd(builder, TimestampEnd):
+    builder.PrependInt64Slot(4, TimestampEnd, 0)
+
+
+def FileDataDefinitionEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/FileDataTable.py` & `dv-1.0.9/dv/fb/FileDataTable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class FileDataTable(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsFileDataTable(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = FileDataTable()
@@ -34,11 +35,22 @@
     # FileDataTable
     def TableLength(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
             return self._tab.VectorLen(o)
         return 0
 
-def FileDataTableStart(builder): builder.StartObject(1)
-def FileDataTableAddTable(builder, Table): builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(Table), 0)
-def FileDataTableStartTableVector(builder, numElems): return builder.StartVector(4, numElems, 4)
-def FileDataTableEnd(builder): return builder.EndObject()
+
+def FileDataTableStart(builder):
+    builder.StartObject(1)
+
+
+def FileDataTableAddTable(builder, Table):
+    builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(Table), 0)
+
+
+def FileDataTableStartTableVector(builder, numElems):
+    return builder.StartVector(4, numElems, 4)
+
+
+def FileDataTableEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/Frame.py` & `dv-1.0.9/dv/fb/Frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class Frame(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsFrame(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = Frame()
@@ -15,100 +16,113 @@
         return x
 
     # Frame
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
 # /// Central timestamp (µs), corresponds to exposure midpoint.
-    # Frame
+# Frame
+
     def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// Start of Frame (SOF) timestamp.
-    # Frame
+# Frame
+
     def TimestampStartOfFrame(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// End of Frame (EOF) timestamp.
-    # Frame
+# Frame
+
     def TimestampEndOfFrame(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// Start of Exposure (SOE) timestamp.
-    # Frame
+# Frame
+
     def TimestampStartOfExposure(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// End of Exposure (EOE) timestamp.
-    # Frame
+# Frame
+
     def TimestampEndOfExposure(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// Pixel format (grayscale, RGB, ...).
-    # Frame
+# Frame
+
     def Format(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int8Flags, o + self._tab.Pos)
         return 0
 
 # /// X axis length in pixels.
-    # Frame
+# Frame
+
     def SizeX(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int16Flags, o + self._tab.Pos)
         return 0
 
 # /// Y axis length in pixels.
-    # Frame
+# Frame
+
     def SizeY(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(18))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int16Flags, o + self._tab.Pos)
         return 0
 
 # /// X axis position (upper left offset) in pixels.
-    # Frame
+# Frame
+
     def PositionX(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(20))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int16Flags, o + self._tab.Pos)
         return 0
 
 # /// Y axis position (upper left offset) in pixels.
-    # Frame
+# Frame
+
     def PositionY(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(22))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int16Flags, o + self._tab.Pos)
         return 0
 
+
 # /// Pixel values, 8bit depth.
-    # Frame
+# Frame
+
     def Pixels(self, j):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
         if o != 0:
             a = self._tab.Vector(o)
-            return self._tab.Get(flatbuffers.number_types.Uint8Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 1))
+            return self._tab.Get(flatbuffers.number_types.Uint8Flags,
+                                 a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 1))
         return 0
 
     # Frame
     def PixelsAsNumpy(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
         if o != 0:
             return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Uint8Flags, o)
@@ -117,21 +131,62 @@
     # Frame
     def PixelsLength(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
         if o != 0:
             return self._tab.VectorLen(o)
         return 0
 
-def FrameStart(builder): builder.StartObject(11)
-def FrameAddTimestamp(builder, timestamp): builder.PrependInt64Slot(0, timestamp, 0)
-def FrameAddTimestampStartOfFrame(builder, timestampStartOfFrame): builder.PrependInt64Slot(1, timestampStartOfFrame, 0)
-def FrameAddTimestampEndOfFrame(builder, timestampEndOfFrame): builder.PrependInt64Slot(2, timestampEndOfFrame, 0)
-def FrameAddTimestampStartOfExposure(builder, timestampStartOfExposure): builder.PrependInt64Slot(3, timestampStartOfExposure, 0)
-def FrameAddTimestampEndOfExposure(builder, timestampEndOfExposure): builder.PrependInt64Slot(4, timestampEndOfExposure, 0)
-def FrameAddFormat(builder, format): builder.PrependInt8Slot(5, format, 0)
-def FrameAddSizeX(builder, sizeX): builder.PrependInt16Slot(6, sizeX, 0)
-def FrameAddSizeY(builder, sizeY): builder.PrependInt16Slot(7, sizeY, 0)
-def FrameAddPositionX(builder, positionX): builder.PrependInt16Slot(8, positionX, 0)
-def FrameAddPositionY(builder, positionY): builder.PrependInt16Slot(9, positionY, 0)
-def FrameAddPixels(builder, pixels): builder.PrependUOffsetTRelativeSlot(10, flatbuffers.number_types.UOffsetTFlags.py_type(pixels), 0)
-def FrameStartPixelsVector(builder, numElems): return builder.StartVector(1, numElems, 1)
-def FrameEnd(builder): return builder.EndObject()
+
+def FrameStart(builder):
+    builder.StartObject(11)
+
+
+def FrameAddTimestamp(builder, timestamp):
+    builder.PrependInt64Slot(0, timestamp, 0)
+
+
+def FrameAddTimestampStartOfFrame(builder, timestampStartOfFrame):
+    builder.PrependInt64Slot(1, timestampStartOfFrame, 0)
+
+
+def FrameAddTimestampEndOfFrame(builder, timestampEndOfFrame):
+    builder.PrependInt64Slot(2, timestampEndOfFrame, 0)
+
+
+def FrameAddTimestampStartOfExposure(builder, timestampStartOfExposure):
+    builder.PrependInt64Slot(3, timestampStartOfExposure, 0)
+
+
+def FrameAddTimestampEndOfExposure(builder, timestampEndOfExposure):
+    builder.PrependInt64Slot(4, timestampEndOfExposure, 0)
+
+
+def FrameAddFormat(builder, format):
+    builder.PrependInt8Slot(5, format, 0)
+
+
+def FrameAddSizeX(builder, sizeX):
+    builder.PrependInt16Slot(6, sizeX, 0)
+
+
+def FrameAddSizeY(builder, sizeY):
+    builder.PrependInt16Slot(7, sizeY, 0)
+
+
+def FrameAddPositionX(builder, positionX):
+    builder.PrependInt16Slot(8, positionX, 0)
+
+
+def FrameAddPositionY(builder, positionY):
+    builder.PrependInt16Slot(9, positionY, 0)
+
+
+def FrameAddPixels(builder, pixels):
+    builder.PrependUOffsetTRelativeSlot(10, flatbuffers.number_types.UOffsetTFlags.py_type(pixels), 0)
+
+
+def FrameStartPixelsVector(builder, numElems):
+    return builder.StartVector(1, numElems, 1)
+
+
+def FrameEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/IMU.py` & `dv-1.0.9/dv/fb/IMU.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class IMU(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsIMU(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = IMU()
@@ -15,107 +16,157 @@
         return x
 
     # IMU
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
 # /// Timestamp (µs).
-    # IMU
+# IMU
+
     def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
         return 0
 
 # /// Temperature, measured in °C.
-    # IMU
+# IMU
+
     def Temperature(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Acceleration in the X axis, measured in g (9.81m/s²).
-    # IMU
+# IMU
+
     def AccelerometerX(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Acceleration in the Y axis, measured in g (9.81m/s²).
-    # IMU
+# IMU
+
     def AccelerometerY(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Acceleration in the Z axis, measured in g (9.81m/s²).
-    # IMU
+# IMU
+
     def AccelerometerZ(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(12))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Rotation in the X axis, measured in °/s.
-    # IMU
+# IMU
+
     def GyroscopeX(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(14))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Rotation in the Y axis, measured in °/s.
-    # IMU
+# IMU
+
     def GyroscopeY(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(16))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Rotation in the Z axis, measured in °/s.
-    # IMU
+# IMU
+
     def GyroscopeZ(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(18))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Magnetometer X axis, measured in µT (magnetic flux density).
-    # IMU
+# IMU
+
     def MagnetometerX(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(20))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
 # /// Magnetometer Y axis, measured in µT (magnetic flux density).
-    # IMU
+# IMU
+
     def MagnetometerY(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(22))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
+
 # /// Magnetometer Z axis, measured in µT (magnetic flux density).
-    # IMU
+# IMU
+
     def MagnetometerZ(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(24))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
         return 0.0
 
-def IMUStart(builder): builder.StartObject(11)
-def IMUAddTimestamp(builder, timestamp): builder.PrependInt64Slot(0, timestamp, 0)
-def IMUAddTemperature(builder, temperature): builder.PrependFloat32Slot(1, temperature, 0.0)
-def IMUAddAccelerometerX(builder, accelerometerX): builder.PrependFloat32Slot(2, accelerometerX, 0.0)
-def IMUAddAccelerometerY(builder, accelerometerY): builder.PrependFloat32Slot(3, accelerometerY, 0.0)
-def IMUAddAccelerometerZ(builder, accelerometerZ): builder.PrependFloat32Slot(4, accelerometerZ, 0.0)
-def IMUAddGyroscopeX(builder, gyroscopeX): builder.PrependFloat32Slot(5, gyroscopeX, 0.0)
-def IMUAddGyroscopeY(builder, gyroscopeY): builder.PrependFloat32Slot(6, gyroscopeY, 0.0)
-def IMUAddGyroscopeZ(builder, gyroscopeZ): builder.PrependFloat32Slot(7, gyroscopeZ, 0.0)
-def IMUAddMagnetometerX(builder, magnetometerX): builder.PrependFloat32Slot(8, magnetometerX, 0.0)
-def IMUAddMagnetometerY(builder, magnetometerY): builder.PrependFloat32Slot(9, magnetometerY, 0.0)
-def IMUAddMagnetometerZ(builder, magnetometerZ): builder.PrependFloat32Slot(10, magnetometerZ, 0.0)
-def IMUEnd(builder): return builder.EndObject()
+
+def IMUStart(builder):
+    builder.StartObject(11)
+
+
+def IMUAddTimestamp(builder, timestamp):
+    builder.PrependInt64Slot(0, timestamp, 0)
+
+
+def IMUAddTemperature(builder, temperature):
+    builder.PrependFloat32Slot(1, temperature, 0.0)
+
+
+def IMUAddAccelerometerX(builder, accelerometerX):
+    builder.PrependFloat32Slot(2, accelerometerX, 0.0)
+
+
+def IMUAddAccelerometerY(builder, accelerometerY):
+    builder.PrependFloat32Slot(3, accelerometerY, 0.0)
+
+
+def IMUAddAccelerometerZ(builder, accelerometerZ):
+    builder.PrependFloat32Slot(4, accelerometerZ, 0.0)
+
+
+def IMUAddGyroscopeX(builder, gyroscopeX):
+    builder.PrependFloat32Slot(5, gyroscopeX, 0.0)
+
+
+def IMUAddGyroscopeY(builder, gyroscopeY):
+    builder.PrependFloat32Slot(6, gyroscopeY, 0.0)
+
+
+def IMUAddGyroscopeZ(builder, gyroscopeZ):
+    builder.PrependFloat32Slot(7, gyroscopeZ, 0.0)
+
+
+def IMUAddMagnetometerX(builder, magnetometerX):
+    builder.PrependFloat32Slot(8, magnetometerX, 0.0)
+
+
+def IMUAddMagnetometerY(builder, magnetometerY):
+    builder.PrependFloat32Slot(9, magnetometerY, 0.0)
+
+
+def IMUAddMagnetometerZ(builder, magnetometerZ):
+    builder.PrependFloat32Slot(10, magnetometerZ, 0.0)
+
+
+def IMUEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/IMUPacket.py` & `dv-1.0.9/dv/fb/Trigger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
-class IMUPacket(object):
+
+class Trigger(object):
     __slots__ = ['_tab']
 
     @classmethod
-    def GetRootAsIMUPacket(cls, buf, offset):
+    def GetRootAsTrigger(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
-        x = IMUPacket()
+        x = Trigger()
         x.Init(buf, n + offset)
         return x
 
-    # IMUPacket
+    # Trigger
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
-    # IMUPacket
-    def Samples(self, j):
+# /// Timestamp (µs).
+# Trigger
+
+    def Timestamp(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
-            x = self._tab.Vector(o)
-            x += flatbuffers.number_types.UOffsetTFlags.py_type(j) * 4
-            x = self._tab.Indirect(x)
-            from .IMU import IMU
-            obj = IMU()
-            obj.Init(self._tab.Bytes, x)
-            return obj
-        return None
+            return self._tab.Get(flatbuffers.number_types.Int64Flags, o + self._tab.Pos)
+        return 0
 
-    # IMUPacket
-    def SamplesLength(self):
-        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+
+# /// Type of trigger that occurred.
+# Trigger
+
+    def Type(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
         if o != 0:
-            return self._tab.VectorLen(o)
+            return self._tab.Get(flatbuffers.number_types.Int8Flags, o + self._tab.Pos)
         return 0
 
-def IMUPacketStart(builder): builder.StartObject(1)
-def IMUPacketAddSamples(builder, samples): builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(samples), 0)
-def IMUPacketStartSamplesVector(builder, numElems): return builder.StartVector(4, numElems, 4)
-def IMUPacketEnd(builder): return builder.EndObject()
+
+def TriggerStart(builder):
+    builder.StartObject(2)
+
+
+def TriggerAddTimestamp(builder, timestamp):
+    builder.PrependInt64Slot(0, timestamp, 0)
+
+
+def TriggerAddType(builder, type):
+    builder.PrependInt8Slot(1, type, 0)
+
+
+def TriggerEnd(builder):
+    return builder.EndObject()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dv-1.0.8/dv/fb/PacketHeader.py` & `dv-1.0.9/dv/fb/PacketHeader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class PacketHeader(object):
     __slots__ = ['_tab']
 
     # PacketHeader
     def Init(self, buf, pos):
         self._tab = flatbuffers.table.Table(buf, pos)
 
     # PacketHeader
-    def StreamID(self): return self._tab.Get(flatbuffers.number_types.Int32Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(0))
+    def StreamID(self):
+        return self._tab.Get(flatbuffers.number_types.Int32Flags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(0))
+
     # PacketHeader
-    def Size(self): return self._tab.Get(flatbuffers.number_types.Int32Flags, self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(4))
+    def Size(self):
+        return self._tab.Get(flatbuffers.number_types.Int32Flags,
+                             self._tab.Pos + flatbuffers.number_types.UOffsetTFlags.py_type(4))
+
 
 def CreatePacketHeader(builder, StreamID, Size):
     builder.Prep(4, 8)
     builder.PrependInt32(Size)
     builder.PrependInt32(StreamID)
     return builder.Offset()
```

### Comparing `dv-1.0.8/dv/fb/TriggerPacket.py` & `dv-1.0.9/dv/fb/TriggerPacket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
 import flatbuffers
 
+
 class TriggerPacket(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAsTriggerPacket(cls, buf, offset):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = TriggerPacket()
@@ -34,11 +35,22 @@
     # TriggerPacket
     def TriggersLength(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         if o != 0:
             return self._tab.VectorLen(o)
         return 0
 
-def TriggerPacketStart(builder): builder.StartObject(1)
-def TriggerPacketAddTriggers(builder, triggers): builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(triggers), 0)
-def TriggerPacketStartTriggersVector(builder, numElems): return builder.StartVector(4, numElems, 4)
-def TriggerPacketEnd(builder): return builder.EndObject()
+
+def TriggerPacketStart(builder):
+    builder.StartObject(1)
+
+
+def TriggerPacketAddTriggers(builder, triggers):
+    builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(triggers), 0)
+
+
+def TriggerPacketStartTriggersVector(builder, numElems):
+    return builder.StartVector(4, numElems, 4)
+
+
+def TriggerPacketEnd(builder):
+    return builder.EndObject()
```

### Comparing `dv-1.0.8/dv/fb/TriggerType.py` & `dv-1.0.9/dv/fb/TriggerType.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # automatically generated by the FlatBuffers compiler, do not modify
 
 # namespace: dv
 
+
 class TriggerType(object):
-# /// A timestamp reset occurred.
+    # /// A timestamp reset occurred.
     TIMESTAMP_RESET = 0
-# /// A rising edge was detected (External Input module on device).
+    # /// A rising edge was detected (External Input module on device).
     EXTERNAL_SIGNAL_RISING_EDGE = 1
-# /// A falling edge was detected (External Input module on device).
+    # /// A falling edge was detected (External Input module on device).
     EXTERNAL_SIGNAL_FALLING_EDGE = 2
-# /// A pulse was detected (External Input module on device).
+    # /// A pulse was detected (External Input module on device).
     EXTERNAL_SIGNAL_PULSE = 3
-# /// A rising edge was generated (External Generator module on device).
+    # /// A rising edge was generated (External Generator module on device).
     EXTERNAL_GENERATOR_RISING_EDGE = 4
-# /// A falling edge was generated (External Generator module on device).
+    # /// A falling edge was generated (External Generator module on device).
     EXTERNAL_GENERATOR_FALLING_EDGE = 5
-# /// An APS frame capture has started (Frame Event will follow).
+    # /// An APS frame capture has started (Frame Event will follow).
     APS_FRAME_START = 6
-# /// An APS frame capture has completed (Frame Event is contemporary).
+    # /// An APS frame capture has completed (Frame Event is contemporary).
     APS_FRAME_END = 7
-# /// An APS frame exposure has started (Frame Event will follow).
+    # /// An APS frame exposure has started (Frame Event will follow).
     APS_EXPOSURE_START = 8
-# /// An APS frame exposure has completed (Frame Event will follow).
+    # /// An APS frame exposure has completed (Frame Event will follow).
     APS_EXPOSURE_END = 9
-
```

### Comparing `dv-1.0.8/dv/fb/util.py` & `dv-1.0.9/dv/fb/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import imp
 
+
 def import_numpy():
     """
     Returns the numpy module if it exists on the system,
     otherwise returns None.
     """
     try:
         imp.find_module('numpy')
```

### Comparing `dv-1.0.8/dv.egg-info/SOURCES.txt` & `dv-1.0.9/dv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dv-1.0.8/setup.py` & `dv-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from setuptools import setup
 
+
 def get_version_from_file():
-      with open('VERSION.txt', 'r') as version_file:
-            tag = version_file.read()
-      return tag
+    with open('VERSION.txt', 'r') as version_file:
+        tag = version_file.read()
+    return tag
 
 
 setup(name='dv',
       version=get_version_from_file(),
       description='Library to connect to DV event based vision software',
       url='https://gitlab.com/inivation/dv/dv-python/',
       author='iniVation AG',
       author_email='support@inivation.com',
       license='AGPLv3',
       packages=['dv', 'dv.fb'],
-      install_requires=[
-        'flatbuffers',
-        'numpy',
-        'lz4',
-        'zstd'
-      ],
+      install_requires=['flatbuffers', 'numpy', 'lz4', 'zstd'],
       python_requires='>=3',
       zip_safe=False)
```

