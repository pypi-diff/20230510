# Comparing `tmp/soda-core-dremio-3.0.33.tar.gz` & `tmp/soda-core-dremio-3.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.33.tar", last modified: Tue Apr 25 14:15:15 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.34.tar", last modified: Wed May 10 12:22:52 2023, max compression
```

## Comparing `soda-core-dremio-3.0.33.tar` & `soda-core-dremio-3.0.34.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-25 14:14:25.000000 soda-core-dremio-3.0.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-04-25 14:14:25.000000 soda-core-dremio-3.0.33/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-25 14:15:15.000000 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-04-25 14:15:15.000000 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:15:15.000000 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-25 14:15:15.000000 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-25 14:15:15.000000 soda-core-dremio-3.0.33/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:15.646595 soda-core-dremio-3.0.33/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-25 14:14:25.000000 soda-core-dremio-3.0.33/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-10 12:22:20.000000 soda-core-dremio-3.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-05-10 12:22:20.000000 soda-core-dremio-3.0.34/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-10 12:22:52.000000 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-10 12:22:52.000000 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:22:52.000000 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-10 12:22:52.000000 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:22:52.000000 soda-core-dremio-3.0.34/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:22:52.887353 soda-core-dremio-3.0.34/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-10 12:22:20.000000 soda-core-dremio-3.0.34/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.0.33/setup.py` & `soda-core-dremio-3.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-dremio"
-package_version = "3.0.33"
+package_version = "3.0.34"
 description = "Soda Core Dremio Package"
 
 requires = [f"soda-core=={package_version}", "pyodbc", "pyarrow"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-dremio-3.0.33/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.34/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*

