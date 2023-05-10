# Comparing `tmp/skylibs-0.7.2.tar.gz` & `tmp/skylibs-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skylibs-0.7.2.tar", last modified: Fri Nov  4 16:36:30 2022, max compression
+gzip compressed data, was "skylibs-0.7.3.tar", last modified: Wed May 10 16:55:09 2023, max compression
```

## Comparing `skylibs-0.7.2.tar` & `skylibs-0.7.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.699386 skylibs-0.7.2/
--rw-rw-rw-   0        0        0     7370 2021-05-18 02:18:22.000000 skylibs-0.7.2/LICENSE
--rw-rw-rw-   0        0        0      327 2022-11-04 16:36:30.699386 skylibs-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     7089 2022-11-04 16:36:00.000000 skylibs-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.687064 skylibs-0.7.2/envmap/
--rw-rw-rw-   0        0        0      138 2022-04-24 22:04:07.000000 skylibs-0.7.2/envmap/__init__.py
--rw-rw-rw-   0        0        0    24033 2022-04-26 01:35:39.000000 skylibs-0.7.2/envmap/environmentmap.py
--rw-rw-rw-   0        0        0     7890 2022-04-26 03:39:30.000000 skylibs-0.7.2/envmap/projections.py
--rw-rw-rw-   0        0        0      932 2021-06-13 20:35:56.000000 skylibs-0.7.2/envmap/rotations.py
--rw-rw-rw-   0        0        0      565 2021-05-18 02:18:22.000000 skylibs-0.7.2/envmap/test_environmentmap.py
--rw-rw-rw-   0        0        0     1322 2021-05-18 02:18:22.000000 skylibs-0.7.2/envmap/tetrahedronSolidAngle.py
--rw-rw-rw-   0        0        0     1040 2021-05-18 02:18:22.000000 skylibs-0.7.2/envmap/xmlhelper.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.687351 skylibs-0.7.2/ezexr/
--rw-rw-rw-   0        0        0     9216 2022-10-29 21:57:14.000000 skylibs-0.7.2/ezexr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.687811 skylibs-0.7.2/hdrio/
--rw-rw-rw-   0        0        0     4111 2022-10-29 21:57:14.000000 skylibs-0.7.2/hdrio/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.689102 skylibs-0.7.2/hdrtools/
--rw-rw-rw-   0        0        0      118 2022-10-29 21:57:14.000000 skylibs-0.7.2/hdrtools/__init__.py
--rw-rw-rw-   0        0        0     2038 2021-05-18 02:18:22.000000 skylibs-0.7.2/hdrtools/gsolve.py
--rw-rw-rw-   0        0        0     4025 2022-10-29 21:57:14.000000 skylibs-0.7.2/hdrtools/sunutils.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.690368 skylibs-0.7.2/hdrtools/tonemapping/
--rw-rw-rw-   0        0        0     4025 2021-05-18 02:18:22.000000 skylibs-0.7.2/hdrtools/tonemapping/__init__.py
--rw-rw-rw-   0        0        0      108 2021-10-09 06:14:32.000000 skylibs-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       86 2022-11-04 16:36:30.699386 skylibs-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      752 2022-04-24 22:13:30.000000 skylibs-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.690610 skylibs-0.7.2/skydb/
--rw-rw-rw-   0        0        0     5185 2021-05-18 02:18:22.000000 skylibs-0.7.2/skydb/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.691145 skylibs-0.7.2/skylibs/
--rw-rw-rw-   0        0        0       23 2022-11-04 16:33:54.000000 skylibs-0.7.2/skylibs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.696324 skylibs-0.7.2/skylibs.egg-info/
--rw-rw-rw-   0        0        0      327 2022-11-04 16:36:30.000000 skylibs-0.7.2/skylibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2022-11-04 16:36:30.000000 skylibs-0.7.2/skylibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-04 16:36:30.000000 skylibs-0.7.2/skylibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-11-04 16:36:30.000000 skylibs-0.7.2/skylibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       71 2022-11-04 16:36:30.000000 skylibs-0.7.2/skylibs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.697721 skylibs-0.7.2/test/
--rw-rw-rw-   0        0        0     7949 2022-04-26 03:41:14.000000 skylibs-0.7.2/test/test_envmap.py
--rw-rw-rw-   0        0        0      249 2022-05-28 18:37:10.000000 skylibs-0.7.2/test/test_sph.py
--rw-rw-rw-   0        0        0     2652 2022-10-29 21:57:14.000000 skylibs-0.7.2/test/test_sunutils.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:36:30.698985 skylibs-0.7.2/tools3d/
--rw-rw-rw-   0        0        0     4610 2021-05-18 02:18:22.000000 skylibs-0.7.2/tools3d/__init__.py
--rw-rw-rw-   0        0        0     1555 2021-05-18 02:18:22.000000 skylibs-0.7.2/tools3d/display.py
--rw-rw-rw-   0        0        0     2400 2021-05-18 02:18:22.000000 skylibs-0.7.2/tools3d/spharm.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.837750 skylibs-0.7.3/
+-rw-rw-rw-   0        0        0     7370 2021-05-18 02:18:22.000000 skylibs-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0      295 2023-05-10 16:55:09.837750 skylibs-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7155 2023-01-17 16:44:30.000000 skylibs-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.777128 skylibs-0.7.3/envmap/
+-rw-rw-rw-   0        0        0      138 2022-04-24 22:04:07.000000 skylibs-0.7.3/envmap/__init__.py
+-rw-rw-rw-   0        0        0    26904 2023-05-10 16:48:31.000000 skylibs-0.7.3/envmap/environmentmap.py
+-rw-rw-rw-   0        0        0     8532 2023-02-08 16:30:06.000000 skylibs-0.7.3/envmap/projections.py
+-rw-rw-rw-   0        0        0     1162 2023-02-08 16:30:21.000000 skylibs-0.7.3/envmap/rotations.py
+-rw-rw-rw-   0        0        0     1322 2021-05-18 02:18:22.000000 skylibs-0.7.3/envmap/tetrahedronSolidAngle.py
+-rw-rw-rw-   0        0        0     1040 2021-05-18 02:18:22.000000 skylibs-0.7.3/envmap/xmlhelper.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.777728 skylibs-0.7.3/ezexr/
+-rw-rw-rw-   0        0        0     9201 2023-03-20 16:12:57.000000 skylibs-0.7.3/ezexr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.778339 skylibs-0.7.3/hdrio/
+-rw-rw-rw-   0        0        0     4111 2022-12-21 14:34:07.000000 skylibs-0.7.3/hdrio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.788154 skylibs-0.7.3/hdrtools/
+-rw-rw-rw-   0        0        0      160 2023-02-08 17:01:07.000000 skylibs-0.7.3/hdrtools/__init__.py
+-rw-rw-rw-   0        0        0     2038 2021-05-18 02:18:22.000000 skylibs-0.7.3/hdrtools/gsolve.py
+-rw-rw-rw-   0        0        0     5046 2023-02-08 17:01:07.000000 skylibs-0.7.3/hdrtools/sunutils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.792289 skylibs-0.7.3/hdrtools/tonemapping/
+-rw-rw-rw-   0        0        0     4025 2021-05-18 02:18:22.000000 skylibs-0.7.3/hdrtools/tonemapping/__init__.py
+-rw-rw-rw-   0        0        0      108 2021-10-09 06:14:32.000000 skylibs-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-05-10 16:55:09.838876 skylibs-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      785 2022-12-21 14:33:15.000000 skylibs-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.795354 skylibs-0.7.3/skydb/
+-rw-rw-rw-   0        0        0     5389 2022-12-21 14:33:15.000000 skylibs-0.7.3/skydb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.796487 skylibs-0.7.3/skylibs/
+-rw-rw-rw-   0        0        0       23 2023-05-10 16:51:54.000000 skylibs-0.7.3/skylibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.808349 skylibs-0.7.3/skylibs.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-05-10 16:55:09.000000 skylibs-0.7.3/skylibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-05-10 16:55:09.000000 skylibs-0.7.3/skylibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:55:09.000000 skylibs-0.7.3/skylibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-10 16:55:09.000000 skylibs-0.7.3/skylibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       71 2023-05-10 16:55:09.000000 skylibs-0.7.3/skylibs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.826133 skylibs-0.7.3/test/
+-rw-rw-rw-   0        0        0      637 2023-05-10 16:50:16.000000 skylibs-0.7.3/test/test_blur.py
+-rw-rw-rw-   0        0        0    10992 2023-02-08 16:48:58.000000 skylibs-0.7.3/test/test_envmap.py
+-rw-rw-rw-   0        0        0     4108 2023-02-08 16:30:06.000000 skylibs-0.7.3/test/test_projections.py
+-rw-rw-rw-   0        0        0      249 2023-02-08 17:01:20.000000 skylibs-0.7.3/test/test_sph.py
+-rw-rw-rw-   0        0        0     7966 2023-02-08 17:01:07.000000 skylibs-0.7.3/test/test_sunutils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:09.837750 skylibs-0.7.3/tools3d/
+-rw-rw-rw-   0        0        0     4610 2021-05-18 02:18:22.000000 skylibs-0.7.3/tools3d/__init__.py
+-rw-rw-rw-   0        0        0     1555 2021-05-18 02:18:22.000000 skylibs-0.7.3/tools3d/display.py
+-rw-rw-rw-   0        0        0     2400 2021-05-18 02:18:22.000000 skylibs-0.7.3/tools3d/spharm.py
```

### Comparing `skylibs-0.7.2/LICENSE` & `skylibs-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/README.md` & `skylibs-0.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 - `.getHemisphere(normal)`: returns a mask of the hemisphere visible from a surface with `normal`.
 - `.setHemisphereValue(normal, value)`: sets all pixels visible from a surface with `normal` to `value`.
 - `.getMeanLightVectors(normals)`: compute the mean light vector of the environment map for the given normals.
 - `.project(vfov, rotation_matrix, ar, resolution, projection, mode)`: Extract a rectified image from the panorama, simulating a camera with field-of-view `vfov`, extrinsics `rotation_matrix`, aspect ratio `ar`, `resolution`.
 - `.embed(self, vfov, rotation_matrix, image)`: inverse of `project`, embeds an image in the environment map.
 - `.imageCoordinates()`: returns the (u, v) coordinates at each pixel center.
 - `.worldCoordinates()`: returns the (x, y, z, valid) world coordinates for each pixel center, with mask `valid` (anything outside this mask does not project to the world).
-- `.world2image(x, y, z)`: returns the (u, v) coordinates of the vector (x, y, z).
+- `.world2image(x, y, z)`: returns the (u, v) coordinates of the vector (x, y, z). Pixel coordinates can be obtained with `floor(u)` and `floor(v)`.
 - `.image2world(u, v)`: returns the (x, y, z) coordinates of the coordinates (u, v).
 - `.interpolate(u, v, valid)`: interpolates the envmap to coordinates (u, v) masked with valid.
 
 
 ### Projection, cropping, simulating a camera
 
 To perform a crop from `pano.jpg`:
```

### Comparing `skylibs-0.7.2/envmap/environmentmap.py` & `skylibs-0.7.3/envmap/environmentmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import pathlib
 from copy import deepcopy
 from decimal import Decimal
 
+from tqdm import tqdm
 import numpy as np
-from scipy.ndimage.interpolation import map_coordinates, zoom
+from scipy.ndimage import map_coordinates, zoom
 from skimage.transform import resize_local_mean, downscale_local_mean
 
 from hdrio import imread
-
 from .tetrahedronSolidAngle import tetrahedronSolidAngle
 from .projections import *
 from .xmlhelper import EnvmapXMLParser
 from .rotations import rotx, roty, rotz
 
 
 SUPPORTED_FORMATS = [
@@ -72,19 +72,19 @@
             # We received the filename
             self.data = imread(str(im))
         elif isinstance(im, int):
             # We received a single scalar
             if self.format_ == 'latlong':
                 self.data = np.zeros((im, im*2, channels))
             elif self.format_ == 'skylatlong':
-                    self.data = np.zeros((im, im*4, channels))
+                self.data = np.zeros((im, im*4, channels))
             elif self.format_ == 'cube':
                 self.data = np.zeros((im, round(3/4*im), channels))
             else:
-                    self.data = np.zeros((im, im, channels))
+                self.data = np.zeros((im, im, channels))
         elif type(im).__module__ == np.__name__:
             # We received a numpy array
             self.data = np.asarray(im, dtype='double')
 
             if copy:
                 self.data = self.data.copy()
         else:
@@ -102,15 +102,15 @@
                 "Sphere/Angular formats must have the same width/height")
         elif self.format_ == 'latlong':
             assert 2*self.data.shape[0] == self.data.shape[1], (
                 "LatLong format width should be twice the height")
         elif self.format_ == 'skylatlong':
             assert 4*self.data.shape[0] == self.data.shape[1], (
                 "SkyLatLong format width should be four times the height")
-        
+
         assert self.data.ndim == 3, "Expected 3-dim array. For grayscale, use [h,w,1]."
 
     @classmethod
     def fromSkybox(cls, top, bottom, left, right, front, back):
         """Create an environment map from skybox (cube) captures. Six images
         must be provided, one for each side of the virtual cube. This function
         will return an EnvironmentMap object.
@@ -220,19 +220,51 @@
             'latlong': world2latlong,
             'skylatlong': world2skylatlong,
             'sphere': world2sphere,
             'cube': world2cube,
         }.get(self.format_)
         return func(x, y, z)
 
+
+    def world2pixel(self, x, y, z):
+        """Returns the (u, v) coordinates (in the interval defined by the MxN image)."""
+
+        # Get (u,v) in [-1, 1] interval
+        u,v = self.world2image(x, y, z)
+
+        # de-Normalize coordinates to interval defined by the MxN image
+        u = np.floor(u*self.data.shape[1]).astype(int)
+        v = np.floor(v*self.data.shape[0]).astype(int)
+
+        return u, v
+
+
+    def pixel2world(self, u, v):
+        """Returns the (x, y, z) coordinates for pixel cordinates (u,v)(in the interval defined by the MxN image)."""
+
+        # Normalize coordinates to [-1, 1] interval
+        u = (u+0.5) / self.data.shape[1]
+        v = (v+0.5) / self.data.shape[0]
+
+        # Get (x, y, z) 
+        x, y, z, v = self.image2world(u, v)
+
+        return x, y, z, v
+
     def interpolate(self, u, v, valid=None, order=1, filter=True):
-        """"Interpolate to get the desired pixel values."""
+        """
+        Interpolate to get the desired pixel values.
+
+        :param order: Interpolation order (0: nearest, 1: linear, ..., 5).
+        :type order: integer (0,1,...,5)
+        """
+
         u = u.copy()
         v = v.copy()
-        
+
         # Repeat the first and last rows/columns for interpolation purposes
         h, w, d = self.data.shape
         source = np.empty((h + 2, w + 2, d))
 
         source[1:-1, 1:-1] = self.data
         source[0,1:-1] = self.data[0,:]; source[0,0] = self.data[0,0]; source[0,-1] = self.data[0,-1]
         source[-1,1:-1] = self.data[-1,:]; source[-1,0] = self.data[-1,0]; source[-1,-1] = self.data[-1,-1]
@@ -270,112 +302,121 @@
 
         mask = np.invert(valid)
         if mask.sum() > 0:
             self.data[np.tile(mask[:,:,None], (1, 1, self.data.shape[2]))] = np.tile(self.backgroundColor, (mask.sum(),))
 
         return self
 
-    def convertTo(self, targetFormat, targetDim=None):
+    def convertTo(self, targetFormat, targetDim=None, order=1):
         """
         Convert to another format.
 
         :param targetFormat: Target format.
         :param targetDim: Target dimension.
-        :type targetFormat: string
-        :type targetFormat: integer
+        :param order: Interpolation order (0: nearest, 1: linear, ..., 5).
 
+        :type targetFormat: string
+        :type targetDim: integer
+        :type order: integer (0,1,...,5)
         """
         self.validate()
-
         assert targetFormat.lower() in SUPPORTED_FORMATS, (
             "Unknown format: {}".format(targetFormat))
+        assert order in range(6), "Spline interpolation order must be between 0 and 5."
 
         if not targetDim:
             # By default, number of rows
             targetDim = self.data.shape[0]
 
         eTmp = EnvironmentMap(targetDim, targetFormat)
         dx, dy, dz, valid = eTmp.worldCoordinates()
         u, v = self.world2image(dx, dy, dz)
         self.format_ = targetFormat.lower()
-        self.interpolate(u, v, valid)
+        self.interpolate(u, v, valid, order)
 
         return self
 
-    def rotate(self, dcm):
+    def rotate(self, dcm, order=1):
         """
         Rotate the environment map.
 
-        :param input: Rotation information (currently only 3x3 numpy matrix)
+        :param dcm: Rotation information (currently only 3x3 numpy matrix)
+        :param order: Integer interpolation order (0: nearest, 1: linear, ..., 5).
+
         """
-        self.validate()
 
+        self.validate()
         assert type(dcm).__module__ == np.__name__ and dcm.ndim == 2 and dcm.shape == (3, 3)
+        assert order in range(6), "Spline interpolation order must be between 0 and 5."
+
         dx, dy, dz, valid = self.worldCoordinates()
 
         ptR = np.dot(dcm, np.vstack((dx.flatten(), dy.flatten(), dz.flatten())))
         dx, dy, dz = ptR[0].reshape(dx.shape), ptR[1].reshape(dy.shape), ptR[2].reshape(dz.shape)
 
         dx = np.clip(dx, -1, 1)
         dy = np.clip(dy, -1, 1)
         dz = np.clip(dz, -1, 1)
 
         u, v = self.world2image(dx, dy, dz)
-        self.interpolate(u, v, valid)
+        self.interpolate(u, v, valid, order)
 
         return self
 
     def resize(self, targetSize, order=1, debug=False):
         """
         Resize the current environnement map to targetSize.
-        The energy-preserving "pixel mixing" alrogithm is used when downscaling.
+        The energy-preserving "pixel mixing" algorithm is used when downscaling unless 
+        order is set to 0 (nearest neighbor interpolation).
 
         `targetSize` is either the desired `height` or `(height, width)`.
-        `order` is only used when upsampling.
+        `order` is the order of the spline interpolation (0: nearest, 1: linear, ..., 5).
+
         """
+
         self.validate()
+        assert order in range(6), "Spline interpolation order must be between 0 and 5."
 
         if not isinstance(targetSize, tuple):
             if self.format_ == 'latlong':
                 targetSize = (targetSize, 2*targetSize)
             elif self.format_ == 'skylatlong':
                 targetSize = (targetSize, 4*targetSize)
             elif self.format_ == 'cube':
                 targetSize = (targetSize, round(3/4*targetSize))
             else:
                 targetSize = (targetSize, targetSize)
         
-        # downsampling
-        if targetSize[0] < self.data.shape[0]:
+        if debug == True:
+            old_mean = self.data.mean()
 
-            if debug == True:
-                old_mean = self.data.mean()
+        # downsampling
+        if targetSize[0] < self.data.shape[0] and order != 0:
 
             # check if integer
             if (Decimal(self.data.shape[0]) / Decimal(targetSize[0])) % 1 == 0:
                 if debug is True:
                     print("integer resize")
                 fac = self.data.shape[0] // targetSize[0]
                 self.data = downscale_local_mean(self.data, (fac, fac, 1))
             else:    
+                if debug is True:
+                    print("non-integer resize")
                 self.data = resize_local_mean(self.data, targetSize, grid_mode=True, preserve_range=True)
 
-            if debug == True:
-                print("Energy difference in resize: {:.04f}".format(self.data.mean()/old_mean - 1.))
-
-            return self
-        
-        # upsampling
-        _size = []
-        for i in range(2):
-            _size.append(targetSize[i] / self.data.shape[i] if targetSize[i] > 1. else targetSize[i])
+        else: # upsampling or nearest neighbor
+            _size = []
+            for i in range(2):
+                _size.append(targetSize[i] / self.data.shape[i] if targetSize[i] > 1. else targetSize[i])
+            _size.append(1.0)
+            self.data = zoom(self.data, _size, order=order)
 
-        _size.append(1.0)
+        if debug is True:
+            print("Energy difference in resize: {:.04f}".format(self.data.mean()/old_mean - 1.))
 
-        self.data = zoom(self.data, _size, order=order)
         return self
 
     def toIntensity(self, mode="ITU BT.709", colorspace="linear"):
         """
         Converts the environment map to grayscale.
 
         `mode` can be either :
@@ -385,15 +426,15 @@
         `colorspace`: either "sRGB" or "linear"
         """
         self.validate()
 
         if self.data.shape[2] != 3:
             print("Envmap does not have 3 channels. This function won't do anything.")
             return self
-        
+
         if colorspace.lower() == "sRGB":
             if self.data.max() > 1.:
                 raise Exception("Error during sRGB to linear conversion: data is > 1. Please linearize "
                                 "the data beforehand or normalize it [0, 1].")
             self.data = self.data**2.2
 
         if mode == "ITU BT.601":
@@ -408,28 +449,27 @@
         if colorspace.lower() == "sRGB":
             self.data = self.data**(1./2.2)
 
         return self
 
     def getHemisphere(self, normal, channels=True):
         """
-        
         normal: 
         """
         normal = np.asarray(normal, dtype=np.float32).reshape((-1))
         assert normal.size == 3, "unknown normal shape, should have 3 elements"
         normal /= np.linalg.norm(normal)
 
         x, y, z, _ = self.worldCoordinates()
         xyz = np.dstack((x, y, z))
 
         mask = xyz.dot(normal) > 0
         if channels == False:
             return mask
-        
+
         return np.tile(mask[:,:,None], (1, 1, self.data.shape[2]))
 
     def setHemisphereValue(self, normal, value):
         """Sets an whole hemisphere defined by `normal` to a given `value`."""
 
         mask = self.getHemisphere(normal, channels=True)
 
@@ -463,22 +503,50 @@
 
         intensity = deepcopy(self).toIntensity()
         meanlight = visibility * intensity.data * solidAngles[:,:,np.newaxis]
         meanlight = np.nansum(xyz[...,np.newaxis] * meanlight[...,np.newaxis].transpose((0,1,3,2)), (0, 1))
 
         return meanlight
 
-    def embed(self, vfov, rotation_matrix, image):
-        """Projects an image onto the environment map.
+    def blur(self, kappa):
+        """
+        Blurs the environment map, taking into account the format.
+        Uses the von Mises-Fisher notation (`kappa` >= 0 for blur bandwidth, higher values are sharper)
+        """
+
+        x, y, z, _ = self.worldCoordinates()
+        xyz = np.dstack((x, y, z)).reshape((-1, 3))
+
+        h, w, c = self.data.shape[:3]
+        data = self.data.reshape((-1, c))
+        sa = self.solidAngles().reshape((-1, 1))
+
+        C3 = kappa/(4*np.pi*np.sinh(kappa))
+
+        result = np.empty((h*w, c), dtype=np.float32)
+
+        for i in tqdm(range(xyz.shape[0])):
+            normal = xyz[i:i+1,:]
+            result[i,:] = np.sum(data*sa*C3*np.exp(kappa*np.sum(xyz*normal, 1, keepdims=True)), 0)
+
+        self.data = result.reshape((h, w, c))
+        return self
+
+    def embed(self, vfov, rotation_matrix, image, order=1):
+        """
+        Projects an image onto the environment map.
 
         :vfov: Vertical Field of View (degrees).
         :rotation_matrix: Camera rotation matrix.
-        :image: The image to project."""
+        :image: The image to project.
+        :param order: Integer interpolation order (0: nearest, 1: linear, ..., 5).
+        """
 
         self.validate()
+        assert order in range(6), "Spline interpolation order must be between 0 and 5."
 
         targetDim = self.data.shape[0]
         targetFormat = self.format_
 
         eTmp = EnvironmentMap(targetDim, targetFormat)
         dx, dy, dz, valid = eTmp.worldCoordinates()
         ar = image.shape[1]/image.shape[0]
@@ -506,35 +574,39 @@
 
         uv = M.dot(xyz)
         u = (uv[0,:]/uv[2,:]).reshape(self.data.shape[:2])
         v = (uv[1,:]/uv[2,:]).reshape(self.data.shape[:2])
 
         self.format_ = targetFormat.lower()
         self.data = image.copy()[:,::-1,...]
-        self.interpolate(u, v, valid)
+        self.interpolate(u, v, valid, order)
         return self
 
     def project(self, vfov, rotation_matrix, ar=4./3., resolution=(640, 480),
-                projection="perspective", mode="normal"):
-        """Perform a projection onto a plane ("_simulates_" a camera).
+                projection="perspective", mode="normal", order=1):
+        """
+        Perform a projection onto a plane ("_simulates_" a camera).
 
         Note: this function does not modify the foreshortening present in the
         environment map.
 
         :vfov: Vertical Field of View (degrees).
         :rotation_matrix: Camera rotation matrix.
         :ar: Aspect ratio (width / height), defaults to 4/3.
         :resolution: Output size in (cols, rows), defaults to (640,480).
         :projection: perspective (default) or orthographic.
         :mode: "normal": perform crop (default)
                "mask": show pixel mask in the envmap,
                "normal+uv": returns (crop, u, v), where (u,v) are the coordinates
-                            of the crop."""
+                            of the crop.
+        :param order: Integer interpolation order (0: nearest, 1: linear, ..., 5).
+        """
 
         self.validate()
+        assert order in range(6), "Spline interpolation order must be between 0 and 5."
 
         coords = self._cameraCoordinates(vfov, rotation_matrix, ar,
                                          resolution, projection, mode)
 
         if mode == "mask":
             return coords
 
@@ -542,15 +614,15 @@
         if target.format_ != "latlong":
             target = target.convertTo("LatLong")
 
         # Get image coordinates from world sphere coordinates
         u, v = target.world2image(coords[0,:], coords[1,:], coords[2,:])
         u, v = u.reshape(resolution[::-1]), v.reshape(resolution[::-1])
 
-        crop = target.interpolate(u, v).data
+        crop = target.interpolate(u, v, order=order).data
 
         if mode == "normal+uv":
             return crop, u, v
 
         return crop
 
     def _cameraCoordinates(self, vfov, rotation_matrix, ar=4./3., resolution=(640, 480),
```

### Comparing `skylibs-0.7.2/envmap/projections.py` & `skylibs-0.7.3/envmap/projections.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,284 +1,297 @@
-import numpy as np
-from numpy import logical_and as land, logical_or as lor
-
-
-def world2latlong(x, y, z):
-    """Get the (u, v) coordinates of the point defined by (x, y, z) for
-    a latitude-longitude map."""
-    u = 1 + (1 / np.pi) * np.arctan2(x, -z)
-    v = (1 / np.pi) * np.arccos(y)
-    # because we want [0,1] interval
-    u = u / 2
-    return u, v
-
-
-def world2skylatlong(x, y, z):
-    """Get the (u, v) coordinates of the point defined by (x, y, z) for
-    a sky-latitude-longitude map (the zenith hemisphere of a latlong map)."""
-    u = 1 + (1 / np.pi) * np.arctan2(x, -z)
-    v = (1 / np.pi) * np.arccos(y) * 2
-    # because we want [0,1] interval
-    u = u / 2
-    return u, v
-
-
-def world2angular(x, y, z):
-    """Get the (u, v) coordinates of the point defined by (x, y, z) for
-    an angular map."""
-    # world -> angular
-
-    # take advantage of the division by zero handling of numpy
-    x, y, z = np.asarray(x), np.asarray(y), np.asarray(z)
-
-    denum = (2 * np.pi * np.sqrt(x**2 + y**2))
-    rAngular = np.arccos(-z) / denum
-    v = np.atleast_1d(0.5 - rAngular * y)
-    u = np.atleast_1d(0.5 + rAngular * x)
-    
-    u[~np.isfinite(rAngular)] = 0.5
-    # handle [0, 0, -1]
-    v[np.isnan(rAngular)] = 0.5
-    # handle [0, 0, 1]
-    v[np.isinf(rAngular)] = 0.
-
-    if u.size == 1:
-        return u.item(), v.item()
-
-    return u, v
-
-
-def latlong2world(u, v):
-    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
-    for a latlong map."""
-    u = u * 2
-
-    # lat-long -> world
-    thetaLatLong = np.pi * (u - 1)
-    phiLatLong = np.pi * v
-
-    x = np.sin(phiLatLong) * np.sin(thetaLatLong)
-    y = np.cos(phiLatLong)
-    z = -np.sin(phiLatLong) * np.cos(thetaLatLong)
-
-    valid = np.ones(x.shape, dtype='bool')
-    return x, y, z, valid
-
-
-def skylatlong2world(u, v):
-    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
-    for a latlong map."""
-    u = u * 2
-
-    # lat-long -> world
-    thetaLatLong = np.pi * (u - 1)
-    phiLatLong = np.pi * v / 2
-
-    x = np.sin(phiLatLong) * np.sin(thetaLatLong)
-    y = np.cos(phiLatLong)
-    z = -np.sin(phiLatLong) * np.cos(thetaLatLong)
-
-    valid = np.ones(x.shape, dtype='bool')
-    return x, y, z, valid
-
-
-def angular2world(u, v):
-    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
-    for an angular map."""
-    # angular -> world
-    thetaAngular = np.arctan2(-2 * v + 1, 2 * u - 1)
-    phiAngular = np.pi * np.sqrt((2 * u - 1)**2 + (2 * v - 1)**2)
-
-    x = np.sin(phiAngular) * np.cos(thetaAngular)
-    y = np.sin(phiAngular) * np.sin(thetaAngular)
-    z = -np.cos(phiAngular)
-
-    r = (u - 0.5)**2 + (v - 0.5)**2
-    valid = r <= .25  # .5**2
-
-    return x, y, z, valid
-
-
-def skyangular2world(u, v):
-    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
-    for a sky angular map."""
-    # skyangular -> world
-    thetaAngular = np.arctan2(-2 * v + 1, 2 * u - 1)  # azimuth
-    phiAngular = np.pi / 2 * np.sqrt((2 * u - 1)**2 + (2 * v - 1)**2)  # zenith
-
-    x = np.sin(phiAngular) * np.cos(thetaAngular)
-    z = np.sin(phiAngular) * np.sin(thetaAngular)
-    y = np.cos(phiAngular)
-
-    r = (u - 0.5)**2 + (v - 0.5)**2
-    valid = r <= .25  # .5^2
-
-    return x, y, z, valid
-
-
-def world2skyangular(x, y, z):
-    """Get the (u, v) coordinates of the point defined by (x, y, z) for
-    a sky angular map."""
-    # world -> skyangular
-    thetaAngular = np.arctan2(x, z)  # azimuth
-    phiAngular = np.arctan2(np.sqrt(x**2 + z**2), y)  # zenith
-
-    r = phiAngular / (np.pi / 2)
-
-    u = 1. / 2 + r * np.sin(thetaAngular) / 2 
-    v = 1. / 2 - r * np.cos(thetaAngular) / 2
-
-    return u, v
-
-
-def sphere2world(u, v):
-    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
-    for the sphere map."""
-    u = u * 2 - 1
-    v = v * 2 - 1
-
-    # sphere -> world
-    r = np.sqrt(u**2 + v**2)
-    theta = np.arctan2(u, -v)
-
-    phi = np.zeros(theta.shape)
-    valid = r <= 1
-    phi[valid] = 2 * np.arcsin(r[valid])
-
-    x = np.sin(phi) * np.sin(theta)
-    y = np.sin(phi) * np.cos(theta)
-    z = -np.cos(phi)
-    return x, y, z, valid
-
-
-def world2sphere(x, y, z):
-    # world -> sphere
-
-    # take advantage of the division by zero handling of numpy
-    x, y, z = np.asarray(x), np.asarray(y), np.asarray(z)
-    
-    denum = (2 * np.sqrt(x**2 + y**2))
-    r = np.sin(.5 * np.arccos(-z)) / denum
-
-    u = np.atleast_1d(.5 + r * x)
-    v = np.atleast_1d(.5 - r * y)
-
-    u[~np.isfinite(r)] = 0.5
-    # handle [0, 0, -1]
-    v[np.isnan(r)] = 0.5
-    # handle [0, 0, 1]
-    v[np.isinf(r)] = 0.
-
-    if u.size == 1:
-        return u.item(), v.item()
-
-    return u, v
-
-
-def world2cube(x, y, z):
-    # world -> cube
-    x = np.atleast_1d(np.asarray(x))
-    y = np.atleast_1d(np.asarray(y))
-    z = np.atleast_1d(np.asarray(z))
-    u = np.zeros(x.shape)
-    v = np.zeros(x.shape)
-
-    # forward
-    indForward = np.nonzero(
-        land(land(z <= 0, z <= -np.abs(x)), z <= -np.abs(y)))
-    u[indForward] = 1.5 - 0.5 * x[indForward] / z[indForward]
-    v[indForward] = 1.5 + 0.5 * y[indForward] / z[indForward]
-
-    # backward
-    indBackward = np.nonzero(
-        land(land(z >= 0,  z >= np.abs(x)),  z >= np.abs(y)))
-    u[indBackward] = 1.5 + 0.5 * x[indBackward] / z[indBackward]
-    v[indBackward] = 3.5 + 0.5 * y[indBackward] / z[indBackward]
-
-    # down
-    indDown = np.nonzero(
-        land(land(y <= 0,  y <= -np.abs(x)),  y <= -np.abs(z)))
-    u[indDown] = 1.5 - 0.5 * x[indDown] / y[indDown]
-    v[indDown] = 2.5 - 0.5 * z[indDown] / y[indDown]
-
-    # up
-    indUp = np.nonzero(land(land(y >= 0,  y >= np.abs(x)),  y >= np.abs(z)))
-    u[indUp] = 1.5 + 0.5 * x[indUp] / y[indUp]
-    v[indUp] = 0.5 - 0.5 * z[indUp] / y[indUp]
-
-    # left
-    indLeft = np.nonzero(
-        land(land(x <= 0,  x <= -np.abs(y)),  x <= -np.abs(z)))
-    u[indLeft] = 0.5 + 0.5 * z[indLeft] / x[indLeft]
-    v[indLeft] = 1.5 + 0.5 * y[indLeft] / x[indLeft]
-
-    # right
-    indRight = np.nonzero(land(land(x >= 0,  x >= np.abs(y)),  x >= np.abs(z)))
-    u[indRight] = 2.5 + 0.5 * z[indRight] / x[indRight]
-    v[indRight] = 1.5 - 0.5 * y[indRight] / x[indRight]
-
-    # bring back in the [0,1] intervals
-    u = u / 3.
-    v = v / 4.
-    return u, v
-
-
-def cube2world(u, v):
-    # [u,v] = meshgrid(0:3/(3*dim-1):3, 0:4/(4*dim-1):4);
-    # u and v are in the [0,1] interval, so put them back to [0,3]
-    # and [0,4]
-    u = u * 3
-    v = v * 4
-
-    x = np.zeros(u.shape)
-    y = np.zeros(u.shape)
-    z = np.zeros(u.shape)
-    valid = np.zeros(u.shape, dtype='bool')
-
-    # up
-    indUp = land(land(u >= 1, u < 2), v < 1)
-    x[indUp] = (u[indUp] - 1.5) * 2
-    y[indUp] = 1
-    z[indUp] = (v[indUp] - 0.5) * -2
-
-    # left
-    indLeft = land(land(u < 1, v >= 1), v < 2)
-    x[indLeft] = -1
-    y[indLeft] = (v[indLeft] - 1.5) * -2
-    z[indLeft] = (u[indLeft] - 0.5) * -2
-
-    # forward
-    indForward = land(land(land(u >= 1, u < 2), v >= 1), v < 2)
-    x[indForward] = (u[indForward] - 1.5) * 2
-    y[indForward] = (v[indForward] - 1.5) * -2
-    z[indForward] = -1
-
-    # right
-    indRight = land(land(u >= 2, v >= 1), v < 2)
-    x[indRight] = 1
-    y[indRight] = (v[indRight] - 1.5) * -2
-    z[indRight] = (u[indRight] - 2.5) * 2
-
-    # down
-    indDown = land(land(land(u >= 1, u < 2), v >= 2), v < 3)
-    x[indDown] = (u[indDown] - 1.5) * 2
-    y[indDown] = -1
-    z[indDown] = (v[indDown] - 2.5) * 2
-
-    # backward
-    indBackward = land(land(u >= 1, u < 2), v >= 3)
-    x[indBackward] = (u[indBackward] - 1.5) * 2
-    y[indBackward] = (v[indBackward] - 3.5) * 2
-    z[indBackward] = 1
-
-    # normalize
-    # np.hypot(x, y, z) #sqrt(x.^2 + y.^2 + z.^2);
-    norm = np.sqrt(x**2 + y**2 + z**2)
-    x = x / norm
-    y = y / norm
-    z = z / norm
-
-    # return valid indices
-    valid_ind = lor(
-        lor(lor(indUp, indLeft), lor(indForward, indRight)), lor(indDown, indBackward))
-    valid[valid_ind] = 1
-    return x, y, z, valid
+import numpy as np
+from numpy import logical_and as land, logical_or as lor
+
+
+def world2latlong(x, y, z):
+    """Get the (u, v) coordinates of the point defined by (x, y, z) for
+    a latitude-longitude map."""
+    u = 1 + (1 / np.pi) * np.arctan2(x, -z)
+    v = (1 / np.pi) * np.arccos(y)
+    # because we want [0,1] interval
+    u = u / 2
+    return u, v
+
+
+def world2skylatlong(x, y, z):
+    """Get the (u, v) coordinates of the point defined by (x, y, z) for
+    a sky-latitude-longitude map (the zenith hemisphere of a latlong map)."""
+    u = 1 + (1 / np.pi) * np.arctan2(x, -z)
+    v = (1 / np.pi) * np.arccos(y) * 2
+    # because we want [0,1] interval
+    u = u / 2
+    return u, v
+
+
+def world2angular(x, y, z):
+    """Get the (u, v) coordinates of the point defined by (x, y, z) for
+    an angular map."""
+    # world -> angular
+
+    # take advantage of the division by zero handling of numpy
+    x, y, z = np.asarray(x), np.asarray(y), np.asarray(z)
+
+    denum = (2 * np.pi * np.sqrt(x**2 + y**2))
+    rAngular = np.arccos(-z) / denum
+    v = np.atleast_1d(0.5 - rAngular * y)
+    u = np.atleast_1d(0.5 + rAngular * x)
+    
+    u[~np.isfinite(rAngular)] = 0.5
+    # handle [0, 0, -1]
+    v[np.isnan(rAngular)] = 0.5
+    # handle [0, 0, 1]
+    v[np.isinf(rAngular)] = 0.
+
+    if u.size == 1:
+        return u.item(), v.item()
+
+    return u, v
+
+
+def latlong2world(u, v):
+    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
+    for a latlong map."""
+    u = u * 2
+
+    # lat-long -> world
+    thetaLatLong = np.pi * (u - 1)
+    phiLatLong = np.pi * v
+
+    x = np.sin(phiLatLong) * np.sin(thetaLatLong)
+    y = np.cos(phiLatLong)
+    z = -np.sin(phiLatLong) * np.cos(thetaLatLong)
+
+    valid = np.ones(x.shape, dtype='bool')
+    return x, y, z, valid
+
+
+def skylatlong2world(u, v):
+    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
+    for a latlong map."""
+    u = u * 2
+
+    # lat-long -> world
+    thetaLatLong = np.pi * (u - 1)
+    phiLatLong = np.pi * v / 2
+
+    x = np.sin(phiLatLong) * np.sin(thetaLatLong)
+    y = np.cos(phiLatLong)
+    z = -np.sin(phiLatLong) * np.cos(thetaLatLong)
+
+    valid = np.ones(x.shape, dtype='bool')
+    return x, y, z, valid
+
+
+def angular2world(u, v):
+    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
+    for an angular map."""
+    # angular -> world
+    thetaAngular = np.arctan2(-2 * v + 1, 2 * u - 1)
+    phiAngular = np.pi * np.sqrt((2 * u - 1)**2 + (2 * v - 1)**2)
+
+    x = np.sin(phiAngular) * np.cos(thetaAngular)
+    y = np.sin(phiAngular) * np.sin(thetaAngular)
+    z = -np.cos(phiAngular)
+
+    r = (u - 0.5)**2 + (v - 0.5)**2
+    valid = r <= .25  # .5**2
+
+    return x, y, z, valid
+
+
+def skyangular2world(u, v):
+    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
+    for a sky angular map."""
+    # skyangular -> world
+    thetaAngular = np.arctan2(-2 * v + 1, 2 * u - 1)  # azimuth
+    phiAngular = np.pi / 2 * np.sqrt((2 * u - 1)**2 + (2 * v - 1)**2)  # zenith
+
+    x = np.sin(phiAngular) * np.cos(thetaAngular)
+    z = np.sin(phiAngular) * np.sin(thetaAngular)
+    y = np.cos(phiAngular)
+
+    r = (u - 0.5)**2 + (v - 0.5)**2
+    valid = r <= .25  # .5^2
+
+    return x, y, z, valid
+
+
+def world2skyangular(x, y, z):
+    """Get the (u, v) coordinates of the point defined by (x, y, z) for
+    a sky angular map."""
+    # world -> skyangular
+    thetaAngular = np.arctan2(x, z)  # azimuth
+    phiAngular = np.arctan2(np.sqrt(x**2 + z**2), y)  # zenith
+
+    r = phiAngular / (np.pi / 2)
+
+    u = 1. / 2 + r * np.sin(thetaAngular) / 2 
+    v = 1. / 2 - r * np.cos(thetaAngular) / 2
+
+    return u, v
+
+
+def sphere2world(u, v):
+    """Get the (x, y, z, valid) coordinates of the point defined by (u, v)
+    for the sphere map."""
+    u = u * 2 - 1
+    v = v * 2 - 1
+
+    # sphere -> world
+    r = np.sqrt(u**2 + v**2)
+    theta = np.arctan2(u, -v)
+
+    phi = np.zeros(theta.shape)
+    valid = r <= 1
+    phi[valid] = 2 * np.arcsin(r[valid])
+
+    x = np.sin(phi) * np.sin(theta)
+    y = np.sin(phi) * np.cos(theta)
+    z = -np.cos(phi)
+    return x, y, z, valid
+
+
+def world2sphere(x, y, z):
+    # world -> sphere
+
+    # take advantage of the division by zero handling of numpy
+    x, y, z = np.asarray(x), np.asarray(y), np.asarray(z)
+    
+    denum = (2 * np.sqrt(x**2 + y**2))
+    with np.errstate(divide='ignore', invalid='ignore'):
+        r = np.sin(.5 * np.arccos(-z)) / denum
+
+    u = np.atleast_1d(.5 + r * x)
+    v = np.atleast_1d(.5 - r * y)
+
+    u[~np.isfinite(r)] = 0.5
+    # handle [0, 0, -1]
+    v[np.isnan(r)] = 0.5
+    # handle [0, 0, 1]
+    v[np.isinf(r)] = 0.
+
+    if u.size == 1:
+        return u.item(), v.item()
+
+    return u, v
+
+
+def world2cube(x, y, z):
+    # world -> cube
+    x = np.atleast_1d(np.asarray(x))
+    y = np.atleast_1d(np.asarray(y))
+    z = np.atleast_1d(np.asarray(z))
+    u = np.zeros(x.shape)
+    v = np.zeros(x.shape)
+
+    # forward
+    indForward = np.nonzero(
+        land(land(z <= 0, z <= -np.abs(x)), z <= -np.abs(y)))
+    u[indForward] = 1.5 - 0.5 * x[indForward] / z[indForward]
+    v[indForward] = 1.5 + 0.5 * y[indForward] / z[indForward]
+
+    # backward
+    indBackward = np.nonzero(
+        land(land(z >= 0,  z >= np.abs(x)),  z >= np.abs(y)))
+    u[indBackward] = 1.5 + 0.5 * x[indBackward] / z[indBackward]
+    v[indBackward] = 3.5 + 0.5 * y[indBackward] / z[indBackward]
+
+    # down
+    indDown = np.nonzero(
+        land(land(y <= 0,  y <= -np.abs(x)),  y <= -np.abs(z)))
+    u[indDown] = 1.5 - 0.5 * x[indDown] / y[indDown]
+    v[indDown] = 2.5 - 0.5 * z[indDown] / y[indDown]
+
+    # up
+    indUp = np.nonzero(land(land(y >= 0,  y >= np.abs(x)),  y >= np.abs(z)))
+    u[indUp] = 1.5 + 0.5 * x[indUp] / y[indUp]
+    v[indUp] = 0.5 - 0.5 * z[indUp] / y[indUp]
+
+    # left
+    indLeft = np.nonzero(
+        land(land(x <= 0,  x <= -np.abs(y)),  x <= -np.abs(z)))
+    u[indLeft] = 0.5 + 0.5 * z[indLeft] / x[indLeft]
+    v[indLeft] = 1.5 + 0.5 * y[indLeft] / x[indLeft]
+
+    # right
+    indRight = np.nonzero(land(land(x >= 0,  x >= np.abs(y)),  x >= np.abs(z)))
+    u[indRight] = 2.5 + 0.5 * z[indRight] / x[indRight]
+    v[indRight] = 1.5 - 0.5 * y[indRight] / x[indRight]
+
+    # bring back in the [0,1] intervals
+    u = u / 3.
+    v = v / 4.
+
+    if u.size == 1:
+        return u.item(), v.item()
+
+    return u, v
+
+
+def cube2world(u, v):
+    u = np.atleast_1d(np.asarray(u))
+    v = np.atleast_1d(np.asarray(v))
+    
+    # [u,v] = meshgrid(0:3/(3*dim-1):3, 0:4/(4*dim-1):4);
+    # u and v are in the [0,1] interval, so put them back to [0,3]
+    # and [0,4]
+    u = u * 3
+    v = v * 4
+
+    x = np.zeros(u.shape)
+    y = np.zeros(u.shape)
+    z = np.zeros(u.shape)
+    valid = np.zeros(u.shape, dtype='bool')
+
+    # up
+    indUp = land(land(u >= 1, u < 2), v < 1)
+    x[indUp] = (u[indUp] - 1.5) * 2
+    y[indUp] = 1
+    z[indUp] = (v[indUp] - 0.5) * -2
+
+    # left
+    indLeft = land(land(u < 1, v >= 1), v < 2)
+    x[indLeft] = -1
+    y[indLeft] = (v[indLeft] - 1.5) * -2
+    z[indLeft] = (u[indLeft] - 0.5) * -2
+
+    # forward
+    indForward = land(land(land(u >= 1, u < 2), v >= 1), v < 2)
+    x[indForward] = (u[indForward] - 1.5) * 2
+    y[indForward] = (v[indForward] - 1.5) * -2
+    z[indForward] = -1
+
+    # right
+    indRight = land(land(u >= 2, v >= 1), v < 2)
+    x[indRight] = 1
+    y[indRight] = (v[indRight] - 1.5) * -2
+    z[indRight] = (u[indRight] - 2.5) * 2
+
+    # down
+    indDown = land(land(land(u >= 1, u < 2), v >= 2), v < 3)
+    x[indDown] = (u[indDown] - 1.5) * 2
+    y[indDown] = -1
+    z[indDown] = (v[indDown] - 2.5) * 2
+
+    # backward
+    indBackward = land(land(u >= 1, u < 2), v >= 3)
+    x[indBackward] = (u[indBackward] - 1.5) * 2
+    y[indBackward] = (v[indBackward] - 3.5) * 2
+    z[indBackward] = 1
+
+    # normalize
+    # np.hypot(x, y, z) #sqrt(x.^2 + y.^2 + z.^2);
+    norm = np.sqrt(x**2 + y**2 + z**2)
+    with np.errstate(divide='ignore', invalid='ignore'):
+        x = x / norm
+        y = y / norm
+        z = z / norm
+
+    # return valid indices
+    valid_ind = lor(
+        lor(lor(indUp, indLeft), lor(indForward, indRight)), lor(indDown, indBackward))
+    valid[valid_ind] = 1
+
+    if x.size == 1:
+        return x.item(), y.item(), z.item(), valid.item()
+
+    return x, y, z, valid
```

### Comparing `skylibs-0.7.2/envmap/rotations.py` & `skylibs-0.7.3/envmap/rotations.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,7 +22,14 @@
 def rotz(theta):
     """
     Produces a counter-clockwise 3D rotation matrix around axis Z with angle `theta` in radians.
     """
     return np.array([[np.cos(theta), -np.sin(theta), 0],
                      [np.sin(theta), np.cos(theta), 0],
                      [0, 0, 1]], dtype='float64')
+
+
+def rot(theta=(0,0,0)):
+    """
+    Produces a counter-clockwise 3D rotation matrix around axis X, Y and Z with angles `theta` in radians.
+    """
+    return np.dot(rotz(theta[2]), np.dot(roty(theta[1]), rotx(theta[0])))
```

### Comparing `skylibs-0.7.2/envmap/tetrahedronSolidAngle.py` & `skylibs-0.7.3/envmap/tetrahedronSolidAngle.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/envmap/xmlhelper.py` & `skylibs-0.7.3/envmap/xmlhelper.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/ezexr/__init__.py` & `skylibs-0.7.3/ezexr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     # Use the attribute "v" of PixelType objects because they have no __eq__
     pixformat_mapping = {Imath.PixelType(Imath.PixelType.FLOAT).v: np.float32,
                          Imath.PixelType(Imath.PixelType.HALF).v: np.float16,
                          Imath.PixelType(Imath.PixelType.UINT).v: np.uint32}
 
     # Get the number of channels
     nc = len(header['channels'])
-    print(nc)
 
     # Check the data type
     dtGlobal = list(header['channels'].values())[0].type
 
     if rgb is True:
         # Create the read buffer if needed
         data = bufferImage if bufferImage is not None else np.empty((h, w, nc), dtype=pixformat_mapping[dtGlobal.v])
```

### Comparing `skylibs-0.7.2/hdrio/__init__.py` & `skylibs-0.7.3/hdrio/__init__.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/hdrtools/gsolve.py` & `skylibs-0.7.3/hdrtools/gsolve.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/hdrtools/tonemapping/__init__.py` & `skylibs-0.7.3/hdrtools/tonemapping/__init__.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/skydb/__init__.py` & `skylibs-0.7.3/skydb/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-import os
-from os import listdir
-from os.path import abspath, isdir, join
-import fnmatch
-import datetime
-
-import numpy as np
-
-from envmap import EnvironmentMap
-from hdrtools import sunutils
-
-
-class SkyDB:
-    def __init__(self, path):
-        """Creates a SkyDB.
-        The path should contain folders named by YYYYMMDD (ie. 20130619 for June 19th 2013).
-        These folders should contain folders named by HHMMSS (ie. 102639 for 10h26 39s).
-        Inside these folders should a file named envmap.exr be located.
-        """
-        p = abspath(path)
-        self.intervals_dates = [join(p, f) for f in listdir(p) if isdir(join(p, f))]
-        self.intervals = list(map(SkyInterval, self.intervals_dates))
-
-
-class SkyInterval:
-    def __init__(self, path):
-        """Represent an interval, usually a day.
-        The path should contain folders named by HHMMSS (ie. 102639 for 10h26 39s).
-        """
-        self.path =  path
-        matches = []
-        for root, dirnames, filenames in os.walk(path):
-            for filename in fnmatch.filter(filenames, 'envmap.exr'):
-                matches.append(join(root, filename))
-
-        self.probes = list(map(SkyProbe, matches))
-        self.reftimes = [x.datetime for x in self.probes]
-
-    @property
-    def sun_visibility(self):
-        """
-        Return sun_visibility of the interval
-        """
-        if len(self.probes) > 0:
-            sun_visibility = sum(1 for x in self.probes if x.sun_visible) / len(self.probes)
-        else:
-            sun_visibility = 0
-        return sun_visibility
-
-    @property
-    def date(self):
-        """
-        :returns: datetime.date object
-        """
-        date = os.path.normpath(self.path).split(os.sep)[-1]
-        infos = {
-            "day": int(date[-2:]),
-            "month": int(date[4:6]),
-            "year": int(date[:4]),
-        }
-        return datetime.date(**infos)
-
-    def closestProbe(self, hours, minutes=0, seconds=0):
-        """
-        Return the SkyProbe object closest to the requested time.
-        TODO : check for day change (if we ask for 6:00 AM and the probe sequence
-            only begins at 7:00 PM and ends at 9:00 PM, then 9:00 PM is actually
-            closer than 7:00 PM and will be wrongly selected; not a big deal but...)
-        TODO : Take the code from skymangler.
-        """
-        cmpdate = datetime.datetime(year=1, month=1, day=1, hour=hours, minute=minutes, second=seconds)
-        idx = np.argmin([np.abs((cmpdate - t).total_seconds()) for t in self.reftimes])
-        return self.probes[idx]
-
-
-class SkyProbe:
-    def __init__(self, path, format_=None):
-        """Represent an environment map among an interval."""
-        self.path = path
-        self.format_ = format_
-
-    def init_properties(self):
-        """
-        Cache properties that are resource intensive to generate.
-        """
-        if not hasattr(self, '_envmap'):
-            self._envmap = self.environment_map
-
-    def remove_envmap(self):
-        """
-        Delete probe's envmap from memory.
-        """
-        del self._envmap
-
-    @property
-    def sun_visible(self):
-        """
-        :returns: boolean, True if the sun is visible, False otherwise.
-        """
-        self.init_properties()
-        return self._envmap.data.max() > 5000
-
-    @property
-    def datetime(self):
-        """Datetime of the capture.
-        :returns: datetime object.
-        """
-        time_ = os.path.normpath(self.path).split(os.sep)[-2]
-        date = os.path.normpath(self.path).split(os.sep)[-3]
-        infos = {
-            "second": int(time_[-2:]),
-            "minute": int(time_[2:4]),
-            "hour": int(time_[:2]),
-            "day": int(date[-2:]),
-            "month": int(date[4:6]),
-            "year": int(date[:4]),
-        }
-
-        if infos["second"] >= 60:
-            infos["second"] = 59
-
-        try:
-            datetime_ = datetime.datetime(**infos)
-        except ValueError:
-            print('error on path:', self.path)
-            raise
-
-        return datetime_
-
-    @property
-    def environment_map(self):
-        """
-        :returns: EnvironmentMap object.
-        """
-        if self.format_:
-            return EnvironmentMap(self.path, self.format_)
-        else:
-            return EnvironmentMap(self.path)
-
-    def sun_position(self, method="coords"):
-        """
-        :returns: (elevation, azimuth)
-        """
-        if method == "intensity":
-            self.init_properties()
-            return sunutils.sunPosFromEnvmap(self._envmap)
-        elif method == "coords":
-            latitude = 46.778969
-            longitude = -71.274914
-            elevation = 125
-
-            if self.datetime < datetime.datetime(2013, 12, 25, 10, 10, 10):
-                latitude, longitude = 40.442794, -79.944115
-                elevation = 300
-
-            d = self.datetime
-            if self.datetime.tzinfo is None:
-                #TODO get timezone from latitude and longitude
-                # d = pytz.timezone('US/Eastern').localize(self.datetime, is_dst=False)
-                d += datetime.timedelta(hours=+4)
-
-
-            return sunutils.sunPosFromCoord(latitude, longitude, d, elevation=elevation)
+import os
+from os import listdir
+from os.path import abspath, isdir, join
+import fnmatch
+import datetime
+
+import numpy as np
+
+from envmap import EnvironmentMap
+from hdrtools import sunutils
+
+
+class SkyDB:
+    def __init__(self, path):
+        """Creates a SkyDB.
+        The path should contain folders named by YYYYMMDD (ie. 20130619 for June 19th 2013).
+        These folders should contain folders named by HHMMSS (ie. 102639 for 10h26 39s).
+        Inside these folders should a file named envmap.exr be located.
+        """
+        p = abspath(path)
+        self.intervals_dates = [join(p, f) for f in listdir(p) if isdir(join(p, f))]
+        self.intervals = list(map(SkyInterval, self.intervals_dates))
+
+
+class SkyInterval:
+    def __init__(self, path):
+        """Represent an interval, usually a day.
+        The path should contain folders named by HHMMSS (ie. 102639 for 10h26 39s).
+        """
+        self.path =  path
+        matches = []
+        for root, dirnames, filenames in os.walk(path):
+            for filename in fnmatch.filter(filenames, 'envmap.exr'):
+                matches.append(join(root, filename))
+
+        self.probes = list(map(SkyProbe, matches))
+        self.reftimes = [x.datetime for x in self.probes]
+
+    @property
+    def sun_visibility(self):
+        """
+        Return sun_visibility of the interval
+        """
+        if len(self.probes) > 0:
+            sun_visibility = sum(1 for x in self.probes if x.sun_visible) / len(self.probes)
+        else:
+            sun_visibility = 0
+        return sun_visibility
+
+    @property
+    def date(self):
+        """
+        :returns: datetime.date object
+        """
+        date = os.path.normpath(self.path).split(os.sep)[-1]
+        infos = {
+            "day": int(date[-2:]),
+            "month": int(date[4:6]),
+            "year": int(date[:4]),
+        }
+        return datetime.date(**infos)
+
+    def closestProbe(self, hours, minutes=0, seconds=0):
+        """
+        Return the SkyProbe object closest to the requested time.
+        TODO : check for day change (if we ask for 6:00 AM and the probe sequence
+            only begins at 7:00 PM and ends at 9:00 PM, then 9:00 PM is actually
+            closer than 7:00 PM and will be wrongly selected; not a big deal but...)
+        TODO : Take the code from skymangler.
+        """
+        cmpdate = datetime.datetime(year=1, month=1, day=1, hour=hours, minute=minutes, second=seconds)
+        idx = np.argmin([np.abs((cmpdate - t).total_seconds()) for t in self.reftimes])
+        return self.probes[idx]
+
+
+class SkyProbe:
+    def __init__(self, path, format_=None):
+        """Represent an environment map among an interval."""
+        self.path = path
+        self.format_ = format_
+
+    def init_properties(self):
+        """
+        Cache properties that are resource intensive to generate.
+        """
+        if not hasattr(self, '_envmap'):
+            self._envmap = self.environment_map
+
+    def remove_envmap(self):
+        """
+        Delete probe's envmap from memory.
+        """
+        del self._envmap
+
+    @property
+    def sun_visible(self):
+        """
+        :returns: boolean, True if the sun is visible, False otherwise.
+        """
+        self.init_properties()
+        return self._envmap.data.max() > 5000
+
+    @property
+    def datetime(self):
+        """Datetime of the capture.
+        :returns: datetime object.
+        """
+        time_ = os.path.normpath(self.path).split(os.sep)[-2]
+        date = os.path.normpath(self.path).split(os.sep)[-3]
+        infos = {
+            "second": int(time_[-2:]),
+            "minute": int(time_[2:4]),
+            "hour": int(time_[:2]),
+            "day": int(date[-2:]),
+            "month": int(date[4:6]),
+            "year": int(date[:4]),
+        }
+
+        if infos["second"] >= 60:
+            infos["second"] = 59
+
+        try:
+            datetime_ = datetime.datetime(**infos)
+        except ValueError:
+            print('error on path:', self.path)
+            raise
+
+        return datetime_
+
+    @property
+    def environment_map(self):
+        """
+        :returns: EnvironmentMap object.
+        """
+        if self.format_:
+            return EnvironmentMap(self.path, self.format_)
+        else:
+            return EnvironmentMap(self.path)
+
+    def sun_position(self, method="coords"):
+        """
+        :returns: (elevation, azimuth)
+        """
+        if method == "intensity":
+            self.init_properties()
+            return sunutils.sunPosFromEnvmap(self._envmap)
+
+        elif method == "coords":
+            # Assume Laval University, Quebec, Canada
+            latitude, longitude = 46.778969, -71.274914
+            elevation = 125
+
+            tz = datetime.timezone(datetime.timedelta(seconds=-17760))
+            if self.datetime < datetime.datetime(2013, 12, 25, 10, 10, 10, tzinfo=tz):
+                # Assume Carnegie Mellon University, Pittsburgh, PA
+                latitude, longitude = 40.442794, -79.944115
+                elevation = 300
+
+            d = self.datetime
+            if self.datetime.tzinfo is None:
+                d += datetime.timedelta(hours=+4)
+
+            return sunutils.sunPosFromCoord(latitude, longitude, d, elevation=elevation)
```

### Comparing `skylibs-0.7.2/skylibs.egg-info/SOURCES.txt` & `skylibs-0.7.3/skylibs.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 envmap/__init__.py
 envmap/environmentmap.py
 envmap/projections.py
 envmap/rotations.py
-envmap/test_environmentmap.py
 envmap/tetrahedronSolidAngle.py
 envmap/xmlhelper.py
 ezexr/__init__.py
 hdrio/__init__.py
 hdrtools/__init__.py
 hdrtools/gsolve.py
 hdrtools/sunutils.py
@@ -20,13 +19,15 @@
 skydb/__init__.py
 skylibs/__init__.py
 skylibs.egg-info/PKG-INFO
 skylibs.egg-info/SOURCES.txt
 skylibs.egg-info/dependency_links.txt
 skylibs.egg-info/requires.txt
 skylibs.egg-info/top_level.txt
+test/test_blur.py
 test/test_envmap.py
+test/test_projections.py
 test/test_sph.py
 test/test_sunutils.py
 tools3d/__init__.py
 tools3d/display.py
 tools3d/spharm.py
```

### Comparing `skylibs-0.7.2/test/test_envmap.py` & `skylibs-0.7.3/test/test_envmap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from itertools import product
 import pytest
 from skimage.transform import resize
 from scipy.ndimage import binary_erosion
-from envmap import EnvironmentMap, rotation_matrix
+from envmap import EnvironmentMap, rotation_matrix, rotations
 from envmap.environmentmap import SUPPORTED_FORMATS
 
 
 np.random.seed(31415926)
 
 
 # pytest [-s] [-k test_convert]
@@ -18,14 +18,33 @@
     e.data = np.random.rand(e.data.shape[0], e.data.shape[1], channels)
     if up_factor != 1.:
         e.data = resize(e.data, [up_factor*x for x in e.data.shape[:2]])
     e.setBackgroundColor(0.)
     return e
 
 
+@pytest.mark.parametrize("format_", SUPPORTED_FORMATS)
+def test_imageCoordinates(format_):
+    s = 64
+    e = EnvironmentMap(s, format_)
+    u, v = e.imageCoordinates()
+
+    s2, s1 = e.data.shape[:2]
+
+    # All rows/columns are the same
+    np.testing.assert_array_almost_equal(np.diff(u, axis=0), 0, decimal=5)
+    np.testing.assert_array_almost_equal(np.diff(v, axis=1), 0, decimal=5)
+    # All the columns/rows are spaced by 1/s
+    np.testing.assert_array_almost_equal(np.diff(u, axis=1), 1/s1, decimal=5)
+    np.testing.assert_array_almost_equal(np.diff(v, axis=0), 1/s2, decimal=5)
+    # First element is (1/s)/2
+    np.testing.assert_array_almost_equal(u[0,0], 1/s1/2, decimal=5)
+    np.testing.assert_array_almost_equal(v[0,0], 1/s2/2, decimal=5)
+
+
 @pytest.mark.parametrize("envmap_type,in_sz,out_sz", product(SUPPORTED_FORMATS, [512, 431, 271], [512, 431, 271]))
 def test_resize_integer(envmap_type, in_sz, out_sz):
     e = get_envmap(in_sz, 1, envmap_type, 1)
     old_energy = e.data.mean()
     old = e.data.copy()
     e = e.copy().resize(out_sz, debug=True)
     new_energy = e.data.mean()
@@ -191,7 +210,61 @@
     e = EnvironmentMap(128, format_)
     if normal == "rand":
         normal = np.random.rand(3) + 1e-4
         normal /= np.linalg.norm(normal)
 
     normal = np.asarray(normal)
     u, v = e.world2image(*normal)
+
+
+@pytest.mark.parametrize("format_1, format_2", product(SUPPORTED_FORMATS, SUPPORTED_FORMATS))
+def test_interpolation_convertTo_discrete_values(format_1, format_2):
+    # test interpolation order 0 (nearest neighbor)
+
+    # converTo() should not change the unique values in the data
+    e_1 = EnvironmentMap(128, format_1)
+    e_1.data = np.random.randint(0,512, size=e_1.data.shape)
+    unique_1 = np.unique(e_1.data)
+        
+    # convertTo()
+    e_2 = e_1.convertTo(format_2, order=0)
+    # e_2 contains nan values... ¯\_(ツ)_/¯
+    unique_2 = [x for x in np.unique(e_2.data) if not np.isnan(x)]
+
+    assert len(unique_2) > 0, f"Format {format_1}->{format_2}: unique_2 is empty"
+    for x in unique_2:
+        assert x in unique_1, f"Format {format_1}->{format_2}: {x} was not in unique_1"
+
+
+@pytest.mark.parametrize("format_", SUPPORTED_FORMATS)
+def test_interpolation_rotate_discrete_values(format_):
+    # rotate() should not change the unique values in the data
+    for i in range(0,360,10):
+        e_1 = EnvironmentMap(128, format_)
+        e_1.data = np.random.randint(0, 512, size=e_1.data.shape)
+        unique_1 = np.unique(e_1.data)
+
+        # Rotate
+        angle = np.deg2rad(i)
+        dcm = rotations.roty(angle)
+        e_2 = e_1.rotate(dcm, order=0)
+
+        unique_2 = np.unique(e_2.data) 
+        assert len(unique_2) > 0, f"Format {format_}: unique_2 is empty"
+        for x in unique_2:
+            assert x in unique_1, f"Format {format_}: {x} was not in {unique_1}"
+
+
+@pytest.mark.parametrize("format_", SUPPORTED_FORMATS)
+def test_interpolation_resize_discrete_values(format_):
+    # scale() should not change the unique values in the data while upscaling
+    for s in [32,64,100,200,256,512]:
+        e_1 = EnvironmentMap(128, format_)
+        e_1.data = np.random.randint(0, 128, size=e_1.data.shape)
+        unique_1 = [ x for x in np.unique(e_1.data) if not np.isnan(x) ]
+
+        e_2 = e_1.resize(s, order=0)
+        unique_2 = [ x for x in np.unique(e_2.data) if not np.isnan(x) ]
+
+        assert len(unique_2) > 0, f"Format {format_}: unique_2 is empty"
+        for x in unique_2:
+            assert x in unique_1 , f"Format {format_}: {x} was not in {unique_1}"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skylibs-0.7.2/tools3d/__init__.py` & `skylibs-0.7.3/tools3d/__init__.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/tools3d/display.py` & `skylibs-0.7.3/tools3d/display.py`

 * *Files identical despite different names*

### Comparing `skylibs-0.7.2/tools3d/spharm.py` & `skylibs-0.7.3/tools3d/spharm.py`

 * *Files identical despite different names*

