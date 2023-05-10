# Comparing `tmp/MaMMUT-pytorch-0.0.3.tar.gz` & `tmp/MaMMUT-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MaMMUT-pytorch-0.0.3.tar", last modified: Sat May  6 01:19:28 2023, max compression
+gzip compressed data, was "MaMMUT-pytorch-0.0.4.tar", last modified: Wed May 10 14:57:31 2023, max compression
```

## Comparing `MaMMUT-pytorch-0.0.3.tar` & `MaMMUT-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 01:19:28.000000 MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/mammut_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/mammut_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/mammut_pytorch/mammut_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:19:28.904896 MaMMUT-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 01:19:16.000000 MaMMUT-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:57:31.225918 MaMMUT-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 14:57:13.000000 MaMMUT-pytorch-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:57:31.225918 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-10 14:57:31.000000 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 14:57:31.000000 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:57:31.000000 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 14:57:31.000000 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 14:57:31.000000 MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-10 14:57:31.225918 MaMMUT-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-10 14:57:13.000000 MaMMUT-pytorch-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:57:31.225918 MaMMUT-pytorch-0.0.4/mammut_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 14:57:13.000000 MaMMUT-pytorch-0.0.4/mammut_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-05-10 14:57:13.000000 MaMMUT-pytorch-0.0.4/mammut_pytorch/mammut_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:57:31.225918 MaMMUT-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-10 14:57:13.000000 MaMMUT-pytorch-0.0.4/setup.py
```

### Comparing `MaMMUT-pytorch-0.0.3/LICENSE` & `MaMMUT-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MaMMUT-pytorch-0.0.3/MaMMUT_pytorch.egg-info/PKG-INFO` & `MaMMUT-pytorch-0.0.4/MaMMUT_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaMMUT-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: MaMMUT - Pytorch
 Home-page: https://github.com/lucidrains/MaMMUT-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,multimodal,attention mechanism,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MaMMUT-pytorch-0.0.3/PKG-INFO` & `MaMMUT-pytorch-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MaMMUT-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: MaMMUT - Pytorch
 Home-page: https://github.com/lucidrains/MaMMUT-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,multimodal,attention mechanism,contrastive learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MaMMUT-pytorch-0.0.3/README.md` & `MaMMUT-pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `MaMMUT-pytorch-0.0.3/mammut_pytorch/mammut_pytorch.py` & `MaMMUT-pytorch-0.0.4/mammut_pytorch/mammut_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 
         if exists(attn_mask):
             attn_mask = rearrange(attn_mask, 'b i j -> b 1 i j')
             sim = sim.masked_fill(~attn_mask, -torch.finfo(sim.dtype).max)
 
         # attention
 
-        sim = sim - sim.amax(dim=-1, keepdim=True).detach()
         attn = sim.softmax(dim=-1)
 
         # aggregate values
 
         out = einsum("b h i j, b j d -> b h i d", attn, v)
 
         # merge heads
@@ -253,15 +252,14 @@
 
         # query / key similarity
 
         sim = einsum('b h i d, b j d -> b h i j', q, k)
 
         # attention
 
-        sim = sim - sim.amax(dim=-1, keepdim=True)
         attn = sim.softmax(dim=-1)
 
         # aggregate
 
         out = einsum('b h i j, b j d -> b h i d', attn, v)
 
         # merge and combine heads
```

### Comparing `MaMMUT-pytorch-0.0.3/setup.py` & `MaMMUT-pytorch-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MaMMUT-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'MaMMUT - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/MaMMUT-pytorch',
   keywords = [
```

