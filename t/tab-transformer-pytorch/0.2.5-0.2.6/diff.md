# Comparing `tmp/tab-transformer-pytorch-0.2.5.tar.gz` & `tmp/tab-transformer-pytorch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab-transformer-pytorch-0.2.5.tar", last modified: Thu Apr  6 01:25:43 2023, max compression
+gzip compressed data, was "tab-transformer-pytorch-0.2.6.tar", last modified: Wed May 10 13:47:06 2023, max compression
```

## Comparing `tab-transformer-pytorch-0.2.5.tar` & `tab-transformer-pytorch-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:25:43.761271 tab-transformer-pytorch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-06 01:25:43.761271 tab-transformer-pytorch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 01:25:43.761271 tab-transformer-pytorch-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:25:43.757272 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-06 01:25:28.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/tab_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 01:25:43.761271 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-06 01:25:43.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-06 01:25:43.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 01:25:43.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 01:25:43.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 01:25:43.000000 tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:47:06.929574 tab-transformer-pytorch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-10 13:47:06.929574 tab-transformer-pytorch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:47:06.929574 tab-transformer-pytorch-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:47:06.929574 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-10 13:46:51.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/tab_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:47:06.929574 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-10 13:47:06.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 13:47:06.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:47:06.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 13:47:06.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 13:47:06.000000 tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/top_level.txt
```

### Comparing `tab-transformer-pytorch-0.2.5/LICENSE` & `tab-transformer-pytorch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tab-transformer-pytorch-0.2.5/PKG-INFO` & `tab-transformer-pytorch-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-transformer-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tab Transformer - Pytorch
 Home-page: https://github.com/lucidrains/tab-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformers,attention mechanism,tabular data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tab-transformer-pytorch-0.2.5/README.md` & `tab-transformer-pytorch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tab-transformer-pytorch-0.2.5/setup.py` & `tab-transformer-pytorch-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tab-transformer-pytorch',
   packages = find_packages(),
-  version = '0.2.5',
+  version = '0.2.6',
   license='MIT',
   description = 'Tab Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/tab-transformer-pytorch',
   keywords = [
     'artificial intelligence',
```

### Comparing `tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/ft_transformer.py` & `tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/ft_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         )
 
     def forward(self, x_categ, x_numer, return_attn = False):
         assert x_categ.shape[-1] == self.num_categories, f'you must pass in {self.num_categories} values for your categories input'
 
         xs = []
         if self.num_unique_categories > 0:
-            x_categ += self.categories_offset
+            x_categ = x_categ + self.categories_offset
 
             x_categ = self.categorical_embeds(x_categ)
 
             xs.append(x_categ)
 
         # add numerically embedded tokens
         if self.num_continuous > 0:
```

### Comparing `tab-transformer-pytorch-0.2.5/tab_transformer_pytorch/tab_transformer_pytorch.py` & `tab-transformer-pytorch-0.2.6/tab_transformer_pytorch/tab_transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `tab-transformer-pytorch-0.2.5/tab_transformer_pytorch.egg-info/PKG-INFO` & `tab-transformer-pytorch-0.2.6/tab_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-transformer-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tab Transformer - Pytorch
 Home-page: https://github.com/lucidrains/tab-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,transformers,attention mechanism,tabular data
 Classifier: Development Status :: 4 - Beta
```

