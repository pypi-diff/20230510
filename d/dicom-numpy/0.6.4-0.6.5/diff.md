# Comparing `tmp/dicom_numpy-0.6.4.tar.gz` & `tmp/dicom_numpy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom_numpy-0.6.4.tar", last modified: Mon May  8 18:53:36 2023, max compression
+gzip compressed data, was "dicom_numpy-0.6.5.tar", last modified: Wed May 10 19:53:28 2023, max compression
```

## Comparing `dicom_numpy-0.6.4.tar` & `dicom_numpy-0.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/dicom_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/combine_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/dicom_numpy/zip_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/dicom_numpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 18:53:36.000000 dicom_numpy-0.6.4/dicom_numpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:53:36.545419 dicom_numpy-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/tests/test_combine_from_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-08 18:53:26.000000 dicom_numpy-0.6.4/tests/test_combine_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:53:28.191320 dicom_numpy-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 19:53:28.191320 dicom_numpy-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:53:28.191320 dicom_numpy-0.6.5/dicom_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/dicom_numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/dicom_numpy/combine_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/dicom_numpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/dicom_numpy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/dicom_numpy/zip_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:53:28.191320 dicom_numpy-0.6.5/dicom_numpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 19:53:28.000000 dicom_numpy-0.6.5/dicom_numpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 19:53:28.000000 dicom_numpy-0.6.5/dicom_numpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:53:28.000000 dicom_numpy-0.6.5/dicom_numpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 19:53:28.000000 dicom_numpy-0.6.5/dicom_numpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 19:53:28.000000 dicom_numpy-0.6.5/dicom_numpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 19:53:28.195320 dicom_numpy-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:53:28.191320 dicom_numpy-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/tests/test_combine_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-10 19:53:17.000000 dicom_numpy-0.6.5/tests/test_combine_slices.py
```

### Comparing `dicom_numpy-0.6.4/LICENSE.txt` & `dicom_numpy-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.4/PKG-INFO` & `dicom_numpy-0.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom_numpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Extract image data into a 3D numpy array from a set of DICOM files.
 Home-page: https://github.com/innolitics/dicom-numpy
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: dicom numpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dicom_numpy-0.6.4/dicom_numpy/combine_slices.py` & `dicom_numpy-0.6.5/dicom_numpy/combine_slices.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
     If `skip_sorting` is set to `True`, `combine_slices` will not attempt to
     sort the slices. This can be useful if the volume must be ordered on other
     tags besides slice position or instance number. This overrides any value
     passed to `sort_by_instance`.
 
     If `c_order_axes` is set to `True`, the returned array will have its axes
-    returned in the order of `(k, i, j)` rather than `(j, i, k)`. This is done
+    returned in the order of `(k, j, i)` rather than `(i, j, k)`. This is done
     to optimize slice accesses by ensuring that each slice is contiguous in
-    memory. By default, this is done by keeping the axes `(j, i, k)` and storing
+    memory. By default, this is done by keeping the axes `(i, j, k)` and storing
     the array using Fortran ordering. This can cause issues with some serialization
     libraries that require C-ordering, such as HDF5. In those cases, the axes may
     be reordered such that slices remain contiguous in memory, but the array is
     returned in C-ordering.
 
     The returned array has the column-major byte-order.
```

### Comparing `dicom_numpy-0.6.4/dicom_numpy/zip_archive.py` & `dicom_numpy-0.6.5/dicom_numpy/zip_archive.py`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.4/dicom_numpy.egg-info/PKG-INFO` & `dicom_numpy-0.6.5/dicom_numpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom-numpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Extract image data into a 3D numpy array from a set of DICOM files.
 Home-page: https://github.com/innolitics/dicom-numpy
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: dicom numpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dicom_numpy-0.6.4/setup.py` & `dicom_numpy-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.4/tests/test_combine_from_zip.py` & `dicom_numpy-0.6.5/tests/test_combine_from_zip.py`

 * *Files identical despite different names*

### Comparing `dicom_numpy-0.6.4/tests/test_combine_slices.py` & `dicom_numpy-0.6.5/tests/test_combine_slices.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,22 @@
 
     def test_no_rescale_if_forced_false(self):
         slice_datasets = [MockSlice(np.ones((10, 20), dtype=np.uint8), 0, RescaleSlope=2, RescaleIntercept=3)]
         voxels = _merge_slice_pixel_arrays(slice_datasets, rescale=False)
         assert voxels.dtype == np.uint8
 
     def test_c_ordering(self):
+        # Note that the shape returned by pydicom's `pixel_array` is [j, i]
         slices = [
             MockSlice(np.ones((10, 20), dtype=np.uint8), 0, RescaleSlope=2, RescaleIntercept=3),
             MockSlice(np.ones((10, 20), dtype=np.uint8), 1, RescaleSlope=2, RescaleIntercept=3),
         ]
         voxels = _merge_slice_pixel_arrays(slices, c_order_axes=True)
         assert voxels.flags.c_contiguous
+        # Assert that the axes order is [k, j, i]
         assert voxels.shape == (2, 10, 20)
 
 
 class TestValidateSlicesFormUniformGrid:
     def test_missing_middle_slice_strict(self, axial_slices):
         """
         By default, all slices must be present. Slice position is determined
```

