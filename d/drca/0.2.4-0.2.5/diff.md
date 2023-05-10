# Comparing `tmp/drca-0.2.4-py3-none-any.whl.zip` & `tmp/drca-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9372 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    32209 b- defN 23-May-03 04:07 drca/DR_assisted_CA.py
+Zip file size: 9802 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    34370 b- defN 23-May-10 06:31 drca/DR_assisted_CA.py
 -rw-rw-rw-  2.0 fat       29 b- defN 23-Feb-15 11:13 drca/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      239 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      520 b- defN 23-May-03 04:10 drca-0.2.4.dist-info/RECORD
-7 files, 34174 bytes uncompressed, 8454 bytes compressed:  75.3%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-10 08:21 drca-0.2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      239 b- defN 23-May-10 08:21 drca-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 08:21 drca-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-May-10 08:21 drca-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      520 b- defN 23-May-10 08:21 drca-0.2.5.dist-info/RECORD
+7 files, 36335 bytes uncompressed, 8884 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: drca/DR_assisted_CA.py
 Comment: 
 
 Filename: drca/__init__.py
 Comment: 
 
-Filename: drca-0.2.4.dist-info/LICENSE
+Filename: drca-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: drca-0.2.4.dist-info/METADATA
+Filename: drca-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: drca-0.2.4.dist-info/WHEEL
+Filename: drca-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: drca-0.2.4.dist-info/top_level.txt
+Filename: drca-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: drca-0.2.4.dist-info/RECORD
+Filename: drca-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## drca/DR_assisted_CA.py

```diff
@@ -7,14 +7,15 @@
 import tifffile
 
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.cm as cm
 import matplotlib.colors as mcolors
 from matplotlib.colors import ListedColormap
+from matplotlib.colors import hsv_to_rgb
 
 from sklearn.decomposition import NMF, PCA
 from sklearn.manifold import TSNE
 from sklearn.cluster import OPTICS
 
 import ipywidgets as pyw
 import time
@@ -319,56 +320,100 @@
 
         elif len(comp_axes) == 3:
             self.X = np.stack((self.aDR_coeffs[:, comp_axes[0]], self.aDR_coeffs[:, comp_axes[1]], self.aDR_coeffs[:, comp_axes[2]]), axis=1)
             print(self.X.shape)
             
         if quick_visual:    
             center = np.mean(self.X, axis=0)
-            dist_from_center = np.sum((self.X-center)**2, axis=1)
-            max_radius = np.sqrt(np.max(dist_from_center))
+            dist_from_center = np.sqrt(np.sum((self.X-center)**2, axis=1))
+            max_radius = np.max(dist_from_center)
 
             X_shift = self.X - center
 
             r_point = [0, -2*max_radius]
             g_point = [3**(1/2)*max_radius, max_radius]
             b_point = [-3**(1/2)*max_radius, max_radius]
 
             red = np.sqrt(np.sum((X_shift-r_point)**2, axis=1))
+            red = red - np.max(red)*1.5
+            red = -red
             red = red / np.max(red)
             green = np.sqrt(np.sum((X_shift-g_point)**2, axis=1))
+            green = green - np.max(green)*1.5
+            green = -green
             green = green / np.max(green)
             blue = np.sqrt(np.sum((X_shift-b_point)**2, axis=1))
+            blue = blue - np.max(blue)*1.5
+            blue = -blue
             blue = blue / np.max(blue)
             alpha = np.ones_like(red)
             point_colors = np.stack((red, green, blue, alpha), axis=1)
 
-            fig, ax = plt.subplots(1, 1, figsize=(5, 5))
-            ax.scatter(X_shift[:, 0], X_shift[:, 1], s=3, c=point_colors)
-            ax.scatter(center[0], center[1], s=5, c="red")
+            fig, ax = plt.subplots(1, 1, figsize=(7, 7))
+            ax.scatter(r_point[1], r_point[0], s=10, c="red", marker="*")
+            ax.scatter(g_point[1], g_point[0], s=10, c="green", marker="*")
+            ax.scatter(b_point[1], b_point[0], s=10, c="blue", marker="*")
+            ax.scatter(X_shift[:, 1], X_shift[:, 0], s=3, c=point_colors)
+            ax.scatter(center[1], center[0], s=5, c="red", marker="D")
             fig.tight_layout()
             plt.show()
 
-            color_reshape = reshape_coeff(point_colors, self.data_shape)
-            red_reshape = reshape_coeff(np.expand_dims(red, axis=1), self.data_shape)
-            green_reshape = reshape_coeff(np.expand_dims(green, axis=1), self.data_shape)
-            blue_reshape = reshape_coeff(np.expand_dims(blue, axis=1), self.data_shape)
+            self.color_reshape = reshape_coeff(point_colors, self.data_shape)
+            self.red_reshape = reshape_coeff(np.expand_dims(red, axis=1), self.data_shape)
+            self.green_reshape = reshape_coeff(np.expand_dims(green, axis=1), self.data_shape)
+            self.blue_reshape = reshape_coeff(np.expand_dims(blue, axis=1), self.data_shape)
 
             for j in range(self.num_img):
                 fig, ax = plt.subplots(1, 4, figsize=(5*4, 5))
-                ax[0].imshow(color_reshape[j])
+                ax[0].imshow(self.color_reshape[j])
                 ax[0].axis("off")
-                ax[1].imshow(red_reshape[j], cmap="Reds")
+                ax[1].imshow(self.red_reshape[j], cmap="Reds")
                 ax[1].axis("off")
-                ax[2].imshow(green_reshape[j], cmap="Greens")
+                ax[2].imshow(self.green_reshape[j], cmap="Greens")
                 ax[2].axis("off")
-                ax[3].imshow(blue_reshape[j], cmap="Blues")
+                ax[3].imshow(self.blue_reshape[j], cmap="Blues")
                 ax[3].axis("off")
                 fig.tight_layout()
                 plt.show()
 
+            XY = np.zeros((X_shift.shape[0], 3,), dtype=float)
+            dist_scale = dist_from_center / max_radius
+            for i in range(X_shift.shape[0]):
+                XY[i] = np.angle(np.complex(X_shift[i, 1], X_shift[i, 0])) / (2 * np.pi) % 1, 1, dist_scale[i]
+
+            self.Xdir = hsv_to_rgb(XY)
+
+            self.wheel_reshape = reshape_coeff(self.Xdir, self.data_shape)
+
+            x_, y_ = np.meshgrid(np.linspace(-1, 1, 100, endpoint=True), np.linspace(-1, 1, 100, endpoint=True))
+            X_, Y_ = x_ * (x_ ** 2 + y_ ** 2 < 1.0 ** 2), y_ * (x_ ** 2 + y_ ** 2 < 1.0 ** 2)
+            ref_color = np.zeros(X_.shape + (3,), dtype=float)
+
+            rad_map = np.sqrt(X_ ** 2 + Y_ ** 2) / np.amax(np.sqrt(X_ ** 2 + Y_ ** 2))
+            for i in range(X_.shape[0]):
+                for j in range(X_.shape[1]):
+                    ref_color[i, j] = np.angle(np.complex(X_[i, j], Y_[i, j])) / (2 * np.pi) % 1, 1, rad_map[i, j]
+            self.color_wheel = hsv_to_rgb(ref_color)
+
+            fig, ax = plt.subplots(1, 2, figsize=(10, 5))
+            ax[0].scatter(X_shift[:, 1], X_shift[:, 0], s=3, c=self.Xdir, alpha=0.5)
+            ax[0].scatter(center[1], center[0], s=5, c="red", marker="D")
+            ax[1].imshow(self.color_wheel, origin="lower")
+            ax[1].axis("off")
+            fig.tight_layout()
+            plt.show()
+
+            for j in range(self.num_img):
+                fig, ax = plt.subplots(1, 1, figsize=(5*4, 5))
+                ax.imshow(self.wheel_reshape[j])
+                ax.axis("off")
+                fig.tight_layout()
+                plt.show()            
+            
+
     def cluster_analysis(self, method="optics", ini_params=None):
         
         self.fig = plt.figure(figsize=(10, 8))
         G = gridspec.GridSpec(2, 4)
         self.ax1 = plt.subplot(G[0, :])
 
         if self.num_comp_vis == 3:
```

## Comparing `drca-0.2.4.dist-info/LICENSE` & `drca-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

