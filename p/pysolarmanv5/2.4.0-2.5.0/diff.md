# Comparing `tmp/pysolarmanv5-2.4.0.tar.gz` & `tmp/pysolarmanv5-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarmanv5-2.4.0.tar", last modified: Mon Jul 18 23:36:38 2022, max compression
+gzip compressed data, was "pysolarmanv5-2.5.0.tar", last modified: Wed May 10 00:00:49 2023, max compression
```

## Comparing `pysolarmanv5-2.4.0.tar` & `pysolarmanv5-2.5.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2022-07-18 23:36:38.659611 pysolarmanv5-2.4.0/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2022-07-18 23:30:58.000000 pysolarmanv5-2.4.0/LICENSE
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     2389 2022-07-18 23:36:38.659611 pysolarmanv5-2.4.0/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1833 2022-07-18 23:30:58.000000 pysolarmanv5-2.4.0/README.md
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2022-07-18 23:36:38.655611 pysolarmanv5-2.4.0/pysolarmanv5/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      195 2022-07-18 23:30:58.000000 pysolarmanv5-2.4.0/pysolarmanv5/__init__.py
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    20653 2022-07-18 23:30:58.000000 pysolarmanv5-2.4.0/pysolarmanv5/pysolarmanv5.py
-drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2022-07-18 23:36:38.659611 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     2389 2022-07-18 23:36:38.000000 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/PKG-INFO
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      259 2022-07-18 23:36:38.000000 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/SOURCES.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2022-07-18 23:36:38.000000 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/dependency_links.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        8 2022-07-18 23:36:38.000000 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/requires.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2022-07-18 23:36:38.000000 pysolarmanv5-2.4.0/pysolarmanv5.egg-info/top_level.txt
--rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2022-07-18 23:36:38.659611 pysolarmanv5-2.4.0/setup.cfg
--rwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)      878 2022-07-18 23:30:58.000000 pysolarmanv5-2.4.0/setup.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1083 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/LICENSE
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     3327 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/README.md
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1038 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pyproject.toml
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/pysolarmanv5/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      358 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/__init__.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    26107 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)    17728 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5_async.py
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     4134 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/PKG-INFO
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)      360 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/SOURCES.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)        1 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/dependency_links.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       35 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/requires.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       13 2023-05-10 00:00:49.000000 pysolarmanv5-2.5.0/pysolarmanv5.egg-info/top_level.txt
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)       38 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/setup.cfg
+drwxr-xr-x   0 jmccrohan  (1000) jmccrohan  (1000)        0 2023-05-10 00:00:49.141669 pysolarmanv5-2.5.0/tests/
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1329 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/tests/test_aio_solarman.py
+-rw-r--r--   0 jmccrohan  (1000) jmccrohan  (1000)     1061 2023-05-09 23:59:31.000000 pysolarmanv5-2.5.0/tests/test_solarman.py
```

### Comparing `pysolarmanv5-2.4.0/LICENSE` & `pysolarmanv5-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarmanv5-2.4.0/PKG-INFO` & `pysolarmanv5-2.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-Metadata-Version: 2.1
-Name: pysolarmanv5
-Version: 2.4.0
-Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
-Home-page: https://github.com/jmccrohan/pysolarmanv5
-Author: Jonathan McCrohan
-Author-email: jmccrohan@gmail.com
-License: BSD
-Keywords: solarman igen-tech modbus solar inverter solarmanv5
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pysolarmanv5
 
 This is a Python module to interact with Solarman (IGEN-Tech) v5 based solar
 inverter data loggers. Modbus RTU frames can be encapsulated in the proprietary
 Solarman v5 protocol and requests sent to the data logger on port tcp/8899.
 
-This module aims to simplify the Solarman v5 protocol, exposing interfaces
-similar to that of the [uModbus](https://pysolarmanv5.readthedocs.io/) library.
+This module aims to simplify the Solarman v5 protocol, exposing both sync and
+async interfaces similar to that of the [uModbus](https://pysolarmanv5.readthedocs.io/)
+library.
 
 Details of the Solarman v5 protocol have been based on the excellent work of
 [Inverter-Data-Logger by XtheOne](https://github.com/XtheOne/Inverter-Data-Logger/)
 and others.
 
 ## Documentation
 
@@ -33,17 +18,23 @@
 
 The Solarman V5 protocol is documented [here](https://pysolarmanv5.readthedocs.io/en/latest/solarmanv5_protocol.html).
 
 ## Supported Devices
 
 A user contributed list of supported devices is available [here](https://github.com/jmccrohan/pysolarmanv5/issues/11).
 
+If you are unsure if your device is supported, please use the [solarman_scan](https://github.com/jmccrohan/pysolarmanv5/blob/main/utils/solarman_scan.py) 
+utility to find compatible data logging sticks on your local network.
+
 Please note that the **Solis S3-WIFI-ST** data logging stick is **NOT supported**.  
 See [GH issue #8](https://github.com/jmccrohan/pysolarmanv5/issues/8) for further information. 
 
+Some Ethernet data logging sticks have native support Modbus TCP and therefore **do not require pysolarmanv5**.
+See [GH issue #5](https://github.com/jmccrohan/pysolarmanv5/issues/5) for further information. 
+
 ## Dependencies
 
 - pysolarmanv5 requires Python 3.8 or greater.
 - pysolarmanv5 depends on [uModbus](https://github.com/AdvancedClimateSystems/uModbus).
 
 ## Installation
 
@@ -51,14 +42,30 @@
 
 `pip install pysolarmanv5`
 
 To install the latest development version from git, run:
 
 `pip install git+https://github.com/jmccrohan/pysolarmanv5.git`
 
+## Projects using pysolarmanv5
+
+- [NosIreland/solismon3](https://github.com/NosIreland/solismon3)
+- [NosIreland/solismod](https://github.com/NosIreland/solismod)
+- [jmccrohan/ha_pyscript_pysolarmanv5](https://github.com/jmccrohan/ha_pyscript_pysolarmanv5)
+- [YodaDaCoda/hass-solarman-modbus](https://github.com/YodaDaCoda/hass-solarman-modbus)
+- [schwatter/solarman_mqtt](https://github.com/schwatter/solarman_mqtt)
+- [RonnyKempe/solismon](https://github.com/RonnyKempe/solismon)
+- [toledobastos/solarman_battery_autocharge](https://github.com/toledobastos/solarman_battery_autocharge)
+- [AndyTaylorTweet/solis2mqtt](https://github.com/AndyTaylorTweet/solis2mqtt)
+- [pixellos/codereinvented.automation.py](https://github.com/pixellos/codereinvented.automation.py)
+- [cjgwhite/hass-solar](https://github.com/cjgwhite/hass-solar)
+- [imcfarla2003/solarconfig](https://github.com/imcfarla2003/solarconfig)
+- [githubDante/deye-controller](https://github.com/githubDante/deye-controller)
+- [danfoster/solis](https://github.com/danfoster/solis)
+
 ## Contributions
 
 Contributions welcome. Please raise any Issues / Pull Requests via [Github](https://github.com/jmccrohan/pysolarmanv5).
 
 ## License
 
-pysolarmanv5 is licensed under the [MIT License](https://github.com/jmccrohan/pysolarmanv5/blob/master/LICENSE). Copyright (c) 2022 Jonathan McCrohan
+pysolarmanv5 is licensed under the [MIT License](https://github.com/jmccrohan/pysolarmanv5/blob/master/LICENSE). Copyright (c) 2023 Jonathan McCrohan
```

### Comparing `pysolarmanv5-2.4.0/pysolarmanv5/pysolarmanv5.py` & `pysolarmanv5-2.5.0/pysolarmanv5/pysolarmanv5.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 """pysolarmanv5.py"""
+import queue
 import struct
 import socket
 import logging
+import select
+from threading import Thread, Event
+from multiprocessing import Queue
+from typing import Any
+from random import randrange
 
 from umodbus.client.serial import rtu
 
 
 class V5FrameError(Exception):
     """V5 Frame Validation Error"""
 
@@ -47,14 +53,21 @@
     :type logger: Logger, optional
     :param socket: TCP Socket connection to data logging stick. If **socket**
         argument is provided, **address** argument is unused (however, it is
         still required as a positional argument)
     :type socket: Socket, optional
     :raises NoSocketAvailableError: If no network socket is available
 
+    .. versionadded:: v2.5.0
+
+    :param auto_reconnect: Activates the auto-reconnect functionality.
+        PySolarmanV5 will try to keep the connection open. The default is False.
+        Not compatible with custom sockets.
+    :type auto_reconnect: Boolean, optional
+
     .. deprecated:: v2.4.0
 
     :param verbose: Enable verbose logging, defaults to False. Use **logger**
         instead. For compatibility purposes, **verbose**, if enabled, will
         create a logger, and set the logging level to DEBUG.
     :type verbose: bool, optional
 
@@ -79,30 +92,37 @@
         self.serial = serial
 
         self.port = kwargs.get("port", 8899)
         self.mb_slave_id = kwargs.get("mb_slave_id", 1)
         self.verbose = kwargs.get("verbose", False)
         self.socket_timeout = kwargs.get("socket_timeout", 60)
         self.v5_error_correction = kwargs.get("error_correction", False)
+        self.sequence_number = None
 
         if self.verbose:
             self.log.setLevel("DEBUG")
 
         self._v5_frame_def()
 
-        self.sock = kwargs.get("socket", self._create_socket())
-        if self.sock is None:
-            raise NoSocketAvailableError("No socket available")
+        self.sock: socket.socket = None  # noqa
+        self._poll: select.poll = None  # noqa
+        self._sock_fd: int = None  # noqa
+        self._auto_reconnect = False
+        self._data_queue: Queue = None  # noqa
+        self._data_wanted: Event = None  # noqa
+        self._reader_exit: Event = None  # noqa
+        self._reader_thr: Thread = None  # noqa
+        self._socket_setup(kwargs.get("socket"), kwargs.get("auto_reconnect", False))
 
     def _v5_frame_def(self):
         """Define and construct V5 request frame structure."""
         self.v5_start = bytes.fromhex("A5")
         self.v5_length = bytes.fromhex("0000")  # placeholder value
         self.v5_controlcode = struct.pack("<H", 0x4510)
-        self.v5_serial = bytes.fromhex("0000")
+        self.v5_serial = bytes.fromhex("0000")  # placeholder value
         self.v5_loggerserial = struct.pack("<I", self.serial)
         self.v5_frametype = bytes.fromhex("02")
         self.v5_sensortype = bytes.fromhex("0000")
         self.v5_deliverytime = bytes.fromhex("00000000")
         self.v5_powerontime = bytes.fromhex("00000000")
         self.v5_offsettime = bytes.fromhex("00000000")
         self.v5_checksum = bytes.fromhex("00")  # placeholder value
@@ -117,27 +137,43 @@
         :return: Checksum value of V5 frame
         :rtype: int
 
         """
         checksum = 0
         for i in range(1, len(frame) - 2, 1):
             checksum += frame[i] & 0xFF
-        return int((checksum & 0xFF))
+        return int(checksum & 0xFF)
+
+    def _get_next_sequence_number(self):
+        """Get the next sequence number for use in outgoing packets
+
+        If ``sequence_number`` is None, generate a random int as initial value.
+
+        :return: Sequence number
+        :rtype: int
+
+        """
+        if self.sequence_number is None:
+            self.sequence_number = randrange(0x01, 0xFF)
+        else:
+            self.sequence_number = (self.sequence_number + 1) & 0xFF
+        return self.sequence_number
 
     def _v5_frame_encoder(self, modbus_frame):
         """Take a modbus RTU frame and encode it in a V5 data logging stick frame
 
         :param modbus_frame: Modbus RTU frame
         :type modbus_frame: bytes
         :return: V5 frame
         :rtype: bytearray
 
         """
 
         self.v5_length = struct.pack("<H", 15 + len(modbus_frame))
+        self.v5_serial = struct.pack("<H", self._get_next_sequence_number())
 
         v5_header = bytearray(
             self.v5_start
             + self.v5_length
             + self.v5_controlcode
             + self.v5_serial
             + self.v5_loggerserial
@@ -169,19 +205,20 @@
         or be appended to valid ``0x1510`` responses. In this case, the v5_frame
         will contain an invalid checksum.
 
         Validate the following:
 
         1) V5 start and end are correct (``0xA5`` and ``0x15`` respectively)
         2) V5 checksum is correct
-        3) V5 data logger serial number is correct (in most (all?) instances the
+        3) V5 outgoing sequence number has been echoed back to us (byte 5)
+        4) V5 data logger serial number is correct (in most (all?) instances the
            reply is correct, but request can obviously be incorrect)
-        4) V5 control code is correct (``0x1510``)
-        5) v5_frametype contains the correct value (``0x02`` in byte 11)
-        6) Modbus RTU frame length is at least 5 bytes (vast majority of RTU
+        5) V5 control code is correct (``0x1510``)
+        6) v5_frametype contains the correct value (``0x02`` in byte 11)
+        7) Modbus RTU frame length is at least 5 bytes (vast majority of RTU
            frames will be >=6 bytes, but valid 5 byte error/exception RTU frames
            are possible)
 
         :param v5_frame: V5 frame
         :type v5_frame: bytes
         :return: Modbus RTU Frame
         :rtype: bytes
@@ -200,14 +237,16 @@
 
         if (v5_frame[0] != int.from_bytes(self.v5_start, byteorder="big")) or (
             v5_frame[frame_len - 1] != int.from_bytes(self.v5_end, byteorder="big")
         ):
             raise V5FrameError("V5 frame contains invalid start or end values")
         if v5_frame[frame_len - 2] != self._calculate_v5_frame_checksum(v5_frame):
             raise V5FrameError("V5 frame contains invalid V5 checksum")
+        if v5_frame[5] != self.sequence_number:
+            raise V5FrameError("V5 frame contains invalid sequence number")
         if v5_frame[7:11] != self.v5_loggerserial:
             raise V5FrameError("V5 frame contains incorrect data logger serial number")
         if v5_frame[3:5] != struct.pack("<H", 0x1510):
             raise V5FrameError("V5 frame contains incorrect control code")
         if v5_frame[11] != int("02", 16):
             raise V5FrameError("V5 frame contains invalid frametype")
 
@@ -224,21 +263,102 @@
         :param data_logging_stick_frame: V5 frame to transmit
         :type data_logging_stick_frame: bytes
         :return: V5 frame received
         :rtype: bytes
 
         """
         self.log.debug("SENT: " + data_logging_stick_frame.hex(" "))
-
+        if not self._reader_thr.is_alive():
+            raise NoSocketAvailableError("Connection already closed.")
         self.sock.sendall(data_logging_stick_frame)
-        v5_response = self.sock.recv(1024)
+        self._data_wanted.set()
+        try:
+            v5_response = self._data_queue.get(timeout=self.socket_timeout)
+            if v5_response == b"":
+                raise NoSocketAvailableError("Connection closed on read")
+            self._data_wanted.clear()
+        except TimeoutError:
+            raise
 
         self.log.debug("RECD: " + v5_response.hex(" "))
         return v5_response
 
+    def _data_receiver(self):
+        self._poll.register(self.sock.fileno(), select.POLLIN)
+        while True:
+            events = self._poll.poll(500)
+            if self._reader_exit.is_set():
+                return
+            for event in events:
+                # We are registered only for inbound data on a single socket,
+                # so there is no need to check the (fileno, mask) tuples
+                data = self.sock.recv(1024)
+                if data == b"":
+                    self.log.debug(f"[POLL] Socket closed. Reader thread exiting.")
+                    if self._data_wanted.is_set():
+                        try:
+                            self._data_queue.put_nowait(data)
+                        except queue.Full:
+                            pass
+                    self._reconnect()
+                    return
+                elif data.startswith(b"\xa5\x01\x00\x10G"):
+                    # Frame with control code 0x4710 - Counter frame
+                    self.log.debug(f'[{self.serial}] COUNTER: {data.hex(" ")}')
+                    continue
+                if self._data_wanted.is_set():
+                    self._data_queue.put(data, timeout=self.socket_timeout)
+                else:
+                    self.log.debug("[POLL-DISCARDED] RECD: " + data.hex(" "))
+
+    def _reconnect(self):
+        """
+        Reconnect to the data logger if needed
+        """
+        if self._reader_thr.is_alive():
+            try:
+                self.sock.send(b"")
+                self.sock.close()
+            except OSError:
+                pass
+            self._reader_exit.set()
+        if self._auto_reconnect:
+            self.log.debug(
+                f"Auto-Reconnect enabled. Trying to establish a new connection"
+            )
+            self._poll.unregister(self._sock_fd)
+            self.sock = self._create_socket()
+            if self.sock:
+                self._sock_fd = self.sock.fileno()
+                self._reader_exit.clear()
+                self._reader_thr = Thread(target=self._data_receiver, daemon=True)
+                self._reader_thr.start()
+                self.log.debug(f"Auto-Reconnect successful.")
+            else:
+                self.log.debug(f"No socket available! Reconnect failed.")
+        else:
+            self.log.debug("Auto-Reconnect inactive.")
+
+    def disconnect(self) -> None:
+        """
+        Disconnect the socket and set a signal for the reader thread to exit
+
+        :return: None
+
+        """
+        self._data_wanted.clear()
+        try:
+            self.sock.send(b"")
+            self.sock.close()
+        except OSError:
+            pass
+        self._reader_exit.set()
+        self._reader_thr.join(0.5)
+        self._poll.unregister(self._sock_fd)
+
     def _send_receive_modbus_frame(self, mb_request_frame):
         """Encodes mb_frame, sends/receives v5_frame, decodes response
 
         :param mb_request_frame: Modbus RTU frame to transmit
         :type mb_request_frame: bytes
         :return: Modbus RTU frame received
         :rtype: bytes
@@ -268,14 +388,30 @@
             sock = socket.create_connection(
                 (self.address, self.port), self.socket_timeout
             )
         except OSError:
             return None
         return sock
 
+    def _socket_setup(self, sock: Any, auto_reconnect: bool):
+        """Socket setup method"""
+        if isinstance(sock, socket.socket) or sock is None:
+            self.sock = sock if sock else self._create_socket()
+            if self.sock is None:
+                raise NoSocketAvailableError("No socket available")
+            self._poll = select.poll()
+            self._sock_fd = self.sock.fileno()
+            self._auto_reconnect = False if sock else auto_reconnect
+            self._data_queue = Queue(maxsize=1)
+            self._data_wanted = Event()
+            self._reader_exit = Event()
+            self._reader_thr = Thread(target=self._data_receiver, daemon=True)
+            self._reader_thr.start()
+            self.log.debug(f"Socket setup completed... {self.sock}")
+
     @staticmethod
     def twos_complement(val, num_bits):
         """Calculate 2s Complement
 
         :param val: Value to calculate
         :type val: int
         :param num_bits: Number of bits
```

### Comparing `pysolarmanv5-2.4.0/pysolarmanv5.egg-info/PKG-INFO` & `pysolarmanv5-2.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: pysolarmanv5
-Version: 2.4.0
+Version: 2.5.0
 Summary: A Python library for interacting with Solarman (IGEN-Tech) v5 based Solar Data Loggers
-Home-page: https://github.com/jmccrohan/pysolarmanv5
-Author: Jonathan McCrohan
-Author-email: jmccrohan@gmail.com
-License: BSD
-Keywords: solarman igen-tech modbus solar inverter solarmanv5
+Author-email: Jonathan McCrohan <jmccrohan@gmail.com>
+License: MIT License
+Project-URL: homepage, https://github.com/jmccrohan/pysolarmanv5
+Project-URL: repository, https://github.com/jmccrohan/pysolarmanv5
+Project-URL: documentation, https://pysolarmanv5.readthedocs.io/
+Project-URL: changelog, https://pysolarmanv5.readthedocs.io/en/latest/changelog.html
+Keywords: solarman,igen-tech,modbus,solar,inverter,solarmanv5
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pysolarmanv5
 
 This is a Python module to interact with Solarman (IGEN-Tech) v5 based solar
 inverter data loggers. Modbus RTU frames can be encapsulated in the proprietary
 Solarman v5 protocol and requests sent to the data logger on port tcp/8899.
 
-This module aims to simplify the Solarman v5 protocol, exposing interfaces
-similar to that of the [uModbus](https://pysolarmanv5.readthedocs.io/) library.
+This module aims to simplify the Solarman v5 protocol, exposing both sync and
+async interfaces similar to that of the [uModbus](https://pysolarmanv5.readthedocs.io/)
+library.
 
 Details of the Solarman v5 protocol have been based on the excellent work of
 [Inverter-Data-Logger by XtheOne](https://github.com/XtheOne/Inverter-Data-Logger/)
 and others.
 
 ## Documentation
 
@@ -33,17 +37,23 @@
 
 The Solarman V5 protocol is documented [here](https://pysolarmanv5.readthedocs.io/en/latest/solarmanv5_protocol.html).
 
 ## Supported Devices
 
 A user contributed list of supported devices is available [here](https://github.com/jmccrohan/pysolarmanv5/issues/11).
 
+If you are unsure if your device is supported, please use the [solarman_scan](https://github.com/jmccrohan/pysolarmanv5/blob/main/utils/solarman_scan.py) 
+utility to find compatible data logging sticks on your local network.
+
 Please note that the **Solis S3-WIFI-ST** data logging stick is **NOT supported**.  
 See [GH issue #8](https://github.com/jmccrohan/pysolarmanv5/issues/8) for further information. 
 
+Some Ethernet data logging sticks have native support Modbus TCP and therefore **do not require pysolarmanv5**.
+See [GH issue #5](https://github.com/jmccrohan/pysolarmanv5/issues/5) for further information. 
+
 ## Dependencies
 
 - pysolarmanv5 requires Python 3.8 or greater.
 - pysolarmanv5 depends on [uModbus](https://github.com/AdvancedClimateSystems/uModbus).
 
 ## Installation
 
@@ -51,14 +61,30 @@
 
 `pip install pysolarmanv5`
 
 To install the latest development version from git, run:
 
 `pip install git+https://github.com/jmccrohan/pysolarmanv5.git`
 
+## Projects using pysolarmanv5
+
+- [NosIreland/solismon3](https://github.com/NosIreland/solismon3)
+- [NosIreland/solismod](https://github.com/NosIreland/solismod)
+- [jmccrohan/ha_pyscript_pysolarmanv5](https://github.com/jmccrohan/ha_pyscript_pysolarmanv5)
+- [YodaDaCoda/hass-solarman-modbus](https://github.com/YodaDaCoda/hass-solarman-modbus)
+- [schwatter/solarman_mqtt](https://github.com/schwatter/solarman_mqtt)
+- [RonnyKempe/solismon](https://github.com/RonnyKempe/solismon)
+- [toledobastos/solarman_battery_autocharge](https://github.com/toledobastos/solarman_battery_autocharge)
+- [AndyTaylorTweet/solis2mqtt](https://github.com/AndyTaylorTweet/solis2mqtt)
+- [pixellos/codereinvented.automation.py](https://github.com/pixellos/codereinvented.automation.py)
+- [cjgwhite/hass-solar](https://github.com/cjgwhite/hass-solar)
+- [imcfarla2003/solarconfig](https://github.com/imcfarla2003/solarconfig)
+- [githubDante/deye-controller](https://github.com/githubDante/deye-controller)
+- [danfoster/solis](https://github.com/danfoster/solis)
+
 ## Contributions
 
 Contributions welcome. Please raise any Issues / Pull Requests via [Github](https://github.com/jmccrohan/pysolarmanv5).
 
 ## License
 
-pysolarmanv5 is licensed under the [MIT License](https://github.com/jmccrohan/pysolarmanv5/blob/master/LICENSE). Copyright (c) 2022 Jonathan McCrohan
+pysolarmanv5 is licensed under the [MIT License](https://github.com/jmccrohan/pysolarmanv5/blob/master/LICENSE). Copyright (c) 2023 Jonathan McCrohan
```

