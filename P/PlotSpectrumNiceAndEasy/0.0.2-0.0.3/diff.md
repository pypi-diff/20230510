# Comparing `tmp/PlotSpectrumNiceAndEasy-0.0.2.tar.gz` & `tmp/PlotSpectrumNiceAndEasy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlotSpectrumNiceAndEasy-0.0.2.tar", last modified: Wed May 10 16:13:28 2023, max compression
+gzip compressed data, was "PlotSpectrumNiceAndEasy-0.0.3.tar", last modified: Wed May 10 16:30:26 2023, max compression
```

## Comparing `PlotSpectrumNiceAndEasy-0.0.2.tar` & `PlotSpectrumNiceAndEasy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:13:28.251901 PlotSpectrumNiceAndEasy-0.0.2/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-05-02 15:26:10.000000 PlotSpectrumNiceAndEasy-0.0.2/LICENSE
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2794 2023-05-10 16:13:28.251901 PlotSpectrumNiceAndEasy-0.0.2/PKG-INFO
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:13:28.211901 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2502 2023-05-10 16:10:29.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy/PlotSpectrumNiceAndEasy.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      149 2023-05-10 16:11:32.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:13:28.247901 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2794 2023-05-10 16:13:27.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      357 2023-05-10 16:13:27.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-05-10 16:13:27.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       15 2023-05-10 16:13:27.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/requires.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       24 2023-05-10 16:13:27.000000 PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1515 2023-05-02 16:20:18.000000 PlotSpectrumNiceAndEasy-0.0.2/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-05-10 16:13:28.267902 PlotSpectrumNiceAndEasy-0.0.2/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1692 2023-05-10 16:11:32.000000 PlotSpectrumNiceAndEasy-0.0.2/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:30:26.539325 PlotSpectrumNiceAndEasy-0.0.3/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-05-02 15:26:10.000000 PlotSpectrumNiceAndEasy-0.0.3/LICENSE
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2794 2023-05-10 16:30:26.539325 PlotSpectrumNiceAndEasy-0.0.3/PKG-INFO
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:30:26.535325 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2503 2023-05-10 16:29:33.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy/PlotSpectrumNiceAndEasy.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      149 2023-05-10 16:29:33.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-05-10 16:30:26.539325 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2794 2023-05-10 16:30:25.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      357 2023-05-10 16:30:25.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-05-10 16:30:25.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       15 2023-05-10 16:30:25.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/requires.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       24 2023-05-10 16:30:25.000000 PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1515 2023-05-02 16:20:18.000000 PlotSpectrumNiceAndEasy-0.0.3/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-05-10 16:30:26.579326 PlotSpectrumNiceAndEasy-0.0.3/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1692 2023-05-10 16:29:33.000000 PlotSpectrumNiceAndEasy-0.0.3/setup.py
```

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/LICENSE` & `PlotSpectrumNiceAndEasy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/PKG-INFO` & `PlotSpectrumNiceAndEasy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PlotSpectrumNiceAndEasy
-Version: 0.0.2
+Version: 0.0.3
 Summary: It is a Python library for build a very nice spectrum and theory lines of elements. But you can plot an other plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/PlotSpectrumNiceAndEasy
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/PlotSpectrumNiceAndEasy/archive/v0.0.2.zip
+Download-URL: https://github.com/89605502155/PlotSpectrumNiceAndEasy/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy/PlotSpectrumNiceAndEasy.py` & `PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy/PlotSpectrumNiceAndEasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.y_name = y_name
         self.save_name = save_name
         self.x_s = x_s
         self.y_s = y_s
         self.y_l_s = y_l_s
         self.x_l_s = x_l_s
 
-    def main(self, x, y,save=False,timesNewR=False **kwargs):
+    def main(self, x, y,save=False,timesNewR=False, **kwargs):
         if timesNewR:
             mpl.rc('font',family='Times New Roman')
         fig, axs = plt.subplots(figsize=(self.x_s, self.y_s))
         plt.xscale(self.sc_x)
         plt.yscale(self.sc_y)
         axs.plot(x, y, "-", color="blue", lw=self.lw)
```

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/PlotSpectrumNiceAndEasy.egg-info/PKG-INFO` & `PlotSpectrumNiceAndEasy-0.0.3/PlotSpectrumNiceAndEasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PlotSpectrumNiceAndEasy
-Version: 0.0.2
+Version: 0.0.3
 Summary: It is a Python library for build a very nice spectrum and theory lines of elements. But you can plot an other plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/PlotSpectrumNiceAndEasy
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/PlotSpectrumNiceAndEasy/archive/v0.0.2.zip
+Download-URL: https://github.com/89605502155/PlotSpectrumNiceAndEasy/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/README.md` & `PlotSpectrumNiceAndEasy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PlotSpectrumNiceAndEasy-0.0.2/setup.py` & `PlotSpectrumNiceAndEasy-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.2'
+version = '0.0.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PlotSpectrumNiceAndEasy',
     version=version,
```

