# Comparing `tmp/vit-tf2-1.0.1.tar.gz` & `tmp/vit-tf2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vit-tf2-1.0.1.tar", last modified: Wed May 10 05:32:37 2023, max compression
+gzip compressed data, was "dist\vit-tf2-1.0.2.tar", last modified: Wed May 10 06:52:31 2023, max compression
```

## Comparing `vit-tf2-1.0.1.tar` & `vit-tf2-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/
--rw-rw-rw-   0        0        0    11986 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9238 2023-05-10 05:06:52.000000 vit-tf2-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-05-10 05:32:15.000000 vit-tf2-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2/
--rw-rw-rw-   0        0        0       23 2023-05-09 15:30:30.000000 vit-tf2-1.0.1/vit_tf2/__init__.py
--rw-rw-rw-   0        0        0     1287 2023-05-09 14:09:11.000000 vit-tf2-1.0.1/vit_tf2/config.py
--rw-rw-rw-   0        0        0     4947 2023-05-10 04:41:42.000000 vit-tf2-1.0.1/vit_tf2/layers.py
--rw-rw-rw-   0        0        0     5874 2023-05-10 04:41:56.000000 vit-tf2-1.0.1/vit_tf2/utils.py
--rw-rw-rw-   0        0        0    15072 2023-05-10 04:41:41.000000 vit-tf2-1.0.1/vit_tf2/vit.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2.egg-info/
--rw-rw-rw-   0        0        0    11986 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 05:32:37.000000 vit-tf2-1.0.1/vit_tf2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/
+-rw-rw-rw-   0        0        0    11986 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9238 2023-05-10 05:06:52.000000 vit-tf2-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-10 06:41:31.000000 vit-tf2-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/vit_tf2.egg-info/
+-rw-rw-rw-   0        0        0    11986 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/vit_tf2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/vit_tf2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/vit_tf2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:52:31.000000 vit-tf2-1.0.2/vit_tf2.egg-info/top_level.txt
```

### Comparing `vit-tf2-1.0.1/PKG-INFO` & `vit-tf2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-tf2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of ViT model based on tensorflow
 Home-page: https://github.com/djsaber/Keras-ViT
 Author: djsaber
 Author-email: 479719615@qq.com
 License: UNKNOWN
 Description: # vit_tf2
```

### Comparing `vit-tf2-1.0.1/README.md` & `vit-tf2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vit-tf2-1.0.1/setup.py` & `vit-tf2-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="vit-tf2",
-    version="1.0.1",
+    version="1.0.2",
     author="djsaber",
     author_email="479719615@qq.com",
     description="Implementation of ViT model based on tensorflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/djsaber/Keras-ViT",
     packages=setuptools.find_packages(),
```

### Comparing `vit-tf2-1.0.1/vit_tf2.egg-info/PKG-INFO` & `vit-tf2-1.0.2/vit_tf2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-tf2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of ViT model based on tensorflow
 Home-page: https://github.com/djsaber/Keras-ViT
 Author: djsaber
 Author-email: 479719615@qq.com
 License: UNKNOWN
 Description: # vit_tf2
```

