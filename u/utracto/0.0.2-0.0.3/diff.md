# Comparing `tmp/utracto-0.0.2.tar.gz` & `tmp/utracto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utracto-0.0.2.tar", last modified: Wed May 10 12:11:22 2023, max compression
+gzip compressed data, was "utracto-0.0.3.tar", last modified: Wed May 10 12:30:00 2023, max compression
```

## Comparing `utracto-0.0.2.tar` & `utracto-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:11:22.710000 utracto-0.0.2/
--rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1603 2023-05-10 12:11:24.000000 utracto-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-10 12:11:24.000000 utracto-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-10 12:10:22.000000 utracto-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:11:22.730000 utracto-0.0.2/utracto/
--rw-rw-rw-   0        0        0       53 2023-05-10 12:10:50.000000 utracto-0.0.2/utracto/__init__.py
--rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.2/utracto/core.py
--rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.2/utracto/example.py
--rw-rw-rw-   0        0        0     7389 2022-12-12 15:25:56.000000 utracto-0.0.2/utracto/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:11:22.730000 utracto-0.0.2/utracto.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-10 12:11:24.000000 utracto-0.0.2/utracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-10 12:11:24.000000 utracto-0.0.2/utracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:11:24.000000 utracto-0.0.2/utracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-10 12:11:24.000000 utracto-0.0.2/utracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 12:11:24.000000 utracto-0.0.2/utracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:00.460000 utracto-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-05-10 12:30:02.000000 utracto-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:30:02.000000 utracto-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-10 12:29:18.000000 utracto-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:00.460000 utracto-0.0.3/utracto/
+-rw-rw-rw-   0        0        0       74 2023-05-10 12:29:10.000000 utracto-0.0.3/utracto/__init__.py
+-rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.3/utracto/core.py
+-rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.3/utracto/example.py
+-rw-rw-rw-   0        0        0     7389 2022-12-12 15:25:56.000000 utracto-0.0.3/utracto/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:00.470000 utracto-0.0.3/utracto.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-05-10 12:30:02.000000 utracto-0.0.3/utracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-10 12:30:02.000000 utracto-0.0.3/utracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:30:02.000000 utracto-0.0.3/utracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 12:30:02.000000 utracto-0.0.3/utracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 12:30:02.000000 utracto-0.0.3/utracto.egg-info/top_level.txt
```

### Comparing `utracto-0.0.2/LICENSE` & `utracto-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utracto-0.0.2/PKG-INFO` & `utracto-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # U-fiber tractography
 
-Welcome to the UTracto's Github repository! 
+Welcome to the UTracto's Github repository!
+
+[![PyPI](https://img.shields.io/pypi/v/utracto?label=pypi%20package)](https://pypi.org/project/utracto/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/utracto)](https://pypi.org/project/utracto/)
+![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/UTracto)
 
 ## Description
 
 This repository contains a package facilitating the tracking of sub-cortical U-Fibers. The main function of this package is the creation of angular maps, enabling a tractography with a position-dependent maximum angle between tractography steps. The function creating these angular maps is `wmfod_to_angle` in the [`core.py`](https://github.com/DelinteNicolas/UTracto/blob/main/utracto/core.py) file.
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/70629561/207111838-6ec3ba60-fd52-47ad-a469-17a29df74513.png" width="600" />
```

### Comparing `utracto-0.0.2/setup.py` & `utracto-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.2/utracto/core.py` & `utracto-0.0.3/utracto/core.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.2/utracto/utils.py` & `utracto-0.0.3/utracto/utils.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.2/utracto.egg-info/PKG-INFO` & `utracto-0.0.3/utracto.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # U-fiber tractography
 
-Welcome to the UTracto's Github repository! 
+Welcome to the UTracto's Github repository!
+
+[![PyPI](https://img.shields.io/pypi/v/utracto?label=pypi%20package)](https://pypi.org/project/utracto/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/utracto)](https://pypi.org/project/utracto/)
+![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/UTracto)
 
 ## Description
 
 This repository contains a package facilitating the tracking of sub-cortical U-Fibers. The main function of this package is the creation of angular maps, enabling a tractography with a position-dependent maximum angle between tractography steps. The function creating these angular maps is `wmfod_to_angle` in the [`core.py`](https://github.com/DelinteNicolas/UTracto/blob/main/utracto/core.py) file.
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/70629561/207111838-6ec3ba60-fd52-47ad-a469-17a29df74513.png" width="600" />
```

