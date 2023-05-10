# Comparing `tmp/dis_inference-1.1.0.tar.gz` & `tmp/dis_inference-1.1.1.tar.gz`

## Comparing `dis_inference-1.1.0.tar` & `dis_inference-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dis_inference-1.1.0/.flake8
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 dis_inference-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.0/Lenna_dis.png
--rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 dis_inference-1.1.0/cat2_dis.jpg
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dis_inference-1.1.0/environment.yaml
--rw-r--r--   0        0        0    32258 2020-02-02 00:00:00.000000 dis_inference-1.1.0/output_dis.png
--rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.0/test.png
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dis_inference-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0   473831 2020-02-02 00:00:00.000000 dis_inference-1.1.0/assets/Lenna.png
--rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.0/assets/Lenna_dis.png
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/__about__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/__main__.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/cli/__init__.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/models/__init__.py
--rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 dis_inference-1.1.0/src/dis_inference/models/isnet.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dis_inference-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dis_inference-1.1.0/.gitignore
--rw-r--r--   0        0        0    34020 2020-02-02 00:00:00.000000 dis_inference-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 dis_inference-1.1.0/README.md
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 dis_inference-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 dis_inference-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dis_inference-1.1.1/.flake8
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 dis_inference-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.1/Lenna_dis.png
+-rw-r--r--   0        0        0    12887 2020-02-02 00:00:00.000000 dis_inference-1.1.1/cat2_dis.jpg
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dis_inference-1.1.1/environment.yaml
+-rw-r--r--   0        0        0    32258 2020-02-02 00:00:00.000000 dis_inference-1.1.1/output_dis.png
+-rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.1/test.png
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dis_inference-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0   473831 2020-02-02 00:00:00.000000 dis_inference-1.1.1/assets/Lenna.png
+-rw-r--r--   0        0        0    37886 2020-02-02 00:00:00.000000 dis_inference-1.1.1/assets/Lenna_dis.png
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/__about__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/__main__.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/cli/__init__.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/models/__init__.py
+-rw-r--r--   0        0        0    15623 2020-02-02 00:00:00.000000 dis_inference-1.1.1/src/dis_inference/models/isnet.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dis_inference-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 dis_inference-1.1.1/.gitignore
+-rw-r--r--   0        0        0    34020 2020-02-02 00:00:00.000000 dis_inference-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 dis_inference-1.1.1/README.md
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 dis_inference-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 dis_inference-1.1.1/PKG-INFO
```

### Comparing `dis_inference-1.1.0/Lenna_dis.png` & `dis_inference-1.1.1/Lenna_dis.png`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/cat2_dis.jpg` & `dis_inference-1.1.1/cat2_dis.jpg`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/output_dis.png` & `dis_inference-1.1.1/output_dis.png`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/test.png` & `dis_inference-1.1.1/test.png`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/assets/Lenna.png` & `dis_inference-1.1.1/assets/Lenna.png`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/assets/Lenna_dis.png` & `dis_inference-1.1.1/assets/Lenna_dis.png`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/src/dis_inference/cli/__init__.py` & `dis_inference-1.1.1/src/dis_inference/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/src/dis_inference/models/__init__.py` & `dis_inference-1.1.1/src/dis_inference/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/src/dis_inference/models/isnet.py` & `dis_inference-1.1.1/src/dis_inference/models/isnet.py`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/LICENSE.txt` & `dis_inference-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/README.md` & `dis_inference-1.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # DIS-inference
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dis-inference.svg)](https://pypi.org/project/dis-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dis-inference.svg)](https://pypi.org/project/dis-inference)
 
 Inference implementation of Dichotomous Image Segmentation
+
 ## [Highly Accurate Dichotomous Image Segmentation (ECCV 2022)](https://arxiv.org/pdf/2203.03041.pdf)
+
 #### [Xuebin Qin](https://xuebinqin.github.io/), [Hang Dai](https://scholar.google.co.uk/citations?user=6yvjpQQAAAAJ&hl=en), [Xiaobin Hu](https://scholar.google.de/citations?user=3lMuodUAAAAJ&hl=en), [Deng-Ping Fan*](https://dengpingfan.github.io/), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en), [Luc Van Gool](https://scholar.google.com/citations?user=TwMib_QAAAAJ&hl=en).
-[**Project Page**](https://xuebinqin.github.io/dis/index.html), [**Arxiv**](https://arxiv.org/pdf/2203.03041.pdf), [**中文**](https://github.com/xuebinqin/xuebinqin.github.io/blob/main/ECCV2022_DIS_Chinese.pdf).
+
+[**Project Page**](https://xuebinqin.github.io/dis/index.html), [**Arxiv**](https://arxiv.org/pdf/2203.03041.pdf), [**中文
+**](https://github.com/xuebinqin/xuebinqin.github.io/blob/main/ECCV2022_DIS_Chinese.pdf).
 
 <br>
 
-| Origin | DIS |
-|--|--|
-|![Before](assets/Lenna.png)|![After](assets/Lenna_dis.png)|
+| Origin                                                                          | DIS                                                                                |
+|---------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| ![Before](https://github.com/dh031200/DIS-inference/blob/main/assets/Lenna.png) | ![After](https://github.com/dh031200/DIS-inference/blob/main/assets/Lenna_dis.png) |
 
 <br>
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
@@ -26,39 +30,43 @@
 ## Installation
 
 ```console
 pip install dis-inference
 ```
 
 ## Usage
+
 ### CLI
+
 command:  `dis-inference`
-arguments:
-　　--silent(optional) : Whether to print verbose.  Source image
+arguments:--silent(optional) : Whether to print verbose. Source image
+
 ```console
 > dis-inference Lenna.png
 Output saved as `Lenna_dis.png`
 > dis-inference --silent Lenna.png
 ```
 
 ### Python
+
 ```python
 from dis_inference import inference
 
 # 1. Used in memory
 image = inference('Lenna.png')
 cv2.imwrite('Lenna_dis.png', image)
 
 # 2. With save parameter
 image = inference('Lenna.png', save=True)
 ```
 
 ## License
 
-`dis-inference` is distributed under the terms of the [AGPL-3.0-only](https://spdx.org/licenses/AGPL-3.0-only.html) license.
+`dis-inference` is distributed under the terms of the [AGPL-3.0-only](https://spdx.org/licenses/AGPL-3.0-only.html)
+license.
 
 ## Reference
 
 https://github.com/xuebinqin/DIS
 
 ## Citation
```

### Comparing `dis_inference-1.1.0/pyproject.toml` & `dis_inference-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dis_inference-1.1.0/PKG-INFO` & `dis_inference-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dis-inference
-Version: 1.1.0
+Version: 1.1.1
 Summary: Inference implementation for Dichotomous Image Segmentation
 Project-URL: Documentation, https://github.com/unknown/dis-inference#readme
 Project-URL: Issues, https://github.com/unknown/dis-inference/issues
 Project-URL: Source, https://github.com/unknown/dis-inference
 Author-email: dh031200 <imbird0312@gmail.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE.txt
@@ -29,23 +29,27 @@
 
 # DIS-inference
 
 [![PyPI - Version](https://img.shields.io/pypi/v/dis-inference.svg)](https://pypi.org/project/dis-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dis-inference.svg)](https://pypi.org/project/dis-inference)
 
 Inference implementation of Dichotomous Image Segmentation
+
 ## [Highly Accurate Dichotomous Image Segmentation (ECCV 2022)](https://arxiv.org/pdf/2203.03041.pdf)
+
 #### [Xuebin Qin](https://xuebinqin.github.io/), [Hang Dai](https://scholar.google.co.uk/citations?user=6yvjpQQAAAAJ&hl=en), [Xiaobin Hu](https://scholar.google.de/citations?user=3lMuodUAAAAJ&hl=en), [Deng-Ping Fan*](https://dengpingfan.github.io/), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en), [Luc Van Gool](https://scholar.google.com/citations?user=TwMib_QAAAAJ&hl=en).
-[**Project Page**](https://xuebinqin.github.io/dis/index.html), [**Arxiv**](https://arxiv.org/pdf/2203.03041.pdf), [**中文**](https://github.com/xuebinqin/xuebinqin.github.io/blob/main/ECCV2022_DIS_Chinese.pdf).
+
+[**Project Page**](https://xuebinqin.github.io/dis/index.html), [**Arxiv**](https://arxiv.org/pdf/2203.03041.pdf), [**中文
+**](https://github.com/xuebinqin/xuebinqin.github.io/blob/main/ECCV2022_DIS_Chinese.pdf).
 
 <br>
 
-| Origin | DIS |
-|--|--|
-|![Before](assets/Lenna.png)|![After](assets/Lenna_dis.png)|
+| Origin                                                                          | DIS                                                                                |
+|---------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| ![Before](https://github.com/dh031200/DIS-inference/blob/main/assets/Lenna.png) | ![After](https://github.com/dh031200/DIS-inference/blob/main/assets/Lenna_dis.png) |
 
 <br>
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
@@ -55,39 +59,43 @@
 ## Installation
 
 ```console
 pip install dis-inference
 ```
 
 ## Usage
+
 ### CLI
+
 command:  `dis-inference`
-arguments:
-　　--silent(optional) : Whether to print verbose.  Source image
+arguments:--silent(optional) : Whether to print verbose. Source image
+
 ```console
 > dis-inference Lenna.png
 Output saved as `Lenna_dis.png`
 > dis-inference --silent Lenna.png
 ```
 
 ### Python
+
 ```python
 from dis_inference import inference
 
 # 1. Used in memory
 image = inference('Lenna.png')
 cv2.imwrite('Lenna_dis.png', image)
 
 # 2. With save parameter
 image = inference('Lenna.png', save=True)
 ```
 
 ## License
 
-`dis-inference` is distributed under the terms of the [AGPL-3.0-only](https://spdx.org/licenses/AGPL-3.0-only.html) license.
+`dis-inference` is distributed under the terms of the [AGPL-3.0-only](https://spdx.org/licenses/AGPL-3.0-only.html)
+license.
 
 ## Reference
 
 https://github.com/xuebinqin/DIS
 
 ## Citation
```

