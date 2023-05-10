# Comparing `tmp/utracto-0.0.7.tar.gz` & `tmp/utracto-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utracto-0.0.7.tar", last modified: Wed May 10 13:27:04 2023, max compression
+gzip compressed data, was "utracto-0.0.8.tar", last modified: Wed May 10 13:46:33 2023, max compression
```

## Comparing `utracto-0.0.7.tar` & `utracto-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:03.960000 utracto-0.0.7/
--rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-05-10 13:27:06.000000 utracto-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 13:27:06.000000 utracto-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1094 2023-05-10 13:04:52.000000 utracto-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:03.970000 utracto-0.0.7/utracto/
--rw-rw-rw-   0        0        0       74 2023-05-10 13:26:44.000000 utracto-0.0.7/utracto/__init__.py
--rw-rw-rw-   0        0        0     2703 2023-05-10 13:26:56.000000 utracto-0.0.7/utracto/core.py
--rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.7/utracto/example.py
--rw-rw-rw-   0        0        0     5822 2023-05-10 13:10:26.000000 utracto-0.0.7/utracto/tracking.py
--rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.7/utracto/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:27:03.970000 utracto-0.0.7/utracto.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-05-10 13:27:04.000000 utracto-0.0.7/utracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-10 13:27:04.000000 utracto-0.0.7/utracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:27:04.000000 utracto-0.0.7/utracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-10 13:27:04.000000 utracto-0.0.7/utracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 13:27:04.000000 utracto-0.0.7/utracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.840000 utracto-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-05-10 13:46:34.000000 utracto-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:46:34.000000 utracto-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-05-10 13:04:52.000000 utracto-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.840000 utracto-0.0.8/utracto/
+-rw-rw-rw-   0        0        0       74 2023-05-10 13:46:14.000000 utracto-0.0.8/utracto/__init__.py
+-rw-rw-rw-   0        0        0     2703 2023-05-10 13:34:02.000000 utracto-0.0.8/utracto/core.py
+-rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.8/utracto/example.py
+-rw-rw-rw-   0        0        0     5822 2023-05-10 13:10:26.000000 utracto-0.0.8/utracto/tracking.py
+-rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.8/utracto/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.850000 utracto-0.0.8/utracto.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/top_level.txt
```

### Comparing `utracto-0.0.7/LICENSE` & `utracto-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `utracto-0.0.7/PKG-INFO` & `utracto-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.7
+Version: 0.0.8
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `utracto-0.0.7/README.md` & `utracto-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `utracto-0.0.7/setup.py` & `utracto-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.7/utracto/core.py` & `utracto-0.0.8/utracto/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 @author: DELINTE Nicolas
 """
 
 import numpy as np
 from scipy.ndimage import gaussian_filter
-from biname.utils import erosion
+from binama.utils import erosion
 
 
 def wmfod_to_angle(wmfod, max_value: int = 30, min_value: int = 15,
                    wm_edge: float = 0.1, interface: float = 0.08,
                    interface_thickness: int = 3, wm_deep=0.35,
                    smooth_factor: float = .85, float_type: bool = False,
                    only_WM: bool = False):
```

### Comparing `utracto-0.0.7/utracto/tracking.py` & `utracto-0.0.8/utracto/tracking.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.7/utracto/utils.py` & `utracto-0.0.8/utracto/utils.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.7/utracto.egg-info/PKG-INFO` & `utracto-0.0.8/utracto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.7
+Version: 0.0.8
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

