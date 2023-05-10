# Comparing `tmp/napari-clemreg-0.0.1a3.tar.gz` & `tmp/napari-clemreg-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-clemreg-0.0.1a3.tar", last modified: Sun Feb  6 22:04:31 2022, max compression
+gzip compressed data, was "napari-clemreg-0.0.1a4.tar", last modified: Sun Feb  6 23:32:21 2022, max compression
```

## Comparing `napari-clemreg-0.0.1a3.tar` & `napari-clemreg-0.0.1a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.649346 napari-clemreg-0.0.1a3/.github/
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/.github/workflows/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      572 2022-02-04 10:30:25.000000 napari-clemreg-0.0.1a3/.github/workflows/plugin_preview.yml
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      947 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/.gitignore
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/.napari/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      181 2022-02-04 10:30:25.000000 napari-clemreg-0.0.1a3/.napari/config.yml
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1083 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/LICENSE
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      121 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/MANIFEST.in
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3993 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2765 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/README.md
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/docs/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     7505 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/docs/Makefile
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     9442 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/docs/conf.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      468 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/docs/index.rst
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     7029 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/docs/make.bat
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/napari_clemreg/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      405 2022-02-06 20:13:00.000000 napari-clemreg-0.0.1a3/napari_clemreg/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1303 2022-02-06 17:38:00.000000 napari-clemreg-0.0.1a3/napari_clemreg/_dock_widget.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2501 2022-02-06 21:07:47.000000 napari-clemreg-0.0.1a3/napari_clemreg/_reader.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/napari_clemreg/_tests/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/_tests/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      649 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/_tests/test_dock_widget.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/napari_clemreg/widgets/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1219 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/_utils.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3503 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/clean_binary_segmentation.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     8104 2022-02-06 21:41:44.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/data_preprocessing.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1808 2022-02-04 15:50:50.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/em_segmentation.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3831 2022-02-06 16:28:28.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/log_segmentation.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)    12817 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/point_cloud_registration.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2354 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/point_cloud_sampling.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/__init__.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     7432 2022-02-06 19:50:34.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/dataloader.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     7479 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/model.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     2104 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/utils.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3195 2022-02-06 21:21:55.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/utility.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)    15213 2022-02-06 21:58:58.000000 napari-clemreg-0.0.1a3/napari_clemreg/widgets/warp_image_volume.py
-drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     3993 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1196 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        1 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       49 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      148 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       15 2022-02-06 22:04:31.000000 napari-clemreg-0.0.1a3/napari_clemreg.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)        4 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/requirements.txt
--rw-rw-r--   0 daniel    (1001) daniel    (1001)     1441 2022-02-06 22:04:31.653346 napari-clemreg-0.0.1a3/setup.cfg
--rw-rw-r--   0 daniel    (1001) daniel    (1001)       84 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/setup.py
--rw-rw-r--   0 daniel    (1001) daniel    (1001)      853 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a3/tox.ini
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/.github/
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/.github/workflows/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      572 2022-02-04 10:30:25.000000 napari-clemreg-0.0.1a4/.github/workflows/plugin_preview.yml
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      947 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/.gitignore
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/.napari/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      181 2022-02-04 10:30:25.000000 napari-clemreg-0.0.1a4/.napari/config.yml
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1083 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/LICENSE
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      121 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/MANIFEST.in
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3993 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/PKG-INFO
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2765 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/README.md
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/docs/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     7505 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/docs/Makefile
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     9442 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/docs/conf.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      468 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/docs/index.rst
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     7029 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/docs/make.bat
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/napari_clemreg/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      405 2022-02-06 20:13:00.000000 napari-clemreg-0.0.1a4/napari_clemreg/__init__.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1303 2022-02-06 17:38:00.000000 napari-clemreg-0.0.1a4/napari_clemreg/_dock_widget.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2494 2022-02-06 23:30:41.000000 napari-clemreg-0.0.1a4/napari_clemreg/_reader.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/napari_clemreg/_tests/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/_tests/__init__.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      649 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/_tests/test_dock_widget.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/napari_clemreg/widgets/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/__init__.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1219 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/_utils.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3503 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/clean_binary_segmentation.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     8104 2022-02-06 21:41:44.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/data_preprocessing.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1808 2022-02-04 15:50:50.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/em_segmentation.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3831 2022-02-06 16:28:28.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/log_segmentation.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)    12817 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/point_cloud_registration.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2354 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/point_cloud_sampling.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        0 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/__init__.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     7432 2022-02-06 19:50:34.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/dataloader.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     7479 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/model.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     2104 2022-02-04 10:31:47.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/utils.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3195 2022-02-06 21:21:55.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/utility.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)    15213 2022-02-06 21:58:58.000000 napari-clemreg-0.0.1a4/napari_clemreg/widgets/warp_image_volume.py
+drwxrwxr-x   0 daniel    (1001) daniel    (1001)        0 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     3993 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1196 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        1 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       49 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      148 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       15 2022-02-06 23:32:21.000000 napari-clemreg-0.0.1a4/napari_clemreg.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)        4 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/requirements.txt
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)     1441 2022-02-06 23:32:21.709001 napari-clemreg-0.0.1a4/setup.cfg
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)       84 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/setup.py
+-rw-rw-r--   0 daniel    (1001) daniel    (1001)      853 2022-01-19 14:19:54.000000 napari-clemreg-0.0.1a4/tox.ini
```

### Comparing `napari-clemreg-0.0.1a3/.github/workflows/plugin_preview.yml` & `napari-clemreg-0.0.1a4/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/.gitignore` & `napari-clemreg-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/LICENSE` & `napari-clemreg-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/PKG-INFO` & `napari-clemreg-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-clemreg
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A plugin for registering multimodal image volumes based on common segmented structures of interest with point-clouds.
 Home-page: https://github.com/krentzd/napari-clemreg
 Author: Daniel Krentzel
 Author-email: dkrentzel@pm.me
 License: MIT
 Project-URL: Bug Tracker, https://github.com/krentzd/napari-clemreg/issues
 Project-URL: Documentation, https://github.com/krentzd/napari-clemreg#README.md
```

### Comparing `napari-clemreg-0.0.1a3/README.md` & `napari-clemreg-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/docs/Makefile` & `napari-clemreg-0.0.1a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/docs/conf.py` & `napari-clemreg-0.0.1a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/docs/make.bat` & `napari-clemreg-0.0.1a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/_dock_widget.py` & `napari-clemreg-0.0.1a4/napari_clemreg/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/_reader.py` & `napari-clemreg-0.0.1a4/napari_clemreg/_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 def to_czxy(img, metadata):
     m_dims = get_image_dims(metadata)
     if not img.shape[1:] == m_dims:
         src_idx = [img.shape.index(d) for d in m_dims[:2]]
         img = np.moveaxis(img, src_idx, [0, 1])
         return img
-    elif img.shape[1:] == metadata_dims:
+    elif img.shape[1:] == m_dims:
         return img
 
 def tiff_reader(path: str):
     tiff_image = tifffile.imread(path)
     img_metadata = read_metadata(path)
     if len(tiff_image.shape) > 3:
         tiff_image = to_czxy(np.squeeze(tiff_image), img_metadata)
```

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/_tests/test_dock_widget.py` & `napari-clemreg-0.0.1a4/napari_clemreg/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/_utils.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/clean_binary_segmentation.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/clean_binary_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/data_preprocessing.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/em_segmentation.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/em_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/log_segmentation.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/log_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/point_cloud_registration.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/point_cloud_registration.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/point_cloud_sampling.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/point_cloud_sampling.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/dataloader.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/dataloader.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/model.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/model.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/sparse_unet/utils.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/sparse_unet/utils.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/utility.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/utility.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg/widgets/warp_image_volume.py` & `napari-clemreg-0.0.1a4/napari_clemreg/widgets/warp_image_volume.py`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg.egg-info/PKG-INFO` & `napari-clemreg-0.0.1a4/napari_clemreg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-clemreg
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A plugin for registering multimodal image volumes based on common segmented structures of interest with point-clouds.
 Home-page: https://github.com/krentzd/napari-clemreg
 Author: Daniel Krentzel
 Author-email: dkrentzel@pm.me
 License: MIT
 Project-URL: Bug Tracker, https://github.com/krentzd/napari-clemreg/issues
 Project-URL: Documentation, https://github.com/krentzd/napari-clemreg#README.md
```

### Comparing `napari-clemreg-0.0.1a3/napari_clemreg.egg-info/SOURCES.txt` & `napari-clemreg-0.0.1a4/napari_clemreg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-clemreg-0.0.1a3/setup.cfg` & `napari-clemreg-0.0.1a4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-clemreg
-version = 0.0.1a3
+version = 0.0.1a4
 author = Daniel Krentzel
 author_email = dkrentzel@pm.me
 license = MIT
 url = https://github.com/krentzd/napari-clemreg
 description = A plugin for registering multimodal image volumes based on common segmented structures of interest with point-clouds.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `napari-clemreg-0.0.1a3/tox.ini` & `napari-clemreg-0.0.1a4/tox.ini`

 * *Files identical despite different names*

