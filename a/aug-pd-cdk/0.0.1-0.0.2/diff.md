# Comparing `tmp/aug_pd_cdk-0.0.1.tar.gz` & `tmp/aug_pd_cdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug_pd_cdk-0.0.1.tar", last modified: Tue May  9 22:16:21 2023, max compression
+gzip compressed data, was "aug_pd_cdk-0.0.2.tar", last modified: Tue May  9 22:18:34 2023, max compression
```

## Comparing `aug_pd_cdk-0.0.1.tar` & `aug_pd_cdk-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/src/aug_pd_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/src/aug_pd_cdk/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk/_jsii/aug-pd-ckd@0.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:16:09.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:16:21.170977 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-09 22:16:21.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-09 22:16:21.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:16:21.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 22:16:21.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 22:16:21.000000 aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:18:34.437832 aug_pd_cdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-09 22:18:34.437832 aug_pd_cdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:18:34.437832 aug_pd_cdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:18:34.433832 aug_pd_cdk-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:18:34.433832 aug_pd_cdk-0.0.2/src/aug_pd_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:18:34.437832 aug_pd_cdk-0.0.2/src/aug_pd_cdk/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk/_jsii/aug-pd-ckd@0.0.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:18:23.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:18:34.437832 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-09 22:18:34.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-09 22:18:34.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:18:34.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 22:18:34.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 22:18:34.000000 aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/top_level.txt
```

### Comparing `aug_pd_cdk-0.0.1/LICENSE` & `aug_pd_cdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aug_pd_cdk-0.0.1/PKG-INFO` & `aug_pd_cdk-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug_pd_cdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: aug-pd-ckd
 Home-page: https://github.com/Butterneck/aug-pd-ckd.git
 Author: Filippo Pinton<filippo.pinton@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/Butterneck/aug-pd-ckd.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aug_pd_cdk-0.0.1/setup.py` & `aug_pd_cdk-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aug_pd_cdk",
-    "version": "0.0.1",
+    "version": "0.0.2",
     "description": "aug-pd-ckd",
     "license": "Apache-2.0",
     "url": "https://github.com/Butterneck/aug-pd-ckd.git",
     "long_description_content_type": "text/markdown",
     "author": "Filippo Pinton<filippo.pinton@protonmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aug_pd_cdk",
         "aug_pd_cdk._jsii"
     ],
     "package_data": {
         "aug_pd_cdk._jsii": [
-            "aug-pd-ckd@0.0.1.jsii.tgz"
+            "aug-pd-ckd@0.0.2.jsii.tgz"
         ],
         "aug_pd_cdk": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aug_pd_cdk-0.0.1/src/aug_pd_cdk/__init__.py` & `aug_pd_cdk-0.0.2/src/aug_pd_cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aug_pd_cdk-0.0.1/src/aug_pd_cdk.egg-info/PKG-INFO` & `aug_pd_cdk-0.0.2/src/aug_pd_cdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-pd-cdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: aug-pd-ckd
 Home-page: https://github.com/Butterneck/aug-pd-ckd.git
 Author: Filippo Pinton<filippo.pinton@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/Butterneck/aug-pd-ckd.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

