# Comparing `tmp/moddagudu-1.4.tar.gz` & `tmp/moddagudu-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.4.tar", last modified: Wed May 10 17:21:33 2023, max compression
+gzip compressed data, was "moddagudu-1.5.tar", last modified: Wed May 10 17:25:59 2023, max compression
```

## Comparing `moddagudu-1.4.tar` & `moddagudu-1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.876345 moddagudu-1.4/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.4/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 17:21:33.874347 moddagudu-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.864359 moddagudu-1.4/moddagudu/
--rw-rw-rw-   0        0        0       76 2023-05-10 17:10:53.000000 moddagudu-1.4/moddagudu/__init__.py
--rw-rw-rw-   0        0        0     1424 2023-05-10 17:14:50.000000 moddagudu-1.4/moddagudu/mg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.873355 moddagudu-1.4/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:21:33.877347 moddagudu-1.4/setup.cfg
--rw-rw-rw-   0        0        0      219 2023-05-10 17:20:08.000000 moddagudu-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.268175 moddagudu-1.5/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.5/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:25:59.268175 moddagudu-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.236921 moddagudu-1.5/moddagudu/
+-rw-rw-rw-   0        0        0       76 2023-05-10 17:25:29.000000 moddagudu-1.5/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.5/moddagudu/ep.py
+-rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.5/moddagudu/mg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.268175 moddagudu-1.5/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 17:25:59.268175 moddagudu-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      219 2023-05-10 17:25:54.000000 moddagudu-1.5/setup.py
```

### Comparing `moddagudu-1.4/LICENSE.md` & `moddagudu-1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `moddagudu-1.4/moddagudu/mg.py` & `moddagudu-1.5/moddagudu/ep.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-def namaste(name):
-    print('Pedha Manishiki Pranamaalu...')
-    print(name+' garu....koodu maesinaara?')
 import numpy as np
 import librosa
 # from sklearn.metrics.pairwise import cosine_similarity
 
 def compute_cumshot(audio_file):
     # speaker_name = (audio_file.split('/')[-1]).split('.')[0]
     # Apply PCA to reduce the dimensionality of the MFCC features
```

