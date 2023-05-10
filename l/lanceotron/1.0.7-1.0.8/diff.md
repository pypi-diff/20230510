# Comparing `tmp/lanceotron-1.0.7.tar.gz` & `tmp/lanceotron-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanceotron-1.0.7.tar", last modified: Thu Aug 11 15:40:50 2022, max compression
+gzip compressed data, was "dist/lanceotron-1.0.8.tar", last modified: Fri Aug 12 09:14:07 2022, max compression
```

## Comparing `lanceotron-1.0.7.tar` & `lanceotron-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-11 15:40:50.000000 lanceotron-1.0.7/
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    35149 2022-08-10 17:51:21.000000 lanceotron-1.0.7/LICENSE
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      210 2022-08-10 15:06:04.000000 lanceotron-1.0.7/MANIFEST.in
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4720 2022-08-11 15:40:50.000000 lanceotron-1.0.7/PKG-INFO
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4188 2022-08-10 15:06:04.000000 lanceotron-1.0.7/README.md
-drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron/
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      147 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/__init__.py
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     3757 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/cli.py
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    32084 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/lanceotron.py
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    15134 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/modules.py
-drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron/static/
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       38 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/static/__init__.py
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    48467 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/static/standard_scaler_deep_v5_03.p
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      742 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/static/standard_scaler_wide_v5_03.p
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)  1727328 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4799 2022-08-10 15:06:04.000000 lanceotron-1.0.7/lanceotron/utils.py
-drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4720 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/PKG-INFO
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      549 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/SOURCES.txt
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)        1 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/dependency_links.txt
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       51 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/entry_points.txt
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       67 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/requires.txt
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       11 2022-08-11 15:40:50.000000 lanceotron-1.0.7/lanceotron.egg-info/top_level.txt
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       38 2022-08-11 15:40:50.000000 lanceotron-1.0.7/setup.cfg
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     1024 2022-08-11 15:39:57.000000 lanceotron-1.0.7/setup.py
-drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-11 15:40:50.000000 lanceotron-1.0.7/test/
--rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     3357 2022-08-10 15:06:04.000000 lanceotron-1.0.7/test/test_main.py
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:07.000000 lanceotron-1.0.8/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       57 2022-08-12 09:12:26.000000 lanceotron-1.0.8/CHANGELOG.md
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    35149 2022-08-10 17:51:21.000000 lanceotron-1.0.8/LICENSE
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      210 2022-08-10 15:06:04.000000 lanceotron-1.0.8/MANIFEST.in
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4701 2022-08-12 09:14:07.000000 lanceotron-1.0.8/PKG-INFO
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4188 2022-08-10 15:06:04.000000 lanceotron-1.0.8/README.md
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:06.000000 lanceotron-1.0.8/docs/
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:06.000000 lanceotron-1.0.8/docs/api/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      283 2022-08-10 15:06:04.000000 lanceotron-1.0.8/docs/api/modules.md
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      158 2022-08-10 15:06:04.000000 lanceotron-1.0.8/docs/genome_tutorial.md
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     2776 2022-08-10 17:39:17.000000 lanceotron-1.0.8/docs/index.md
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:06.000000 lanceotron-1.0.8/lanceotron/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      147 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/__init__.py
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     3757 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/cli.py
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    32084 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/lanceotron.py
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    15134 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/modules.py
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:07.000000 lanceotron-1.0.8/lanceotron/static/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       38 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/static/__init__.py
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)    48467 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/static/standard_scaler_deep_v5_03.p
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      742 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/static/standard_scaler_wide_v5_03.p
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)  1727328 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4799 2022-08-10 15:06:04.000000 lanceotron-1.0.8/lanceotron/utils.py
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:07.000000 lanceotron-1.0.8/lanceotron.egg-info/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     4701 2022-08-12 09:14:00.000000 lanceotron-1.0.8/lanceotron.egg-info/PKG-INFO
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      679 2022-08-12 09:14:06.000000 lanceotron-1.0.8/lanceotron.egg-info/SOURCES.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)        1 2022-08-12 09:14:00.000000 lanceotron-1.0.8/lanceotron.egg-info/dependency_links.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       50 2022-08-12 09:14:00.000000 lanceotron-1.0.8/lanceotron.egg-info/entry_points.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       67 2022-08-12 09:14:01.000000 lanceotron-1.0.8/lanceotron.egg-info/requires.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       11 2022-08-12 09:14:01.000000 lanceotron-1.0.8/lanceotron.egg-info/top_level.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      371 2022-08-10 15:06:04.000000 lanceotron-1.0.8/mkdocs.yml
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)      177 2022-08-10 15:06:04.000000 lanceotron-1.0.8/requirements.txt
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)       38 2022-08-12 09:14:07.000000 lanceotron-1.0.8/setup.cfg
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     1024 2022-08-12 09:12:05.000000 lanceotron-1.0.8/setup.py
+drwxr-sr-x   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-12 09:14:07.000000 lanceotron-1.0.8/test/
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)        0 2022-08-10 15:06:04.000000 lanceotron-1.0.8/test/__init__.py
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)  8688421 2022-08-10 15:06:04.000000 lanceotron-1.0.8/test/chr22.bw
+-rw-r--r--   0 sriva    (20452) hugheslabgrp (40031)     3357 2022-08-10 15:06:04.000000 lanceotron-1.0.8/test/test_main.py
```

### Comparing `lanceotron-1.0.7/LICENSE` & `lanceotron-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/PKG-INFO` & `lanceotron-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: lanceotron
-Version: 1.0.7
+Version: 1.0.8
 Summary: Command-line interface to the lanceotron deep learning peak caller
-Home-page: UNKNOWN
 Author: Chris Cole, Lance Hentges, Simone G. Riva
 Author-email: simo.riva15@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LHentges/lanceotron/issues
 Project-URL: Source, https://github.com/LHentges/lanceotron
 Keywords: deep learning,peak calling,keras
 Platform: UNKNOWN
```

### Comparing `lanceotron-1.0.7/README.md` & `lanceotron-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/cli.py` & `lanceotron-1.0.8/lanceotron/cli.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/lanceotron.py` & `lanceotron-1.0.8/lanceotron/lanceotron.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/modules.py` & `lanceotron-1.0.8/lanceotron/modules.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/static/standard_scaler_deep_v5_03.p` & `lanceotron-1.0.8/lanceotron/static/standard_scaler_deep_v5_03.p`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/static/standard_scaler_wide_v5_03.p` & `lanceotron-1.0.8/lanceotron/static/standard_scaler_wide_v5_03.p`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5` & `lanceotron-1.0.8/lanceotron/static/wide_and_deep_fully_trained_v5_03.h5`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron/utils.py` & `lanceotron-1.0.8/lanceotron/utils.py`

 * *Files identical despite different names*

### Comparing `lanceotron-1.0.7/lanceotron.egg-info/PKG-INFO` & `lanceotron-1.0.8/lanceotron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: lanceotron
-Version: 1.0.7
+Version: 1.0.8
 Summary: Command-line interface to the lanceotron deep learning peak caller
-Home-page: UNKNOWN
 Author: Chris Cole, Lance Hentges, Simone G. Riva
 Author-email: simo.riva15@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/LHentges/lanceotron/issues
 Project-URL: Source, https://github.com/LHentges/lanceotron
 Keywords: deep learning,peak calling,keras
 Platform: UNKNOWN
```

### Comparing `lanceotron-1.0.7/lanceotron.egg-info/SOURCES.txt` & `lanceotron-1.0.8/lanceotron.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+mkdocs.yml
+requirements.txt
 setup.py
+docs/genome_tutorial.md
+docs/index.md
+docs/api/modules.md
 lanceotron/__init__.py
 lanceotron/cli.py
 lanceotron/lanceotron.py
 lanceotron/modules.py
 lanceotron/utils.py
 lanceotron.egg-info/PKG-INFO
 lanceotron.egg-info/SOURCES.txt
@@ -13,8 +19,10 @@
 lanceotron.egg-info/entry_points.txt
 lanceotron.egg-info/requires.txt
 lanceotron.egg-info/top_level.txt
 lanceotron/static/__init__.py
 lanceotron/static/standard_scaler_deep_v5_03.p
 lanceotron/static/standard_scaler_wide_v5_03.p
 lanceotron/static/wide_and_deep_fully_trained_v5_03.h5
+test/__init__.py
+test/chr22.bw
 test/test_main.py
```

### Comparing `lanceotron-1.0.7/setup.py` & `lanceotron-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='lanceotron',
-   version='1.0.7',
+   version='1.0.8',
    python_requires='>3.6', 
    description='Command-line interface to the lanceotron deep learning peak caller',
    long_description=long_description,
    long_description_content_type="text/markdown",
    project_urls={
        "Bug Tracker": "https://github.com/LHentges/lanceotron/issues",
        "Source": "https://github.com/LHentges/lanceotron"},
    author='Chris Cole, Lance Hentges, Simone G. Riva',
    author_email='simo.riva15@gmail.com',
    packages=['lanceotron', 'lanceotron.static'],  
    include_package_data=True,
    keywords="deep learning, peak calling, keras",
    install_requires = [
-      "pyBigWig",
+      "pybigwig",
       "scikit-learn",
       "numpy",
       "pandas",
       "tensorflow>2",
       "scipy",
       "natsort",
       "tqdm"
```

### Comparing `lanceotron-1.0.7/test/test_main.py` & `lanceotron-1.0.8/test/test_main.py`

 * *Files identical despite different names*

