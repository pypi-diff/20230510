# Comparing `tmp/ptzipcam-0.0.5.tar.gz` & `tmp/ptzipcam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ptzipcam-0.0.5.tar", last modified: Thu Apr 27 22:51:09 2023, max compression
+gzip compressed data, was "ptzipcam-0.0.6.tar", last modified: Wed May 10 16:58:44 2023, max compression
```

## Comparing `ptzipcam-0.0.5.tar` & `ptzipcam-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/setup.cfg
--rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/README.md
--rw-rw-r--   0 ian       (1000) ian       (1000)     3974 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/PKG-INFO
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     3974 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       55 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam.egg-info/requires.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)     1425 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/setup.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-04-27 22:51:09.000000 ptzipcam-0.0.5/ptzipcam/
--rw-rw-r--   0 ian       (1000) ian       (1000)    17536 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/ptz_camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)       89 2023-04-27 22:48:11.000000 ptzipcam-0.0.5/ptzipcam/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/camera.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4111 2023-04-27 22:48:11.000000 ptzipcam-0.0.5/ptzipcam/io.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/video_writer.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/convert.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/logs.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/tracker.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/ptzipcam/ui.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-23 20:49:22.000000 ptzipcam-0.0.5/LICENSE
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1073 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/LICENSE
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3935 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3527 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/README.md
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/ptzipcam/
+-rw-rw-r--   0 ian       (1000) ian       (1000)       89 2023-05-10 16:55:32.000000 ptzipcam-0.0.6/ptzipcam/__init__.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2125 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1563 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/convert.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4111 2023-04-27 22:48:11.000000 ptzipcam-0.0.6/ptzipcam/io.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2019 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/logs.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)    17536 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/ptz_camera.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     4759 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/tracker.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     3061 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/ui.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1404 2023-03-23 20:49:22.000000 ptzipcam-0.0.6/ptzipcam/video_writer.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/ptzipcam.egg-info/
+-rw-r--r--   0 ian       (1000) ian       (1000)     3935 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/PKG-INFO
+-rw-r--r--   0 ian       (1000) ian       (1000)      360 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/SOURCES.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       37 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/requires.txt
+-rw-r--r--   0 ian       (1000) ian       (1000)        9 2023-05-10 16:58:44.000000 ptzipcam-0.0.6/ptzipcam.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-05-10 16:58:44.176881 ptzipcam-0.0.6/setup.cfg
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1472 2023-05-10 16:55:26.000000 ptzipcam-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ptzipcam-0.0.5/README.md` & `ptzipcam-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/PKG-INFO` & `ptzipcam-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: ptzipcam
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for controlling PTZ IP cameras that support ONVIF
-Home-page: UNKNOWN
 Author: Ian Ingram
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,9 +118,7 @@
 
      cp wsdl/wsdl.tar.gz ~/.virtualenvs/ptzipcam_env/lib/python3.7/site-packages/
      cd ~/.virtualenvs/ptzipcam_env/lib/python3.7/site-packages/
      tar xzf wsdl.tar.gz
      rm wsdl.tar.gz
      cd -
 
-
-
```

### Comparing `ptzipcam-0.0.5/ptzipcam.egg-info/PKG-INFO` & `ptzipcam-0.0.6/ptzipcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: ptzipcam
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for controlling PTZ IP cameras that support ONVIF
-Home-page: UNKNOWN
 Author: Ian Ingram
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,9 +118,7 @@
 
      cp wsdl/wsdl.tar.gz ~/.virtualenvs/ptzipcam_env/lib/python3.7/site-packages/
      cd ~/.virtualenvs/ptzipcam_env/lib/python3.7/site-packages/
      tar xzf wsdl.tar.gz
      rm wsdl.tar.gz
      cd -
 
-
-
```

### Comparing `ptzipcam-0.0.5/setup.py` & `ptzipcam-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,33 @@
+"""Setup.py for this project
+
+"""
+
 import os
 import re
 
 import setuptools
 
 
 def read(filename):
+    """Read file using path of this file to find it
+
+    """
     path = os.path.join(os.path.abspath(os.path.dirname(__file__)), filename)
-    with open(path, 'r') as f:
-        return f.read()
+    with open(path, 'r', encoding='utf-8') as readfile:
+        return readfile.read()
 
 
 def find_version(text):
+    """Extract the version from a file
+
+    Using regular expressions to find the string that looks like the
+    version number
+
+    """
     match = re.search(r"^__version__\s*=\s*['\"](.*)['\"]\s*$", text,
                       re.MULTILINE)
     return match.group(1)
 
 
 AUTHOR = "Ian Ingram"
 DESC = "Package for controlling PTZ IP cameras that support ONVIF"
@@ -26,16 +39,16 @@
     long_description_content_type="text/markdown",
     license="MIT",
     version=find_version(read('ptzipcam/__init__.py')),
     author=AUTHOR,
     packages=['ptzipcam'],
     include_package_data=True,
     install_requires=[
-        'numpy==1.18.3',
-        'opencv-python==3.4.2.16',
+        'numpy',
+        'opencv-python',
         'onvif-zeep',
         'camml',
     ],
     extra_require={
         'examples': [
             'pyyaml',
             'imutils',
@@ -44,12 +57,8 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         'Development Status :: 2 - Pre-Alpha',
         'Operating System :: POSIX :: Linux',
     ],
-    # would like to add this as a CLI tool but currently needs config file...
-    # entry_points = {
-    #     'console_scripts': ['aim_ptz_w_keyboard=ptzipcam.utils.aim_ptz_w_keyboard:main']
-    #},
 )
```

### Comparing `ptzipcam-0.0.5/ptzipcam/ptz_camera.py` & `ptzipcam-0.0.6/ptzipcam/ptz_camera.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/camera.py` & `ptzipcam-0.0.6/ptzipcam/camera.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/io.py` & `ptzipcam-0.0.6/ptzipcam/io.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/video_writer.py` & `ptzipcam-0.0.6/ptzipcam/video_writer.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/convert.py` & `ptzipcam-0.0.6/ptzipcam/convert.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/logs.py` & `ptzipcam-0.0.6/ptzipcam/logs.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/tracker.py` & `ptzipcam-0.0.6/ptzipcam/tracker.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/ptzipcam/ui.py` & `ptzipcam-0.0.6/ptzipcam/ui.py`

 * *Files identical despite different names*

### Comparing `ptzipcam-0.0.5/LICENSE` & `ptzipcam-0.0.6/LICENSE`

 * *Files identical despite different names*

