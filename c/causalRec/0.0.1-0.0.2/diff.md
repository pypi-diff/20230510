# Comparing `tmp/causalRec-0.0.1.tar.gz` & `tmp/causalRec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalRec-0.0.1.tar", last modified: Wed May 10 00:29:36 2023, max compression
+gzip compressed data, was "causalRec-0.0.2.tar", last modified: Wed May 10 01:26:14 2023, max compression
```

## Comparing `causalRec-0.0.1.tar` & `causalRec-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 00:29:36.714644 causalRec-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-10 00:29:36.698885 causalRec-0.0.1/BinaryIntRec/
--rw-rw-rw-   0        0        0     7836 2023-05-02 15:41:52.000000 causalRec-0.0.1/BinaryIntRec/CausalTree.R
--rw-rw-rw-   0        0        0    24650 2023-05-04 09:15:32.000000 causalRec-0.0.1/BinaryIntRec/IROImodels.R
--rw-rw-rw-   0        0        0     2768 2023-05-09 01:08:18.000000 causalRec-0.0.1/BinaryIntRec/IROImodels.py
--rw-rw-rw-   0        0        0     2417 2023-05-02 16:09:03.000000 causalRec-0.0.1/BinaryIntRec/Recommendation.R
--rw-rw-rw-   0        0        0      927 2023-05-08 14:04:27.000000 causalRec-0.0.1/BinaryIntRec/__init__.py
--rw-rw-rw-   0        0        0     2928 2023-05-10 00:29:36.714644 causalRec-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2022-06-05 09:17:55.000000 causalRec-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 00:29:36.714644 causalRec-0.0.1/causalRec.egg-info/
--rw-rw-rw-   0        0        0     2928 2023-05-10 00:29:36.000000 causalRec-0.0.1/causalRec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-05-10 00:29:36.000000 causalRec-0.0.1/causalRec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 00:29:36.000000 causalRec-0.0.1/causalRec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-10 00:29:36.000000 causalRec-0.0.1/causalRec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 00:29:36.000000 causalRec-0.0.1/causalRec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-05-04 09:57:00.000000 causalRec-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 00:29:36.714644 causalRec-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     4465 2023-05-09 15:45:27.000000 causalRec-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:26:14.393616 causalRec-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-10 01:26:14.384629 causalRec-0.0.2/BinaryIntRec/
+-rw-rw-rw-   0        0        0     2768 2023-05-09 01:08:18.000000 causalRec-0.0.2/BinaryIntRec/BinaryIntRec.py
+-rw-rw-rw-   0        0        0     7836 2023-05-02 15:41:52.000000 causalRec-0.0.2/BinaryIntRec/CausalTree.R
+-rw-rw-rw-   0        0        0    24650 2023-05-04 09:15:32.000000 causalRec-0.0.2/BinaryIntRec/IROImodels.R
+-rw-rw-rw-   0        0        0     2417 2023-05-02 16:09:03.000000 causalRec-0.0.2/BinaryIntRec/Recommendation.R
+-rw-rw-rw-   0        0        0      940 2023-05-10 01:25:33.000000 causalRec-0.0.2/BinaryIntRec/__init__.py
+-rw-rw-rw-   0        0        0     2928 2023-05-10 01:26:14.393616 causalRec-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1913 2022-06-05 09:17:55.000000 causalRec-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:26:14.391629 causalRec-0.0.2/causalRec.egg-info/
+-rw-rw-rw-   0        0        0     2928 2023-05-10 01:26:14.000000 causalRec-0.0.2/causalRec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-05-10 01:26:14.000000 causalRec-0.0.2/causalRec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:26:14.000000 causalRec-0.0.2/causalRec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-10 01:26:14.000000 causalRec-0.0.2/causalRec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 01:26:14.000000 causalRec-0.0.2/causalRec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-05-04 09:57:00.000000 causalRec-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:26:14.394691 causalRec-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     4465 2023-05-09 15:45:27.000000 causalRec-0.0.2/setup.py
```

### Comparing `causalRec-0.0.1/BinaryIntRec/CausalTree.R` & `causalRec-0.0.2/BinaryIntRec/CausalTree.R`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/BinaryIntRec/IROImodels.R` & `causalRec-0.0.2/BinaryIntRec/IROImodels.R`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/BinaryIntRec/IROImodels.py` & `causalRec-0.0.2/BinaryIntRec/BinaryIntRec.py`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/BinaryIntRec/Recommendation.R` & `causalRec-0.0.2/BinaryIntRec/Recommendation.R`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/BinaryIntRec/__init__.py` & `causalRec-0.0.2/BinaryIntRec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # """init module."""
 
 #!/usr/bin/env python
 # @Author: tuyen
 #"""init module."""
 # from __future__ import absolute_import
 import sys
-from BinaryIntRec import *
+from BinaryIntRec.BinaryIntRec import *
 
 # -------------------------------- VERSION --------------------------------- #
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
 #   X.Y
@@ -22,15 +22,15 @@
 #   X.YbN   # Beta release
 #   X.YrcN  # Release Candidate
 #   X.Y     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 # ---------------------------- GLOBAL VARIABLES ---------------------------- #
 PYTHON_VERSION = sys.version_info[0]
 
 
 __all__ = [  'PYTHON_VERSION', ]
```

### Comparing `causalRec-0.0.1/PKG-INFO` & `causalRec-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalRec
-Version: 0.0.1
+Version: 0.0.2
 Summary: causal Intervention Recommendation
 Home-page: https://github.com/vntuyen/causalRec/
 Author: Tuyen Vu
 Author-email: tuyen.vu@mymail.unisa.edu.au
 License: Apache Software License (Apache 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `causalRec-0.0.1/README.md` & `causalRec-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/causalRec.egg-info/PKG-INFO` & `causalRec-0.0.2/causalRec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalRec
-Version: 0.0.1
+Version: 0.0.2
 Summary: causal Intervention Recommendation
 Home-page: https://github.com/vntuyen/causalRec/
 Author: Tuyen Vu
 Author-email: tuyen.vu@mymail.unisa.edu.au
 License: Apache Software License (Apache 2.0)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `causalRec-0.0.1/license.txt` & `causalRec-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `causalRec-0.0.1/setup.py` & `causalRec-0.0.2/setup.py`

 * *Files identical despite different names*

