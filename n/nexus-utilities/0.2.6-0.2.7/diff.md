# Comparing `tmp/nexus-utilities-0.2.6.tar.gz` & `tmp/nexus-utilities-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.2.6.tar", last modified: Tue May  9 17:03:14 2023, max compression
+gzip compressed data, was "nexus-utilities-0.2.7.tar", last modified: Wed May 10 15:49:00 2023, max compression
```

## Comparing `nexus-utilities-0.2.6.tar` & `nexus-utilities-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:03:14.462470 nexus-utilities-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 17:03:14.458470 nexus-utilities-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:03:14.458470 nexus-utilities-0.2.6/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 17:03:14.000000 nexus-utilities-0.2.6/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-09 17:03:14.000000 nexus-utilities-0.2.6/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:03:14.000000 nexus-utilities-0.2.6/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 17:03:14.000000 nexus-utilities-0.2.6/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 17:03:14.000000 nexus-utilities-0.2.6/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:03:14.458470 nexus-utilities-0.2.6/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:03:14.462470 nexus-utilities-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 17:03:03.000000 nexus-utilities-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:00.285575 nexus-utilities-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 15:49:00.285575 nexus-utilities-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:00.281575 nexus-utilities-0.2.7/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 15:49:00.000000 nexus-utilities-0.2.7/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-10 15:49:00.000000 nexus-utilities-0.2.7/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:49:00.000000 nexus-utilities-0.2.7/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 15:49:00.000000 nexus-utilities-0.2.7/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 15:49:00.000000 nexus-utilities-0.2.7/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:00.285575 nexus-utilities-0.2.7/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:49:00.285575 nexus-utilities-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-10 15:48:49.000000 nexus-utilities-0.2.7/setup.py
```

### Comparing `nexus-utilities-0.2.6/LICENSE.txt` & `nexus-utilities-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/PKG-INFO` & `nexus-utilities-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.6
+Version: 0.2.7
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.6/README.md` & `nexus-utilities-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.2.7/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.6
+Version: 0.2.7
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.6/nexus_utils/config_utils.py` & `nexus-utilities-0.2.7/nexus_utils/config_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Configuration-related utilities"""
 #%%
 import os
-import glob
+import pathlib
+# import glob
 import configparser
-import io
+# import io
 
 #%%
 def read_config_file(config_filepath):
     """Read config .ini file at provided location, using '_local' version instead if found"""
+    if isinstance(config_filepath, str):
+        config_filepath = pathlib.Path(config_filepath)
     config = configparser.ConfigParser()
     break_out_flag = False
     # Locate local config file
     local_config_path = ''
-    for root, dirs, files in os.walk(os.getcwd()):
+    for root, dirs, files in os.walk(config_filepath.parent):
         if break_out_flag == True:
             break
         files = [file for file in files if file.endswith(('.ini'))]
         for file in files:
             if break_out_flag == True:
                 break
             if file == config_filepath.stem + '_local.ini':
-                local_config_path = os.path.join(root, file)
+                # local_config_path = os.path.join(root, file)
+                local_config_path = pathlib.Path(root) / file
                 break_out_flag = True
                 break
-                #fp_local = io.open(local_config_path, 'r', encoding='utf_8_sig')
-    #fp = io.open(config_filepath, 'r', encoding='utf_8_sig')
     config.read([config_filepath, local_config_path])#, encoding='utf-8-sig')
     return config
 
 # %%
```

### Comparing `nexus-utilities-0.2.6/nexus_utils/database_utils.py` & `nexus-utilities-0.2.7/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/nexus_utils/datetime_utils.py` & `nexus-utilities-0.2.7/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/nexus_utils/package_utils.py` & `nexus-utilities-0.2.7/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/nexus_utils/password_utils.py` & `nexus-utilities-0.2.7/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.6/setup.py` & `nexus-utilities-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.2.6',
+    version='0.2.7',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

