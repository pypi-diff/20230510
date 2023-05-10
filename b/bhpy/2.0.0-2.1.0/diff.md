# Comparing `tmp/bhpy-2.0.0.tar.gz` & `tmp/bhpy-2.1.0.tar.gz`

## Comparing `bhpy-2.0.0.tar` & `bhpy-2.1.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bhpy-2.0.0/setup.cfg
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 bhpy-2.0.0/setup.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bhpy-2.0.0/.vscode/launch.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 bhpy-2.0.0/bhpy/__init__.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 bhpy-2.0.0/bhpy/spc_qc_config.py
--rw-r--r--   0        0        0    16175 2020-02-02 00:00:00.000000 bhpy-2.0.0/bhpy/spc_qc_wrapper.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 bhpy-2.0.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 bhpy-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bhpy-2.0.0/README.md
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bhpy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 bhpy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bhpy-2.1.0/setup.cfg
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 bhpy-2.1.0/setup.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bhpy-2.1.0/usedPackages.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bhpy-2.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 bhpy-2.1.0/bhpy/__init__.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 bhpy-2.1.0/bhpy/bh_device_scan_wrapper.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 bhpy-2.1.0/bhpy/spc_qc_config.py
+-rw-r--r--   0        0        0    16403 2020-02-02 00:00:00.000000 bhpy-2.1.0/bhpy/spc_qc_wrapper.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 bhpy-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 bhpy-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bhpy-2.1.0/README.md
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bhpy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 bhpy-2.1.0/PKG-INFO
```

### Comparing `bhpy-2.0.0/setup.py` & `bhpy-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'bhpy',
   packages = ['bhpy'],
-  version = '2.0.0',
+  version = '2.1.0',
   license='MIT License',
   description = "Python bindings to use Becker & Hickls' hardware control dll and API",
   author = 'Marscheck',
   author_email = 'marscheck@becker-hickl.de',
   url = 'https://www.becker-hickl.com/',
-  download_url = 'https://git.becker-hickl.com/products/bhpy/-/archive/v2.0.0/bhpy-v2.0.0.tar.gz',
+  download_url = 'https://git.becker-hickl.com/products/bhpy/-/archive/v2.1.0/bhpy-v2.1.0.tar.gz',
   keywords = ['FLIM', 'Fluorescence lifetime', 'TCSPC', 'photon counting', 'BH', 'Becker&Hickl', 'molecular imaging', 'SPC', 'SPCM'],
   install_requires=[
-    'numpy>=1.23.5,<2',
+    'numpy>=1.24.2,<2',
     'appdirs>=1.4.4,<2'
   ],
   classifiers=[
     'Development Status :: 5 - Production/Stable', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Science/Research',
     'Intended Audience :: Developers',
     'Intended Audience :: Healthcare Industry',
```

### Comparing `bhpy-2.0.0/.vscode/launch.json` & `bhpy-2.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `bhpy-2.0.0/bhpy/spc_qc_config.py` & `bhpy-2.1.0/bhpy/spc_qc_config.py`

 * *Files identical despite different names*

### Comparing `bhpy-2.0.0/bhpy/spc_qc_wrapper.py` & `bhpy-2.1.0/bhpy/spc_qc_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 log = logging.getLogger(__name__)
 
 try:
-  from ctypes import byref, c_int16, addressof, create_string_buffer, Structure, CDLL, POINTER, c_char_p, c_uint8,\
-                     c_uint16, c_uint32, c_bool, c_double, c_int8, c_float, c_void_p, c_uint64, c_int64, Union,\
-                     LittleEndianStructure, c_char, c_int32
+  from ctypes import byref, c_int16, create_string_buffer, Structure, CDLL, POINTER, c_char_p, c_uint8,\
+                     c_uint16, c_uint32, c_bool, c_double, c_int8, c_float, c_void_p, c_uint64, c_int64,\
+                     Union, LittleEndianStructure, c_char, c_int32
   import argparse
   import numpy as np
   import numpy.typing as npt
   import pathlib
   import re
   import threading
+  import winreg
 except ModuleNotFoundError as err:
   # Error handling
   log.error(err)
 
 class ModuleInit(Structure):
   _fields_ = [("deviceNr", c_uint8),
               ("initialized", c_bool),
@@ -35,16 +36,26 @@
 class HardwareError(IOError):
   pass
 
 class SpcQcDllWrapper:
   versionStr = ""
   versionStrBuf = create_string_buffer(128)
 
-  def __init__(self, filename):
-    self.__dll = CDLL(filename)
+  def __init__(self, dllPath = None):
+    if dllPath is None:
+      spcmPath = winreg.QueryValueEx(winreg.OpenKey(winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER), 'SOFTWARE\\BH\\SPCM'), "FilePath")[0]
+      dllPath = pathlib.Path(spcmPath).parent / "DLL/spc_qc_104.dll"
+    else:
+      dllPath = pathlib.Path(dllPath)
+    
+    try:
+      self.__dll = CDLL(str(dllPath.absolute()))
+    except FileNotFoundError as e:
+      log.error(e)
+      raise
 
     self.__get_dll_version = self.__dll.get_dll_version
     self.__get_dll_version.argtypes = [c_char_p, c_uint8]
     self.__get_dll_version.restype = c_int16
 
     self.__get_dll_version(self.versionStrBuf, c_uint8(128))
     self.versionStr = str(self.versionStrBuf.value)[2:-1]
@@ -54,14 +65,16 @@
     minor = int(match.group(2))
     patch = int(match.group(3))
     if (major != 2):
       raise RuntimeError(f"Unable to load DLL: incompatible version. Version is: {major}.{minor}.{patch} Expected >= 2.0.0, < 3")
 
     self.__deinit_data_collection = self.__dll.deinit_data_collection
 
+    self.__deinit_data_collections = self.__dll.deinit_data_collections
+
     self.__deinit = self.__dll.deinit
     self.__deinit.restype = c_uint8
 
     self.__get_events_from_buffer = self.__dll.get_events_from_buffer
     self.__get_events_from_buffer.argtypes = [c_void_p, c_uint32, c_uint8]
     self.__get_events_from_buffer.restype = c_int64
 
@@ -187,14 +200,17 @@
     self.__write_setting = self.__dll.write_setting
     self.__write_setting.argtypes = [c_uint16, c_uint32]
     self.__write_setting.restype = c_uint32
 
   def deinit_data_collection(self):
     self.__deinit_data_collection()
 
+  def deinit_data_collections(self):
+    self.__deinit_data_collections()
+
   def deinit(self):
     return self.__deinit()
 
   def get_events_from_buffer(self, buffer: npt.NDArray[np.uint32], maxEvents, cardNumber, filterMTOs: bool=False):
     getEvents = self.__get_events_from_buffer if filterMTOs else self.__get_raw_events_from_buffer
     arg2 = c_uint32(maxEvents)
     arg3 = c_uint8(cardNumber)
@@ -403,30 +419,22 @@
 
   def write_setting(self, settingId, value):
     arg1 = c_uint16(settingId)
     arg2 = c_uint32(value)
     return self.__write_setting(arg1, arg2)
 
 def main():
-  home_drive = pathlib.Path.home().drive
-  parser = argparse.ArgumentParser(prog="bhPy", description="SPC-QC-104 dll wrapper that provides python bindings to use Becker&Hickls' SPC-QC-104 hardware through the dll")
-  parser.add_argument('dll_path', nargs='?', default=f'{home_drive}/Program Files (x86)/BH/SPCM/spc_qc_104.dll')
+  parser = argparse.ArgumentParser(prog="SPC-QC-104 DLL Wrapper", description="SPC-QC-104 dll wrapper that provides python bindings to use Becker&Hickls' SPC-QC-104 hardware through the dll")
+  parser.add_argument('dll_path', nargs='?', default=None)
 
   args = parser.parse_args()
 
   dll_path = pathlib.Path(args.dll_path)
 
-  print(dll_path)
-
-  if not dll_path.exists:
-    dll_path = pathlib.Path(f"{home_drive}/Program Files/BH/SPCM/spc_qc_104.dll")
-    if not dll_path.exists:
-      print(".../spc_qc_104.dll was neither found at default location nor at the specified path")
-      exit()
-
-  spcQcDll = SpcQcDllWrapper(str(dll_path))
+  spcQcDll = SpcQcDllWrapper(dll_path)
   print(spcQcDll.versionStr)
   spcQcDll.init([0], emulateHardware=True)
   print(spcQcDll.serialNumber)
+  input("press enter...")
 
 if __name__ == '__main__':
   main()
```

### Comparing `bhpy-2.0.0/.gitignore` & `bhpy-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bhpy-2.0.0/LICENSE.txt` & `bhpy-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bhpy-2.0.0/pyproject.toml` & `bhpy-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bhpy"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Marscheck", email="marscheck@becker-hickl.de" },
 ]
 dependencies = [
-  "numpy >= 1.23.5, <2",
+  "numpy >= 1.24.2, <2",
   "appdirs >= 1.4.4, <2"
 ]
 description = "Python bindings to use Becker & Hickls' hardware control dll and API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT License" }
 keywords = ['FLIM', 'Fluorescence lifetime', 'TCSPC', 'photon counting', 'BH', 'Becker&Hickl', 'molecular imaging', 'SPC', 'SPCM']
@@ -34,8 +34,8 @@
     'Programming Language :: Python :: 3.11',
     'Operating System :: OS Independent',
 ]
 
 [project.urls]
 "Homepage" = "https://www.becker-hickl.com"
 "Bug Tracker" = "https://github.com/bhmarscheck/bhpy/issues"
-"Download" = "https://git.becker-hickl.com/products/bhpy/-/archive/v2.0.0/bhpy-v2.0.0.tar.gz"
+"Download" = "https://git.becker-hickl.com/products/bhpy/-/archive/v2.1.0/bhpy-v2.1.0.tar.gz"
```

### Comparing `bhpy-2.0.0/PKG-INFO` & `bhpy-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bhpy
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python bindings to use Becker & Hickls' hardware control dll and API
 Project-URL: Homepage, https://www.becker-hickl.com
 Project-URL: Bug Tracker, https://github.com/bhmarscheck/bhpy/issues
-Project-URL: Download, https://git.becker-hickl.com/products/bhpy/-/archive/v2.0.0/bhpy-v2.0.0.tar.gz
+Project-URL: Download, https://git.becker-hickl.com/products/bhpy/-/archive/v2.1.0/bhpy-v2.1.0.tar.gz
 Author-email: Marscheck <marscheck@becker-hickl.de>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: BH,Becker&Hickl,FLIM,Fluorescence lifetime,SPC,SPCM,TCSPC,molecular imaging,photon counting
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
@@ -22,11 +22,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Python: >=3.8
 Requires-Dist: appdirs<2,>=1.4.4
-Requires-Dist: numpy<2,>=1.23.5
+Requires-Dist: numpy<2,>=1.24.2
 Description-Content-Type: text/markdown
 
 # bhPy
```

