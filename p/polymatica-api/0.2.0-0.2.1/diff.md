# Comparing `tmp/polymatica_api-0.2.0.tar.gz` & `tmp/polymatica_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.2.0.tar", last modified: Wed May 10 18:58:42 2023, max compression
+gzip compressed data, was "polymatica_api-0.2.1.tar", last modified: Wed May 10 19:08:57 2023, max compression
```

## Comparing `polymatica_api-0.2.0.tar` & `polymatica_api-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.312589 polymatica_api-0.2.0/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.2.0/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 18:58:42.312380 polymatica_api-0.2.0/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.2.0/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.310971 polymatica_api-0.2.0/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     2870 2023-05-10 18:57:42.000000 polymatica_api-0.2.0/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.2.0/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.2.0/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     2674 2023-05-10 18:55:53.000000 polymatica_api-0.2.0/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 18:58:42.312100 polymatica_api-0.2.0/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-10 18:58:42.000000 polymatica_api-0.2.0/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-10 18:58:42.312656 polymatica_api-0.2.0/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-10 18:58:35.000000 polymatica_api-0.2.0/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 19:08:57.740695 polymatica_api-0.2.1/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.2.1/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 19:08:57.740459 polymatica_api-0.2.1/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.2.1/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 19:08:57.738972 polymatica_api-0.2.1/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     2940 2023-05-10 19:08:13.000000 polymatica_api-0.2.1/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.2.1/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.2.1/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     2674 2023-05-10 18:55:53.000000 polymatica_api-0.2.1/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-10 19:08:57.740140 polymatica_api-0.2.1/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-10 19:08:57.000000 polymatica_api-0.2.1/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-10 19:08:57.000000 polymatica_api-0.2.1/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-10 19:08:57.000000 polymatica_api-0.2.1/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-10 19:08:57.000000 polymatica_api-0.2.1/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-10 19:08:57.000000 polymatica_api-0.2.1/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-10 19:08:57.740759 polymatica_api-0.2.1/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-10 19:08:47.000000 polymatica_api-0.2.1/setup.py
```

### Comparing `polymatica_api-0.2.0/LICENSE` & `polymatica_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.0/PKG-INFO` & `polymatica_api-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.2.0/README.md` & `polymatica_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.0/polymatica_api/__init__.py` & `polymatica_api-0.2.1/polymatica_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import requests
 import urllib.parse
 
 
 HOST_ROUTE = dict(
     dataset='/proxy/manager/api/v1/dataset',
     data_dataset='/proxy/manager/api/v1/data/dataset',
-    write_line='/api/v1/data-line/{id}',
-    write_lines='/api/v1/data-line/{id}/rows',
-    delete_line='/api/v1/data-line/{id}/{uid}',
-    update_line='/api/v1/data-line/{id}/{uid}',
-    dataset_create='/api/v1/dataset-local'
+    write_line='/proxy/manager/api/v1/data-line/{id}',
+    write_lines='/proxy/manager/api/v1/data-line/{id}/rows',
+    delete_line='/proxy/manager/api/v1/data-line/{id}/{uid}',
+    update_line='/proxy/manager/api/v1/data-line/{id}/{uid}',
+    dataset_create='/proxy/manager/api/v1/dataset-local'
 )
 
 
 class PolymaticaAPI:
     _host: str
     _session: requests.Session
```

### Comparing `polymatica_api-0.2.0/polymatica_api/data_option.py` & `polymatica_api-0.2.1/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.0/polymatica_api/types.py` & `polymatica_api-0.2.1/polymatica_api/types.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.2.0/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.2.1/polymatica_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica-api
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.2.0/setup.py` & `polymatica_api-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.2.0",
+    version="0.2.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

