# Comparing `tmp/mask2bbox-0.0.6.tar.gz` & `tmp/mask2bbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.6.tar", last modified: Mon May  8 12:59:22 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.7.tar", last modified: Wed May 10 08:36:28 2023, max compression
```

## Comparing `mask2bbox-0.0.6.tar` & `mask2bbox-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.094933 mask2bbox-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.094933 mask2bbox-0.0.6/src/mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/_bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/src/mask2bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 12:59:22.000000 mask2bbox-0.0.6/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:22.098933 mask2bbox-0.0.6/tests/test_mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 12:59:11.000000 mask2bbox-0.0.6/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.412374 mask2bbox-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.6/LICENSE.txt` & `mask2bbox-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.6/PKG-INFO` & `mask2bbox-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -60,27 +60,31 @@
 all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
 all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+### 0.0.7 - Improved functionality
+Improvements in IoU calculation
+
+### 0.0.6 - Added functionality
 
 ### 0.0.5 - Added functionality
 
 - IoU related operations:
   - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+Example of `boxes.plot_to_mask()`
 ![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
```

### Comparing `mask2bbox-0.0.6/README.md` & `mask2bbox-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,27 +43,31 @@
 all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
 all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+### 0.0.7 - Improved functionality
+Improvements in IoU calculation
+
+### 0.0.6 - Added functionality
 
 ### 0.0.5 - Added functionality
 
 - IoU related operations:
   - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+Example of `boxes.plot_to_mask()`
 ![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
```

### Comparing `mask2bbox-0.0.6/setup.py` & `mask2bbox-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.6",
+    version="0.0.7",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `mask2bbox-0.0.6/src/mask2bbox/_bboxes.py` & `mask2bbox-0.0.7/src/mask2bbox/_bboxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 from matplotlib import pyplot as plt
 
 
 # Create a bbox class
 class BBoxes:
     """Class to calculate and represent bounding boxes from a mask file"""
-    n: int
     bbox: np.ndarray
 
     # Constructor
     def __init__(self, mask_file):
         # Read in the mask file
         self.mask = io.imread(mask_file)
 
@@ -165,21 +164,30 @@
         x2 = min(box1[2], box2[2])
         y1 = max(box1[3], box2[3])
         y2 = min(box1[4], box2[4])
 
         # Calculate intersection area
         intersection = max(0, x2 - x1) * max(0, y2 - y1)
 
+        # If intersection is 0 IoU is 0
+        if intersection == 0:
+            return 0
+
         # Calculate union area
-        area1 = (box1[3] - box1[1]) * (box1[4] - box1[2])
-        area2 = (box2[3] - box2[1]) * (box2[4] - box2[2])
+        area1 = (box1[2] - box1[1]) * (box1[4] - box1[3])
+        area2 = (box2[2] - box2[1]) * (box2[4] - box2[3])
         union = area1 + area2 - intersection
 
         # Calculate and return IoU
-        return intersection / union
+        iou = intersection / union
+
+        if intersection > union:
+            print(intersection, union, iou)
+
+        return iou
 
     @property
     def iou_matrix(self) -> ndarray:
         n = self.__len__()
         # compute the size of the matrix based on the length of the array
         size = n * (n - 1) // 2
 
@@ -217,13 +225,15 @@
         v = iou_matrix[x, y]
         x = self.bboxes[x, 0]
         y = self.bboxes[y, 0]
 
         return np.array([x, y]).T, v
 
     def save_iou(self, output_file: str) -> None:
+        pairs, values = self.overlapping_pairs()
+
         # Save the IoU matrix to a csv file
-        np.savetxt(output_file, self.iou_matrix, delimiter=",")
+        np.savetxt(output_file, pairs, delimiter=",", fmt="%d")
 
     def save_csv(self, output_file: str) -> None:
         # Save the bounding boxes to a csv file
         np.savetxt(output_file, self.bboxes, delimiter=",", fmt="%d")
```

### Comparing `mask2bbox-0.0.6/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.0.7/src/mask2bbox/mask2bbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,16 @@
                          help="Number of pixels to expand the bounding boxes.")
     options.add_argument("-fs", "--filter-small", dest="filter_small", action="store", type=int, required=False,
                          default=0, help="Filter bounding boxes smaller than the provided value [default=0].")
     options.add_argument("-fl", "--filter-large", dest="filter_large", action="store", type=int, required=False,
                          default=0, help="Filter bounding boxes larger than the provided value [default=0].")
     options.add_argument("-r", "--remove-edge", dest="remove_edge", action="store_true", required=False,
                          default=False, help="Remove bounding boxes that are on the edge of the image.")
+    options.add_argument("-fo", "--filter-overlap", dest="filter_overlap", action="store_true", required=False,
+                         default=False, help="Filter bounding boxes that overlap.")
 
     # Add a group of arguments for output
     output = parser.add_argument_group(title="Output", description="Output arguments for the script.")
     output.add_argument("-o", "--output", dest="output", action="store", type=str, required=True,
                         help="Path to the output file with the bounding boxes.")
     output.add_argument("-p", "--plot", dest="plot", action="store", type=str, required=False, default=None,
                         help="Path to the output file with the bounding boxes.")
@@ -47,24 +49,25 @@
 
     # Parse arguments
     args = parser.parse_args()
 
     # Standardize paths
     args.mask = Path(args.mask).resolve()
     args.output = Path(args.output).resolve()
+    args.save_iou = Path(args.save_iou).resolve() if args.save_iou is not None else None
     args.plot = Path(args.plot).resolve() if args.plot is not None else None
 
     # Return arguments
     return args
 
 
 def main(args):
     # Create a BBoxes object and get the bounding boxes
     mask_boxes = BBoxes(args.mask)
-    print(f"Total number of bounding boxes     = {mask_boxes.n}")
+    print(f"Total number of bounding boxes     = {len(mask_boxes)}")
 
     # Expand the bounding boxes
     mask_boxes.expand(n=args.expand)
     print(f"Expanding bounding boxes by        = {args.expand}")
 
     # Filter small bounding boxes
     if args.filter_small > 0:
@@ -72,32 +75,37 @@
         mask_boxes.filter_identities(mask_boxes.are_dims_smaller_than((args.filter_small, args.filter_small)))
 
     # Filter large bounding boxes
     if args.filter_large > 0:
         print(f"Keeping bounding boxes larger than = ({args.filter_large}x{args.filter_large})")
         mask_boxes.filter_identities(mask_boxes.are_dims_larger_than((args.filter_large, args.filter_large)))
 
+    # Filter overlapping
+    if args.filter_overlap:
+        print("Removing overlapping bounding boxes")
+        mask_boxes.filter_identities(mask_boxes.are_overlapping())
+
     # Remove bounding boxes on the edge
     if args.remove_edge:
         print("Removing bounding boxes on the edge")
         mask_boxes.remove_edge_boxes()
 
     # Plot bounding boxes
     if args.plot is not None:
-        print(f"Saving plot to                    = {args.plot}")
+        print(f"Saving plot to                     = {args.plot}")
         mask_boxes.plot_to_mask(args.plot)
 
     # Save IoU matrix
     if args.save_iou is not None:
-        print(f"Saving IoU matrix to              = {args.save_iou}")
+        print(f"Saving IoU matrix to               = {args.save_iou}")
         mask_boxes.save_iou(args.save_iou)
 
     # Save file
     print(f"Saving bounding boxes to           = {args.output}")
-    print(f"Number of bounding boxes saved:    = {mask_boxes.n}")
+    print(f"Number of bounding boxes saved:    = {len(mask_boxes)}")
     mask_boxes.save_csv(args.output)
 
 
 # Run main
 if __name__ == "__main__":
     # Get arguments
     args = get_arguments()
```

### Comparing `mask2bbox-0.0.6/src/mask2bbox.egg-info/PKG-INFO` & `mask2bbox-0.0.7/src/mask2bbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -60,27 +60,31 @@
 all_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
 all_boxes.save_csv("path/to/bounding_boxes.csv")
 ```
 
 ## Version Notes
+### 0.0.7 - Improved functionality
+Improvements in IoU calculation
+
+### 0.0.6 - Added functionality
 
 ### 0.0.5 - Added functionality
 
 - IoU related operations:
   - `boxes.get_iou_matrix()` - Gets the IoU of all the bounding boxes.
   - `boxes.are_overlaping()` - Returns identities where the IoU is greater than 0
   - `boxes.overlaping_pais()` - Returns the pairs of bounding boxes that are overlaping.
   - `boxes.save_iou()` - Saves the IoU matrix to a csv file.
 
 - Plots
   - `boxes.plot_to_mask()` Plots the bounding boxes on the mask image.
 
-Example of `boxes.plot_to_mask()` where only the overlapping bounding boxes are highlighted.
+Example of `boxes.plot_to_mask()`
 ![](tests/plot.png)
 
 ### 0.0.4 - Added functionality
 Now is possible to extract:
 - Bounding boxes dimensions `BBoxes.get_bbox_dims()`
 - Bounding boxes area `BBoxes.get_bbox_areas()`
 - Bounding boxes center `BBoxes.get_bbox_centers()`
```

