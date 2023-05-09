# Comparing `tmp/pyrtma-1.2.2.tar.gz` & `tmp/pyrtma-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtma-1.2.2.tar", last modified: Tue Feb 21 18:14:50 2023, max compression
+gzip compressed data, was "pyrtma-1.2.3.tar", last modified: Tue May  9 22:43:56 2023, max compression
```

## Comparing `pyrtma-1.2.2.tar` & `pyrtma-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:14:50.337706 pyrtma-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-21 18:14:41.000000 pyrtma-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-02-21 18:14:50.337706 pyrtma-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-02-21 18:14:41.000000 pyrtma-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-21 18:14:41.000000 pyrtma-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 18:14:50.337706 pyrtma-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:14:50.333706 pyrtma-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:14:50.337706 pyrtma-1.2.2/src/pyrtma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-02-21 18:14:41.000000 pyrtma-1.2.2/src/pyrtma/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:14:50.337706 pyrtma-1.2.2/src/pyrtma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-02-21 18:14:50.000000 pyrtma-1.2.2/src/pyrtma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-21 18:14:50.000000 pyrtma-1.2.2/src/pyrtma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 18:14:50.000000 pyrtma-1.2.2/src/pyrtma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 18:14:50.000000 pyrtma-1.2.2/src/pyrtma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 18:14:50.337706 pyrtma-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-21 18:14:41.000000 pyrtma-1.2.2/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-02-21 18:14:41.000000 pyrtma-1.2.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-21 18:14:41.000000 pyrtma-1.2.2/tests/test_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:43:56.728638 pyrtma-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-09 22:43:47.000000 pyrtma-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-09 22:43:56.728638 pyrtma-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-09 22:43:47.000000 pyrtma-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-09 22:43:47.000000 pyrtma-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:43:56.728638 pyrtma-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:43:56.724638 pyrtma-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:43:56.724638 pyrtma-1.2.3/src/pyrtma/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-05-09 22:43:47.000000 pyrtma-1.2.3/src/pyrtma/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:43:56.724638 pyrtma-1.2.3/src/pyrtma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-09 22:43:56.000000 pyrtma-1.2.3/src/pyrtma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 22:43:56.000000 pyrtma-1.2.3/src/pyrtma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:43:56.000000 pyrtma-1.2.3/src/pyrtma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 22:43:56.000000 pyrtma-1.2.3/src/pyrtma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:43:56.724638 pyrtma-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-09 22:43:47.000000 pyrtma-1.2.3/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-09 22:43:47.000000 pyrtma-1.2.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-09 22:43:47.000000 pyrtma-1.2.3/tests/test_message.py
```

### Comparing `pyrtma-1.2.2/LICENSE` & `pyrtma-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtma-1.2.2/PKG-INFO` & `pyrtma-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-1.2.2/README.md` & `pyrtma-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrtma-1.2.2/pyproject.toml` & `pyrtma-1.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrtma"
-version = "1.2.2"
+# version defined in pyrtma.__version__.py
 authors = [
   { name="David Weir", email="dmw109@pitt.edu" },
   { name="Jeff Weiss", email="jmw182@pitt.edu" },
   { name="Tyler Madonna", email="tjm159@pitt.edu" },
   { name="Tyler Simpson", email="tws21@pitt.edu" },
 ]
 description = "A Python client for RTMA/Dragonfly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "pyrtma.__version__"}
 
 [project.urls]
 "Homepage" = "https://github.com/pitt-rnel/pyrtma"
 "Bug Tracker" = "https://github.com/pitt-rnel/pyrtma/issues"
```

### Comparing `pyrtma-1.2.2/src/pyrtma/_core.py` & `pyrtma-1.2.3/src/pyrtma/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""pyrtma._core
+
+Core RTMA message definitions and functions"""
 import ctypes
 import json
 
 from dataclasses import dataclass
 from collections import ChainMap
 from typing import Type, ClassVar, Optional, Any, Dict, ChainMap
```

### Comparing `pyrtma-1.2.2/src/pyrtma/client.py` & `pyrtma-1.2.3/src/pyrtma/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""pyrtma.client module
+
+Includes :py:class:`~Client` class and associated exception classes
+"""
 import socket
 import select
 import time
 import os
 import ctypes
 
 from ._core import *
@@ -61,25 +65,37 @@
 class InvalidDestinationHost(ClientError):
     """Raised when client tries to send to an invalid host."""
 
     pass
 
 
 def requires_connection(func):
+    """Decorator wrapper for Client methods that require a connection"""
+
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if not self.connected:
             raise NotConnectedError
         else:
             return func(self, *args, **kwargs)
 
     return wrapper
 
 
 class Client(object):
+    """RTMA Client interface
+
+    Args:
+        module_id (optional): Static module ID, which must be unique.
+            Defaults to 0, which generates a dynamic module ID.
+        host_id (optional): Host ID. Defaults to 0.
+        timecode (optional): Add additional timecode fields to message
+            header, used by some projects at RNEL. Defaults to False.
+    """
+
     def __init__(
         self,
         module_id: int = 0,
         host_id: int = 0,
         timecode: bool = False,
     ):
         self._module_id = module_id
@@ -91,23 +107,36 @@
         self._recv_buffer = bytearray(1024**2)
 
     def __del__(self):
         if self._connected:
             try:
                 self.disconnect()
             except ClientError:
-                """Siliently ignore any errors at this point."""
+                """Silently ignore any errors at this point."""
                 pass
 
     def connect(
         self,
         server_name: str = "localhost:7111",
         logger_status: bool = False,
         daemon_status: bool = False,
     ):
+        """Connect to message manager server
+
+        Args:
+            server_name (optional): IP_addr:port_num string associated with message manager.
+                Defaults to "localhost:7111".
+            logger_status (optional): Flag to declare client as a logger module.
+                Logger modules are automatically subscribed to all message types.
+                Defaults to False.
+            daemon_status (optional): Flag to declare client as a daemon. Defaults to False.
+
+        Raises:
+            MessageManagerNotFound: Unable to connect to message manager
+        """
         addr, port = server_name.split(":")
         self._server = (addr, int(port))
 
         # Create the tcp socket
         self._sock = socket.socket(
             family=socket.AF_INET, type=socket.SOCK_STREAM, proto=socket.IPPROTO_TCP
         )
@@ -135,54 +164,66 @@
         ack_msg = self.wait_for_acknowledgement()
 
         # save own module ID from ACK if asked to be assigned dynamic ID
         if self._module_id == 0:
             self._module_id = ack_msg.header.dest_mod_id
 
     def disconnect(self):
+        """Disconnect from message manager server"""
         try:
             if self._connected:
                 self.send_signal(MT_DISCONNECT)
                 ack_msg = self.wait_for_acknowledgement(timeout=0.5)
         except AcknowledgementTimeout:
             pass
         finally:
             self._sock.close()
             self._connected = False
 
     @property
     def server(self) -> Tuple[str, int]:
+        """Message manager server address as a (IP_addr, port_num) tuple"""
         return self._server
 
     @property
     def ip_addr(self) -> str:
+        """Message manager IP address string"""
         return self._server[0]
 
     @property
     def port(self) -> int:
+        """Message manager port number"""
         return self._server[1]
 
     @property
     def connected(self) -> bool:
+        """Status of connection to message manager server"""
         return self._connected
 
     @property
     def msg_count(self) -> int:
+        """Count of messages that have been sent"""
         return self._msg_count
 
     @property
     def module_id(self) -> int:
+        """Numeric module ID of client"""
         return self._module_id
 
     @property
     def header_cls(self) -> Type[MessageHeader]:
+        """Class defining the RTMA message header"""
         return self._header_cls
 
     @requires_connection
     def send_module_ready(self):
+        """Send a signal to message manager that client is ready
+
+        This method also sends the client's process ID to message manager.
+        """
         msg = MODULE_READY()
         msg.pid = os.getpid()
         self.send_message(msg)
 
     def _subscription_control(self, msg_list: List[int], ctrl_msg: str):
         if not isinstance(msg_list, list):
             msg_list = [msg_list]
@@ -200,36 +241,76 @@
 
         for msg_type in msg_list:
             msg.msg_type = msg_type
             self.send_message(msg)
 
     @requires_connection
     def subscribe(self, msg_list: List[int]):
+        """Subscribe to message types
+
+        Calling this method multiple times will add to, and not replace,
+        the list of subscribed messages.
+
+        Args:
+            msg_list: A list of numeric message IDs to subscribe to
+        """
         self._subscription_control(msg_list, "Subscribe")
 
     @requires_connection
     def unsubscribe(self, msg_list: List[int]):
+        """Unsubscribe from message types
+
+        Args:
+            msg_list: A list of numeric message IDs to unsubscribe to
+        """
         self._subscription_control(msg_list, "Unsubscribe")
 
     @requires_connection
     def pause_subscription(self, msg_list: List[int]):
+        """Pause subscription to message types
+
+        Args:
+            msg_list (List[int]): A list of numeric message IDs to temporarily unsubscribe to
+        """
         self._subscription_control(msg_list, "PauseSubscription")
 
     @requires_connection
     def resume_subscription(self, msg_list: List[int]):
+        """Resume subscription to message types
+
+        Args:
+            msg_list (List[int]): A list of paused message IDs to resubscribe to
+        """
         self._subscription_control(msg_list, "ResumeSubscription")
 
     @requires_connection
     def send_signal(
         self,
         signal_type: int,
         dest_mod_id: int = 0,
         dest_host_id: int = 0,
         timeout: float = -1,
     ):
+        """Send a signal
+
+        A signal is a message type without an associated data payload.
+        Only a unique message type ID is required to send a signal.
+        To send a message with data, see :py:func:`send_message`.
+
+        Args:
+            signal_type: Numeric message type ID of signal
+            dest_mod_id (optional): Specific module ID to send to. Defaults to 0 (broadcast).
+            dest_host_id (optional): Specific host ID to send to. Defaults to 0 (broadcast).
+            timeout (optional): Timeout in seconds to wait for socket to be available for sending.
+                Defaults to -1 (blocking).
+
+        Raises:
+            InvalidDestinationModule: Specified destination module is invalid
+            InvalidDestinationHost: Specified destination host is invalid
+        """
         # Verify that the module & host ids are valid
         if dest_mod_id < 0 or dest_mod_id > MAX_MODULES:
             raise InvalidDestinationModule(f"Invalid dest_mod_id  of [{dest_mod_id}]")
 
         if dest_host_id < 0 or dest_host_id > MAX_HOSTS:
             raise InvalidDestinationHost(f"Invalid dest_host_id of [{dest_host_id}]")
 
@@ -265,14 +346,30 @@
     def send_message(
         self,
         msg_data: MessageData,
         dest_mod_id: int = 0,
         dest_host_id: int = 0,
         timeout: float = -1,
     ):
+        """Send a message
+
+        A message is a packet that contains a defined data payload.
+        To send a message without associated data, see :py:func:`send_signal`.
+
+        Args:
+            msg_data: Object containing the message to send
+            dest_mod_id (optional): Specific module ID to send to. Defaults to 0 (broadcast).
+            dest_host_id (optional): Specific host ID to send to. Defaults to 0 (broadcast).
+            timeout (optional): Timeout in seconds to wait for socket to be available for sending.
+                Defaults to -1 (blocking).
+
+        Raises:
+            InvalidDestinationModule: Specified destination module is invalid
+            InvalidDestinationHost: Specified destination host is invalid
+        """
         # Verify that the module & host ids are valid
         if dest_mod_id < 0 or dest_mod_id > MAX_MODULES:
             raise InvalidDestinationModule(f"Invalid dest_mod_id of [{dest_mod_id}]")
 
         if dest_host_id < 0 or dest_host_id > MAX_HOSTS:
             raise InvalidDestinationHost(f"Invalid dest_host_id of [{dest_host_id}]")
 
@@ -313,14 +410,27 @@
             self._connected = False
             raise ConnectionLost from e
 
     @requires_connection
     def read_message(
         self, timeout: Union[int, float] = -1, ack=False
     ) -> Optional[Message]:
+        """Read a message
+
+        Args:
+            timeout (optional): Timeout to wait for a message to be available for reading.
+                Defaults to -1 (blocking).
+            ack (optional): Reserved for future use. Defaults to False.
+
+        Raises:
+            ConnectionLost: Connection error to message manager server
+
+        Returns:
+            Message object. If no message is read before timeout, returns None.
+        """
         if timeout >= 0:
             readfds, writefds, exceptfds = select.select([self._sock], [], [], timeout)
         else:
             readfds, writefds, exceptfds = select.select(
                 [self._sock], [], []
             )  # blocking
 
@@ -358,15 +468,30 @@
                     self._connected = False
                     raise ConnectionLost
             except ConnectionError:
                 raise ConnectionLost
 
         return Message(header, data)
 
-    def wait_for_acknowledgement(self, timeout: float = 3):
+    def wait_for_acknowledgement(self, timeout: float = 3) -> Message:
+        """Wait for acknowledgement from message manager module
+
+        Used internally when acknowledgement replies from message manager are expected
+
+        TODO rename to _wait_for_acknowledgement()?
+
+        Args:
+            timeout (optional): Timeout in seconds to wait for ack message. Defaults to 3.
+
+        Raises:
+            AcknowledgementTimeout: Ack not received from message manager
+
+        Returns:
+            Ack message
+        """
         ret = 0
 
         # Wait Forever
         if timeout == -1:
             while True:
                 msg = self.read_message(ack=True)
                 if msg is not None:
@@ -388,14 +513,24 @@
                 time_remaining = timeout - time_waited
 
             raise AcknowledgementTimeout(
                 "Failed to receive Acknowlegement from MessageManager"
             )
 
     def discard_messages(self, timeout: float = 1) -> bool:
+        """Read and discard messages in socket buffer up to timeout
+
+        Args:
+            timeout (optional): Maximum time in seconds to loop through message buffer.
+                Defaults to 1.
+
+        Returns:
+            True if all messages have been read, False if messages remain in buffer
+        """
+
         """Read and discard messages in socket buffer up to timeout.
         Returns: True if all messages available have been read.
         """
         msg = 1
         time_remaining = timeout
         start_time = time.perf_counter()
         while msg is not None and time_remaining > 0:
```

### Comparing `pyrtma-1.2.2/src/pyrtma/compile.py` & `pyrtma-1.2.3/src/pyrtma/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""pyrtma.compile Message Type Compiler
+"""
+
 from io import TextIOWrapper
 import re
 from typing import List, Dict, Optional
 
 from ._core import ctypes_map
 
 
@@ -211,15 +214,14 @@
     assert name.startswith("MDF_")
     basename = name[4:]
     msg_id = "MT_" + basename
     template = f"""
 # Signal Definition
 @pyrtma.msg_def
 class {name}(pyrtma.MessageData):
-    _pack_ = True
     _fields_ = []
     type_id = {msg_id}
     type_name = \"{basename}\"
 
 """
     return template
```

### Comparing `pyrtma-1.2.2/src/pyrtma/constants.py` & `pyrtma-1.2.3/src/pyrtma/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""pyrtma.constants module
+
+Includes core message type IDs and other constants
+"""
+
 import ctypes
 
 MAX_MODULES = 200
 DYN_MOD_ID_START = 100
 MAX_HOSTS = 5
 MAX_MESSAGE_TYPES = 10000
 MIN_STREAM_TYPE = 9000
```

### Comparing `pyrtma-1.2.2/src/pyrtma/manager.py` & `pyrtma-1.2.3/src/pyrtma/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""pyrtma.manager module
+
+Contains :py:class:`~MessageManager` class
+"""
+
 import socket
 import select
 import argparse
 import logging
 import time
 import random
 import ctypes
@@ -13,14 +18,19 @@
 from typing import Dict, List, Tuple, Set, Type, Union, Optional
 from dataclasses import dataclass
 from collections import defaultdict, Counter
 
 
 @dataclass
 class Module:
+    """Module dataclass
+
+    Used internally by MessageManager to manage connections to each client module.
+    """
+
     conn: socket.socket
     address: Tuple[str, int]
     header_cls: Type[MessageHeader]
     id: int = 0
     pid: int = 0
     connected: bool = False
     is_logger: bool = False
@@ -47,14 +57,19 @@
         return f"Module ID: {self.id} @ {self.address[0]}:{self.address[1]}"
 
     def __hash__(self):
         return self.conn.__hash__()
 
 
 class MessageManager:
+    """MessageManager class
+
+    RTMA Message Manager server implemented in python.
+    """
+
     _keep_running = True
 
     def __init__(
         self,
         ip_address: Union[str, int] = socket.INADDR_ANY,
         port: int = 7111,
         timecode=False,
@@ -260,18 +275,25 @@
     def forward_message(
         self,
         header: MessageHeader,
         data: Union[bytes, MessageData],
         wlist: List[socket.socket],
     ):
         """Forward a message from other modules
+
         The given message will be forwarded to:
+
             - all subscribed logger modules (ALWAYS)
             - if the message has a destination address, and it is subscribed to by that destination it will be forwarded only there
             - if the message has no destination address, it will be forwarded to all subscribed modules
+
+        Args:
+            header: Message Header
+            data: Message Data
+            wlist: sockets ready for writing
         """
 
         dest_mod_id = header.dest_mod_id
         dest_host_id = header.dest_host_id
 
         # Verify that the module & host ids are valid
         if dest_mod_id < 0 or dest_mod_id > MAX_MODULES:
@@ -458,14 +480,15 @@
             self.send_timing_message(wlist)
             self.t_last_message_count = time.time()
 
     def close(self):
         self._keep_running = False
 
     def run(self):
+        """Start the message manager server"""
         try:
             while self._keep_running:
                 rlist, _, _ = select.select(
                     self.modules.keys(), [], [], self.read_timeout
                 )
 
                 # Check for an incoming connection request
```

### Comparing `pyrtma-1.2.2/src/pyrtma.egg-info/PKG-INFO` & `pyrtma-1.2.3/src/pyrtma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-1.2.2/tests/test_encoding.py` & `pyrtma-1.2.3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `pyrtma-1.2.2/tests/test_integration.py` & `pyrtma-1.2.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyrtma-1.2.2/tests/test_message.py` & `pyrtma-1.2.3/tests/test_message.py`

 * *Files identical despite different names*

