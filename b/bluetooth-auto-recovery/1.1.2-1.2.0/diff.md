# Comparing `tmp/bluetooth_auto_recovery-1.1.2.tar.gz` & `tmp/bluetooth_auto_recovery-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.1.2.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.2.0.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.1.2.tar` & `bluetooth_auto_recovery-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/LICENSE
--rw-r--r--   0        0        0     3840 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/README.md
--rw-r--r--   0        0        0     2490 2023-05-04 12:36:06.029043 bluetooth_auto_recovery-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-04 12:36:05.973041 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:36:05.129024 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    22119 2023-05-04 12:36:05.133024 bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3840 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/README.md
+-rw-r--r--   0        0        0     2490 2023-05-10 13:17:24.884225 bluetooth_auto_recovery-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-10 13:17:24.840223 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    22347 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.2.0/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.1.2/LICENSE` & `bluetooth_auto_recovery-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.1.2/README.md` & `bluetooth_auto_recovery-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.1.2/pyproject.toml` & `bluetooth_auto_recovery-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.1.2"
+version = "1.2.0"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_auto_recovery-1.1.2/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/recover.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,18 +538,23 @@
             adapter.timeout,
         )
         timed_out_getting_powered = True
 
     # Do not attempt to power off if it timed out getting the power state
     # as it likely means the adapter interface is frozen and will not respond to
     # power off commands so we need to proceed to bounce the interface
-    if not timed_out_getting_powered and not await _execute_power_off(
-        adapter, name, power_state_before_reset
-    ):
-        return False
+    if not timed_out_getting_powered:
+        try:
+            await _execute_power_off(adapter, name, power_state_before_reset)
+        except asyncio.TimeoutError:
+            _LOGGER.warning(
+                "Could not reset the power state of the Bluetooth adapter %s due to timeout after %s seconds",
+                name,
+                adapter.timeout,
+            )
 
     try:
         await _bounce_adapter_interface(adapter)
     except Exception as ex:  # pylint: disable=broad-except
         _LOGGER.warning("Could not cycle the Bluetooth adapter %s: %s", name, ex)
 
     return await _execute_power_on(adapter, name, power_state_before_reset)
```

### Comparing `bluetooth_auto_recovery-1.1.2/PKG-INFO` & `bluetooth_auto_recovery-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-auto-recovery
-Version: 1.1.2
+Version: 1.2.0
 Summary: Recover bluetooth adapters that are in an stuck state
 Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.1.2 Summary:
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.2.0 Summary:
 Recover bluetooth adapters that are in an stuck state Home-page: https://
 github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

