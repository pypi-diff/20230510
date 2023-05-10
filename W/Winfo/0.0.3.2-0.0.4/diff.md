# Comparing `tmp/Winfo-0.0.3.2.tar.gz` & `tmp/Winfo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.3.2.tar", last modified: Thu Apr 13 19:36:32 2023, max compression
+gzip compressed data, was "Winfo-0.0.4.tar", last modified: Wed May 10 20:28:45 2023, max compression
```

## Comparing `Winfo-0.0.3.2.tar` & `Winfo-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.773516 Winfo-0.0.3.2/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.3.2/LICENSE
--rw-rw-rw-   0        0        0     6162 2023-04-13 19:36:32.772516 Winfo-0.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5714 2023-04-11 23:13:18.000000 Winfo-0.0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.759517 Winfo-0.0.3.2/Winfo/
--rw-rw-rw-   0        0        0     2686 2023-04-11 23:02:28.000000 Winfo-0.0.3.2/Winfo/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.3.2/Winfo/cpu.py
--rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.3.2/Winfo/disk.py
--rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.3.2/Winfo/ethernet.py
--rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.3.2/Winfo/gpu.py
--rw-rw-rw-   0        0        0      607 2023-04-13 19:35:23.000000 Winfo-0.0.3.2/Winfo/internet.py
--rw-rw-rw-   0        0        0     1312 2023-04-13 19:32:57.000000 Winfo-0.0.3.2/Winfo/memory.py
--rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.3.2/Winfo/motherboard.py
--rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.3.2/Winfo/software.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:36:32.771517 Winfo-0.0.3.2/Winfo.egg-info/
--rw-rw-rw-   0        0        0     6162 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 19:36:32.000000 Winfo-0.0.3.2/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:36:32.773516 Winfo-0.0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-13 19:36:05.000000 Winfo-0.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:45.471866 Winfo-0.0.4/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6685 2023-05-10 20:28:45.470869 Winfo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6287 2023-05-10 20:22:39.000000 Winfo-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:45.461868 Winfo-0.0.4/Winfo/
+-rw-rw-rw-   0        0        0     2709 2023-05-10 20:04:34.000000 Winfo-0.0.4/Winfo/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-05-10 20:23:23.000000 Winfo-0.0.4/Winfo/audio.py
+-rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.4/Winfo/cpu.py
+-rw-rw-rw-   0        0        0      982 2023-05-10 19:42:35.000000 Winfo-0.0.4/Winfo/disk.py
+-rw-rw-rw-   0        0        0      683 2023-05-10 19:45:13.000000 Winfo-0.0.4/Winfo/ethernet.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.4/Winfo/gpu.py
+-rw-rw-rw-   0        0        0      607 2023-04-13 19:35:23.000000 Winfo-0.0.4/Winfo/internet.py
+-rw-rw-rw-   0        0        0     1312 2023-05-10 20:27:16.000000 Winfo-0.0.4/Winfo/memory.py
+-rw-rw-rw-   0        0        0      481 2023-05-10 19:44:27.000000 Winfo-0.0.4/Winfo/motherboard.py
+-rw-rw-rw-   0        0        0     1400 2023-05-10 20:21:29.000000 Winfo-0.0.4/Winfo/software.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:28:45.468865 Winfo-0.0.4/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     6685 2023-05-10 20:28:45.000000 Winfo-0.0.4/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-10 20:28:45.000000 Winfo-0.0.4/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 20:28:45.000000 Winfo-0.0.4/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 20:28:45.000000 Winfo-0.0.4/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 20:28:45.471866 Winfo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-05-10 20:24:01.000000 Winfo-0.0.4/setup.py
```

### Comparing `Winfo-0.0.3.2/LICENSE` & `Winfo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.2/PKG-INFO` & `Winfo-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.3.2
+Version: 0.0.4
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
-Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Winfo
@@ -135,15 +134,15 @@
 - Get MAC Address (Please read disclaimer, which can be found in the source code of this project)
 - List all recognized Network Adapters
 
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
-print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
+print("List of all Network Adapters as a Python list: " + str(Winfo.ethernet.listadapters()))
 ```
 
 - Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
@@ -190,27 +189,43 @@
 
 ```Python
 import Winfo
 
 print("My Motherboard is an " + Winfo.motherboard.getname() + " , made by " + Winfo.motherboard.getmanufacturer())
 ```
 
+### Audio Device Information
+
+- Get a list of all connected audio devices (also shows virtual devices)
+- Get a list of all the manufacturers of those
+
+```Python
+import Winfo
+
+print("All my audio devices as a Python list: " + str(Winfo.audio.listall()))
+print("And the manufacturers: "  + str(Winfo.audio.listmanufacturers()))
+```
+
+- Like all the other lists, you can make them look prettier, by doing it the same way, that was mentioned above
+
 ### Software Information
 
 - Get current Windows version
 - Get current Windows release
 - Get device name
 - Get user name
+- Get where your system is located (Partition)
 
 ```Python
 import Winfo
 
 print("I'm current running Windows " + Winfo.software.system() + " on version " + Winfo.software.version())
 print("I named my computer " + Winfo.software.devicename())
 print("I'm logged in as " + Winfo.software.username())
+print("My system partition is at " + Winfo.software.where())
 ```
 ## Questions you might have:
 
 - Q: How can I install this library? A: pip install Winfo
 - Q: MacOS/Linux/BSD Support? A: Windows-only.
 - Q: What can I do with the code? A: Read the license (CC BY-SA 4.0)
```

### Comparing `Winfo-0.0.3.2/README.md` & `Winfo-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 - Get MAC Address (Please read disclaimer, which can be found in the source code of this project)
 - List all recognized Network Adapters
 
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
-print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
+print("List of all Network Adapters as a Python list: " + str(Winfo.ethernet.listadapters()))
 ```
 
 - Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
@@ -177,27 +177,43 @@
 
 ```Python
 import Winfo
 
 print("My Motherboard is an " + Winfo.motherboard.getname() + " , made by " + Winfo.motherboard.getmanufacturer())
 ```
 
+### Audio Device Information
+
+- Get a list of all connected audio devices (also shows virtual devices)
+- Get a list of all the manufacturers of those
+
+```Python
+import Winfo
+
+print("All my audio devices as a Python list: " + str(Winfo.audio.listall()))
+print("And the manufacturers: "  + str(Winfo.audio.listmanufacturers()))
+```
+
+- Like all the other lists, you can make them look prettier, by doing it the same way, that was mentioned above
+
 ### Software Information
 
 - Get current Windows version
 - Get current Windows release
 - Get device name
 - Get user name
+- Get where your system is located (Partition)
 
 ```Python
 import Winfo
 
 print("I'm current running Windows " + Winfo.software.system() + " on version " + Winfo.software.version())
 print("I named my computer " + Winfo.software.devicename())
 print("I'm logged in as " + Winfo.software.username())
+print("My system partition is at " + Winfo.software.where())
 ```
 ## Questions you might have:
 
 - Q: How can I install this library? A: pip install Winfo
 - Q: MacOS/Linux/BSD Support? A: Windows-only.
 - Q: What can I do with the code? A: Read the license (CC BY-SA 4.0)
```

### Comparing `Winfo-0.0.3.2/Winfo/__init__.py` & `Winfo-0.0.4/Winfo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,7 +60,8 @@
 from Winfo import gpu
 from Winfo import disk
 from Winfo import memory
 from Winfo import motherboard
 from Winfo import software
 from Winfo import ethernet
 from Winfo import internet
+from Winfo import audio
```

### Comparing `Winfo-0.0.3.2/Winfo/cpu.py` & `Winfo-0.0.4/Winfo/cpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.2/Winfo/disk.py` & `Winfo-0.0.4/Winfo/disk.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,8 +22,9 @@
         raise IndexError("Disk Index invalid.")
     elif index < 0:
         raise IndexError("Disk Index invalid.")
     elif size == "":
         raise IndexError("Disk Index invalid.")
     elif size == "           \r\r":
         raise IndexError("Disk Index invalid.")
-    return int(size)
+    else:
+        return int(size)
```

### Comparing `Winfo-0.0.3.2/Winfo/ethernet.py` & `Winfo-0.0.4/Winfo/ethernet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from subprocess import check_output
 
 def macaddr():
     """
-    DISCLAIMER
+    ## DISCLAIMER
     
     May not be true!
     
     If it isn't true, please don't contact us, because this function basically gets it from the getmac-Command in Windows.
     So this basically relies on Windows' Shell.
     
     """
```

### Comparing `Winfo-0.0.3.2/Winfo/gpu.py` & `Winfo-0.0.4/Winfo/gpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.2/Winfo/internet.py` & `Winfo-0.0.4/Winfo/internet.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.2/Winfo/memory.py` & `Winfo-0.0.4/Winfo/memory.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.3.2/Winfo/software.py` & `Winfo-0.0.4/Winfo/software.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,14 @@
     getdevname = rawdecoded.strip("SystemName").rstrip("\n").replace("\n", "")
     return getdevname
 
 def username():
     raw = check_output(["echo", "%USERNAME%"], shell=True)
     rawdecoded = raw.decode()
     getusername = rawdecoded.replace("\n", "")
-    return getusername
+    return getusername
+
+def where():
+    raw = check_output(["wmic", "bootconfig", "get", "Caption"])
+    rawdecoded = raw.decode()
+    getpart = rawdecoded.replace("Caption", "", 1).replace("\n", "")
+    return getpart
```

### Comparing `Winfo-0.0.3.2/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.4/Winfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.3.2
+Version: 0.0.4
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
-Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Winfo
@@ -135,15 +134,15 @@
 - Get MAC Address (Please read disclaimer, which can be found in the source code of this project)
 - List all recognized Network Adapters
 
 ```Python
 import Winfo
 
 print("My MAC Address is: " + Winfo.ethernet.macaddr())
-print("List of all Network Adapters as a Python list: " + Winfo.ethernet.listadapters())
+print("List of all Network Adapters as a Python list: " + str(Winfo.ethernet.listadapters()))
 ```
 
 - Like with the Disklist and the getSpeedAll, you can make the list returned from Winfo.ethernet.listadapters() way prettier by doing this:
 
 ```Python
 import Winfo
 
@@ -190,27 +189,43 @@
 
 ```Python
 import Winfo
 
 print("My Motherboard is an " + Winfo.motherboard.getname() + " , made by " + Winfo.motherboard.getmanufacturer())
 ```
 
+### Audio Device Information
+
+- Get a list of all connected audio devices (also shows virtual devices)
+- Get a list of all the manufacturers of those
+
+```Python
+import Winfo
+
+print("All my audio devices as a Python list: " + str(Winfo.audio.listall()))
+print("And the manufacturers: "  + str(Winfo.audio.listmanufacturers()))
+```
+
+- Like all the other lists, you can make them look prettier, by doing it the same way, that was mentioned above
+
 ### Software Information
 
 - Get current Windows version
 - Get current Windows release
 - Get device name
 - Get user name
+- Get where your system is located (Partition)
 
 ```Python
 import Winfo
 
 print("I'm current running Windows " + Winfo.software.system() + " on version " + Winfo.software.version())
 print("I named my computer " + Winfo.software.devicename())
 print("I'm logged in as " + Winfo.software.username())
+print("My system partition is at " + Winfo.software.where())
 ```
 ## Questions you might have:
 
 - Q: How can I install this library? A: pip install Winfo
 - Q: MacOS/Linux/BSD Support? A: Windows-only.
 - Q: What can I do with the code? A: Read the license (CC BY-SA 4.0)
```

### Comparing `Winfo-0.0.3.2/setup.py` & `Winfo-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.3.2",
+    version="0.0.4",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
-        "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

