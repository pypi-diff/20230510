# Comparing `tmp/earthquakereport-indonesia-0.1.3.tar.gz` & `tmp/earthquakereport-indonesia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthquakereport-indonesia-0.1.3.tar", last modified: Fri May  5 09:12:15 2023, max compression
+gzip compressed data, was "earthquakereport-indonesia-0.1.4.tar", last modified: Wed May 10 14:57:42 2023, max compression
```

## Comparing `earthquakereport-indonesia-0.1.3.tar` & `earthquakereport-indonesia-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.842114 earthquakereport-indonesia-0.1.3/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.3/LICENSE
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-05 09:12:15.841737 earthquakereport-indonesia-0.1.3/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      596 2023-05-04 09:24:44.000000 earthquakereport-indonesia-0.1.3/README.md
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.839984 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/PKG-INFO
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/SOURCES.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/dependency_links.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-05 09:12:15.000000 earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/top_level.txt
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-05 09:12:15.842225 earthquakereport-indonesia-0.1.3/setup.cfg
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-05 07:53:04.000000 earthquakereport-indonesia-0.1.3/setup.py
-drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-05 09:12:15.840650 earthquakereport-indonesia-0.1.3/updateGempa/
--rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     2540 2023-05-05 07:41:53.000000 earthquakereport-indonesia-0.1.3/updateGempa/__init__.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-10 14:57:42.602986 earthquakereport-indonesia-0.1.4/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)    35149 2023-05-04 09:21:22.000000 earthquakereport-indonesia-0.1.4/LICENSE
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-10 14:57:42.602709 earthquakereport-indonesia-0.1.4/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      596 2023-05-04 09:24:44.000000 earthquakereport-indonesia-0.1.4/README.md
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-10 14:57:42.601811 earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1233 2023-05-10 14:57:42.000000 earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/PKG-INFO
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)      250 2023-05-10 14:57:42.000000 earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)        1 2023-05-10 14:57:42.000000 earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       12 2023-05-10 14:57:42.000000 earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/top_level.txt
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)       38 2023-05-10 14:57:42.603068 earthquakereport-indonesia-0.1.4/setup.cfg
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     1018 2023-05-10 14:48:47.000000 earthquakereport-indonesia-0.1.4/setup.py
+drwxr-xr-x   0 hasanrachmatullah   (501) staff       (20)        0 2023-05-10 14:57:42.602253 earthquakereport-indonesia-0.1.4/updateGempa/
+-rw-r--r--   0 hasanrachmatullah   (501) staff       (20)     3900 2023-05-10 14:38:51.000000 earthquakereport-indonesia-0.1.4/updateGempa/__init__.py
```

### Comparing `earthquakereport-indonesia-0.1.3/LICENSE` & `earthquakereport-indonesia-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.3/PKG-INFO` & `earthquakereport-indonesia-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `earthquakereport-indonesia-0.1.3/README.md` & `earthquakereport-indonesia-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `earthquakereport-indonesia-0.1.3/earthquakereport_indonesia.egg-info/PKG-INFO` & `earthquakereport-indonesia-0.1.4/earthquakereport_indonesia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakereport-indonesia
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package will provide the most update of Indonesian bureau of Forecast (BMKG)
 Home-page: https://github.com/ganirh0612/indonesiaEarthquakeReport
 Author: Hasan Gani
 Author-email: ganirh0612@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `earthquakereport-indonesia-0.1.3/setup.py` & `earthquakereport-indonesia-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="earthquakereport-indonesia",
-    version="0.1.3",
+    version="0.1.4",
     author="Hasan Gani",
     author_email="ganirh0612@gmail.com",
     description="This package will provide the most update of Indonesian bureau of Forecast (BMKG)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ganirh0612/indonesiaEarthquakeReport",
     project_urls={
```

