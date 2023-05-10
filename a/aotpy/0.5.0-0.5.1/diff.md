# Comparing `tmp/aotpy-0.5.0.tar.gz` & `tmp/aotpy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.5.0.tar", last modified: Tue May  2 23:06:33 2023, max compression
+gzip compressed data, was "aotpy-0.5.1.tar", last modified: Wed May 10 15:48:30 2023, max compression
```

## Comparing `aotpy-0.5.0.tar` & `aotpy-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.643905 aotpy-0.5.0/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2991 2023-05-02 23:06:33.643905 aotpy-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.574897 aotpy-0.5.0/aotpy/
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.606175 aotpy-0.5.0/aotpy/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2991 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.621804 aotpy-0.5.0/aotpy/core/
--rw-rw-rw-   0        0        0      580 2023-04-19 14:10:55.000000 aotpy-0.5.0/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.5.0/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     3945 2023-05-02 11:25:41.000000 aotpy-0.5.0/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     2227 2023-05-02 09:36:11.000000 aotpy-0.5.0/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0      675 2023-05-02 18:16:26.000000 aotpy-0.5.0/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1177 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/core/geometry.py
--rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.5.0/aotpy/core/image.py
--rw-rw-rw-   0        0        0     4706 2023-05-02 09:40:01.000000 aotpy-0.5.0/aotpy/core/loop.py
--rw-rw-rw-   0        0        0     8912 2023-05-02 18:10:07.000000 aotpy-0.5.0/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.5.0/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4059 2023-05-02 18:40:18.000000 aotpy-0.5.0/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.5.0/aotpy/core/time.py
--rw-rw-rw-   0        0        0     2728 2023-05-02 09:43:55.000000 aotpy-0.5.0/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.621804 aotpy-0.5.0/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.5.0/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.5.0/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.637398 aotpy-0.5.0/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.5.0/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    27403 2023-05-02 18:52:02.000000 aotpy-0.5.0/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    43200 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     8853 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31196 2023-05-02 18:26:21.000000 aotpy-0.5.0/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.643905 aotpy-0.5.0/aotpy/translators/
--rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.5.0/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0    11807 2023-05-02 17:53:53.000000 aotpy-0.5.0/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.5.0/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7404 2023-05-02 17:56:25.000000 aotpy-0.5.0/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0     8553 2023-05-02 18:43:53.000000 aotpy-0.5.0/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0     6487 2023-05-02 17:55:46.000000 aotpy-0.5.0/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0     1024 2023-05-02 23:06:33.643905 aotpy-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.018127 aotpy-0.5.1/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2991 2023-05-10 15:48:30.018127 aotpy-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.936101 aotpy-0.5.1/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.5.1/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.965396 aotpy-0.5.1/aotpy/core/
+-rw-rw-rw-   0        0        0      580 2023-04-19 14:10:55.000000 aotpy-0.5.1/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.5.1/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.5.1/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     2227 2023-05-02 09:36:11.000000 aotpy-0.5.1/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.5.1/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1177 2023-05-02 18:40:00.000000 aotpy-0.5.1/aotpy/core/geometry.py
+-rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.5.1/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     4706 2023-05-02 09:40:01.000000 aotpy-0.5.1/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0     8912 2023-05-02 18:10:07.000000 aotpy-0.5.1/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.5.1/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4059 2023-05-02 18:40:18.000000 aotpy-0.5.1/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.5.1/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     2728 2023-05-02 09:43:55.000000 aotpy-0.5.1/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.967349 aotpy-0.5.1/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.5.1/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.5.1/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.008363 aotpy-0.5.1/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.5.1/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    27401 2023-05-03 11:20:21.000000 aotpy-0.5.1/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    43132 2023-05-03 10:32:11.000000 aotpy-0.5.1/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.5.1/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31576 2023-05-03 10:58:25.000000 aotpy-0.5.1/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.015198 aotpy-0.5.1/aotpy/translators/
+-rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.5.1/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0    11862 2023-05-03 11:33:12.000000 aotpy-0.5.1/aotpy/translators/aof.py
+-rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.5.1/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7404 2023-05-02 17:56:25.000000 aotpy-0.5.1/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0     8553 2023-05-02 18:43:53.000000 aotpy-0.5.1/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0     6487 2023-05-02 17:55:46.000000 aotpy-0.5.1/aotpy/translators/naomi.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.950748 aotpy-0.5.1/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2991 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.017151 aotpy-0.5.1/data/
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.5.1/data/__init__.py
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      982 2023-05-10 15:48:30.020080 aotpy-0.5.1/setup.cfg
```

### Comparing `aotpy-0.5.0/LICENSE` & `aotpy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/PKG-INFO` & `aotpy-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.5.0/README.md` & `aotpy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/aotpy.egg-info/PKG-INFO` & `aotpy-0.5.1/aotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.5.0/aotpy/aotpy.egg-info/SOURCES.txt` & `aotpy-0.5.1/aotpy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-aotpy/aotpy.egg-info/PKG-INFO
-aotpy/aotpy.egg-info/SOURCES.txt
-aotpy/aotpy.egg-info/dependency_links.txt
-aotpy/aotpy.egg-info/requires.txt
-aotpy/aotpy.egg-info/top_level.txt
+aotpy/__init__.py
+aotpy.egg-info/PKG-INFO
+aotpy.egg-info/SOURCES.txt
+aotpy.egg-info/dependency_links.txt
+aotpy.egg-info/requires.txt
+aotpy.egg-info/top_level.txt
 aotpy/core/__init__.py
 aotpy/core/aberration.py
 aotpy/core/ao_system.py
 aotpy/core/atmosphere.py
 aotpy/core/base.py
 aotpy/core/geometry.py
 aotpy/core/image.py
@@ -28,8 +29,9 @@
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
 aotpy/translators/__init__.py
 aotpy/translators/aof.py
 aotpy/translators/base.py
 aotpy/translators/ciao.py
 aotpy/translators/eso.py
-aotpy/translators/naomi.py
+aotpy/translators/naomi.py
+data/__init__.py
```

### Comparing `aotpy-0.5.0/aotpy/core/__init__.py` & `aotpy-0.5.1/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/aberration.py` & `aotpy-0.5.1/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/ao_system.py` & `aotpy-0.5.1/aotpy/core/ao_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     wavefront_correctors: list[WavefrontCorrector] = field(default_factory=list)
     """List of all wavefront correctors in the system."""
 
     loops: list[Loop] = field(default_factory=list)
     """List of all loops in the system."""
 
-    def write_to_file(self, filename: str | os.PathLike, **kwargs):
+    def write_to_file(self, filename: str | os.PathLike, **kwargs) -> None:
         """
         Writes `AOSystem` to a file. The writing function is deduced by the extension in the specified `filename`.
 
         Parameters
         ----------
         filename
             Path to the file to be written.
@@ -82,15 +82,15 @@
             WriterClass = _AVAILABLE_WRITERS[ext.lower()]
         except KeyError:
             raise ValueError(f"No available writer for extension '{ext}'. "
                              f"Available extensions: {str(list(_AVAILABLE_WRITERS.keys()))[1:-1]}")
         WriterClass(self).write(filename, **kwargs)
 
     @staticmethod
-    def read_from_file(filename: str | os.PathLike, **kwargs):
+    def read_from_file(filename: str | os.PathLike, **kwargs) -> 'AOSystem':
         """
         Reads `AOSystem` from a file. The reading function is deduced by the extension in the specified `filename`.
 
         Parameters
         ----------
         filename
             Path to the file to be read.
```

### Comparing `aotpy-0.5.0/aotpy/core/atmosphere.py` & `aotpy-0.5.1/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/base.py` & `aotpy-0.5.1/aotpy/core/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 This module contains a classes used as a base for the rest of the core of aotpy.
 """
 
 from collections import namedtuple
-from collections.abc import MutableSequence, Collection
 from dataclasses import dataclass
 
 __all__ = ['Referenceable', 'Coordinates']
 
 Coordinates = namedtuple('Coordinates', 'x y')
```

### Comparing `aotpy-0.5.0/aotpy/core/geometry.py` & `aotpy-0.5.1/aotpy/core/geometry.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/image.py` & `aotpy-0.5.1/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/loop.py` & `aotpy-0.5.1/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/optical_sensor.py` & `aotpy-0.5.1/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/source.py` & `aotpy-0.5.1/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/telescope.py` & `aotpy-0.5.1/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/time.py` & `aotpy-0.5.1/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/core/wavefront_corrector.py` & `aotpy-0.5.1/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/io/base.py` & `aotpy-0.5.1/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/io/fits/_keywords.py` & `aotpy-0.5.1/aotpy/io/fits/_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains data that defines the AOT FITS format itself, including the specific FITS keywords and tables used.
 Not meant to be imported by users.
 """
 
 import re
 from dataclasses import dataclass
 
-CURRENT_AOT_VERSION = '0.5.0'
+CURRENT_AOT_VERSION = '0.5'
 
 
 @dataclass
 class AOTField:
     name: str
     format: str
     unit: str
```

### Comparing `aotpy-0.5.0/aotpy/io/fits/reader.py` & `aotpy-0.5.1/aotpy/io/fits/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,14 @@
 
 
 class FITSReader(SystemReader):
     def _initialize_data(self) -> None:
         """
         Initialize data structures necessary for reading the file.
         """
-        self._primary_header: fits.Header = None
-        self._system: aotpy.AOSystem = None
-
         self._images: dict[str, list] = {}
         self._time: dict[str, list] = {}
         self._geometries: dict[str, list] = {}
         self._aberrations: dict[str, list] = {}
         self._telescopes: dict[str, list] = {}
         self._sources: dict[str, list] = {}
         self._detectors: dict[str, list] = {}
@@ -108,16 +105,16 @@
         self._extra_header: list[fits.Card] = []
         self._extra_hdus: fits.HDUList = fits.HDUList()
         self._extra_columns: dict[str, list[fits.Column]] = {}
         self._extra_objects: list[aotpy.Referenceable] = []
 
     def _read(self, **kwargs) -> tuple[aotpy.AOSystem, list]:
         with fits.open(self._filename, **kwargs) as hdus:
-            self._primary_header = hdus[0].header
-            self._system = self._check_header()
+            self._primary_header: fits.Header = hdus[0].header
+            self._system: aotpy.AOSystem = self._check_header()
 
             if hdus[0].data is not None:
                 raise ValueError('Primary HDU must have no data.')
             for table in kw.MANDATORY_TABLE_SET:
                 if table not in hdus:
                     raise ValueError(f"Missing mandatory binary table '{table}'.")
```

### Comparing `aotpy-0.5.0/aotpy/io/fits/utils.py` & `aotpy-0.5.1/aotpy/io/fits/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,16 +113,14 @@
 
     Parameters
     ----------
     hdus
         List of HDUs from which `Image` is to be extracted.
     index: int, optional
         Index of the HDU that contains the image data. If omitted, the first HDU containing image data is assumed.
-    **kwargs
-        Keyword arguments passed on as options to the file handling function.
     """
     name, data, unit, _time, metadata = _get_image_fields_from_hdus(hdus, index)
     image = aotpy.Image(name=name, data=data, unit=unit, metadata=metadata)
     image._time = _time
     return image
```

### Comparing `aotpy-0.5.0/aotpy/io/fits/writer.py` & `aotpy-0.5.1/aotpy/io/fits/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,32 @@
     FITSWriter(system).write(filename, **kwargs)
 
 
 class FITSWriter(SystemWriter):
     def __init__(self, system: aotpy.AOSystem) -> None:
         self._system = system
 
-        self._tables: dict[str, dict[str, tuple[object, dict[str, object]]]] = {}
+        self._tables: dict[str, dict[
+            str, tuple[aotpy.Referenceable, dict[str, numbers.Integral | numbers.Real | list | np.ndarray | str]]]] = {}
+        """The outer dictionary converts from table name to the table dictionary. The table dictionary converts from the
+        object uid to a tuple. This tuple contains the object itself and a dictionary that converts from the field names
+        to the values present in the object."""
 
         self._images: dict[str, aotpy.Image] = {}
 
         self._handle_data()
 
         primary_hdu = self._create_primary_hdu()
         bintable_hdus = self._create_bintable_hdus()
         image_hdus = self._create_image_hdus()
         self._hdus = fits.HDUList([primary_hdu, *bintable_hdus, *image_hdus])
 
     def write(self, filename: str | os.PathLike, **kwargs) -> None:
         self.get_hdus().writeto(filename, **kwargs)
-    
+
     def get_hdus(self) -> fits.HDUList:
         """
         Get the list of HDUs that compose the AOT FITS file for the initialized system.
         Returns
         -------
             `HDUList` that composes the AOT FITS file for the initialized system.
         """
@@ -141,15 +145,16 @@
                 raise NotImplementedError
 
             converted[field.name] = value
 
         table[obj.uid] = (obj, converted)
         return True
 
-    def _create_row_reference(self, uid: str) -> str:
+    @staticmethod
+    def _create_row_reference(uid: str) -> str:
         return f'{kw.ROW_REFERENCE}<{uid}>'
 
     def _handle_time(self, time: aotpy.Time) -> str | None:
         if time is None:
             return None
         if time.timestamps and time.frame_numbers and len(time.timestamps) != len(time.frame_numbers):
             raise ValueError(f"Error in Time '{time.uid}': If both 'timestamps' and 'frame_numbers' are non-null, they"
```

### Comparing `aotpy-0.5.0/aotpy/translators/aof.py` & `aotpy-0.5.1/aotpy/translators/aof.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         self.system.date_beginning = datetime.utcfromtimestamp(lgs_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(lgs_timestamps[-1])
         lgs_frame_numbers = lgs_loop_frame['FrameCounter']
         lgs_time = aotpy.Time('LGS Loop Time', timestamps=lgs_timestamps.tolist(),
                               frame_numbers=lgs_frame_numbers.tolist())
 
         aof_data_path = importlib.resources.files('data') / 'AOF'
-        subaperture_mask = image_from_file(aof_data_path / 'subap.fits')
+        with importlib.resources.as_file(aof_data_path / 'subap.fits') as p:
+            subaperture_mask = image_from_file(p)
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         dsm_positions = aotpy.Image('DSM_positions', lgs_loop_frame['DSM_Positions'][:, self.dsm_valid])
         m2c = image_from_file(path_lgs / 'LGSCtr.ACT_POS_MODAL_PROJECTION.fits')
         lgs_tfz_num = aotpy.Image('LGSCtr.A_TERMS', fits.getdata(path_lgs / 'LGSCtr.A_TERMS.fits').T)
         lgs_tfz_den = aotpy.Image('LGSCtr.B_TERMS', fits.getdata(path_lgs / 'LGSCtr.B_TERMS.fits').T)
         jit_tfz_num = fits.getdata(path_lgs / 'JitCtr.A_TERMS.fits').T
```

### Comparing `aotpy-0.5.0/aotpy/translators/base.py` & `aotpy-0.5.1/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/translators/ciao.py` & `aotpy-0.5.1/aotpy/translators/ciao.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/translators/eso.py` & `aotpy-0.5.1/aotpy/translators/eso.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/aotpy/translators/naomi.py` & `aotpy-0.5.1/aotpy/translators/naomi.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.0/setup.cfg` & `aotpy-0.5.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 352e 300d 0a61 7574 686f  n = 0.5.0..autho
+00000020: 6e20 3d20 302e 352e 310d 0a61 7574 686f  n = 0.5.1..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
@@ -41,24 +41,22 @@
 00000280: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 00000290: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
 000002a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
 000002b0: 332e 3130 0d0a 696e 7374 616c 6c5f 7265  3.10..install_re
 000002c0: 7175 6972 6573 203d 200d 0a09 6173 7472  quires = ...astr
 000002d0: 6f70 793e 3d35 2e31 2e31 0d0a 096e 756d  opy>=5.1.1...num
 000002e0: 7079 3e3d 312e 3230 0d0a 0d0a 5b6f 7074  py>=1.20....[opt
-000002f0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000300: 6e64 5d0d 0a77 6865 7265 203d 2061 6f74  nd]..where = aot
-00000310: 7079 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  py....[options.p
-00000320: 6163 6b61 6765 5f64 6174 615d 0d0a 6461  ackage_data]..da
-00000330: 7461 203d 202a 2e66 6974 730d 0a0d 0a5b  ta = *.fits....[
-00000340: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
-00000350: 6571 7569 7265 5d0d 0a65 736f 6172 6368  equire]..esoarch
-00000360: 6976 6520 3d20 0d0a 0970 7976 6f3e 3d31  ive = ...pyvo>=1
-00000370: 2e34 0d0a 7361 7666 696c 6573 203d 200d  .4..savfiles = .
-00000380: 0a09 7363 6970 793e 3d31 2e33 0d0a 646f  ..scipy>=1.3..do
-00000390: 6373 203d 200d 0a09 7370 6869 6e78 0d0a  cs = ...sphinx..
-000003a0: 0973 7068 696e 782d 7274 642d 7468 656d  .sphinx-rtd-them
-000003b0: 650d 0a61 6c6c 203d 200d 0a09 7079 766f  e..all = ...pyvo
-000003c0: 3e3d 312e 340d 0a09 7363 6970 793e 3d31  >=1.4...scipy>=1
-000003d0: 2e33 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .3....[egg_info]
-000003e0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000003f0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000002f0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+00000300: 615d 0d0a 6461 7461 203d 202a 2e66 6974  a]..data = *.fit
+00000310: 730d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  s....[options.ex
+00000320: 7472 6173 5f72 6571 7569 7265 5d0d 0a65  tras_require]..e
+00000330: 736f 6172 6368 6976 6520 3d20 0d0a 0970  soarchive = ...p
+00000340: 7976 6f3e 3d31 2e34 0d0a 7361 7666 696c  yvo>=1.4..savfil
+00000350: 6573 203d 200d 0a09 7363 6970 793e 3d31  es = ...scipy>=1
+00000360: 2e33 0d0a 646f 6373 203d 200d 0a09 7370  .3..docs = ...sp
+00000370: 6869 6e78 0d0a 0973 7068 696e 782d 7274  hinx...sphinx-rt
+00000380: 642d 7468 656d 650d 0a61 6c6c 203d 200d  d-theme..all = .
+00000390: 0a09 7079 766f 3e3d 312e 340d 0a09 7363  ..pyvo>=1.4...sc
+000003a0: 6970 793e 3d31 2e33 0d0a 0d0a 5b65 6767  ipy>=1.3....[egg
+000003b0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000003c0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000003d0: 2030 0d0a 0d0a                            0....
```

