# Comparing `tmp/image_frequency_analysis-0.2.1.tar.gz` & `tmp/image_frequency_analysis-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.1.tar", last modified: Sun Apr 23 16:17:33 2023, max compression
+gzip compressed data, was "image_frequency_analysis-0.2.2.tar", last modified: Wed May 10 13:03:57 2023, max compression
```

## Comparing `image_frequency_analysis-0.2.1.tar` & `image_frequency_analysis-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:17:33.656262 image_frequency_analysis-0.2.1/
--rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1800 2023-04-23 16:17:33.655311 image_frequency_analysis-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2023-04-23 16:15:13.000000 image_frequency_analysis-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 16:17:33.535153 image_frequency_analysis-0.2.1/image_frequency_analysis/
--rw-rw-rw-   0        0        0     1648 2023-04-23 16:15:13.000000 image_frequency_analysis-0.2.1/image_frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     4870 2023-04-23 16:15:13.000000 image_frequency_analysis-0.2.1/image_frequency_analysis/frequency_analysis.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:17:33.652701 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0     1800 2023-04-23 16:17:32.000000 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-04-23 16:17:33.000000 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:17:32.000000 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-23 16:17:32.000000 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-23 16:17:32.000000 image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 16:17:33.657255 image_frequency_analysis-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-04-23 16:17:05.000000 image_frequency_analysis-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.778496 image_frequency_analysis-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1647 2023-05-10 13:03:57.777498 image_frequency_analysis-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-05-10 13:03:27.000000 image_frequency_analysis-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.768498 image_frequency_analysis-0.2.2/image_frequency_analysis/
+-rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/image_frequency_analysis/__init__.py
+-rw-rw-rw-   0        0        0     6507 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/image_frequency_analysis/frequency_analysis.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:57.775524 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/
+-rw-rw-rw-   0        0        0     1647 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-10 13:03:57.000000 image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:03:57.778496 image_frequency_analysis-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.2/setup.py
```

### Comparing `image_frequency_analysis-0.2.1/LICENSE` & `image_frequency_analysis-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.1/PKG-INFO` & `image_frequency_analysis-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: image_frequency_analysis
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Author: M Thivagar
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Image Frequency Analysis
 
 This package is build to combine all the steps that are done as part of the
@@ -21,31 +22,28 @@
 
 `pip install image_frequency_analysis` - when installing through a command prompt
 
 
 ## Using the package
 Once you have installed you can use the package by importing the image_frequency_analysis method from the package
 
-` from image_frequency_analysis import image_frequency_analysis as ifa `
+` import image_frequency_analysis as ifa `
 
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
-` ifa('sandstone.tif') `
+` ifa.FrequencyAnalysis('sandstone.tif') `
 
 **Sample Output:**
 
-![image](https://user-images.githubusercontent.com/51501788/233843791-a3fc6c79-ea7f-43ed-8e13-da91caf21749.png)
+![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
 
 
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
-` help(ifa) ` or `help(image_frequency_analysis`
+` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
 
-
-For request of any new feature or an issue please raise an issue
-with the appropriate label as Bug or Enhancement - [Raise Issue](https://github.com/thivagar-manickam/image_frequency_analysis/issues)
```

### Comparing `image_frequency_analysis-0.2.1/README.md` & `image_frequency_analysis-0.2.2/image_frequency_analysis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: image-frequency-analysis
+Version: 0.2.2
+Summary: A package to perform image frequency analysis using the Fourier Transform method
+Author: M Thivagar
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Image Frequency Analysis
 
 This package is build to combine all the steps that are done as part of the
 frequency analysis using the Fourier transform approach.
 
 
 
@@ -12,31 +22,28 @@
 
 `pip install image_frequency_analysis` - when installing through a command prompt
 
 
 ## Using the package
 Once you have installed you can use the package by importing the image_frequency_analysis method from the package
 
-` from image_frequency_analysis import image_frequency_analysis as ifa `
+` import image_frequency_analysis as ifa `
 
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
-` ifa('sandstone.tif') `
+` ifa.FrequencyAnalysis('sandstone.tif') `
 
 **Sample Output:**
 
-![image](https://user-images.githubusercontent.com/51501788/233843791-a3fc6c79-ea7f-43ed-8e13-da91caf21749.png)
+![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
 
 
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
-` help(ifa) ` or `help(image_frequency_analysis`
-
+` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
 
-For request of any new feature or an issue please raise an issue
-with the appropriate label as Bug or Enhancement - [Raise Issue](https://github.com/thivagar-manickam/image_frequency_analysis/issues)
```

### Comparing `image_frequency_analysis-0.2.1/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.2/image_frequency_analysis/frequency_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 
 
 class FrequencyAnalysis:
+    """
+    This definition invokes the Frequency Analysis class
+    to apply the Transformation on the image based on the
+    attributes passed to the class
+
+    Attributes:
+
+    image_path - This is the file path for the image on which the transformation needs to be applied
+
+    filter_radius - This property defines to what extent the low or high frequency value needs to be allowed to
+                    pass through in the filtering process. Default value = 80
+
+    high_pass_filter - This is a boolean value which indicates to use the default high pass filter mask on the image.
+                    Default value = False
+
+    low_pass_filter - This is a boolean value which indicates to use the default low pass filter mask on the image.
+                    Default value = False
+
+    When both the high_pass_filter and low_pass_filter is False, by default high pass filter mask is applied on the image.
+
+    Throws value error when both high_pass_filter and low_pass_filter value are set to be True.
+
+    """
     def __init__(
         self,
         image_path,
         filter_radius=80,
         high_pass_filter=False,
         low_pass_filter=False,
     ):
+        self.mask_area = None
+        self.fft_image = None
+        self.dft_image = None
+        self.column_center = None
+        self.row_center = None
+        self.rows = None
+        self.columns = None
         self.image_path = image_path
         self.radius = filter_radius
         self.high_pass_filter = high_pass_filter
         self.low_pass_filter = low_pass_filter
         self.image = self.load_image(self.image_path)
 
-        if not high_pass_filter and not low_pass_filter:
-            self.high_pass_filter = True
-
         self.perform_image_frequency_analysis()
 
     """
     Definition to load the image into the
     image object which will be used for further
     processing
     """
@@ -108,15 +135,16 @@
         plt.imshow(self.image)
 
         plt.subplot(1, 3, 2)
         plt.title("Frequency Shifted Mask")
         plt.imshow(frequency_shift_magnitude, cmap="gray")
 
         plt.subplot(1, 3, 3)
-        plt.title("Image post applying the filter mask")
+        filter_type = "Low Pass filter" if self.low_pass_filter else "High Pass Filter"
+        plt.title(f"Image post applying the {filter_type} mask")
         plt.imshow(image, cmap="gray")
 
     def perform_filtering_and_inverse_transform(self, mask):
         frequency_shift = self.fft_image * mask
 
         frequency_mask_magnitude = 20 * np.log(
             cv2.magnitude(frequency_shift[:, :, 0], frequency_shift[:, :, 1]) + 1
@@ -143,14 +171,23 @@
     def perform_low_pass_filter_analysis(self):
         lpf_mask = self.get_low_pass_filter_mask_matrix()
         lpf_mask[self.mask_area] = 1
 
         return self.perform_filtering_and_inverse_transform(lpf_mask)
 
     def perform_image_frequency_analysis(self):
+        if self.high_pass_filter and self.low_pass_filter:
+            raise ValueError(
+                        "Both high_pass_filter and low_pass_filter flag cannot be True. Please choose only one type "
+                        "of filter"
+                    )
+
+        if not self.high_pass_filter and not self.low_pass_filter:
+            self.high_pass_filter = True
+
         self.calculate_dft_of_image()
 
         self.perform_frequency_shifting()
 
         self.set_rows_columns_details()
 
         self.calculate_mask_area()
@@ -159,7 +196,8 @@
             final_image = self.perform_high_pass_filter_analysis()
         else:
             final_image = self.perform_low_pass_filter_analysis()
 
         final_image = (final_image / final_image.max() * 255).astype("uint8")
 
         return final_image
+
```

### Comparing `image_frequency_analysis-0.2.1/image_frequency_analysis.egg-info/PKG-INFO` & `image_frequency_analysis-0.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: image-frequency-analysis
-Version: 0.2.1
-Summary: A package to perform image frequency analysis using the Fourier Transform method
-Author: M Thivagar
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Image Frequency Analysis
 
 This package is build to combine all the steps that are done as part of the
 frequency analysis using the Fourier transform approach.
 
 
 
@@ -21,31 +12,28 @@
 
 `pip install image_frequency_analysis` - when installing through a command prompt
 
 
 ## Using the package
 Once you have installed you can use the package by importing the image_frequency_analysis method from the package
 
-` from image_frequency_analysis import image_frequency_analysis as ifa `
+` import image_frequency_analysis as ifa `
 
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
-` ifa('sandstone.tif') `
+` ifa.FrequencyAnalysis('sandstone.tif') `
 
 **Sample Output:**
 
-![image](https://user-images.githubusercontent.com/51501788/233843791-a3fc6c79-ea7f-43ed-8e13-da91caf21749.png)
+![image](https://github.com/thivagar-manickam/image_frequency_analysis/assets/51501788/e94cc29b-a7a5-4768-aebf-5e4a17a92517)
 
 
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
-` help(ifa) ` or `help(image_frequency_analysis`
-
+` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
 
-For request of any new feature or an issue please raise an issue
-with the appropriate label as Bug or Enhancement - [Raise Issue](https://github.com/thivagar-manickam/image_frequency_analysis/issues)
```

### Comparing `image_frequency_analysis-0.2.1/setup.py` & `image_frequency_analysis-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="image_frequency_analysis",
-    version="0.2.1",
+    version="0.2.2",
     author="M Thivagar",
     packages=find_packages(),
     install_requires=["opencv-python", "numpy", "pandas", "matplotlib"],
     python_requires=">=3.6",
-    homepage="https://github.com/thivagar-manickam/image_frequency_analysis",
     description="A package to perform image frequency analysis using the Fourier Transform method",
-    bugtracker="https://github.com/thivagar-manickam/image_frequency_analysis/issues",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    license="MIT",
 )
```

