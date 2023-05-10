# Comparing `tmp/funcx-endpoint-2.0.2a1.tar.gz` & `tmp/funcx-endpoint-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.0.2a1.tar", last modified: Mon May  8 22:01:50 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.0.3.tar", last modified: Wed May 10 20:42:19 2023, max compression
```

## Comparing `funcx-endpoint-2.0.2a1.tar` & `funcx-endpoint-2.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.005654 funcx-endpoint-2.0.2a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 funcx-endpoint-2.0.2a1/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-05-08 22:01:50.005712 funcx-endpoint-2.0.2a1/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-20 03:21:56.000000 funcx-endpoint-2.0.2a1/PyPI.md
--rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/README.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.003799 funcx-endpoint-2.0.2a1/funcx_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.004601 funcx-endpoint-2.0.2a1/funcx_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.004796 funcx-endpoint-2.0.2a1/funcx_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)       89 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.004969 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.005484 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-20 15:03:07.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      101 2023-04-20 03:22:06.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/high_throughput/funcx_manager.py
--rw-r--r--   0 lei        (501) staff       (20)      114 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/executors/high_throughput/funcx_worker.py
--rw-r--r--   0 lei        (501) staff       (20)      245 2023-05-08 21:59:12.000000 funcx-endpoint-2.0.2a1/funcx_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:50.004492 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2042 2023-05-08 22:01:49.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      662 2023-05-08 22:01:50.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-08 22:01:49.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      329 2023-05-08 22:01:49.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)       33 2023-05-08 22:01:49.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       15 2023-05-08 22:01:49.000000 funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-05-08 22:01:50.005962 funcx-endpoint-2.0.2a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2032 2023-05-08 21:59:03.000000 funcx-endpoint-2.0.2a1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.003884 funcx-endpoint-2.0.3/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 20:09:04.000000 funcx-endpoint-2.0.3/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     2040 2023-05-10 20:42:19.003969 funcx-endpoint-2.0.3/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1115 2023-04-17 20:09:04.000000 funcx-endpoint-2.0.3/PyPI.md
+-rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.001111 funcx-endpoint-2.0.3/funcx_endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)      122 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002254 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002479 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)       89 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002658 funcx-endpoint-2.0.3/funcx_endpoint/executors/
+-rw-r--r--   0 chris      (501) staff       (20)      107 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.003656 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-20 15:45:45.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      101 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/funcx_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)      114 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.3/funcx_endpoint/executors/high_throughput/funcx_worker.py
+-rw-r--r--   0 chris      (501) staff       (20)      243 2023-05-10 20:21:13.000000 funcx-endpoint-2.0.3/funcx_endpoint/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:42:19.002116 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2040 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      662 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      329 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)       31 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       15 2023-05-10 20:42:18.000000 funcx-endpoint-2.0.3/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      305 2023-05-10 20:42:19.004303 funcx-endpoint-2.0.3/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     2030 2023-05-10 20:20:51.000000 funcx-endpoint-2.0.3/setup.py
```

### Comparing `funcx-endpoint-2.0.2a1/LICENSE` & `funcx-endpoint-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.2a1/PKG-INFO` & `funcx-endpoint-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.2a1
+Version: 2.0.3
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.2a1/PyPI.md` & `funcx-endpoint-2.0.3/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.0.3/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.2a1
+Version: 2.0.3
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.0.2a1/funcx_endpoint.egg-info/SOURCES.txt` & `funcx-endpoint-2.0.3/funcx_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.2a1/setup.py` & `funcx-endpoint-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint>=2.0.2a1",
+    "globus-compute-endpoint==2.0.3",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
```

