# Comparing `tmp/myoquant-0.3.1.tar.gz` & `tmp/myoquant-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myoquant-0.3.1.tar", max compression
+gzip compressed data, was "myoquant-0.3.3.tar", max compression
```

## Comparing `myoquant-0.3.1.tar` & `myoquant-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    34523 2022-11-17 11:09:05.681340 myoquant-0.3.1/LICENSE
--rw-r--r--   0        0        0     6253 2023-01-19 15:22:57.198718 myoquant-0.3.1/README.md
--rw-r--r--   0        0        0        0 2022-11-17 11:09:05.681340 myoquant-0.3.1/myoquant/__init__.py
--rw-r--r--   0        0        0      571 2023-01-19 14:35:23.538715 myoquant-0.3.1/myoquant/__main__.py
--rw-r--r--   0        0        0        0 2022-11-30 10:00:33.355328 myoquant-0.3.1/myoquant/commands/__init__.py
--rw-r--r--   0        0        0     3599 2022-12-05 12:16:17.250043 myoquant-0.3.1/myoquant/commands/docs.py
--rw-r--r--   0        0        0     9748 2023-01-19 13:53:06.568720 myoquant-0.3.1/myoquant/commands/run_atp.py
--rw-r--r--   0        0        0    13818 2022-12-05 12:16:17.250043 myoquant-0.3.1/myoquant/commands/run_he.py
--rw-r--r--   0        0        0    11258 2023-01-20 14:49:57.438422 myoquant-0.3.1/myoquant/commands/run_sdh.py
--rw-r--r--   0        0        0     4580 2023-01-24 10:39:31.016334 myoquant-0.3.1/myoquant/src/ATP_analysis.py
--rw-r--r--   0        0        0     8667 2023-01-23 14:49:57.230712 myoquant-0.3.1/myoquant/src/HE_analysis.py
--rw-r--r--   0        0        0     3865 2023-01-24 09:50:00.106346 myoquant-0.3.1/myoquant/src/SDH_analysis.py
--rw-r--r--   0        0        0        0 2022-11-30 10:00:33.355328 myoquant-0.3.1/myoquant/src/__init__.py
--rw-r--r--   0        0        0     6084 2023-01-23 14:56:12.500727 myoquant-0.3.1/myoquant/src/common_func.py
--rw-r--r--   0        0        0     2673 2022-12-05 12:16:17.250043 myoquant-0.3.1/myoquant/src/draw_line.py
--rw-r--r--   0        0        0     3319 2022-12-05 12:16:17.250043 myoquant-0.3.1/myoquant/src/gradcam.py
--rw-r--r--   0        0        0    15363 2022-11-30 10:00:33.355328 myoquant-0.3.1/myoquant/src/random_brightness.py
--rw-r--r--   0        0        0     1123 2023-01-24 10:39:17.116322 myoquant-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7518 1970-01-01 00:00:00.000000 myoquant-0.3.1/setup.py
--rw-r--r--   0        0        0     7550 1970-01-01 00:00:00.000000 myoquant-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-16 19:47:14.112913 myoquant-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6253 2023-02-11 20:09:37.818948 myoquant-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/__init__.py
+-rw-r--r--   0        0        0     1473 2023-05-10 12:40:33.520835 myoquant-0.3.3/myoquant/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/__init__.py
+-rw-r--r--   0        0        0     3599 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/docs.py
+-rw-r--r--   0        0        0    11882 2023-05-10 12:40:33.564835 myoquant-0.3.3/myoquant/commands/run_atp.py
+-rw-r--r--   0        0        0    13818 2023-01-16 19:47:14.112913 myoquant-0.3.3/myoquant/commands/run_he.py
+-rw-r--r--   0        0        0    11258 2023-02-11 20:09:37.842948 myoquant-0.3.3/myoquant/commands/run_sdh.py
+-rw-r--r--   0        0        0     6274 2023-05-10 12:40:33.584834 myoquant-0.3.3/myoquant/src/ATP_analysis.py
+-rw-r--r--   0        0        0     8667 2023-02-11 20:09:37.874947 myoquant-0.3.3/myoquant/src/HE_analysis.py
+-rw-r--r--   0        0        0     3865 2023-02-11 20:09:37.878947 myoquant-0.3.3/myoquant/src/SDH_analysis.py
+-rw-r--r--   0        0        0        0 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/__init__.py
+-rw-r--r--   0        0        0     6809 2023-05-10 12:40:33.584834 myoquant-0.3.3/myoquant/src/common_func.py
+-rw-r--r--   0        0        0     2673 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/draw_line.py
+-rw-r--r--   0        0        0     3319 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/gradcam.py
+-rw-r--r--   0        0        0    15363 2023-01-16 19:47:14.116913 myoquant-0.3.3/myoquant/src/random_brightness.py
+-rw-r--r--   0        0        0     1123 2023-05-10 12:44:13.334072 myoquant-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7550 1970-01-01 00:00:00.000000 myoquant-0.3.3/PKG-INFO
```

### Comparing `myoquant-0.3.1/LICENSE` & `myoquant-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/README.md` & `myoquant-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/commands/docs.py` & `myoquant-0.3.3/myoquant/commands/docs.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/commands/run_atp.py` & `myoquant-0.3.3/myoquant/commands/run_atp.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,40 @@
         max=254,
         help="Fiber intensity threshold to differenciate between the two fiber types. If not specified, the analysis will try to deduce it.",
     ),
     cellpose_diameter: int = typer.Option(
         None,
         help="Approximative single cell diameter in pixel for CellPose detection. If not specified, Cellpose will try to deduce it.",
     ),
+    channel: int = typer.Option(
+        None,
+        help="Image channel to use for the analysis. If not specified, the analysis will be performed on all three channels.",
+    ),
+    channel_first: bool = typer.Option(
+        False,
+        help="If the channel is the first dimension of the image, set this to True. False by default.",
+    ),
+    rescale_exposure: bool = typer.Option(
+        False,
+        help="Rescale the image exposure if your image is not in the 0 255 forma, False by default.",
+    ),
+    n_classes: int = typer.Option(
+        2,
+        max=10,
+        help="The number of classes of cell to detect. If not specified this is defaulted to two classes.",
+    ),
+    intensity_method: str = typer.Option(
+        "median",
+        help="The method to use to compute the intensity of the cell. Can be either 'median' or 'mean'.",
+    ),
+    erosion: int = typer.Option(
+        False,
+        max=45,
+        help="Perform an erosion on the cells images to remove signal in the cell membrane (usefull for fluo). Expressed in percentage of the cell radius",
+    ),
     export_map: bool = typer.Option(
         True,
         help="Export the original image with cells painted by classification label.",
     ),
     export_stats: bool = typer.Option(
         True, help="Export per fiber and per nuclei stat table."
     ),
@@ -106,14 +132,15 @@
             label2rgb,
             blend_image_with_label,
             HiddenPrints,
         )
         from ..src.ATP_analysis import run_atp_analysis
         import numpy as np
         from PIL import Image
+        from skimage.exposure import rescale_intensity
 
         try:
             from imageio.v2 import imread
         except ImportError:
             from imageio import imread
 
     if output_path is None:
@@ -131,15 +158,25 @@
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         TimeElapsedColumn(),
         transient=False,
     ) as progress:
         progress.add_task(description="Reading all inputs...", total=None)
         image_ndarray = imread(image_path)
-
+        if channel is not None:
+            if channel_first:
+                # Put the channel as third dimension instead of first
+                image_ndarray = np.moveaxis(image_ndarray, 0, -1)
+            image_ndarray = image_ndarray[:, :, channel]
+        if rescale_exposure:
+            image_ndarray = rescale_intensity(
+                image_ndarray,
+                in_range=(np.amin(image_ndarray), np.amax(image_ndarray)),
+                out_range=np.uint8,
+            )
         if mask_path is not None:
             mask_ndarray = imread(mask_path)
             if np.unique(mask_ndarray).shape[0] != 2:
                 console.print(
                     "The mask image should be a binary image with only 2 values (0 and 1).",
                     style="red",
                 )
@@ -196,29 +233,39 @@
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         TimeElapsedColumn(),
         transient=False,
     ) as progress:
         progress.add_task(description="Detecting fiber types...", total=None)
-        result_df, full_label_map, df_cellpose_details = run_atp_analysis(
-            image_ndarray, mask_cellpose, intensity_threshold
+        result_df, full_label_map, df_cellpose_details, fig = run_atp_analysis(
+            image_ndarray,
+            mask_cellpose,
+            intensity_threshold,
+            n_classes,
+            intensity_method,
+            erosion,
         )
     if export_map:
         with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             TimeElapsedColumn(),
             transient=False,
         ) as progress:
             progress.add_task(
                 description="Blending label and original image together...", total=None
             )
             labelRGB_map = label2rgb(image_ndarray, full_label_map)
-            overlay_img = blend_image_with_label(image_ndarray, labelRGB_map)
+            if channel is not None:
+                overlay_img = blend_image_with_label(
+                    image_ndarray, labelRGB_map, fluo=True
+                )
+            else:
+                overlay_img = blend_image_with_label(image_ndarray, labelRGB_map)
             overlay_filename = image_path.stem + "_label_blend.tiff"
             overlay_img.save(output_path / overlay_filename)
 
     # Construct the summary table, print all output in stdout and save files in output folder.
     table.add_column("Feature", justify="left", style="cyan")
     table.add_column("Raw Count", justify="center", style="magenta")
     table.add_column("Proportion (%)", justify="right", style="green")
@@ -235,14 +282,19 @@
         output_path / csv_name,
         index=False,
     )
     console.print(
         f"💾 OUTPUT: Summary Table saved as {output_path/csv_name}",
         style="green",
     )
+    plot_name = image_path.stem + "_intensity_plot.png"
+    fig.savefig(output_path / plot_name)
+    console.print(
+        f"💾 OUTPUT: Intensity Plot saved as {output_path/plot_name}", style="green"
+    )
     if export_map:
         console.print(
             f"💾 OUTPUT: Overlay image saved as {output_path/overlay_filename}",
             style="green",
         )
     if export_stats:
         df_cellpose_details.drop("image", axis=1).to_csv(
```

### Comparing `myoquant-0.3.1/myoquant/commands/run_he.py` & `myoquant-0.3.3/myoquant/commands/run_he.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/commands/run_sdh.py` & `myoquant-0.3.3/myoquant/commands/run_sdh.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/src/HE_analysis.py` & `myoquant-0.3.3/myoquant/src/HE_analysis.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/src/SDH_analysis.py` & `myoquant-0.3.3/myoquant/src/SDH_analysis.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/src/common_func.py` & `myoquant-0.3.3/myoquant/src/common_func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Module that contains function common to both nuclei (HE/Fluo) and mitochondria analysis (SDH)
 """
 import os
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 import sys
+import math
+
 import tensorflow as tf
 import torch
 from cellpose.models import Cellpose
 from csbdeep.utils import normalize
 from stardist.models import StarDist2D
 from tensorflow import keras
 import numpy as np
 from PIL import Image
 from skimage.measure import regionprops_table
+from skimage.morphology import binary_erosion
 import pandas as pd
 
 # from .gradcam import make_gradcam_heatmap, save_and_display_gradcam
 from .random_brightness import RandomBrightness
 
+import imageio
+
 tf.random.set_seed(42)
 np.random.seed(42)
 
 if len(tf.config.list_physical_devices("GPU")) >= 1:
     use_GPU = True
     tf.config.experimental.set_memory_growth(
         tf.config.list_physical_devices("GPU")[0], True
@@ -164,20 +169,31 @@
             "perimeter",
         ],
     )
     df_stardist = pd.DataFrame(props_stardist)
     return df_stardist
 
 
-def extract_single_image(raw_image, df_props, index):
+def extract_single_image(raw_image, df_props, index, erosion=None):
     single_entity_img = raw_image[
         df_props.iloc[index, 5] : df_props.iloc[index, 7],
         df_props.iloc[index, 6] : df_props.iloc[index, 8],
     ].copy()
-    single_entity_mask = df_props.iloc[index, 9]
+    surface_area = df_props.iloc[index, 1]
+    cell_radius = math.sqrt(surface_area / math.pi)
+    single_entity_mask = df_props.iloc[index, 9].copy()
+    if erosion is not None:
+        erosion_size = cell_radius * (
+            erosion / 100
+        )  # Erosion in percentage of the cell radius
+        for i in range(int(erosion_size)):
+            single_entity_mask = binary_erosion(
+                single_entity_mask, out=single_entity_mask
+            )
+
     single_entity_img[~single_entity_mask] = 0
     return single_entity_img
 
 
 def label2rgb(img_ndarray, label_map):
     """Convert a label map to RGB image
 
@@ -188,14 +204,22 @@
     Returns:
         nd.array: RGB image of the label map with 3 colors (white, green, red) for 3 classes (background, control, abnormal)
     """
     label_to_color = {
         0: [255, 255, 255],
         1: [15, 157, 88],
         2: [219, 68, 55],
+        3: [100, 128, 170],
+        4: [231, 204, 143],
+        5: [202, 137, 115],
+        6: [178, 143, 172],
+        7: [144, 191, 207],
+        8: [148, 187, 187],
+        9: [78, 86, 105],
+        10: [245, 90, 87],
     }
     img_rgb = np.zeros((img_ndarray.shape[0], img_ndarray.shape[1], 3), dtype=np.uint8)
 
     for gray, rgb in label_to_color.items():
         img_rgb[label_map == gray, :] = rgb
     return img_rgb
```

### Comparing `myoquant-0.3.1/myoquant/src/draw_line.py` & `myoquant-0.3.3/myoquant/src/draw_line.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/src/gradcam.py` & `myoquant-0.3.3/myoquant/src/gradcam.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/myoquant/src/random_brightness.py` & `myoquant-0.3.3/myoquant/src/random_brightness.py`

 * *Files identical despite different names*

### Comparing `myoquant-0.3.1/pyproject.toml` & `myoquant-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myoquant"
-version = "0.3.1"
+version = "0.3.3"
 description = "MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images."
 authors = ["Corentin Meyer <corentin.meyer@etu.unistra.fr>"]
 maintainers = ["Corentin Meyer <corentin.meyer@etu.unistra.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://lbgi.fr/MyoQuant/"
 repository = "https://github.com/lambda-science/MyoQuant"
```

### Comparing `myoquant-0.3.1/setup.py` & `myoquant-0.3.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: myoquant
+Version: 0.3.3
+Summary: MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images.
+Home-page: https://lbgi.fr/MyoQuant/
+License: AGPL-3.0-or-later
+Keywords: histology,quantification,biology,deep-learning
+Author: Corentin Meyer
+Author-email: corentin.meyer@etu.unistra.fr
+Maintainer: Corentin Meyer
+Maintainer-email: corentin.meyer@etu.unistra.fr
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: cellpose (>=2.1.0,<3.0.0)
+Requires-Dist: csbdeep (>=0.7.2,<0.8.0)
+Requires-Dist: imageio (>=2.21.1,<3.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: rich
+Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
+Requires-Dist: stardist (>=0.8.3,<0.9.0)
+Requires-Dist: tensorflow (>=2.9.1,<3.0.0)
+Requires-Dist: typer (>=0.6.1,<0.7.0)
+Project-URL: Repository, https://github.com/lambda-science/MyoQuant
+Description-Content-Type: text/markdown
 
-packages = \
-['myoquant', 'myoquant.commands', 'myoquant.src']
+![Twitter Follow](https://img.shields.io/twitter/follow/corentinm_py?style=social) ![Demo Version](https://img.shields.io/badge/Demo-https%3A%2F%2Flbgi.fr%2FMyoQuant%2F-9cf) ![PyPi](https://img.shields.io/badge/PyPi-https%3A%2F%2Fpypi.org%2Fproject%2Fmyoquant%2F-blueviolet) ![Pypi verison](https://img.shields.io/pypi/v/myoquant) ![PyPi Python Version](https://img.shields.io/pypi/pyversions/myoquant) ![PyPi Format](https://img.shields.io/pypi/format/myoquant) ![GitHub last commit](https://img.shields.io/github/last-commit/lambda-science/MyoQuant) ![GitHub](https://img.shields.io/github/license/lambda-science/MyoQuant)
 
-package_data = \
-{'': ['*']}
+# MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images
 
-install_requires = \
-['cellpose>=2.1.0,<3.0.0',
- 'csbdeep>=0.7.2,<0.8.0',
- 'imageio>=2.21.1,<3.0.0',
- 'pandas>=1.4.3,<2.0.0',
- 'rich',
- 'scikit-image>=0.19.3,<0.20.0',
- 'scikit-learn>=1.2.0,<2.0.0',
- 'seaborn>=0.12.2,<0.13.0',
- 'stardist>=0.8.3,<0.9.0',
- 'tensorflow>=2.9.1,<3.0.0',
- 'typer>=0.6.1,<0.7.0']
-
-entry_points = \
-{'console_scripts': ['myoquant = myoquant.__main__:app']}
-
-setup_kwargs = {
-    'name': 'myoquant',
-    'version': '0.3.1',
-    'description': 'MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images.',
-    'long_description': '![Twitter Follow](https://img.shields.io/twitter/follow/corentinm_py?style=social) ![Demo Version](https://img.shields.io/badge/Demo-https%3A%2F%2Flbgi.fr%2FMyoQuant%2F-9cf) ![PyPi](https://img.shields.io/badge/PyPi-https%3A%2F%2Fpypi.org%2Fproject%2Fmyoquant%2F-blueviolet) ![Pypi verison](https://img.shields.io/pypi/v/myoquant) ![PyPi Python Version](https://img.shields.io/pypi/pyversions/myoquant) ![PyPi Format](https://img.shields.io/pypi/format/myoquant) ![GitHub last commit](https://img.shields.io/github/last-commit/lambda-science/MyoQuant) ![GitHub](https://img.shields.io/github/license/lambda-science/MyoQuant)\n\n# MyoQuant🔬: a tool to automatically quantify pathological features in muscle fiber histology images\n\n<p align="center">\n  <img src="https://i.imgur.com/mzALgZL.png" alt="MyoQuant Banner" style="border-radius: 25px;" />\n</p>\n\nMyoQuant🔬 is a command-line tool to automatically quantify pathological features in muscle fiber histology images.  \nIt is built using CellPose, Stardist, custom neural-network models and image analysis techniques to automatically analyze myopathy histology images.  \nCurrently MyoQuant is capable of quantifying centralization of nuclei in muscle fiber with HE staining, anomaly in the mitochondria distribution in muscle fibers with SDH staining and the number of type 1 muscle fiber vs type 2 muscle fiber with ATP staining.\n\nAn online demo with a web interface is available at [https://lbgi.fr/MyoQuant/](https://lbgi.fr/MyoQuant/). This project is free and open-source under the AGPL license, feel free to fork and contribute to the development.\n\n#### _Warning: This tool is still in early phases and active development._\n\n## How to install\n\n### Installing from PyPi (Preferred)\n\n**MyoQuant package is officially available on PyPi (pip) repository. [https://pypi.org/project/myoquant/](https://pypi.org/project/myoquant/) ![Pypi verison](https://img.shields.io/pypi/v/myoquant)**\n\nUsing pip, you can simply install MyoQuant in a python environment with a simple: `pip install myoquant`\n\n### Installing from sources (Developers)\n\n1. Clone this repository using `git clone https://github.com/lambda-science/MyoQuant.git`\n2. Create a virtual environment by using `python -m venv .venv`\n3. Activate the venv by using `source .venv/bin/activate`\n4. Install MyoQuant by using `pip install -e .`\n\n## How to Use\n\nTo use the command-line tool, first activate your venv in which MyoQuant is installed: `source .venv/bin/activate`  \nThen you can perform SDH or HE analysis. You can use the command `myoquant --help` to list available commands.\n\n## 💡Full command documentation is avaliable here: [CLI Documentation](https://github.com/lambda-science/MyoQuant/blob/main/CLI_Documentation.md)\n\n- **For SDH Image Analysis** the command is:  \n  `myoquant sdh-analysis IMAGE_PATH`  \n  Don\'t forget to run `myoquant sdh-analysis --help` for information about options.\n- **For HE Image Analysis** the command is:  \n  `myoquant he-analysis IMAGE_PATH`  \n   Don\'t forget to run `myoquant he-analysis --help` for information about options.\n- **For ATP Image Analysis** the command is:  \n  `myoquant atp-analysis IMAGE_PATH`  \n   Don\'t forget to run `myoquant atp-analysis --help` for information about options.\n\n_If you\'re running into an issue such as `myoquant: command not found` please check if you activated your virtual environment with the package installed. And also you can try to run it with the full command: `python -m myoquant sdh-analysis --help`_\n\n## Contact\n\nCreator and Maintainer: [**Corentin Meyer**, 3rd year PhD Student in the CSTB Team, ICube — CNRS — Unistra](https://cmeyer.fr) <corentin.meyer@etu.unistra.fr>\n\n## Citing MyoQuant🔬\n\n[placeholder]\n\n## Examples\n\nFor HE Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_he.jpg)  \nFor SDH Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_sdh.jpg)  \nFor ATP Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_atp.jpg)\n\n1. Example of successful SDH analysis output with: `myoquant sdh-analysis sample_sdh.jpg`\n\n![image](https://user-images.githubusercontent.com/20109584/210328050-11b0b6d5-28ec-41a4-b9d3-264962d04fa3.png)\n![image](https://i.imgur.com/4Nlnwdx.png) 2. Example of HE analysis: `myoquant he-analysis sample_he.jpg`\n\n![image](https://i.imgur.com/q2cXgIf.png)\n\n3. Example of ATP analysis with: `myoquan atp-analysis sample_atp.jpg`\n\n![image](https://i.imgur.com/2ceiOx8.png)\n\n## Advanced information\n\n### Model path and manual download\n\nFor the SDH Analysis our custom model will be downloaded and placed inside the myoquant package directory. You can also download it manually here: [https://lbgi.fr/~meyer/SDH_models/model.h5](https://lbgi.fr/~meyer/SDH_models/model.h5) and then you can place it in the directory of your choice and provide the path to the model file using:  \n`myoquant sdh-analysis IMAGE_PATH --model_path /path/to/model.h5`\n\n### HuggingFace🤗 repositories for Data and Model\n\nIn a effort to push for open-science, MyoQuant [SDH dataset](https://huggingface.co/datasets/corentinm7/MyoQuant-SDH-Data) and [model](https://huggingface.co/corentinm7/MyoQuant-SDH-Model) and availiable on HuggingFace🤗\n\n## Partners\n\n<p align="center">\n  <img src="https://i.imgur.com/m5OGthE.png" alt="Partner Banner" style="border-radius: 25px;" />\n</p>\n\nMyoQuant is born within the collaboration between the [CSTB Team @ ICube](https://cstb.icube.unistra.fr/en/index.php/Home) led by Julie D. Thompson, the [Morphological Unit of the Institute of Myology of Paris](https://www.institut-myologie.org/en/recherche-2/neuromuscular-investigation-center/morphological-unit/) led by Teresinha Evangelista, the [imagery platform MyoImage of Center of Research in Myology](https://recherche-myologie.fr/technologies/myoimage/) led by Bruno Cadot, [the photonic microscopy platform of the IGMBC](https://www.igbmc.fr/en/plateformes-technologiques/photonic-microscopy) led by Bertrand Vernay and the [Pathophysiology of neuromuscular diseases team @ IGBMC](https://www.igbmc.fr/en/igbmc/a-propos-de-ligbmc/directory/jocelyn-laporte) led by Jocelyn Laporte\n',
-    'author': 'Corentin Meyer',
-    'author_email': 'corentin.meyer@etu.unistra.fr',
-    'maintainer': 'Corentin Meyer',
-    'maintainer_email': 'corentin.meyer@etu.unistra.fr',
-    'url': 'https://lbgi.fr/MyoQuant/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+<p align="center">
+  <img src="https://i.imgur.com/mzALgZL.png" alt="MyoQuant Banner" style="border-radius: 25px;" />
+</p>
 
+MyoQuant🔬 is a command-line tool to automatically quantify pathological features in muscle fiber histology images.  
+It is built using CellPose, Stardist, custom neural-network models and image analysis techniques to automatically analyze myopathy histology images.  
+Currently MyoQuant is capable of quantifying centralization of nuclei in muscle fiber with HE staining, anomaly in the mitochondria distribution in muscle fibers with SDH staining and the number of type 1 muscle fiber vs type 2 muscle fiber with ATP staining.
+
+An online demo with a web interface is available at [https://lbgi.fr/MyoQuant/](https://lbgi.fr/MyoQuant/). This project is free and open-source under the AGPL license, feel free to fork and contribute to the development.
+
+#### _Warning: This tool is still in early phases and active development._
+
+## How to install
+
+### Installing from PyPi (Preferred)
+
+**MyoQuant package is officially available on PyPi (pip) repository. [https://pypi.org/project/myoquant/](https://pypi.org/project/myoquant/) ![Pypi verison](https://img.shields.io/pypi/v/myoquant)**
+
+Using pip, you can simply install MyoQuant in a python environment with a simple: `pip install myoquant`
+
+### Installing from sources (Developers)
+
+1. Clone this repository using `git clone https://github.com/lambda-science/MyoQuant.git`
+2. Create a virtual environment by using `python -m venv .venv`
+3. Activate the venv by using `source .venv/bin/activate`
+4. Install MyoQuant by using `pip install -e .`
+
+## How to Use
+
+To use the command-line tool, first activate your venv in which MyoQuant is installed: `source .venv/bin/activate`  
+Then you can perform SDH or HE analysis. You can use the command `myoquant --help` to list available commands.
+
+## 💡Full command documentation is avaliable here: [CLI Documentation](https://github.com/lambda-science/MyoQuant/blob/main/CLI_Documentation.md)
+
+- **For SDH Image Analysis** the command is:  
+  `myoquant sdh-analysis IMAGE_PATH`  
+  Don't forget to run `myoquant sdh-analysis --help` for information about options.
+- **For HE Image Analysis** the command is:  
+  `myoquant he-analysis IMAGE_PATH`  
+   Don't forget to run `myoquant he-analysis --help` for information about options.
+- **For ATP Image Analysis** the command is:  
+  `myoquant atp-analysis IMAGE_PATH`  
+   Don't forget to run `myoquant atp-analysis --help` for information about options.
+
+_If you're running into an issue such as `myoquant: command not found` please check if you activated your virtual environment with the package installed. And also you can try to run it with the full command: `python -m myoquant sdh-analysis --help`_
+
+## Contact
+
+Creator and Maintainer: [**Corentin Meyer**, 3rd year PhD Student in the CSTB Team, ICube — CNRS — Unistra](https://cmeyer.fr) <corentin.meyer@etu.unistra.fr>
+
+## Citing MyoQuant🔬
+
+[placeholder]
+
+## Examples
+
+For HE Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_he.jpg)  
+For SDH Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_sdh.jpg)  
+For ATP Staining analysis, you can download this sample image: [HERE](https://www.lbgi.fr/~meyer/SDH_models/sample_atp.jpg)
+
+1. Example of successful SDH analysis output with: `myoquant sdh-analysis sample_sdh.jpg`
+
+![image](https://user-images.githubusercontent.com/20109584/210328050-11b0b6d5-28ec-41a4-b9d3-264962d04fa3.png)
+![image](https://i.imgur.com/4Nlnwdx.png) 2. Example of HE analysis: `myoquant he-analysis sample_he.jpg`
+
+![image](https://i.imgur.com/q2cXgIf.png)
+
+3. Example of ATP analysis with: `myoquan atp-analysis sample_atp.jpg`
+
+![image](https://i.imgur.com/2ceiOx8.png)
+
+## Advanced information
+
+### Model path and manual download
+
+For the SDH Analysis our custom model will be downloaded and placed inside the myoquant package directory. You can also download it manually here: [https://lbgi.fr/~meyer/SDH_models/model.h5](https://lbgi.fr/~meyer/SDH_models/model.h5) and then you can place it in the directory of your choice and provide the path to the model file using:  
+`myoquant sdh-analysis IMAGE_PATH --model_path /path/to/model.h5`
+
+### HuggingFace🤗 repositories for Data and Model
+
+In a effort to push for open-science, MyoQuant [SDH dataset](https://huggingface.co/datasets/corentinm7/MyoQuant-SDH-Data) and [model](https://huggingface.co/corentinm7/MyoQuant-SDH-Model) and availiable on HuggingFace🤗
+
+## Partners
+
+<p align="center">
+  <img src="https://i.imgur.com/m5OGthE.png" alt="Partner Banner" style="border-radius: 25px;" />
+</p>
+
+MyoQuant is born within the collaboration between the [CSTB Team @ ICube](https://cstb.icube.unistra.fr/en/index.php/Home) led by Julie D. Thompson, the [Morphological Unit of the Institute of Myology of Paris](https://www.institut-myologie.org/en/recherche-2/neuromuscular-investigation-center/morphological-unit/) led by Teresinha Evangelista, the [imagery platform MyoImage of Center of Research in Myology](https://recherche-myologie.fr/technologies/myoimage/) led by Bruno Cadot, [the photonic microscopy platform of the IGMBC](https://www.igbmc.fr/en/plateformes-technologiques/photonic-microscopy) led by Bertrand Vernay and the [Pathophysiology of neuromuscular diseases team @ IGBMC](https://www.igbmc.fr/en/igbmc/a-propos-de-ligbmc/directory/jocelyn-laporte) led by Jocelyn Laporte
 
-setup(**setup_kwargs)
```

