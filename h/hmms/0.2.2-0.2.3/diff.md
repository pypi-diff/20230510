# Comparing `tmp/hmms-0.2.2.tar.gz` & `tmp/hmms-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmms-0.2.2.tar", last modified: Wed May 10 10:49:10 2023, max compression
+gzip compressed data, was "hmms-0.2.3.tar", last modified: Wed May 10 14:43:08 2023, max compression
```

## Comparing `hmms-0.2.2.tar` & `hmms-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 10:49:10.142739 hmms-0.2.2/
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     7048 2023-02-27 08:13:23.000000 hmms-0.2.2/LICENSE
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      165 2023-05-10 10:48:57.000000 hmms-0.2.2/MANIFEST.in
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      943 2023-05-10 10:49:10.142739 hmms-0.2.2/PKG-INFO
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)     1734 2023-02-27 08:49:45.000000 hmms-0.2.2/README
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1816 2023-02-27 10:09:27.000000 hmms-0.2.2/README.md
-drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 10:49:10.142739 hmms-0.2.2/hmms/
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      102 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/__init__.py
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      234 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/__main__.py
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1858 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/art.py
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)  2189110 2023-02-27 09:31:26.000000 hmms-0.2.2/hmms/cthmm.c
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    40246 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/cthmm.pyx
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)   999629 2023-02-27 09:31:26.000000 hmms-0.2.2/hmms/dthmm.c
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    20635 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/dthmm.pyx
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)   266375 2023-02-27 09:31:27.000000 hmms-0.2.2/hmms/hmm.c
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      225 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/hmm.pxd
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      253 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/hmm.pyx
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     3990 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms/train.py
-drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 10:49:10.142739 hmms-0.2.2/hmms.egg-info/
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      943 2023-05-10 10:49:10.000000 hmms-0.2.2/hmms.egg-info/PKG-INFO
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      475 2023-05-10 10:49:10.000000 hmms-0.2.2/hmms.egg-info/SOURCES.txt
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        1 2023-05-10 10:49:10.000000 hmms-0.2.2/hmms.egg-info/dependency_links.txt
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        1 2023-02-27 09:15:30.000000 hmms-0.2.2/hmms.egg-info/not-zip-safe
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)       45 2023-05-10 10:49:10.000000 hmms-0.2.2/hmms.egg-info/requires.txt
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        5 2023-05-10 10:49:10.000000 hmms-0.2.2/hmms.egg-info/top_level.txt
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)   228548 2023-02-27 08:13:23.000000 hmms-0.2.2/hmms.ipynb
--rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      122 2023-02-27 08:13:23.000000 hmms-0.2.2/requirements.txt
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)       63 2023-05-10 10:49:10.142739 hmms-0.2.2/setup.cfg
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1490 2023-05-10 10:28:48.000000 hmms-0.2.2/setup.py
-drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 10:49:10.142739 hmms-0.2.2/test/
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     2141 2023-02-27 08:13:23.000000 hmms-0.2.2/test/common.py
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    29774 2023-02-27 08:13:23.000000 hmms-0.2.2/test/experiments.py
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     8386 2023-02-27 08:13:23.000000 hmms-0.2.2/test/test_cthmm.py
--rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     7415 2023-02-27 08:13:23.000000 hmms-0.2.2/test/test_dthmm.py
+drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 14:43:08.208656 hmms-0.2.3/
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     7048 2023-02-27 08:13:23.000000 hmms-0.2.3/LICENSE
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      165 2023-05-10 10:48:57.000000 hmms-0.2.3/MANIFEST.in
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)     2792 2023-05-10 14:43:08.208656 hmms-0.2.3/PKG-INFO
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)     1734 2023-02-27 08:49:45.000000 hmms-0.2.3/README
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1816 2023-02-27 10:09:27.000000 hmms-0.2.3/README.md
+drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 14:43:08.208656 hmms-0.2.3/hmms/
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      102 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/__init__.py
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      234 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/__main__.py
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1858 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/art.py
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)  2189110 2023-02-27 09:31:26.000000 hmms-0.2.3/hmms/cthmm.c
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    40246 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/cthmm.pyx
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)   999629 2023-02-27 09:31:26.000000 hmms-0.2.3/hmms/dthmm.c
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    20635 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/dthmm.pyx
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)   266375 2023-02-27 09:31:27.000000 hmms-0.2.3/hmms/hmm.c
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      225 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/hmm.pxd
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)      253 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/hmm.pyx
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     3990 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms/train.py
+drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 14:43:08.208656 hmms-0.2.3/hmms.egg-info/
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)     2792 2023-05-10 14:43:08.000000 hmms-0.2.3/hmms.egg-info/PKG-INFO
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      475 2023-05-10 14:43:08.000000 hmms-0.2.3/hmms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        1 2023-05-10 14:43:08.000000 hmms-0.2.3/hmms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        1 2023-02-27 09:15:30.000000 hmms-0.2.3/hmms.egg-info/not-zip-safe
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)       45 2023-05-10 14:43:08.000000 hmms-0.2.3/hmms.egg-info/requires.txt
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)        5 2023-05-10 14:43:08.000000 hmms-0.2.3/hmms.egg-info/top_level.txt
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)   228548 2023-02-27 08:13:23.000000 hmms-0.2.3/hmms.ipynb
+-rw-rw-r--   0 jamaisvu  (1000) jamaisvu  (1000)      122 2023-02-27 08:13:23.000000 hmms-0.2.3/requirements.txt
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)       63 2023-05-10 14:43:08.208656 hmms-0.2.3/setup.cfg
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     1579 2023-05-10 14:42:29.000000 hmms-0.2.3/setup.py
+drwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)        0 2023-05-10 14:43:08.208656 hmms-0.2.3/test/
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     2141 2023-02-27 08:13:23.000000 hmms-0.2.3/test/common.py
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)    29774 2023-02-27 08:13:23.000000 hmms-0.2.3/test/experiments.py
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     8386 2023-02-27 08:13:23.000000 hmms-0.2.3/test/test_cthmm.py
+-rwxrwxr-x   0 jamaisvu  (1000) jamaisvu  (1000)     7415 2023-02-27 08:13:23.000000 hmms-0.2.3/test/test_dthmm.py
```

### Comparing `hmms-0.2.2/LICENSE` & `hmms-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/README` & `hmms-0.2.3/README`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/README.md` & `hmms-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/art.py` & `hmms-0.2.3/hmms/art.py`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/cthmm.c` & `hmms-0.2.3/hmms/cthmm.c`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/cthmm.pyx` & `hmms-0.2.3/hmms/cthmm.pyx`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/dthmm.c` & `hmms-0.2.3/hmms/dthmm.c`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/dthmm.pyx` & `hmms-0.2.3/hmms/dthmm.pyx`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/hmm.c` & `hmms-0.2.3/hmms/hmm.c`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms/train.py` & `hmms-0.2.3/hmms/train.py`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/hmms.ipynb` & `hmms-0.2.3/hmms.ipynb`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/setup.py` & `hmms-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from Cython.Build import cythonize
 import numpy
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
-
 setup(
     name='hmms',
-    version='0.2.2',
+    version='0.2.3',
     description='Efficient discrete and continuous-time hidden Markov model library able to handle hundreds of hidden states',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Lukas Lopatovsky',
     author_email='lopatovsky@gmail.com',
     license='Public Domain',
     keywords='Hidden Markov Model,Continuous-time Hidden Markov Model,HMM,CT-HMM,DT-HMM',
     url='https://github.com/lopatovsky/CT-HMM',
     packages=find_packages(),
     zip_safe=False,
```

### Comparing `hmms-0.2.2/test/common.py` & `hmms-0.2.3/test/common.py`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/test/experiments.py` & `hmms-0.2.3/test/experiments.py`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/test/test_cthmm.py` & `hmms-0.2.3/test/test_cthmm.py`

 * *Files identical despite different names*

### Comparing `hmms-0.2.2/test/test_dthmm.py` & `hmms-0.2.3/test/test_dthmm.py`

 * *Files identical despite different names*

