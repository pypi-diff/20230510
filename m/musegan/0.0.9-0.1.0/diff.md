# Comparing `tmp/musegan-0.0.9.tar.gz` & `tmp/musegan-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.0.9.tar", last modified: Tue May  9 07:18:13 2023, max compression
+gzip compressed data, was "musegan-0.1.0.tar", last modified: Wed May 10 06:49:20 2023, max compression
```

## Comparing `musegan-0.0.9.tar` & `musegan-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.944824 musegan-0.0.9/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1507 2023-05-09 07:18:13.944824 musegan-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      892 2023-05-09 05:17:56.000000 musegan-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.913599 musegan-0.0.9/musegan/
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.929197 musegan-0.0.9/musegan/musegan/
--rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.0.9/musegan/musegan/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-08 13:43:49.000000 musegan-0.0.9/musegan/musegan/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.944824 musegan-0.0.9/musegan/musegan/archs/
--rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.0.9/musegan/musegan/archs/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.0.9/musegan/musegan/archs/bar_generator.py
--rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.0.9/musegan/musegan/archs/critic.py
--rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.0.9/musegan/musegan/archs/generator.py
--rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.0.9/musegan/musegan/archs/temp_network.py
--rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.0.9/musegan/musegan/archs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.944824 musegan-0.0.9/musegan/musegan/dataset/
--rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.0.9/musegan/musegan/dataset/__init__.py
--rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.0.9/musegan/musegan/dataset/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.944824 musegan-0.0.9/musegan/musegan/trainner/
--rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.0.9/musegan/musegan/trainner/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.0.9/musegan/musegan/trainner/criterion.py
--rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.0.9/musegan/musegan/trainner/trainer.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:18:13.929197 musegan-0.0.9/musegan/musegan.egg-info/
--rw-rw-rw-   0        0        0     1507 2023-05-09 07:18:13.000000 musegan-0.0.9/musegan/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-05-09 07:18:13.000000 musegan-0.0.9/musegan/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:18:13.000000 musegan-0.0.9/musegan/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 07:18:13.000000 musegan-0.0.9/musegan/musegan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      736 2023-05-09 07:18:13.944824 musegan-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.206512 musegan-0.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2828 2023-05-10 06:49:20.206512 musegan-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-05-10 06:38:22.000000 musegan-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.176479 musegan-0.1.0/musegan/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.196366 musegan-0.1.0/musegan/musegan/
+-rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.1.0/musegan/musegan/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 08:17:02.000000 musegan-0.1.0/musegan/musegan/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.206512 musegan-0.1.0/musegan/musegan/archs/
+-rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.1.0/musegan/musegan/archs/__init__.py
+-rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.1.0/musegan/musegan/archs/bar_generator.py
+-rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.1.0/musegan/musegan/archs/critic.py
+-rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.1.0/musegan/musegan/archs/generator.py
+-rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.1.0/musegan/musegan/archs/temp_network.py
+-rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.1.0/musegan/musegan/archs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.206512 musegan-0.1.0/musegan/musegan/dataset/
+-rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.1.0/musegan/musegan/dataset/__init__.py
+-rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.1.0/musegan/musegan/dataset/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.206512 musegan-0.1.0/musegan/musegan/trainner/
+-rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.1.0/musegan/musegan/trainner/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.1.0/musegan/musegan/trainner/criterion.py
+-rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.1.0/musegan/musegan/trainner/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:20.196366 musegan-0.1.0/musegan/musegan.egg-info/
+-rw-rw-rw-   0        0        0     2828 2023-05-10 06:49:20.000000 musegan-0.1.0/musegan/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-05-10 06:49:20.000000 musegan-0.1.0/musegan/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:49:20.000000 musegan-0.1.0/musegan/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 06:49:20.000000 musegan-0.1.0/musegan/musegan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      736 2023-05-10 06:49:20.216423 musegan-0.1.0/setup.cfg
```

### Comparing `musegan-0.0.9/LICENSE` & `musegan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/PKG-INFO` & `musegan-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.9
+Version: 0.1.0
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,25 +13,60 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
-A Pytorch implementation of MuseGAN
-Only linux BSD support due to SharedArray usage
+![PyPI - License](https://img.shields.io/pypi/l/musegan)
+[![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/musegan)
+
+- A Pytorch implementation of MuseGAN
+- ***Note :*** Only linux BSD support due to SharedArray usage which is a linux only pip package
+
+
 
-:star: Star this project on GitHub — it helps!
 
 [MuseGAN](https://arxiv.org/abs/1709.06298) is a generative model which allows to
 generate music.
 
+Usage
+=======
+The musegan package contains all the schema needed to train and generate your own music in MIDI format.
+There are two ways of using the musegan package;
+
+1. Using the PYPI package.
+   - To use it use the command: `pip install musegan` to install all the necessary packages
+
+2. Building from the source 
+   - First clone the repository to your local directory with `git`
+   - Open your local Terminal/Command Shell and run the following commands
+    ```shell
+    cd musegan-pytorch # change directory to the cloned repository
+    #use any of the following some will work dependent on your operating system
+    #try
+    python3 setup.py develop
+    #or
+    pip install .
+    #or
+    pip install -e
+    ```
+    - To test run the following in your python terminal;
+    ```py
+    >> import musegan
+    >> print(musegan__version__)
+    # which should return the latest musegan version according to the time you read this
+    0.0.9
+    ```
+    Now you should be able to use zthe musegan packages
+    
 ## Table of content
 
-- [Training](#train)
+- [Training](https://github.com/cliffordkleinsr/musegan-pytorch/edit/dev/README.md#training)
 - [License](#license)
 - [Links](#links)
 
 ## Training 
 
 See this [colab](https://colab.research.google.com/drive/1NF2t1dvqxeblZfd7BL4Gfn4SW-xEzgGg?authuser=3#scrollTo=9bj_FWvAArPI)  notebook for more details of training process.
 * The model components and utils are under `musegan/archs` folder.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `musegan-0.0.9/musegan/musegan/archs/bar_generator.py` & `musegan-0.1.0/musegan/musegan/archs/bar_generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/archs/critic.py` & `musegan-0.1.0/musegan/musegan/archs/critic.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/archs/generator.py` & `musegan-0.1.0/musegan/musegan/archs/generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/archs/temp_network.py` & `musegan-0.1.0/musegan/musegan/archs/temp_network.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/archs/utils.py` & `musegan-0.1.0/musegan/musegan/archs/utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/dataset/data_utils.py` & `musegan-0.1.0/musegan/musegan/dataset/data_utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/trainner/criterion.py` & `musegan-0.1.0/musegan/musegan/trainner/criterion.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan/trainner/trainer.py` & `musegan-0.1.0/musegan/musegan/trainner/trainer.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/musegan/musegan.egg-info/PKG-INFO` & `musegan-0.1.0/musegan/musegan.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.9
+Version: 0.1.0
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,25 +13,60 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
-A Pytorch implementation of MuseGAN
-Only linux BSD support due to SharedArray usage
+![PyPI - License](https://img.shields.io/pypi/l/musegan)
+[![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/musegan)
+
+- A Pytorch implementation of MuseGAN
+- ***Note :*** Only linux BSD support due to SharedArray usage which is a linux only pip package
+
+
 
-:star: Star this project on GitHub — it helps!
 
 [MuseGAN](https://arxiv.org/abs/1709.06298) is a generative model which allows to
 generate music.
 
+Usage
+=======
+The musegan package contains all the schema needed to train and generate your own music in MIDI format.
+There are two ways of using the musegan package;
+
+1. Using the PYPI package.
+   - To use it use the command: `pip install musegan` to install all the necessary packages
+
+2. Building from the source 
+   - First clone the repository to your local directory with `git`
+   - Open your local Terminal/Command Shell and run the following commands
+    ```shell
+    cd musegan-pytorch # change directory to the cloned repository
+    #use any of the following some will work dependent on your operating system
+    #try
+    python3 setup.py develop
+    #or
+    pip install .
+    #or
+    pip install -e
+    ```
+    - To test run the following in your python terminal;
+    ```py
+    >> import musegan
+    >> print(musegan__version__)
+    # which should return the latest musegan version according to the time you read this
+    0.0.9
+    ```
+    Now you should be able to use zthe musegan packages
+    
 ## Table of content
 
-- [Training](#train)
+- [Training](https://github.com/cliffordkleinsr/musegan-pytorch/edit/dev/README.md#training)
 - [License](#license)
 - [Links](#links)
 
 ## Training 
 
 See this [colab](https://colab.research.google.com/drive/1NF2t1dvqxeblZfd7BL4Gfn4SW-xEzgGg?authuser=3#scrollTo=9bj_FWvAArPI)  notebook for more details of training process.
 * The model components and utils are under `musegan/archs` folder.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `musegan-0.0.9/musegan/musegan.egg-info/SOURCES.txt` & `musegan-0.1.0/musegan/musegan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musegan-0.0.9/setup.cfg` & `musegan-0.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7573 6567 616e 0d0a 7665 7273   = musegan..vers
-00000020: 696f 6e20 3d20 302e 302e 390d 0a61 7574  ion = 0.0.9..aut
+00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
 00000030: 686f 7220 3d20 436c 6966 666f 7264 204e  hor = Clifford N
 00000040: 6a6f 726f 6765 0d0a 6175 7468 6f72 5f65  joroge..author_e
 00000050: 6d61 696c 203d 2063 6e6a 6f72 6f67 6540  mail = cnjoroge@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 7974 6f72  iption = A pytor
 00000080: 6368 2069 6d70 6c65 6d65 6e74 6174 696f  ch implementatio
 00000090: 6e20 6f66 206d 7573 6567 616e 0d0a 6c6f  n of musegan..lo
```

