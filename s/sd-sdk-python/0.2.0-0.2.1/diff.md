# Comparing `tmp/sd_sdk_python-0.2.0.tar.gz` & `tmp/sd_sdk_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_sdk_python-0.2.0.tar", max compression
+gzip compressed data, was "sd_sdk_python-0.2.1.tar", max compression
```

## Comparing `sd_sdk_python-0.2.0.tar` & `sd_sdk_python-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-05-04 19:40:43.161475 sd_sdk_python-0.2.0/LICENSE
--rw-r--r--   0        0        0      636 2023-05-04 19:40:43.161475 sd_sdk_python-0.2.0/README.md
--rw-r--r--   0        0        0      500 2023-05-04 19:40:43.161475 sd_sdk_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2783 2023-05-04 19:40:43.161475 sd_sdk_python-0.2.0/sd_sdk_python/__init__.py
--rw-r--r--   0        0        0    12285 2023-05-04 19:40:43.165475 sd_sdk_python-0.2.0/sd_sdk_python/sd_sdk.py
--rw-r--r--   0        0        0    13130 2023-05-04 19:40:43.165475 sd_sdk_python-0.2.0/sd_sdk_python/sd_sdk_wireless.py
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/README.md
+-rw-r--r--   0        0        0     1080 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2783 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/__init__.py
+-rw-r--r--   0        0        0    12488 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk.py
+-rw-r--r--   0        0        0    13130 2023-05-10 20:55:33.005424 sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk_wireless.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 sd_sdk_python-0.2.1/PKG-INFO
```

### Comparing `sd_sdk_python-0.2.0/LICENSE` & `sd_sdk_python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.0/README.md` & `sd_sdk_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.0/sd_sdk_python/__init__.py` & `sd_sdk_python-0.2.1/sd_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.0/sd_sdk_python/sd_sdk.py` & `sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,19 @@
 @dataclass
 class Ezairo:
     sd: object
     interface: object
     device_info: object
     product: object
 
+    def __post_init__(self):
+        if type(self.device_info) == self.sd.DeviceInfo:
+            # Convert to richer dataclass automatically
+            self.device_info = DeviceInfo(self.device_info)
+
     def load_param_file(self, param_file, configure_device=False, write_manufacturer_data=False, write_voice_alerts=False):
         if self.product is not None:
             self.product.LoadParamFile(str(param_file), configure_device, write_manufacturer_data, write_voice_alerts)
 
     def reset(self,):
         if self.product is not None:
             self.product.ResetDevice()
```

### Comparing `sd_sdk_python-0.2.0/sd_sdk_python/sd_sdk_wireless.py` & `sd_sdk_python-0.2.1/sd_sdk_python/sd_sdk_wireless.py`

 * *Files identical despite different names*

### Comparing `sd_sdk_python-0.2.0/PKG-INFO` & `sd_sdk_python-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 Metadata-Version: 2.1
 Name: sd-sdk-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python helper module for the Sound Designer SDK
+Home-page: https://github.com/markmelvin-onsemi/sd-sdk-python
+License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@onsemi.com
 Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 
 # sd-sdk-python
 This module is a Python helper module for the Sound Designer SDK
 
 This Python module depends on a copy of the Sound Designer SDK being accessible on your computer. Make sure you have unzipped the Sound Designer SDK somewhere and then set the environment variable `SD_SDK_ROOT` to the root folder of the unzipped SDK, or to the path containing the Windows binaries (.dlls), Python module (`sd.pyd`), and `sd.config` file.
```

