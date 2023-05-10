# Comparing `tmp/aeppl-nightly-0.1.4.dev20230508.tar.gz` & `tmp/aeppl-nightly-0.1.4.dev20230509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.4.dev20230508.tar", last modified: Mon May  8 00:29:27 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.4.dev20230509.tar", last modified: Tue May  9 00:30:40 2023, max compression
```

## Comparing `aeppl-nightly-0.1.4.dev20230508.tar` & `aeppl-nightly-0.1.4.dev20230509.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 00:29:27.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-08 00:29:27.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:29:27.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:29:26.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 00:29:27.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 00:29:27.000000 aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:29:27.071431 aeppl-nightly-0.1.4.dev20230508/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-08 00:29:14.000000 aeppl-nightly-0.1.4.dev20230508/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:30:40.487449 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 00:30:40.000000 aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:30:40.491449 aeppl-nightly-0.1.4.dev20230509/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-09 00:30:29.000000 aeppl-nightly-0.1.4.dev20230509/versioneer.py
```

### Comparing `aeppl-nightly-0.1.4.dev20230508/LICENSE` & `aeppl-nightly-0.1.4.dev20230509/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230509/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230508
+Version: 0.1.4.dev20230509
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230508/README.md` & `aeppl-nightly-0.1.4.dev20230509/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/abstract.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/censoring.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/convolutions.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/cumsum.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/dists.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/logprob.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/mixture.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/printing.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/rewriting.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/scan.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/tensor.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/transforms.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl/utils.py` & `aeppl-nightly-0.1.4.dev20230509/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230508
+Version: 0.1.4.dev20230509
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230508/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.4.dev20230509/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/setup.cfg` & `aeppl-nightly-0.1.4.dev20230509/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/setup.py` & `aeppl-nightly-0.1.4.dev20230509/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_abstract.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_censoring.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_convolutions.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_cumsum.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_dist.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_logprob.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_mixture.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_printing.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_rewriting.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_scan.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_tensor.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_transforms.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/tests/test_utils.py` & `aeppl-nightly-0.1.4.dev20230509/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230508/versioneer.py` & `aeppl-nightly-0.1.4.dev20230509/versioneer.py`

 * *Files identical despite different names*
