# Comparing `tmp/decimer_segmentation-1.1.2.tar.gz` & `tmp/decimer_segmentation-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decimer_segmentation-1.1.2.tar", last modified: Thu May  4 08:59:45 2023, max compression
+gzip compressed data, was "decimer_segmentation-1.1.3.tar", last modified: Wed May 10 06:29:57 2023, max compression
```

## Comparing `decimer_segmentation-1.1.2.tar` & `decimer_segmentation-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1070 2023-05-04 08:58:28.000000 decimer_segmentation-1.1.2/LICENSE
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     7419 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/PKG-INFO
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     6534 2023-05-04 08:58:28.000000 decimer_segmentation-1.1.2/README.md
-drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/decimer_segmentation/
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      378 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/__init__.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    16596 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/complete_structure.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    12581 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/decimer_segmentation.py
-drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     9768 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/config.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)   128564 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/model.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    13932 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/moldetect.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    34493 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/utils.py
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    19506 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/visualize.py
-drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     7419 2023-05-04 08:59:45.000000 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/PKG-INFO
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      584 2023-05-04 08:59:45.000000 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)        1 2023-05-04 08:59:45.000000 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      111 2023-05-04 08:59:45.000000 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/requires.txt
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       21 2023-05-04 08:59:45.000000 decimer_segmentation-1.1.2/decimer_segmentation.egg-info/top_level.txt
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       38 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/setup.cfg
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1415 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/setup.py
-drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-04 08:59:45.170689 decimer_segmentation-1.1.2/tests/
--rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     5147 2023-05-04 08:58:29.000000 decimer_segmentation-1.1.2/tests/test_mask_expansion.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1070 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/LICENSE
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     7841 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/PKG-INFO
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     6956 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/README.md
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/decimer_segmentation/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      378 2023-05-10 06:28:49.000000 decimer_segmentation-1.1.3/decimer_segmentation/__init__.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    16596 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/complete_structure.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    12581 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/decimer_segmentation.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     9768 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/config.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)   128564 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/model.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    13932 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/moldetect.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    34493 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/utils.py
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)    19506 2023-05-10 06:27:57.000000 decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/visualize.py
+drwxrwxr-x   0 kohulan   (1000) kohulan   (1000)        0 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     7841 2023-05-10 06:29:57.000000 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      555 2023-05-10 06:29:57.000000 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)        1 2023-05-10 06:29:57.000000 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)      111 2023-05-10 06:29:57.000000 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/requires.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       21 2023-05-10 06:29:57.000000 decimer_segmentation-1.1.3/decimer_segmentation.egg-info/top_level.txt
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)       38 2023-05-10 06:29:57.443122 decimer_segmentation-1.1.3/setup.cfg
+-rw-rw-r--   0 kohulan   (1000) kohulan   (1000)     1623 2023-05-10 06:28:34.000000 decimer_segmentation-1.1.3/setup.py
```

### Comparing `decimer_segmentation-1.1.2/LICENSE` & `decimer_segmentation-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/PKG-INFO` & `decimer_segmentation-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decimer_segmentation
-Version: 1.1.2
+Version: 1.1.3
 Summary: DECIMER Segmentation - Extraction of chemical structure depictions from scientific literature
 Home-page: https://github.com/Kohulan/DECIMER-Image-Segmentation
 Author: Kohulan Rajan
 Author-email: kohulan.rajan@uni-jena.de
 Maintainer: Kohulan Rajan
 Maintainer-email: kohulan.rajan@uni-jena.de
 License: MIT
@@ -22,15 +22,18 @@
 License-File: LICENSE
 
 # DECIMER-Image-Segmentation
 [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIt)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-blue.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/commit-activity)
 [![GitHub issues](https://img.shields.io/github/issues/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/issues/)
 [![GitHub contributors](https://img.shields.io/github/contributors/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/contributors/)
+[![tensorflow](https://img.shields.io/badge/TensorFlow-2.10.1-FF6F00.svg?style=flat&logo=tensorflow)](https://www.tensorflow.org)
 [![DOI](https://zenodo.org/badge/268631290.svg)](https://zenodo.org/badge/latestdoi/268631290)
+[![GitHub release](https://img.shields.io/github/release/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/decimer-segmentation.svg)](https://pypi.python.org/pypi/decimer-segmentation/)
 
 Chemistry looks back at many decades of publications on chemical compounds, their structures and properties, in scientific articles. Liberating this knowledge (semi-)automatically and making it available to the world in open-access databases is a current challenge. Apart from mining textual information, Optical Chemical Structure Recognition (OCSR), the translation of an image of a chemical structure into a machine-readable representation, is part of this workflow. As the OCSR process requires an image containing a chemical structure, there is a need for a publicly available tool that automatically recognizes and segments chemical structure depictions from scientific publications. This is especially important for older documents which are only available as scanned pages. Here, we present DECIMER (Deep lEarning for Chemical IMagE Recognition) Segmentation, the first open-source, deep learning-based tool for automated recognition and segmentation of chemical structures from the scientific literature.
 
 The workflow is divided into two main stages. During the detection step, a deep learning model recognizes chemical structure depictions and creates masks which define their positions on the input page. Subsequently, potentially incomplete masks are expanded in a post-processing workflow. The performance of DECIMER Segmentation has been manually evaluated on three sets of publications from different publishers. The approach operates on bitmap images of journal pages to be applicable also to older articles before the introduction of vector images in PDFs. 
 
 By making the source code and the trained model publicly available, we hope to contribute to the development of comprehensive chemical data extraction workflows. In order to facilitate access to DECIMER Segmentation, we also developed a web application. The web application, available at https://decimer.ai, lets the user upload a pdf file and retrieve the segmented structure depictions.
```

### Comparing `decimer_segmentation-1.1.2/README.md` & `decimer_segmentation-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # DECIMER-Image-Segmentation
 [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIt)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-blue.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/commit-activity)
 [![GitHub issues](https://img.shields.io/github/issues/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/issues/)
 [![GitHub contributors](https://img.shields.io/github/contributors/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/contributors/)
+[![tensorflow](https://img.shields.io/badge/TensorFlow-2.10.1-FF6F00.svg?style=flat&logo=tensorflow)](https://www.tensorflow.org)
 [![DOI](https://zenodo.org/badge/268631290.svg)](https://zenodo.org/badge/latestdoi/268631290)
+[![GitHub release](https://img.shields.io/github/release/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/decimer-segmentation.svg)](https://pypi.python.org/pypi/decimer-segmentation/)
 
 Chemistry looks back at many decades of publications on chemical compounds, their structures and properties, in scientific articles. Liberating this knowledge (semi-)automatically and making it available to the world in open-access databases is a current challenge. Apart from mining textual information, Optical Chemical Structure Recognition (OCSR), the translation of an image of a chemical structure into a machine-readable representation, is part of this workflow. As the OCSR process requires an image containing a chemical structure, there is a need for a publicly available tool that automatically recognizes and segments chemical structure depictions from scientific publications. This is especially important for older documents which are only available as scanned pages. Here, we present DECIMER (Deep lEarning for Chemical IMagE Recognition) Segmentation, the first open-source, deep learning-based tool for automated recognition and segmentation of chemical structures from the scientific literature.
 
 The workflow is divided into two main stages. During the detection step, a deep learning model recognizes chemical structure depictions and creates masks which define their positions on the input page. Subsequently, potentially incomplete masks are expanded in a post-processing workflow. The performance of DECIMER Segmentation has been manually evaluated on three sets of publications from different publishers. The approach operates on bitmap images of journal pages to be applicable also to older articles before the introduction of vector images in PDFs. 
 
 By making the source code and the trained model publicly available, we hope to contribute to the development of comprehensive chemical data extraction workflows. In order to facilitate access to DECIMER Segmentation, we also developed a web application. The web application, available at https://decimer.ai, lets the user upload a pdf file and retrieve the segmented structure depictions.
```

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/complete_structure.py` & `decimer_segmentation-1.1.3/decimer_segmentation/complete_structure.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/decimer_segmentation.py` & `decimer_segmentation-1.1.3/decimer_segmentation/decimer_segmentation.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/config.py` & `decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/config.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/model.py` & `decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/model.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/moldetect.py` & `decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/moldetect.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/utils.py` & `decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/utils.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation/mrcnn/visualize.py` & `decimer_segmentation-1.1.3/decimer_segmentation/mrcnn/visualize.py`

 * *Files identical despite different names*

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation.egg-info/PKG-INFO` & `decimer_segmentation-1.1.3/decimer_segmentation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decimer-segmentation
-Version: 1.1.2
+Version: 1.1.3
 Summary: DECIMER Segmentation - Extraction of chemical structure depictions from scientific literature
 Home-page: https://github.com/Kohulan/DECIMER-Image-Segmentation
 Author: Kohulan Rajan
 Author-email: kohulan.rajan@uni-jena.de
 Maintainer: Kohulan Rajan
 Maintainer-email: kohulan.rajan@uni-jena.de
 License: MIT
@@ -22,15 +22,18 @@
 License-File: LICENSE
 
 # DECIMER-Image-Segmentation
 [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIt)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-blue.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/commit-activity)
 [![GitHub issues](https://img.shields.io/github/issues/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/issues/)
 [![GitHub contributors](https://img.shields.io/github/contributors/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/graphs/contributors/)
+[![tensorflow](https://img.shields.io/badge/TensorFlow-2.10.1-FF6F00.svg?style=flat&logo=tensorflow)](https://www.tensorflow.org)
 [![DOI](https://zenodo.org/badge/268631290.svg)](https://zenodo.org/badge/latestdoi/268631290)
+[![GitHub release](https://img.shields.io/github/release/Kohulan/DECIMER-Image-Segmentation.svg)](https://GitHub.com/Kohulan/DECIMER-Image-Segmentation/releases/)
+[![PyPI version fury.io](https://badge.fury.io/py/decimer-segmentation.svg)](https://pypi.python.org/pypi/decimer-segmentation/)
 
 Chemistry looks back at many decades of publications on chemical compounds, their structures and properties, in scientific articles. Liberating this knowledge (semi-)automatically and making it available to the world in open-access databases is a current challenge. Apart from mining textual information, Optical Chemical Structure Recognition (OCSR), the translation of an image of a chemical structure into a machine-readable representation, is part of this workflow. As the OCSR process requires an image containing a chemical structure, there is a need for a publicly available tool that automatically recognizes and segments chemical structure depictions from scientific publications. This is especially important for older documents which are only available as scanned pages. Here, we present DECIMER (Deep lEarning for Chemical IMagE Recognition) Segmentation, the first open-source, deep learning-based tool for automated recognition and segmentation of chemical structures from the scientific literature.
 
 The workflow is divided into two main stages. During the detection step, a deep learning model recognizes chemical structure depictions and creates masks which define their positions on the input page. Subsequently, potentially incomplete masks are expanded in a post-processing workflow. The performance of DECIMER Segmentation has been manually evaluated on three sets of publications from different publishers. The approach operates on bitmap images of journal pages to be applicable also to older articles before the introduction of vector images in PDFs. 
 
 By making the source code and the trained model publicly available, we hope to contribute to the development of comprehensive chemical data extraction workflows. In order to facilitate access to DECIMER Segmentation, we also developed a web application. The web application, available at https://decimer.ai, lets the user upload a pdf file and retrieve the segmented structure depictions.
```

### Comparing `decimer_segmentation-1.1.2/decimer_segmentation.egg-info/SOURCES.txt` & `decimer_segmentation-1.1.3/decimer_segmentation.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 decimer_segmentation.egg-info/dependency_links.txt
 decimer_segmentation.egg-info/requires.txt
 decimer_segmentation.egg-info/top_level.txt
 decimer_segmentation/mrcnn/config.py
 decimer_segmentation/mrcnn/model.py
 decimer_segmentation/mrcnn/moldetect.py
 decimer_segmentation/mrcnn/utils.py
-decimer_segmentation/mrcnn/visualize.py
-tests/test_mask_expansion.py
+decimer_segmentation/mrcnn/visualize.py
```

### Comparing `decimer_segmentation-1.1.2/setup.py` & `decimer_segmentation-1.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 #!/usr/bin/env python
 
 import setuptools
+import platform
+
+if (platform.processor() == 'arm' or platform.processor() == 'i386') and platform.system() == 'Darwin':
+    tensorflow_os = "tensorflow-macos==2.10.0"
+else:
+    tensorflow_os = "tensorflow==2.10.1"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="decimer_segmentation",
-    version="1.1.2",
+    version="1.1.3",
     author="Kohulan Rajan",
     author_email="kohulan.rajan@uni-jena.de",
     maintainer="Kohulan Rajan",
     maintainer_email="kohulan.rajan@uni-jena.de",
     description="DECIMER Segmentation - Extraction of chemical structure depictions from scientific literature",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kohulan/DECIMER-Image-Segmentation",
     packages=setuptools.find_packages(),
     license="MIT",
     install_requires=[
-        "tensorflow==2.10.1",
+        tensorflow_os,
         "numpy>=1.2.0",
         "scikit-image>=0.2.0",
         "pillow",
         "opencv-python",
         "matplotlib",
         "imantics",
         "IPython",
```

