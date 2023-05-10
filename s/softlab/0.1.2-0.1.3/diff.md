# Comparing `tmp/softlab-0.1.2.tar.gz` & `tmp/softlab-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softlab-0.1.2.tar", last modified: Tue May  9 08:44:53 2023, max compression
+gzip compressed data, was "softlab-0.1.3.tar", last modified: Wed May 10 10:09:23 2023, max compression
```

## Comparing `softlab-0.1.2.tar` & `softlab-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.823058 softlab-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-04-06 01:30:34.000000 softlab-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1790 2023-05-09 08:44:53.823058 softlab-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      801 2023-03-20 12:22:50.000000 softlab-0.1.2/README.rst
--rw-rw-rw-   0        0        0     1758 2023-05-09 08:20:36.000000 softlab-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 08:44:53.823058 softlab-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      116 2023-04-06 01:30:25.000000 softlab-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.778086 softlab-0.1.2/softlab/
--rw-rw-rw-   0        0        0        7 2023-04-06 01:33:45.000000 softlab-0.1.2/softlab/VERSION.txt
--rw-rw-rw-   0        0        0      240 2023-04-06 00:57:52.000000 softlab-0.1.2/softlab/__init__.py
--rw-rw-rw-   0        0        0      162 2023-04-06 00:56:55.000000 softlab-0.1.2/softlab/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.798059 softlab-0.1.2/softlab/huo/
--rw-rw-rw-   0        0        0      844 2023-04-06 13:18:20.000000 softlab-0.1.2/softlab/huo/__init__.py
--rw-rw-rw-   0        0        0    16433 2023-04-06 02:03:05.000000 softlab-0.1.2/softlab/huo/impl_scheduler.py
--rw-rw-rw-   0        0        0    22207 2023-04-07 06:51:33.000000 softlab-0.1.2/softlab/huo/process.py
--rw-rw-rw-   0        0        0     5023 2023-03-20 13:26:07.000000 softlab-0.1.2/softlab/huo/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.800058 softlab-0.1.2/softlab/jin/
--rw-rw-rw-   0        0        0      477 2023-04-21 09:58:05.000000 softlab-0.1.2/softlab/jin/__init__.py
--rw-rw-rw-   0        0        0     5366 2023-05-06 07:46:12.000000 softlab-0.1.2/softlab/jin/miscellaneous.py
--rw-rw-rw-   0        0        0    16815 2023-04-23 01:51:47.000000 softlab-0.1.2/softlab/jin/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.801060 softlab-0.1.2/softlab/mu/
--rw-rw-rw-   0        0        0      127 2023-04-06 00:57:38.000000 softlab-0.1.2/softlab/mu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.803058 softlab-0.1.2/softlab/mu/notebooks/
--rw-rw-rw-   0        0        0      420 2023-04-06 01:47:29.000000 softlab-0.1.2/softlab/mu/notebooks/__init__.py
--rw-rw-rw-   0        0        0    29371 2023-04-06 01:45:02.000000 softlab-0.1.2/softlab/mu/notebooks/file_selector.py
--rw-rw-rw-   0        0        0     2087 2023-04-06 03:44:55.000000 softlab-0.1.2/softlab/mu/notebooks/interactive.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.804059 softlab-0.1.2/softlab/mu/services/
--rw-rw-rw-   0        0        0       42 2023-04-06 00:47:11.000000 softlab-0.1.2/softlab/mu/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.805058 softlab-0.1.2/softlab/shui/
--rw-rw-rw-   0        0        0      180 2023-03-24 07:46:43.000000 softlab-0.1.2/softlab/shui/__init__.py
--rw-rw-rw-   0        0        0     6207 2023-03-20 12:22:50.000000 softlab-0.1.2/softlab/shui/backend.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.809057 softlab-0.1.2/softlab/shui/data/
--rw-rw-rw-   0        0        0      358 2023-04-07 01:17:53.000000 softlab-0.1.2/softlab/shui/data/__init__.py
--rw-rw-rw-   0        0        0    20076 2023-04-06 17:00:29.000000 softlab-0.1.2/softlab/shui/data/backend.py
--rw-rw-rw-   0        0        0    20538 2023-04-07 03:02:21.000000 softlab-0.1.2/softlab/shui/data/base.py
--rw-rw-rw-   0        0        0     4138 2023-04-07 06:42:47.000000 softlab-0.1.2/softlab/shui/data/io.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.811058 softlab-0.1.2/softlab/shui/profile/
--rw-rw-rw-   0        0        0      460 2023-03-20 12:41:44.000000 softlab-0.1.2/softlab/shui/profile/__init__.py
--rw-rw-rw-   0        0        0    11738 2023-03-20 13:13:21.000000 softlab-0.1.2/softlab/shui/profile/base.py
--rw-rw-rw-   0        0        0     8581 2023-03-20 13:14:53.000000 softlab-0.1.2/softlab/shui/profile/manage.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.816058 softlab-0.1.2/softlab/tu/
--rw-rw-rw-   0        0        0      634 2023-04-17 10:06:01.000000 softlab-0.1.2/softlab/tu/__init__.py
--rw-rw-rw-   0        0        0    11362 2023-04-23 01:34:28.000000 softlab-0.1.2/softlab/tu/device.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.822059 softlab-0.1.2/softlab/tu/dsp/
--rw-rw-rw-   0        0        0     4152 2023-05-09 02:26:54.000000 softlab-0.1.2/softlab/tu/dsp/__init__.py
--rw-rw-rw-   0        0        0    14217 2023-03-21 06:25:46.000000 softlab-0.1.2/softlab/tu/dsp/base.py
--rw-rw-rw-   0        0        0    12348 2023-05-09 02:05:40.000000 softlab-0.1.2/softlab/tu/dsp/common.py
--rw-rw-rw-   0        0        0     4877 2023-04-20 10:26:25.000000 softlab-0.1.2/softlab/tu/dsp/iq_modulation.py
--rw-rw-rw-   0        0        0     1695 2023-03-21 06:22:09.000000 softlab-0.1.2/softlab/tu/dsp/noise.py
--rw-rw-rw-   0        0        0     3971 2023-03-21 06:25:18.000000 softlab-0.1.2/softlab/tu/dsp/operate.py
--rw-rw-rw-   0        0        0     8952 2023-05-09 02:06:57.000000 softlab-0.1.2/softlab/tu/dsp/window.py
--rw-rw-rw-   0        0        0     3463 2023-03-20 12:22:50.000000 softlab-0.1.2/softlab/tu/helpers.py
--rw-rw-rw-   0        0        0      962 2023-03-20 13:33:02.000000 softlab-0.1.2/softlab/tu/limited_attribute.py
--rw-rw-rw-   0        0        0    11270 2023-04-17 10:04:10.000000 softlab-0.1.2/softlab/tu/parameter.py
--rw-rw-rw-   0        0        0     5091 2023-03-20 12:22:50.000000 softlab-0.1.2/softlab/tu/station.py
--rw-rw-rw-   0        0        0    11857 2023-04-04 07:47:01.000000 softlab-0.1.2/softlab/tu/visa.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:44:53.794088 softlab-0.1.2/softlab.egg-info/
--rw-rw-rw-   0        0        0     1790 2023-05-09 08:44:53.000000 softlab-0.1.2/softlab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-05-09 08:44:53.000000 softlab-0.1.2/softlab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:44:53.000000 softlab-0.1.2/softlab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-06 01:30:52.000000 softlab-0.1.2/softlab.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       97 2023-05-09 08:44:53.000000 softlab-0.1.2/softlab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 08:44:53.000000 softlab-0.1.2/softlab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.535704 softlab-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-06 01:30:34.000000 softlab-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1790 2023-05-10 10:09:23.535704 softlab-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2023-03-20 12:22:50.000000 softlab-0.1.3/README.rst
+-rw-rw-rw-   0        0        0     1726 2023-05-10 10:05:57.000000 softlab-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:09:23.536702 softlab-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      116 2023-04-06 01:30:25.000000 softlab-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.486643 softlab-0.1.3/softlab/
+-rw-rw-rw-   0        0        0        7 2023-05-10 10:08:54.000000 softlab-0.1.3/softlab/VERSION.txt
+-rw-rw-rw-   0        0        0      240 2023-04-06 00:57:52.000000 softlab-0.1.3/softlab/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-04-06 00:56:55.000000 softlab-0.1.3/softlab/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.510192 softlab-0.1.3/softlab/huo/
+-rw-rw-rw-   0        0        0      844 2023-04-06 13:18:20.000000 softlab-0.1.3/softlab/huo/__init__.py
+-rw-rw-rw-   0        0        0    16433 2023-04-06 02:03:05.000000 softlab-0.1.3/softlab/huo/impl_scheduler.py
+-rw-rw-rw-   0        0        0    22207 2023-04-07 06:51:33.000000 softlab-0.1.3/softlab/huo/process.py
+-rw-rw-rw-   0        0        0     5023 2023-03-20 13:26:07.000000 softlab-0.1.3/softlab/huo/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.512193 softlab-0.1.3/softlab/jin/
+-rw-rw-rw-   0        0        0      477 2023-04-21 09:58:05.000000 softlab-0.1.3/softlab/jin/__init__.py
+-rw-rw-rw-   0        0        0     5366 2023-05-06 07:46:12.000000 softlab-0.1.3/softlab/jin/miscellaneous.py
+-rw-rw-rw-   0        0        0    16815 2023-04-23 01:51:47.000000 softlab-0.1.3/softlab/jin/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.513192 softlab-0.1.3/softlab/mu/
+-rw-rw-rw-   0        0        0      127 2023-04-06 00:57:38.000000 softlab-0.1.3/softlab/mu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.515193 softlab-0.1.3/softlab/mu/notebooks/
+-rw-rw-rw-   0        0        0      420 2023-04-06 01:47:29.000000 softlab-0.1.3/softlab/mu/notebooks/__init__.py
+-rw-rw-rw-   0        0        0    29371 2023-04-06 01:45:02.000000 softlab-0.1.3/softlab/mu/notebooks/file_selector.py
+-rw-rw-rw-   0        0        0     2087 2023-04-06 03:44:55.000000 softlab-0.1.3/softlab/mu/notebooks/interactive.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.516193 softlab-0.1.3/softlab/mu/services/
+-rw-rw-rw-   0        0        0       42 2023-04-06 00:47:11.000000 softlab-0.1.3/softlab/mu/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.518193 softlab-0.1.3/softlab/shui/
+-rw-rw-rw-   0        0        0      180 2023-03-24 07:46:43.000000 softlab-0.1.3/softlab/shui/__init__.py
+-rw-rw-rw-   0        0        0     6207 2023-03-20 12:22:50.000000 softlab-0.1.3/softlab/shui/backend.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.521193 softlab-0.1.3/softlab/shui/data/
+-rw-rw-rw-   0        0        0      358 2023-04-07 01:17:53.000000 softlab-0.1.3/softlab/shui/data/__init__.py
+-rw-rw-rw-   0        0        0    20076 2023-04-06 17:00:29.000000 softlab-0.1.3/softlab/shui/data/backend.py
+-rw-rw-rw-   0        0        0    20538 2023-04-07 03:02:21.000000 softlab-0.1.3/softlab/shui/data/base.py
+-rw-rw-rw-   0        0        0     4138 2023-04-07 06:42:47.000000 softlab-0.1.3/softlab/shui/data/io.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.523696 softlab-0.1.3/softlab/shui/profile/
+-rw-rw-rw-   0        0        0      460 2023-03-20 12:41:44.000000 softlab-0.1.3/softlab/shui/profile/__init__.py
+-rw-rw-rw-   0        0        0    11738 2023-03-20 13:13:21.000000 softlab-0.1.3/softlab/shui/profile/base.py
+-rw-rw-rw-   0        0        0     8581 2023-03-20 13:14:53.000000 softlab-0.1.3/softlab/shui/profile/manage.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.528703 softlab-0.1.3/softlab/tu/
+-rw-rw-rw-   0        0        0      634 2023-04-17 10:06:01.000000 softlab-0.1.3/softlab/tu/__init__.py
+-rw-rw-rw-   0        0        0    11362 2023-04-23 01:34:28.000000 softlab-0.1.3/softlab/tu/device.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.534702 softlab-0.1.3/softlab/tu/dsp/
+-rw-rw-rw-   0        0        0     4152 2023-05-09 02:26:54.000000 softlab-0.1.3/softlab/tu/dsp/__init__.py
+-rw-rw-rw-   0        0        0    14217 2023-03-21 06:25:46.000000 softlab-0.1.3/softlab/tu/dsp/base.py
+-rw-rw-rw-   0        0        0    12348 2023-05-09 02:05:40.000000 softlab-0.1.3/softlab/tu/dsp/common.py
+-rw-rw-rw-   0        0        0     4877 2023-04-20 10:26:25.000000 softlab-0.1.3/softlab/tu/dsp/iq_modulation.py
+-rw-rw-rw-   0        0        0     1695 2023-03-21 06:22:09.000000 softlab-0.1.3/softlab/tu/dsp/noise.py
+-rw-rw-rw-   0        0        0     3971 2023-03-21 06:25:18.000000 softlab-0.1.3/softlab/tu/dsp/operate.py
+-rw-rw-rw-   0        0        0     8952 2023-05-09 02:06:57.000000 softlab-0.1.3/softlab/tu/dsp/window.py
+-rw-rw-rw-   0        0        0     3463 2023-03-20 12:22:50.000000 softlab-0.1.3/softlab/tu/helpers.py
+-rw-rw-rw-   0        0        0      962 2023-03-20 13:33:02.000000 softlab-0.1.3/softlab/tu/limited_attribute.py
+-rw-rw-rw-   0        0        0    11270 2023-04-17 10:04:10.000000 softlab-0.1.3/softlab/tu/parameter.py
+-rw-rw-rw-   0        0        0     5091 2023-03-20 12:22:50.000000 softlab-0.1.3/softlab/tu/station.py
+-rw-rw-rw-   0        0        0    11857 2023-04-04 07:47:01.000000 softlab-0.1.3/softlab/tu/visa.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:23.506211 softlab-0.1.3/softlab.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-05-10 10:09:23.000000 softlab-0.1.3/softlab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-05-10 10:09:23.000000 softlab-0.1.3/softlab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:09:23.000000 softlab-0.1.3/softlab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-06 01:30:52.000000 softlab-0.1.3/softlab.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       81 2023-05-10 10:09:23.000000 softlab-0.1.3/softlab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 10:09:23.000000 softlab-0.1.3/softlab.egg-info/top_level.txt
```

### Comparing `softlab-0.1.2/LICENSE` & `softlab-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/PKG-INFO` & `softlab-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolkit to build software-defined laboratory
 Author-email: Edward Chou <prettyage.new@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/hoolheart/softlab
 Keywords: science,laboratory,toolkit
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `softlab-0.1.2/README.rst` & `softlab-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/pyproject.toml` & `softlab-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,16 @@
     "plotly",
     "numpy",
     "scipy",
     "pandas",
     "imageio",
     "ipywidgets",
     "pyvisa",
-    "logging",
     "uuid",
     "h5py",
-    "sqlite3",
     "asyncio",
 ]
 
 [project.urls]
 Homepage = "https://github.com/hoolheart/softlab"
 
 [tool.setuptools]
```

### Comparing `softlab-0.1.2/softlab/huo/__init__.py` & `softlab-0.1.3/softlab/huo/__init__.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/huo/impl_scheduler.py` & `softlab-0.1.3/softlab/huo/impl_scheduler.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/huo/process.py` & `softlab-0.1.3/softlab/huo/process.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/huo/scheduler.py` & `softlab-0.1.3/softlab/huo/scheduler.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/jin/miscellaneous.py` & `softlab-0.1.3/softlab/jin/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/jin/validator.py` & `softlab-0.1.3/softlab/jin/validator.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/mu/notebooks/file_selector.py` & `softlab-0.1.3/softlab/mu/notebooks/file_selector.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/mu/notebooks/interactive.py` & `softlab-0.1.3/softlab/mu/notebooks/interactive.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/backend.py` & `softlab-0.1.3/softlab/shui/backend.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/data/backend.py` & `softlab-0.1.3/softlab/shui/data/backend.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/data/base.py` & `softlab-0.1.3/softlab/shui/data/base.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/data/io.py` & `softlab-0.1.3/softlab/shui/data/io.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/profile/base.py` & `softlab-0.1.3/softlab/shui/profile/base.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/shui/profile/manage.py` & `softlab-0.1.3/softlab/shui/profile/manage.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/__init__.py` & `softlab-0.1.3/softlab/tu/__init__.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/device.py` & `softlab-0.1.3/softlab/tu/device.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/__init__.py` & `softlab-0.1.3/softlab/tu/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/base.py` & `softlab-0.1.3/softlab/tu/dsp/base.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/common.py` & `softlab-0.1.3/softlab/tu/dsp/common.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/iq_modulation.py` & `softlab-0.1.3/softlab/tu/dsp/iq_modulation.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/noise.py` & `softlab-0.1.3/softlab/tu/dsp/noise.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/operate.py` & `softlab-0.1.3/softlab/tu/dsp/operate.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/dsp/window.py` & `softlab-0.1.3/softlab/tu/dsp/window.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/helpers.py` & `softlab-0.1.3/softlab/tu/helpers.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/limited_attribute.py` & `softlab-0.1.3/softlab/tu/limited_attribute.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/parameter.py` & `softlab-0.1.3/softlab/tu/parameter.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/station.py` & `softlab-0.1.3/softlab/tu/station.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab/tu/visa.py` & `softlab-0.1.3/softlab/tu/visa.py`

 * *Files identical despite different names*

### Comparing `softlab-0.1.2/softlab.egg-info/PKG-INFO` & `softlab-0.1.3/softlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softlab
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolkit to build software-defined laboratory
 Author-email: Edward Chou <prettyage.new@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/hoolheart/softlab
 Keywords: science,laboratory,toolkit
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `softlab-0.1.2/softlab.egg-info/SOURCES.txt` & `softlab-0.1.3/softlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

