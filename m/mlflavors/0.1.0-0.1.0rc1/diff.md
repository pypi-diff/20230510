# Comparing `tmp/mlflavors-0.1.0.tar.gz` & `tmp/mlflavors-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflavors-0.1.0.tar", last modified: Wed May 10 13:18:11 2023, max compression
+gzip compressed data, was "mlflavors-0.1.0rc1.tar", last modified: Fri May  5 15:03:50 2023, max compression
```

## Comparing `mlflavors-0.1.0.tar` & `mlflavors-0.1.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:11.561338 mlflavors-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 13:18:11.561338 mlflavors-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-10 13:18:01.000000 mlflavors-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:11.557338 mlflavors-0.1.0/mlflavors/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/orbit.py
--rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/sdv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)    20126 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:11.561338 mlflavors-0.1.0/mlflavors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 13:18:01.000000 mlflavors-0.1.0/mlflavors/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:11.561338 mlflavors-0.1.0/mlflavors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 13:18:11.000000 mlflavors-0.1.0/mlflavors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-10 13:18:11.000000 mlflavors-0.1.0/mlflavors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:18:11.000000 mlflavors-0.1.0/mlflavors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-10 13:18:11.000000 mlflavors-0.1.0/mlflavors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 13:18:11.000000 mlflavors-0.1.0/mlflavors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-10 13:18:01.000000 mlflavors-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 13:18:11.561338 mlflavors-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-10 13:18:01.000000 mlflavors-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:18:11.561338 mlflavors-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-10 13:18:01.000000 mlflavors-0.1.0/tests/test_orbit_model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-10 13:18:01.000000 mlflavors-0.1.0/tests/test_pyod_model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-10 13:18:01.000000 mlflavors-0.1.0/tests/test_sdv_model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-10 13:18:01.000000 mlflavors-0.1.0/tests/test_sktime_model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-10 13:18:01.000000 mlflavors-0.1.0/tests/test_statsforecast_model_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:50.489960 mlflavors-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-05 15:03:50.489960 mlflavors-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:50.485959 mlflavors-0.1.0rc1/mlflavors/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/sdv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20126 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:50.485959 mlflavors-0.1.0rc1/mlflavors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/mlflavors/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:50.485959 mlflavors-0.1.0rc1/mlflavors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-05 15:03:50.000000 mlflavors-0.1.0rc1/mlflavors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-05 15:03:50.000000 mlflavors-0.1.0rc1/mlflavors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:03:50.000000 mlflavors-0.1.0rc1/mlflavors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 15:03:50.000000 mlflavors-0.1.0rc1/mlflavors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 15:03:50.000000 mlflavors-0.1.0rc1/mlflavors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 15:03:50.489960 mlflavors-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:03:50.489960 mlflavors-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/tests/test_orbit_model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/tests/test_pyod_model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/tests/test_sdv_model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/tests/test_sktime_model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-05 15:03:36.000000 mlflavors-0.1.0rc1/tests/test_statsforecast_model_export.py
```

### Comparing `mlflavors-0.1.0/mlflavors/orbit.py` & `mlflavors-0.1.0rc1/mlflavors/orbit.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors/pyod.py` & `mlflavors-0.1.0rc1/mlflavors/pyod.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors/sdv.py` & `mlflavors-0.1.0rc1/mlflavors/sdv.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors/sktime.py` & `mlflavors-0.1.0rc1/mlflavors/sktime.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors/statsforecast.py` & `mlflavors-0.1.0rc1/mlflavors/statsforecast.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors/utils/data.py` & `mlflavors-0.1.0rc1/mlflavors/utils/data.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/mlflavors.egg-info/SOURCES.txt` & `mlflavors-0.1.0rc1/mlflavors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/pyproject.toml` & `mlflavors-0.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/setup.py` & `mlflavors-0.1.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """The file configures the Python package."""
 
 from setuptools import find_packages, setup
 
 from mlflavors.version import __version__
 
 PACKAGE_REQUIREMENTS = [
+    "datasetsforecast==0.0.8",
     "mlflow",
+    "scikit-learn",
+    "orbit-ml",
+    "pmdarima",
     "sktime",
     "statsforecast",
     "pyod",
     "sdv",
 ]
 
-ORBIT_REQUIREMENTS = [
-    "orbit-ml",
-]
-
 DEV_REQUIREMENTS = [
-    "datasetsforecast==0.0.8",
-    "pmdarima",
     "pre-commit",
     "pytest",
     "pytest-cov",
     "setuptools",
     "tomli",
+]
+
+DOC_REQUIREMENTS = [
     "nbsphinx==0.9.1",
     "numpydoc==1.5.0",
     "sphinx_rtd_theme==1.1.1",
     "sphinx==5.3.0",
-    "urllib3<2",
 ]
 
 setup(
     name="mlflavors",
     description="""
         MLflavors: A collection of custom MLflow flavors.
         """,
@@ -47,13 +47,13 @@
         "Documentation": "https://mlflavors.readthedocs.io/en/latest/",
     },
     packages=find_packages(exclude=["tests", "tests.*", "examples"]),
     setup_requires=["setuptools", "wheel"],
     install_requires=PACKAGE_REQUIREMENTS,
     extras_require={
         "dev": DEV_REQUIREMENTS,
-        "orbit": ORBIT_REQUIREMENTS,
+        "docs": DOC_REQUIREMENTS,
     },
     version=__version__,
     keywords="machine-learning ai mlflow",
     python_requires=">=3.7",
 )
```

### Comparing `mlflavors-0.1.0/tests/test_orbit_model_export.py` & `mlflavors-0.1.0rc1/tests/test_orbit_model_export.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/tests/test_pyod_model_export.py` & `mlflavors-0.1.0rc1/tests/test_pyod_model_export.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/tests/test_sdv_model_export.py` & `mlflavors-0.1.0rc1/tests/test_sdv_model_export.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/tests/test_sktime_model_export.py` & `mlflavors-0.1.0rc1/tests/test_sktime_model_export.py`

 * *Files identical despite different names*

### Comparing `mlflavors-0.1.0/tests/test_statsforecast_model_export.py` & `mlflavors-0.1.0rc1/tests/test_statsforecast_model_export.py`

 * *Files identical despite different names*

