# Comparing `tmp/educelab-imgproc-0.2.0.tar.gz` & `tmp/educelab-imgproc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educelab-imgproc-0.2.0.tar", last modified: Thu Apr  6 00:39:22 2023, max compression
+gzip compressed data, was "educelab-imgproc-0.3.0.tar", last modified: Wed May 10 16:09:48 2023, max compression
```

## Comparing `educelab-imgproc-0.2.0.tar` & `educelab-imgproc-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-04-06 00:39:22.228844 educelab-imgproc-0.2.0/
--rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab-imgproc-0.2.0/LICENSE
--rw-r--r--   0 seth       (501) staff       (20)     1357 2023-04-06 00:39:22.228888 educelab-imgproc-0.2.0/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab-imgproc-0.2.0/README.md
--rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab-imgproc-0.2.0/pyproject.toml
--rw-r--r--   0 seth       (501) staff       (20)       39 2023-03-30 17:42:22.000000 educelab-imgproc-0.2.0/requirements.txt
--rw-r--r--   0 seth       (501) staff       (20)      918 2023-04-06 00:39:22.229118 educelab-imgproc-0.2.0/setup.cfg
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-04-06 00:39:22.226660 educelab-imgproc-0.2.0/src/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-04-06 00:39:22.226596 educelab-imgproc-0.2.0/src/educelab/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-04-06 00:39:22.228145 educelab-imgproc-0.2.0/src/educelab/imgproc/
--rw-r--r--   0 seth       (501) staff       (20)      243 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/__init__.py
--rw-r--r--   0 seth       (501) staff       (20)      833 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/adjust.py
--rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/conversion.py
--rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/correction.py
--rw-r--r--   0 seth       (501) staff       (20)     2236 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/enhance.py
--rw-r--r--   0 seth       (501) staff       (20)     1643 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/exiftool.py
--rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/pca.py
--rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab-imgproc-0.2.0/src/educelab/imgproc/roi.py
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-04-06 00:39:22.228728 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/
--rw-r--r--   0 seth       (501) staff       (20)     1357 2023-04-06 00:39:22.000000 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      533 2023-04-06 00:39:22.000000 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/SOURCES.txt
--rw-r--r--   0 seth       (501) staff       (20)        1 2023-04-06 00:39:22.000000 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/dependency_links.txt
--rw-r--r--   0 seth       (501) staff       (20)       72 2023-04-06 00:39:22.000000 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/requires.txt
--rw-r--r--   0 seth       (501) staff       (20)        9 2023-04-06 00:39:22.000000 educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/top_level.txt
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 16:09:48.299147 educelab-imgproc-0.3.0/
+-rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab-imgproc-0.3.0/LICENSE
+-rw-r--r--   0 seth       (501) staff       (20)     1357 2023-05-10 16:09:48.299193 educelab-imgproc-0.3.0/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab-imgproc-0.3.0/README.md
+-rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab-imgproc-0.3.0/pyproject.toml
+-rw-r--r--   0 seth       (501) staff       (20)       45 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.0/requirements.txt
+-rw-r--r--   0 seth       (501) staff       (20)      918 2023-05-10 16:09:48.299436 educelab-imgproc-0.3.0/setup.cfg
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 16:09:48.296680 educelab-imgproc-0.3.0/src/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 16:09:48.296612 educelab-imgproc-0.3.0/src/educelab/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 16:09:48.298471 educelab-imgproc-0.3.0/src/educelab/imgproc/
+-rw-r--r--   0 seth       (501) staff       (20)      281 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/__init__.py
+-rw-r--r--   0 seth       (501) staff       (20)      833 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/adjust.py
+-rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/conversion.py
+-rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/correction.py
+-rw-r--r--   0 seth       (501) staff       (20)     3912 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/enhance.py
+-rw-r--r--   0 seth       (501) staff       (20)     1643 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/exiftool.py
+-rw-r--r--   0 seth       (501) staff       (20)      241 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/filters.py
+-rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/pca.py
+-rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.0/src/educelab/imgproc/roi.py
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 16:09:48.299049 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/
+-rw-r--r--   0 seth       (501) staff       (20)     1357 2023-05-10 16:09:48.000000 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      565 2023-05-10 16:09:48.000000 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/SOURCES.txt
+-rw-r--r--   0 seth       (501) staff       (20)        1 2023-05-10 16:09:48.000000 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/dependency_links.txt
+-rw-r--r--   0 seth       (501) staff       (20)       78 2023-05-10 16:09:48.000000 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/requires.txt
+-rw-r--r--   0 seth       (501) staff       (20)        9 2023-05-10 16:09:48.000000 educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/top_level.txt
```

### Comparing `educelab-imgproc-0.2.0/LICENSE` & `educelab-imgproc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/PKG-INFO` & `educelab-imgproc-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.2.0
+Version: 0.3.0
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.2.0/README.md` & `educelab-imgproc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/setup.cfg` & `educelab-imgproc-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = educelab-imgproc
-version = 0.2.0
+version = 0.3.0
 author = Seth Parker
 author_email = c.seth.parker@uky.edu
 description = EduceLab image processing module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://educelab.gitlab.io/educelab-imgproc/
 download_url = https://gitlab.com/educelab/educelab-imgproc
```

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/adjust.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/adjust.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/conversion.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/conversion.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/correction.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/correction.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/exiftool.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/exiftool.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/pca.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/pca.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab/imgproc/roi.py` & `educelab-imgproc-0.3.0/src/educelab/imgproc/roi.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/PKG-INFO` & `educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.2.0
+Version: 0.3.0
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.2.0/src/educelab_imgproc.egg-info/SOURCES.txt` & `educelab-imgproc-0.3.0/src/educelab_imgproc.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 src/educelab/imgproc/__init__.py
 src/educelab/imgproc/adjust.py
 src/educelab/imgproc/conversion.py
 src/educelab/imgproc/correction.py
 src/educelab/imgproc/enhance.py
 src/educelab/imgproc/exiftool.py
+src/educelab/imgproc/filters.py
 src/educelab/imgproc/pca.py
 src/educelab/imgproc/roi.py
 src/educelab_imgproc.egg-info/PKG-INFO
 src/educelab_imgproc.egg-info/SOURCES.txt
 src/educelab_imgproc.egg-info/dependency_links.txt
 src/educelab_imgproc.egg-info/requires.txt
 src/educelab_imgproc.egg-info/top_level.txt
```

