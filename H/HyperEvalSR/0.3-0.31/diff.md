# Comparing `tmp/HyperEvalSR-0.3.tar.gz` & `tmp/HyperEvalSR-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyperEvalSR-0.3.tar", last modified: Wed May 10 12:30:20 2023, max compression
+gzip compressed data, was "HyperEvalSR-0.31.tar", last modified: Wed May 10 13:01:30 2023, max compression
```

## Comparing `HyperEvalSR-0.3.tar` & `HyperEvalSR-0.31.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:30:20.889132 HyperEvalSR-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:30:20.884813 HyperEvalSR-0.3/HyperEvalSR/
--rw-rw-rw-   0        0        0        0 2023-03-06 08:18:38.000000 HyperEvalSR-0.3/HyperEvalSR/__init__.py
--rw-rw-rw-   0        0        0     8892 2023-05-08 07:44:02.000000 HyperEvalSR-0.3/HyperEvalSR/ev.py
--rw-rw-rw-   0        0        0     1223 2023-05-08 07:35:48.000000 HyperEvalSR-0.3/HyperEvalSR/sr.py
--rw-rw-rw-   0        0        0      482 2023-03-09 11:55:25.000000 HyperEvalSR-0.3/HyperEvalSR/test.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:30:20.888141 HyperEvalSR-0.3/HyperEvalSR.egg-info/
--rw-rw-rw-   0        0        0     8514 2023-05-10 12:30:20.000000 HyperEvalSR-0.3/HyperEvalSR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-10 12:30:20.000000 HyperEvalSR-0.3/HyperEvalSR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:30:20.000000 HyperEvalSR-0.3/HyperEvalSR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 12:30:20.000000 HyperEvalSR-0.3/HyperEvalSR.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 12:30:20.000000 HyperEvalSR-0.3/HyperEvalSR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2023-03-06 08:15:40.000000 HyperEvalSR-0.3/LICENSE
--rw-rw-rw-   0        0        0     8514 2023-05-10 12:30:20.888141 HyperEvalSR-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7111 2023-05-08 13:24:26.000000 HyperEvalSR-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 12:30:20.889132 HyperEvalSR-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-05-10 12:30:12.000000 HyperEvalSR-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/HyperEvalSR/
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:18:38.000000 HyperEvalSR-0.31/HyperEvalSR/__init__.py
+-rw-rw-rw-   0        0        0     8892 2023-05-08 07:44:02.000000 HyperEvalSR-0.31/HyperEvalSR/ev.py
+-rw-rw-rw-   0        0        0    38940 2023-05-10 12:54:15.000000 HyperEvalSR-0.31/HyperEvalSR/sr.py
+-rw-rw-rw-   0        0        0      482 2023-03-09 11:55:25.000000 HyperEvalSR-0.31/HyperEvalSR/test.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/HyperEvalSR.egg-info/
+-rw-rw-rw-   0        0        0     8517 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:01:30.000000 HyperEvalSR-0.31/HyperEvalSR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2023-03-06 08:15:40.000000 HyperEvalSR-0.31/LICENSE
+-rw-rw-rw-   0        0        0     8517 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     7111 2023-05-08 13:24:26.000000 HyperEvalSR-0.31/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-10 13:00:46.000000 HyperEvalSR-0.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:30.250170 HyperEvalSR-0.31/test/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:56:45.000000 HyperEvalSR-0.31/test/test_ev.py
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:56:56.000000 HyperEvalSR-0.31/test/test_sr.py
```

### Comparing `HyperEvalSR-0.3/HyperEvalSR/ev.py` & `HyperEvalSR-0.31/HyperEvalSR/ev.py`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.3/HyperEvalSR.egg-info/PKG-INFO` & `HyperEvalSR-0.31/HyperEvalSR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperEvalSR
-Version: 0.3
+Version: 0.31
 Summary: An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.
 Home-page: https://github.com/jingmengzhiyue/HyperEvalSR
 Author: jingmengzhiyue
 Author-email: jingmengzhiyue@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 - **Erreur Relative Globale Adimensionnelle de Synth猫se (ERGAS)**: Calculates the relative global dimensionless synthesis error.
 - **Structural Similarity Index (SSIM)**: Assesses the structural similarity between the reference and reconstructed images.
 
 ## Installation
 You can use pypi to install HyperEvalSR `pip install HyperEvalSR`
 ## Getting Started 
 `from HyperEvalSR import ev`
+
 The next section describes the definition of evaluation metrics in HyperEvalSR and how they are used.
 
 In this context, we assume that the reference image and the reconstructed image obtained from the algorithm are denoted as $\mathbf{X}$ and $\widehat{\mathbf{X}}$, respectively.
 
 ---
 ## PSNR
 > `res = ev.PSNR(Reference_image, Reconstructed_mage)`
```

### Comparing `HyperEvalSR-0.3/LICENSE` & `HyperEvalSR-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.3/PKG-INFO` & `HyperEvalSR-0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperEvalSR
-Version: 0.3
+Version: 0.31
 Summary: An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.
 Home-page: https://github.com/jingmengzhiyue/HyperEvalSR
 Author: jingmengzhiyue
 Author-email: jingmengzhiyue@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,15 @@
 - **Erreur Relative Globale Adimensionnelle de Synth猫se (ERGAS)**: Calculates the relative global dimensionless synthesis error.
 - **Structural Similarity Index (SSIM)**: Assesses the structural similarity between the reference and reconstructed images.
 
 ## Installation
 You can use pypi to install HyperEvalSR `pip install HyperEvalSR`
 ## Getting Started 
 `from HyperEvalSR import ev`
+
 The next section describes the definition of evaluation metrics in HyperEvalSR and how they are used.
 
 In this context, we assume that the reference image and the reconstructed image obtained from the algorithm are denoted as $\mathbf{X}$ and $\widehat{\mathbf{X}}$, respectively.
 
 ---
 ## PSNR
 > `res = ev.PSNR(Reference_image, Reconstructed_mage)`
```

### Comparing `HyperEvalSR-0.3/README.md` & `HyperEvalSR-0.31/README.md`

 * *Files identical despite different names*

### Comparing `HyperEvalSR-0.3/setup.py` & `HyperEvalSR-0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from re import U
 from struct import pack
 import setuptools
 with open(".\docs\index.md", "r") as f:
     long_description = f.read()
 setuptools.setup(
     name = "HyperEvalSR",
-    version="0.3",
+    version="0.31",
     author = "jingmengzhiyue",
     author_email = "jingmengzhiyue@gmail.com",
     description = "An open source python package for super-resolution/recovery quality evaluation of hyperspectral images, including RMSE, ERGAS, SSIM, RSNR, PSNR, CC, DD, and SAM.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/jingmengzhiyue/HyperEvalSR",
     packages =  setuptools.find_packages(),
```

