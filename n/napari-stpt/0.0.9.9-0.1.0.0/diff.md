# Comparing `tmp/napari-stpt-0.0.9.9.tar.gz` & `tmp/napari-stpt-0.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.0.9.9.tar", last modified: Thu Feb 23 13:09:45 2023, max compression
+gzip compressed data, was "napari-stpt-0.1.0.0.tar", last modified: Wed May 10 16:59:06 2023, max compression
```

## Comparing `napari-stpt-0.0.9.9.tar` & `napari-stpt-0.1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-02-23 13:09:45.669367 napari-stpt-0.0.9.9/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.0.9.9/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-02-23 13:09:45.668367 napari-stpt-0.0.9.9/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.0.9.9/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-02-23 13:09:45.627366 napari-stpt-0.0.9.9/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.0.9.9/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.0.9.9/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)   122969 2023-02-01 18:00:26.000000 napari-stpt-0.0.9.9/napari_stpt/napari_stpt.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-02-23 13:09:45.665367 napari-stpt-0.0.9.9/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       85 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-02-23 13:09:45.000000 napari-stpt-0.0.9.9/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-02-23 13:09:45.670367 napari-stpt-0.0.9.9/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1301 2023-02-23 13:09:06.000000 napari-stpt-0.0.9.9/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 16:59:06.423996 napari-stpt-0.1.0.0/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.0/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-10 16:59:06.420996 napari-stpt-0.1.0.0/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.0/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 16:59:06.286994 napari-stpt-0.1.0.0/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.0/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.0/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)   138850 2023-05-10 16:55:25.000000 napari-stpt-0.1.0.0/napari_stpt/napari_stpt.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 16:59:06.413996 napari-stpt-0.1.0.0/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       78 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-05-10 16:59:06.000000 napari-stpt-0.1.0.0/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-05-10 16:59:06.424996 napari-stpt-0.1.0.0/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1283 2023-05-10 16:58:57.000000 napari-stpt-0.1.0.0/setup.py
```

### Comparing `napari-stpt-0.0.9.9/LICENSE` & `napari-stpt-0.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.0.9.9/PKG-INFO` & `napari-stpt-0.1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.0.9.9
+Version: 0.1.0.0
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.0.9.9/README.md` & `napari-stpt-0.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.0.9.9/napari_stpt/napari_stpt.py` & `napari-stpt-0.1.0.0/napari_stpt/napari_stpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 """
 
 import os
 import sys
 import napari
 import numpy as np
 import xarray as xr
-from qtpy import QtCore, QtWidgets
-from qtpy.QtWidgets import QComboBox, QApplication, QCompleter, QMessageBox
-from qtpy.QtCore import QSortFilterProxyModel, Qt
-#from qtpy.QtCore.Qt import QStringListModel
+
+
+if 'PyQt5' in sys.modules:
+    from qtpy import QtCore, QtWidgets
+    from qtpy.QtWidgets import QComboBox, QApplication, QCompleter, QMessageBox
+    from qtpy.QtCore import QSortFilterProxyModel, Qt
+else:
+    from PySide2 import QtCore, QtWidgets, QtGui
+    from PySide2.QtWidgets import QComboBox, QApplication, QCompleter, QMessageBox
+    from PySide2.QtCore import QSortFilterProxyModel, Qt
+ 
 import SimpleITK as sitk
 from scipy import ndimage, stats
 import cv2
 #from stardist.models import StarDist2D
 from napari_animation import AnimationWidget
 from PIL import Image, ImageDraw
 import random
@@ -22,14 +29,15 @@
 # from stardist.models import StarDist3D
 #from csbdeep.utils import normalize
 #from naparimovie import Movie
 import math
 import gc
 import json
 import tifffile
+import pandas as pd
 
 
 
 class ExtendedComboBox(QComboBox):
     def __init__(self, parent=None):
         super(ExtendedComboBox, self).__init__(parent)
 
@@ -93,15 +101,15 @@
         self.aligned_1 = None
         self.aligned_2 = None
         self.aligned_3 = None
         self.aligned_4 = None
         self.current_output_resolution = None
 
         self.cb_R_Axio = None
-        self.cb_R_Old = None
+        # self.cb_R_Old = None
         self.cb_R_New = None
         self.spacing = [0,0,0]
 
         self.cb_perspective = None
         self.cb_isometric = None
         
         self.origin_x = None
@@ -255,61 +263,158 @@
 
         width = np.mean([size_x, size_y, size_z]) / 500
         
         output_resolution = float(self.pixel_size.text())
         scale_x = float(self.slice_spacing)/float(self.optical_slices) / output_resolution
         self.viewer.add_shapes(np.asarray(line_locations), name = 'bounding box',shape_type='line', scale=(scale_x, 1, 1), edge_color = "white", edge_width = width)
 
-
     def Load(self, text):
+        
+
+        def AlignAXIO(axio_volume, sample_name, slice_names, resolution):
+            
+            sample_name = sample_name[:-5]
+            
+            new_volume = np.zeros(axio_volume.shape)
+
+            df = pd.read_parquet(f"/home/tristan/Shared/imaxt_reg/{sample_name}/{sample_name}_EXT_AXIO_STPT_all_reg.parquet", engine='pyarrow')
+
+            filtered_df = df[(df['ranking'] == 1) & ((df['FLAG'] == 1) | (df['FLAG'] == 0))]
+            #filtered_df = df[(df['ranking'] == 1)]
+            
+            for index, element in enumerate(slice_names):
+                
+                row = filtered_df[filtered_df['D_S'] == element]
+                
+                if not row.empty:
+
+                    axio_location = int(row.iloc[0, 4][1:]) - 1
+
+                    axio_image = axio_volume[index,:,:]
+
+                    #flip image
+                    if row.iloc[0, 8] == 0.0:
+                        axio_image = axio_image[::-1,:]
+                    if row.iloc[0, 8] == 1.0:
+                        axio_image = axio_image[:,::-1]
+
+                    axio_image = np.asarray(axio_image)
+
+                    M = np.array([[row.iloc[0, 24], row.iloc[0, 25], row.iloc[0, 26]/resolution], [row.iloc[0, 27], row.iloc[0, 28], row.iloc[0, 29]/resolution]])
+
+                    rows, cols = axio_image.shape
+                    affine_np_img = cv2.warpAffine(axio_image, M[:2,:], (cols, rows))
+
+                    new_volume[axio_location,:,:] = affine_np_img
+
+            return new_volume
+
         verbose = True
 
-        # Remove previous bounding box
-        if any(i.name == 'bounding box' for i in self.viewer.layers):
-            self.viewer.layers.remove('bounding box')
+        load_in_reference = False
+        
+        
+        if self.aligned_1 is not None or self.aligned_2 is not None or self.aligned_3 is not None or self.aligned_4 is not None:
+            msgBox = QMessageBox()
+            msgBox.setText("Loading...")
+            msgBox.setInformativeText("Load in current reference space?")
+            msgBox.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
+            msgBox.setDefaultButton(QMessageBox.Yes)
+            reply = msgBox.exec_()
+            if reply == QMessageBox.Yes:
+                load_in_reference = True
+                reference_spacing = self.spacing
+    
 
+        if load_in_reference:
+            try:
+                reference_size = self.aligned_1.shape
+            except Exception:
+                pass
+            try:
+                reference_size = self.aligned_2.shape
+            except Exception:
+                pass
+            try:
+                reference_size = self.aligned_3.shape
+            except Exception:
+                pass
+            try:
+                reference_size = self.aligned_4.shape
+            except Exception:
+                pass
+            
+            if verbose:
+                print(f"reference_size: {reference_size}")
+    
+            
         # Remove previous volumes
         try:
-            self.viewer.layers.remove('C1')
+            if not load_in_reference:
+                self.viewer.layers.remove('C1')
             del self.aligned_1
             self.aligned_1 = None
         except Exception:
             pass
         try:
-            self.viewer.layers.remove('C2')
+            if not load_in_reference:
+                self.viewer.layers.remove('C2')
             del self.aligned_2
             self.aligned_2 = None
         except Exception:
             pass
         try:
-            self.viewer.layers.remove('C3')
+            if not load_in_reference:
+                self.viewer.layers.remove('C3')
             del self.aligned_3
             self.aligned_3 = None
         except Exception:
             pass
         try:
-            self.viewer.layers.remove('C4')
+            if not load_in_reference:
+                self.viewer.layers.remove('C4')
             del self.aligned_4
             self.aligned_4 = None
         except Exception:
             pass
 
         # Clear memory
         gc.collect()
 
-        # Pring file to read
-        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
-        self.default_contrast_limits = [0,30]
-        self.thresholdN.setText("0.3")
-        self.channels_start = 1
+        
+        
+        for folder in self.image_folders:
+    
+            if folder == '/data/meds1_c/storage/processed0/stpt/':
+                self.old_method = True
+            else:
+                self.old_method = False
+                
+            file_name = folder + str(self.comboBoxPath.currentText()) + '/mos'
+            if os.path.exists(file_name):
+                self.image_folder = folder
+                break
+            file_name = folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+            if os.path.exists(file_name):
+                self.image_folder = folder
+                break
+                     
+        if verbose:
+            print(f"folder location: " + self.image_folder)
+            
+        
+        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
+        self.default_contrast_limits = [0,30000]
+        self.thresholdN.setText("1000")
+        self.channels_start = 0
         if not os.path.exists(file_name):
-            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
-            self.default_contrast_limits = [0,30000]
-            self.thresholdN.setText("1000")
-            self.channels_start = 0
+            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+            self.default_contrast_limits = [0,30]
+            self.thresholdN.setText("0.3")
+            self.channels_start = 1
         print(file_name)
 
         # Try to read only the meta data using the consolidated flag as True
         # Currently not used
         try:
             self.ds1 = xr.open_zarr(file_name, consolidated=False)
             # print("not trying consolidated")
@@ -325,17 +430,23 @@
             self.spacing = [0,0]
             try:
                 self.spacing[0] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["x"])
                 self.spacing[1] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["y"])
                 # self.spacing[2] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["z"])
             except:
                 print("spacing not defined")
-
+                
+                
+        if load_in_reference:
+            self.spacing = reference_spacing
+            
+            
+                
         if verbose:
-            print(f"spacing ({self.spacing[0]}, {self.spacing[1]}")
+            print(f"spacing ({self.spacing[0]}, {self.spacing[1]})")
 
         # Read the parameters to convert the voxel values (bscale and bzero)
         if self.old_method:
             self.bscale = self.ds1.attrs['bscale']
             self.bzero = self.ds1.attrs['bzero']
         else:
             try:
@@ -575,14 +686,15 @@
                 msg.setWindowTitle("Error")
                 msg.setStandardButtons(QMessageBox.Ok)
                 retval = msg.exec_()
                 return
             
             if self.axio:
                 volume_1_temp = volume_1_temp[:,0,:,:]
+                volume_1_temp = AlignAXIO(volume_1_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
             
             volume_1[0::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
             
             for optical_slice in range(1, self.optical_slices):
                 # volume_1_temp = (ds.sel(channel=self.channels_start, type='mosaic', z=optical_slice).to_array(
                 # ).data * self.bscale + self.bzero).astype(dtype=np.float32)
                 # volume_1[optical_slice::self.optical_slices, :, :] = volume_1_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
@@ -598,17 +710,25 @@
 
             # Normalize the brightness changes between optical sections
             if self.cb_correct_brightness_optical_section.isChecked():
                 print("correcting brightness of optical sections C1")
                 self.Normalize_slices(volume_1, self.optical_slices)
 
             print("aligning C1")
-            self.aligned_1 = self.AlignNew(volume_1, resolution, output_resolution, start_slice_number*self.optical_slices)
+            self.aligned_1 = self.AlignNew(volume_1, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+            
+            if load_in_reference:
+                self.aligned_1 = self.aligned_1[:,0:reference_size[1],0:reference_size[2]]
+                
             self.aligned_1 = self.aligned_1[chop_bottom:self.aligned_1.shape[0]-chop_top,:,:]
             self.shape = self.aligned_1.shape
+            
+            if verbose:
+                print(f"self.shape {self.shape}")
+            
             self.viewer.add_image([self.aligned_1], name='C1', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
                                   blending='additive', colormap='bop purple', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C2.isChecked():
             print("loading C2")
             
             if self.axio:
@@ -655,14 +775,15 @@
                 msg.setWindowTitle("Error")
                 msg.setStandardButtons(QMessageBox.Ok)
                 retval = msg.exec_()
                 return
             
             if self.axio:
                 volume_2_temp = volume_2_temp[:,0,:,:]
+                volume_2_temp = AlignAXIO(volume_2_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
             
             volume_2[0::self.optical_slices, :, :] = volume_2_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
             for optical_slice in range(1, self.optical_slices):
                 
                 try:
                     volume_2_temp = (ds.sel(channel=self.channels_start + 1, type='mosaic', z=optical_slice).to_array(
@@ -677,15 +798,19 @@
 
             # Normalize the brightness changes between optical sections
             if self.cb_correct_brightness_optical_section.isChecked():
                 print("correcting brightness of optical sections C2")
                 self.Normalize_slices(volume_2, self.optical_slices)
 
             print("aligning C2")
-            self.aligned_2 = self.AlignNew(volume_2, resolution, output_resolution, start_slice_number*self.optical_slices)
+            self.aligned_2 = self.AlignNew(volume_2, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+            
+            if load_in_reference:
+                self.aligned_2 = self.aligned_2[:,0:reference_size[1],0:reference_size[2]]
+                
             self.aligned_2 = self.aligned_2[chop_bottom:self.aligned_2.shape[0]-chop_top,:,:]
             self.shape = self.aligned_2.shape
             self.viewer.add_image([self.aligned_2], name='C2', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
                                   blending='additive', colormap='red', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C3.isChecked():
             print("loading C3")
@@ -742,14 +867,15 @@
                 msg.setWindowTitle("Error")
                 msg.setStandardButtons(QMessageBox.Ok)
                 retval = msg.exec_()
                 return
             
             if self.axio:
                 volume_3_temp = volume_3_temp[:,0,:,:]
+                volume_3_temp = AlignAXIO(volume_3_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
             
             volume_3[0::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
             
             for optical_slice in range(1, self.optical_slices):
 #                 volume_3_temp = (ds.sel(channel=self.channels_start + 2, type='mosaic', z=optical_slice).to_array(
 #                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
 #                 volume_3[optical_slice::self.optical_slices, :, :] = volume_3_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
@@ -765,15 +891,19 @@
 
             # Normalize the brightness changes between optical sections
             if self.cb_correct_brightness_optical_section.isChecked():
                 print("correcting brightness of optical sections C3")
                 self.Normalize_slices(volume_3, self.optical_slices)
 
             print("aligning C3")
-            self.aligned_3 = self.AlignNew(volume_3, resolution, output_resolution, start_slice_number*self.optical_slices)
+            self.aligned_3 = self.AlignNew(volume_3, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+            
+            if load_in_reference:
+                self.aligned_3 = self.aligned_3[:,0:reference_size[1],0:reference_size[2]]
+                
             self.aligned_3 = self.aligned_3[chop_bottom:self.aligned_3.shape[0]-chop_top,:,:]
             self.shape = self.aligned_3.shape
             self.viewer.add_image([self.aligned_3], name='C3', scale=(float(self.slice_spacing)/float(self.optical_slices) / output_resolution, 1, 1), 
                                   blending='additive', colormap='green', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C4.isChecked():
             print("loading C4")
@@ -821,14 +951,15 @@
                 msg.setWindowTitle("Error")
                 msg.setStandardButtons(QMessageBox.Ok)
                 retval = msg.exec_()
                 return
             
             if self.axio:
                 volume_4_temp = volume_4_temp[:,0,:,:]
+                volume_4_temp = AlignAXIO(volume_4_temp, str(self.comboBoxPath.currentText()), self.slice_names, resolution)
             
             volume_4[0::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
 
             for optical_slice in range(1, self.optical_slices):
 #                 volume_4_temp = (ds.sel(channel=self.channels_start + 3, type='mosaic', z=optical_slice).to_array(
 #                 ).data * self.bscale + self.bzero).astype(dtype=np.float32)
 #                 volume_4[optical_slice::self.optical_slices, :, :] = volume_4_temp[start_slice_number:end_slice_number+1, start_y:start_y+size_y, start_z:start_z+size_z]
@@ -844,15 +975,19 @@
 
             # Normalize the brightness changes between optical sections
             if self.cb_correct_brightness_optical_section.isChecked():
                 print("correcting brightness of optical sections C4")
                 self.Normalize_slices(volume_4, self.optical_slices)
 
             print("aligning C4")
-            self.aligned_4 = self.AlignNew(volume_4, resolution, output_resolution, start_slice_number*self.optical_slices)
+            self.aligned_4 = self.AlignNew(volume_4, resolution, output_resolution, start_slice_number*self.optical_slices, self.spacing)
+            
+            if load_in_reference:
+                self.aligned_4 = self.aligned_4[:,0:reference_size[1],0:reference_size[2]]
+            
             self.aligned_4 = self.aligned_4[chop_bottom:self.aligned_4.shape[0]-chop_top,:,:]
             self.shape = self.aligned_4.shape
             self.viewer.add_image([self.aligned_4], name='C4', scale=((float(self.slice_spacing)/float(self.optical_slices)) / output_resolution, 1, 1), 
                                   blending='additive', colormap='bop blue', contrast_limits=self.default_contrast_limits)
 
         spacing_loaded = [float(self.slice_spacing)/float(self.optical_slices), output_resolution, output_resolution]
 
@@ -1030,138 +1165,194 @@
         else:
             slice_name = f"S{(z+1):03d}"
         
         
         if self.cb_C1.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
             
             self.layerC1.data = [im1, im2, im4, im8, im16, im32]
 
             # self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
             #                           name='C1', blending='additive', colormap='bop purple', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C2.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
 
             self.layerC2.data = [im1, im2, im4, im8, im16, im32]
             
             # self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
             #                             name='C2', blending='additive', colormap='red', contrast_limits=self.default_contrast_limits)
                 
 
         if self.cb_C3.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
 
             self.layerC3.data = [im1, im2, im4, im8, im16, im32]
             
             # self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
             #                           name='C3', blending='additive', colormap='green', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C4.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
 
             self.layerC4.data = [im1, im2, im4, im8, im16, im32]
             
             # self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
             #                           name='C4', blending='additive', colormap='bop blue', contrast_limits=self.default_contrast_limits)
         
 
@@ -1198,23 +1389,23 @@
             self.viewer.layers.remove('C4')
             del self.aligned_4
             self.aligned_4 = None
         except Exception:
             pass
 
         
-        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
-        self.default_contrast_limits = [0,30]
-        self.thresholdN.setText("0.3")
-        self.channels_start = 1
+        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
+        self.default_contrast_limits = [0,30000]
+        self.thresholdN.setText("1000")
+        self.channels_start = 0
         if not os.path.exists(file_name):
-            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
-            self.default_contrast_limits = [0,30000]
-            self.thresholdN.setText("1000")
-            self.channels_start = 0
+            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+            self.default_contrast_limits = [0,30]
+            self.thresholdN.setText("0.3")
+            self.channels_start = 1
         print(file_name)
         
         self.ds1 = xr.open_zarr(file_name)
         self.ds2 = xr.open_zarr(file_name, group='l.2')
         self.ds4 = xr.open_zarr(file_name, group='l.4')
         self.ds8 = xr.open_zarr(file_name, group='l.8')
         self.ds16 = xr.open_zarr(file_name, group='l.16')
@@ -1264,132 +1455,188 @@
             slice_name = f"S{(z+1):03d}"
             
         print("slice_name: " + slice_name)
 
         if self.cb_C1.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start).data * self.bscale + self.bzero).squeeze()
                 
             self.layerC1 = self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
                                       name='C1', blending='additive', colormap='bop purple', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C2.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 1, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 1, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 1).data * self.bscale + self.bzero).squeeze()
 
             self.layerC2 = self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
                                         name='C2', blending='additive', colormap='red', contrast_limits=self.default_contrast_limits)
                 
 
         if self.cb_C3.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 2, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 2, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 2).data * self.bscale + self.bzero).squeeze()
 
             self.layerC3 = self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
                                       name='C3', blending='additive', colormap='green', contrast_limits=self.default_contrast_limits)
 
         if self.cb_C4.isChecked():
             try:
                 im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
                 im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero)
+                    channel=self.channels_start + 3, type='mosaic', z=optical_slice).data * self.bscale + self.bzero).squeeze()
             except:
-                im1 = (self.ds1[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im2 = (self.ds2[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im4 = (self.ds4[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im8 = (self.ds8[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im16 = (self.ds16[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
-                im32 = (self.ds32[slice_name].sel(
-                    channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero)
+                try:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 3, z=optical_slice).data * self.bscale + self.bzero).squeeze()
+                except:
+                    im1 = (self.ds1[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im2 = (self.ds2[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im4 = (self.ds4[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im8 = (self.ds8[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im16 = (self.ds16[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
+                    im32 = (self.ds32[slice_name].sel(
+                        channel=self.channels_start + 3).data * self.bscale + self.bzero).squeeze()
 
             self.layerC4 = self.viewer.add_image([im1, im2, im4, im8, im16, im32], multiscale=True,
                                       name='C4', blending='additive', colormap='bop blue', contrast_limits=self.default_contrast_limits)
         
         self.loaded_2D = True
         self.loaded_3D = False
 
@@ -1454,37 +1701,38 @@
 
             np_out = sitk.GetArrayFromImage(out)
             aligned[z, :, :] = np_out
 
         return aligned.astype(dtype=np.float32)
 
 
-    def AlignNew(self, volume, resolution, output_resolution, start_slice_number):
-
+    def AlignNew(self, volume, resolution, output_resolution, start_slice_number, current_spacing):
+        print("------------------------------------------------------------------------")
+        print(f"spacing({self.spacing[0]}, {self.spacing[1]})")
         size_multiplier = (resolution*0.1*self.spacing[0])/output_resolution
         size = (volume.shape[0], int(size_multiplier*volume.shape[1]), int(size_multiplier*volume.shape[2]))
         aligned = np.zeros(size, dtype=np.float32)
         size2D = (int(size_multiplier*volume.shape[2]), int(size_multiplier*volume.shape[1]))
 
         z_size = volume.shape[0]
         
         for z in range(0, z_size):
 
             fixed = sitk.GetImageFromArray(volume[z, :, :])
             fixed.SetOrigin((0, 0))
 
 
             slice_name = self.slice_names[z+start_slice_number]
-            if self.old_method:
-                current_spacing = (self.ds1[slice_name].attrs['scale'])
-            else:
-                current_spacing = [0,0,0]
-                current_spacing[0] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["x"])
-                current_spacing[1] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["y"])
-                #current_spacing[2] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["z"])
+            # if self.old_method:
+            #     current_spacing = (self.ds1[slice_name].attrs['scale'])
+            # else:
+            #     current_spacing = [0,0,0]
+            #     current_spacing[0] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["x"])
+            #     current_spacing[1] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["y"])
+            #     #current_spacing[2] = 10 * float(json.loads(self.ds1[slice_name].attrs['scale'])["z"])
 
             fixed.SetSpacing([resolution*0.1*current_spacing[1],resolution*0.1*current_spacing[0]])
 
             transform = sitk.Euler2DTransform()
             
             
             align_pos = z + start_slice_number
@@ -1871,22 +2119,44 @@
 
         self.viewer.layers['Shapes'].visible = False
 
 
 
     def on_combobox_changed(self):
         
+        for folder in self.image_folders:
+    
+            if folder == '/data/meds1_c/storage/processed0/stpt/':
+                self.old_method = True
+            else:
+                self.old_method = False
+                
+            file_name = folder + str(self.comboBoxPath.currentText()) + '/mos'
+            if os.path.exists(file_name):
+                self.image_folder = folder
+                break
+            file_name = folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+            if os.path.exists(file_name):
+                self.image_folder = folder
+                break
+                     
+        print(f"folder location: " + self.image_folder)
+            
+            
 
-        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
-        self.default_contrast_limits = [0,30]
-        self.thresholdN.setText("0.3")
+        file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
+        self.default_contrast_limits = [0,30000]
+        self.thresholdN.setText("1000")
+        self.channels_start = 0
         if not os.path.exists(file_name):
-            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
-            self.default_contrast_limits = [0,30000]
-            self.thresholdN.setText("1000")
+            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+            self.default_contrast_limits = [0,30]
+            self.thresholdN.setText("0.3")
+            self.channels_start = 1
+        print(file_name)
         
         
         if os.path.exists(file_name + '/.zmetadata'):
             print("metadata is available")
             
             try:
                 ds = xr.open_zarr(file_name, consolidated=True)
@@ -2104,23 +2374,24 @@
             slice_name = self.slice_names[z]
 
 
             output_resolution = float(self.pixel_size.text())
             spacing = (output_resolution, output_resolution)
 
             
-            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
-            self.default_contrast_limits = [0,30]
-            self.thresholdN.setText("0.3")
-            self.channels_start = 1
+            file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
+            self.default_contrast_limits = [0,30000]
+            self.thresholdN.setText("1000")
+            self.channels_start = 0
             if not os.path.exists(file_name):
-                file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos'
-                self.default_contrast_limits = [0,30000]
-                self.thresholdN.setText("1000")
-                self.channels_start = 0
+                file_name = self.image_folder + str(self.comboBoxPath.currentText()) + '/mos.zarr'
+                self.default_contrast_limits = [0,30]
+                self.thresholdN.setText("0.3")
+                self.channels_start = 1
+            print(file_name)
                 
             ds32 = xr.open_zarr(file_name, group='l.32')
             im32 = (ds32[slice_name].sel(
                 channel=self.channels_start + 2, type='mosaic', z=0).data * self.bscale + self.bzero).astype(dtype=np.float32)
 
             image_itk = sitk.GetImageFromArray(im32)
             image_itk.SetSpacing(spacing)
@@ -2269,43 +2540,46 @@
                 self.comboBoxPath.addItem(i)
         
     def MethodChanged(self):
 
         if self.cb_R_Axio.isChecked():
             self.old_method = False
             self.axio = True
-            self.image_folder = '/storage/processed/axio/'
+            self.image_folders = {
+                '/storage/imaxt.processed.2022/axio/',
+                '/storage/processed.2022/axio/',
+            }
             print("setting axio method")
-        elif self.cb_R_Old.isChecked():
-            self.old_method = True
-            self.axio = False
-            self.image_folder = '/data/meds1_c/storage/processed0/stpt/'
-            print("setting old method")
         else:
             self.old_method = False
             self.axio = False
-            self.image_folder = '/storage/processed/stpt/'
-            print("setting new method")
+            self.image_folders = {
+                '/storage/processed.2022/stpt/',
+                '/storage/processed/stpt/',
+                '/storage/imaxt.processed.2022/stpt/',
+                '/data/meds1_c/storage/processed0/stpt/'
+            }
+            print("setting STPT method")
 
         file_list = []
-
-        print(sys.platform)
-        if sys.platform == 'linux':
-            self.search_folder = QtWidgets.QLineEdit(self.image_folder)
-            if os.path.exists(self.search_folder.text()):
-                for f in os.scandir(self.search_folder.text()):
-                    if f.is_dir():
-                        if os.path.exists(f.path + "/mos.zarr"):
-                            s = f.path
-                            s = s.replace(self.search_folder.text(), '')
-                            file_list.append(s)
-                        elif os.path.exists(f.path + "/mos"):
-                            s = f.path
-                            s = s.replace(self.search_folder.text(), '')
-                            file_list.append(s)
+        for folder in self.image_folders:
+            print(sys.platform)
+            if sys.platform == 'linux':
+                self.search_folder = QtWidgets.QLineEdit(folder)
+                if os.path.exists(self.search_folder.text()):
+                    for f in os.scandir(self.search_folder.text()):
+                        if f.is_dir():
+                            if os.path.exists(f.path + "/mos.zarr"):
+                                s = f.path
+                                s = s.replace(self.search_folder.text(), '')
+                                file_list.append(s)
+                            elif os.path.exists(f.path + "/mos"):
+                                s = f.path
+                                s = s.replace(self.search_folder.text(), '')
+                                file_list.append(s)
                                 
         else:
             self.search_folder = QtWidgets.QLineEdit('N:/stpt/')
         
         print(file_list)
 
         file_list.sort()
@@ -2372,28 +2646,28 @@
         widget = QtWidgets.QWidget()
         layout = QtWidgets.QVBoxLayout()
         vbox = QtWidgets.QVBoxLayout()
 
         cb_group1 = QtWidgets.QButtonGroup()
         hbox = QtWidgets.QHBoxLayout()
         hbox.addStretch(1)
-        self.cb_R_Axio = QtWidgets.QRadioButton('Axio')
+        self.cb_R_Axio = QtWidgets.QRadioButton('AXI')
         self.cb_R_Axio.setChecked(False)
         self.cb_R_Axio.toggled.connect(self.MethodChanged)
         hbox.addWidget(self.cb_R_Axio)
-        self.cb_R_Old = QtWidgets.QRadioButton('STPT Old')
-        self.cb_R_Old.setChecked(False)
-        self.cb_R_Old.toggled.connect(self.MethodChanged)
-        hbox.addWidget(self.cb_R_Old)
-        self.cb_R_New = QtWidgets.QRadioButton('STPT New')
+        # self.cb_R_Old = QtWidgets.QRadioButton('STPT Old')
+        # self.cb_R_Old.setChecked(False)
+        # self.cb_R_Old.toggled.connect(self.MethodChanged)
+        # hbox.addWidget(self.cb_R_Old)
+        self.cb_R_New = QtWidgets.QRadioButton('STPT')
         self.cb_R_New.setChecked(True)
         self.cb_R_New.toggled.connect(self.MethodChanged)
         hbox.addWidget(self.cb_R_New)
         cb_group1.addButton(self.cb_R_Axio)
-        cb_group1.addButton(self.cb_R_Old)
+        # cb_group1.addButton(self.cb_R_Old)
         cb_group1.addButton(self.cb_R_New)
         
         bSelectFolder = QtWidgets.QPushButton('Select folder')
         bSelectFolder.clicked.connect(self.SelectFolder)
         hbox.addWidget(bSelectFolder)
         
         hbox.addStretch(1)
@@ -2401,28 +2675,34 @@
         
         
         
         
         hbox = QtWidgets.QHBoxLayout()
         self.comboBoxPath = ExtendedComboBox()
 
-        self.image_folder = '/storage/processed/stpt/'
+        self.image_folders = {
+            '/storage/processed.2022/stpt/',
+            '/storage/processed/stpt/',
+            '/storage/imaxt.processed.2022/stpt/',
+            '/data/meds1_c/storage/processed0/stpt/'
+        }
         file_list = []
-        self.search_folder = QtWidgets.QLineEdit(self.image_folder)
-        if os.path.exists(self.search_folder.text()):
-            for f in os.scandir(self.search_folder.text()):
-                if f.is_dir():
-                    if os.path.exists(f.path + "/mos.zarr"):
-                        s = f.path
-                        s = s.replace(self.search_folder.text(), '')
-                        file_list.append(s)
-                    elif os.path.exists(f.path + "/mos"):
-                        s = f.path
-                        s = s.replace(self.search_folder.text(), '')
-                        file_list.append(s)
+        for folder in self.image_folders:
+            self.search_folder = QtWidgets.QLineEdit(folder)
+            if os.path.exists(self.search_folder.text()):
+                for f in os.scandir(self.search_folder.text()):
+                    if f.is_dir():
+                        if os.path.exists(f.path + "/mos.zarr"):
+                            s = f.path
+                            s = s.replace(self.search_folder.text(), '')
+                            file_list.append(s)
+                        elif os.path.exists(f.path + "/mos"):
+                            s = f.path
+                            s = s.replace(self.search_folder.text(), '')
+                            file_list.append(s)
 
         
         file_list.sort()
         
         self.axio = False
 
         self.comboBoxPath.clear()
```

### Comparing `napari-stpt-0.0.9.9/napari_stpt.egg-info/PKG-INFO` & `napari-stpt-0.1.0.0/napari_stpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.0.9.9
+Version: 0.1.0.0
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.0.9.9/setup.py` & `napari-stpt-0.1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.0.9.9",
+    version="0.1.0.0",
     description="napari viewer which can read stpt images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
@@ -30,15 +30,14 @@
     ],
     packages=["napari_stpt"],
     include_package_data=True,
     install_requires=[
         'opencv-python==4.5.1.48',
         'napari',
         'numpy',
-        'xarray',
+        'zarr',
         'SimpleITK',
-        'qtpy',
         'napari-animation',
         'tifffile'
     ],
     entry_points={"console_scripts": ["napari-stpt=napari_stpt.__main__:main"]},
 )
```

