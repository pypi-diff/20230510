# Comparing `tmp/multiviewdata-0.6.tar.gz` & `tmp/multiviewdata-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiviewdata-0.6.tar", last modified: Wed May 10 11:50:56 2023, max compression
+gzip compressed data, was "dist/multiviewdata-0.7.tar", last modified: Wed May 10 14:29:21 2023, max compression
```

## Comparing `multiviewdata-0.6.tar` & `multiviewdata-0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-10 11:50:56.000000 multiviewdata-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-10 11:50:45.000000 multiviewdata-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/test/test_outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/torchdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/cars3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/cub.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/mediamill.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/mfeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/mirflickr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/tgca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/wiw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchdatasets/xrmb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/torchmodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/cars3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/cub.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/mfeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/wiw.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/torchmodels/xrmb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:45.000000 multiviewdata-0.6/multiviewdata/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-10 11:50:55.000000 multiviewdata-0.6/multiviewdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-10 11:50:56.000000 multiviewdata-0.6/multiviewdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:50:55.000000 multiviewdata-0.6/multiviewdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 11:50:55.000000 multiviewdata-0.6/multiviewdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 11:50:55.000000 multiviewdata-0.6/multiviewdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:50:56.000000 multiviewdata-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-10 11:50:54.000000 multiviewdata-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-10 14:29:21.000000 multiviewdata-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-10 14:29:04.000000 multiviewdata-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/test/test_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/torchdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/cars3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/cub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/mediamill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/mfeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/mirflickr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14770 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/tgca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/wiw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchdatasets/xrmb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/torchmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/cars3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/cub.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/mfeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/wiw.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/torchmodels/xrmb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:04.000000 multiviewdata-0.7/multiviewdata/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 14:29:21.000000 multiviewdata-0.7/multiviewdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:29:21.000000 multiviewdata-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-10 14:29:18.000000 multiviewdata-0.7/setup.py
```

### Comparing `multiviewdata-0.6/PKG-INFO` & `multiviewdata-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiviewdata
-Version: 0.6
+Version: 0.7
 Summary: Packaged data modules for multiview learning benchmarks
 Home-page: UNKNOWN
 Author: James Chapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: UNKNOWN
 Description: [![DOI](https://zenodo.org/badge/465287085.svg)](https://zenodo.org/badge/latestdoi/465287085)
         ![Build Status](https://github.com/jameschapman19/multiviewdata/actions/workflows/python-package.yml/badge.svg)
```

### Comparing `multiviewdata-0.6/README.md` & `multiviewdata-0.7/README.md`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/test/test_outputs.py` & `multiviewdata-0.7/multiviewdata/test/test_outputs.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/cars3d.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/cars3d.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/cub.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/cub.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/generic.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/generic.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/mediamill.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/mediamill.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/mfeat.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/mfeat.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/mirflickr.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/mirflickr.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/mnist.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         self.flatten = flatten
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, idx):
         x_a, label = self.dataset[idx]
-        x_b = x_a[:, :, 14:]/255.
-        x_a = x_a[:, :, :14]/255.
+        x_b = x_a[:, :, 14:]
+        x_a = x_a[:, :, :14]
         if self.flatten:
             x_a = torch.flatten(x_a)
             x_b = torch.flatten(x_b)
         return {"views": (x_a, x_b), "label": label, "index": idx}
 
 
 class NoisyMNIST(Dataset):
```

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/tgca.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/tgca.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/twitter.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/twitter.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/wiw.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/wiw.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchdatasets/xrmb.py` & `multiviewdata-0.7/multiviewdata/torchdatasets/xrmb.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchmodels/cars3d.py` & `multiviewdata-0.7/multiviewdata/torchmodels/cars3d.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchmodels/cub.py` & `multiviewdata-0.7/multiviewdata/torchmodels/cub.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchmodels/mnist.py` & `multiviewdata-0.7/multiviewdata/torchmodels/mnist.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata/torchmodels/wiw.py` & `multiviewdata-0.7/multiviewdata/torchmodels/wiw.py`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/multiviewdata.egg-info/PKG-INFO` & `multiviewdata-0.7/multiviewdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiviewdata
-Version: 0.6
+Version: 0.7
 Summary: Packaged data modules for multiview learning benchmarks
 Home-page: UNKNOWN
 Author: James Chapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: UNKNOWN
 Description: [![DOI](https://zenodo.org/badge/465287085.svg)](https://zenodo.org/badge/latestdoi/465287085)
         ![Build Status](https://github.com/jameschapman19/multiviewdata/actions/workflows/python-package.yml/badge.svg)
```

### Comparing `multiviewdata-0.6/multiviewdata.egg-info/SOURCES.txt` & `multiviewdata-0.7/multiviewdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiviewdata-0.6/setup.py` & `multiviewdata-0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("./requirements.txt", "r") as f:
     REQUIRED_PACKAGES = f.read()
 
 setup(
     name="multiviewdata",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     url="",
     license="",
     author="James Chapman",
     author_email="james.chapman.19@ucl.ac.uk",
     install_requires=REQUIRED_PACKAGES,
     description="Packaged data modules for multiview learning benchmarks",
```

