# Comparing `tmp/solarkit-0.1.1.tar.gz` & `tmp/solarkit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarkit-0.1.1.tar", last modified: Mon May  8 17:31:06 2023, max compression
+gzip compressed data, was "solarkit-0.1.5.tar", last modified: Wed May 10 20:05:22 2023, max compression
```

## Comparing `solarkit-0.1.1.tar` & `solarkit-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.176398 solarkit-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2003 2023-05-08 17:31:06.175897 solarkit-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-05-08 17:28:30.000000 solarkit-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 17:31:06.176398 solarkit-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1053 2023-05-08 17:30:45.000000 solarkit-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.168896 solarkit-0.1.1/solarkit/
--rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-0.1.1/solarkit/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1.1/solarkit/planet.py
--rw-rw-rw-   0        0        0     2876 2023-05-08 17:27:06.000000 solarkit-0.1.1/solarkit/solar_system.py
--rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-0.1.1/solarkit/utils.py
--rw-rw-rw-   0        0        0    11976 2023-05-08 17:27:06.000000 solarkit-0.1.1/solarkit/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:31:06.173897 solarkit-0.1.1/solarkit.egg-info/
--rw-rw-rw-   0        0        0     2003 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 17:31:06.000000 solarkit-0.1.1/solarkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.919225 solarkit-0.1.5/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2003 2023-05-10 20:05:22.918723 solarkit-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-05-08 17:28:30.000000 solarkit-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 20:05:22.919726 solarkit-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2023-05-10 20:04:38.000000 solarkit-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.912225 solarkit-0.1.5/solarkit/
+-rw-rw-rw-   0        0        0      290 2023-05-08 17:26:35.000000 solarkit-0.1.5/solarkit/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1.5/solarkit/planet.py
+-rw-rw-rw-   0        0        0     2876 2023-05-08 17:27:06.000000 solarkit-0.1.5/solarkit/solar_system.py
+-rw-rw-rw-   0        0        0     2099 2023-05-08 17:26:57.000000 solarkit-0.1.5/solarkit/utils.py
+-rw-rw-rw-   0        0        0    12598 2023-05-10 20:02:59.000000 solarkit-0.1.5/solarkit/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:05:22.917224 solarkit-0.1.5/solarkit.egg-info/
+-rw-rw-rw-   0        0        0     2003 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 20:05:22.000000 solarkit-0.1.5/solarkit.egg-info/top_level.txt
```

### Comparing `solarkit-0.1.1/LICENSE` & `solarkit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.1/PKG-INFO` & `solarkit-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1.1
+Version: 0.1.5
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solarkit-0.1.1/README.md` & `solarkit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.1/setup.py` & `solarkit-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.1"
+VERSION = "0.1.5"
 DESCRIPTION = "Visualise a solar system and do cool stuff with it"
 
 # Setting up
 setup(
     name="solarkit",
     version=VERSION,
     author="Carlos Lorenzo",
```

### Comparing `solarkit-0.1.1/solarkit/planet.py` & `solarkit-0.1.5/solarkit/planet.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.1/solarkit/solar_system.py` & `solarkit-0.1.5/solarkit/solar_system.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.1/solarkit/utils.py` & `solarkit-0.1.5/solarkit/utils.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.1.1/solarkit/viewer.py` & `solarkit-0.1.5/solarkit/viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict
 import os
+from io import StringIO
 
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 
 from solarkit.solar_system import Solar_System
 from solarkit.planet import Planet
 
 
@@ -75,22 +77,27 @@
             
             #set aspect ratio to 1
             RATIO = 1.0
             x_left, x_right = self.ax.get_xlim()
             y_low, y_high = self.ax.get_ylim()
             self.ax.set_aspect(abs((x_right - x_left)/(y_low - y_high)) * RATIO)
     
+    def server_mode(self) -> None:
+        """
+        Allow matplotlib to work when not in main thread (when running in server) 
+        """
+        matplotlib.use("Agg")
     
-    def add_grid(self):
+    def add_grid(self) -> None:
         """
         Adds a grid
         """
         plt.grid()
     
-    def add_legend(self):
+    def add_legend(self) -> None:
         """
         Adds a legend
         """
         plt.legend()
     
     def lable_axes(self, x_lable: str = " x (AU)", y_lable: str = "y (AU)", z_lable: str = "z (AU)"):
         """
@@ -110,28 +117,43 @@
     def show_plot(self):
         """
         Show drawn figure (calls plt.show())
         """
         plt.show()
     
     def save_figure(self, path: str, filename: str) -> None:
-        """_summary_
+        """
+        Save figure as image
 
         Args:
             path (str): directory where the image will be stored
             filename (str): name of image
         """
         
 
         if not os.path.exists(path):
             os.mkdir(path)
         
         plt.savefig(f"{path}/{filename}", dpi=250)
         
-          
+    def get_figure_data(self) -> str:
+        """
+        Get the figure data of Viewer object to embed into browser (for example)
+
+        Returns:
+            str: Figure data to be embedded in html
+        """
+        
+        imgdata = StringIO()
+        self.fig.savefig(imgdata, format='svg')
+        imgdata.seek(0)
+        
+        return imgdata.getvalue()
+    
+           
     def plot_orbit(self, orbit_data: Dict[str, List[float]]) -> None:
         """
         Plots the orbit of a planet
 
         Args:
             orbit_data Dict: {name: planet name, 
                     c: colour,
```

### Comparing `solarkit-0.1.1/solarkit.egg-info/PKG-INFO` & `solarkit-0.1.5/solarkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.1.1
+Version: 0.1.5
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

