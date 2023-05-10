# Comparing `tmp/primerJinn-0.1.1.dev1.tar.gz` & `tmp/primerJinn-0.1.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerJinn-0.1.1.dev1.tar", last modified: Wed May 10 01:10:05 2023, max compression
+gzip compressed data, was "primerJinn-0.1.2.dev1.tar", last modified: Wed May 10 16:27:16 2023, max compression
```

## Comparing `primerJinn-0.1.1.dev1.tar` & `primerJinn-0.1.2.dev1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 01:10:05.746414 primerJinn-0.1.1.dev1/
--rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 01:10:05.746147 primerJinn-0.1.1.dev1/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     9746 2023-05-10 01:04:40.000000 primerJinn-0.1.1.dev1/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 01:10:05.745944 primerJinn-0.1.1.dev1/primerJinn.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 01:10:05.000000 primerJinn-0.1.1.dev1/primerJinn.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-10 01:10:05.746464 primerJinn-0.1.1.dev1/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-10 00:53:12.000000 primerJinn-0.1.1.dev1/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 16:27:16.908419 primerJinn-0.1.2.dev1/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 16:27:16.908159 primerJinn-0.1.2.dev1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     9746 2023-05-10 01:04:40.000000 primerJinn-0.1.2.dev1/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-10 16:27:16.907977 primerJinn-0.1.2.dev1/primerJinn.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10175 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-10 16:27:16.000000 primerJinn-0.1.2.dev1/primerJinn.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-10 16:27:16.908463 primerJinn-0.1.2.dev1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-10 16:27:07.000000 primerJinn-0.1.2.dev1/setup.py
```

### Comparing `primerJinn-0.1.1.dev1/PKG-INFO` & `primerJinn-0.1.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.1.dev1
+Version: 0.1.2.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
```

### Comparing `primerJinn-0.1.1.dev1/README.md` & `primerJinn-0.1.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `primerJinn-0.1.1.dev1/primerJinn.egg-info/PKG-INFO` & `primerJinn-0.1.2.dev1/primerJinn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.1.dev1
+Version: 0.1.2.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
```

### Comparing `primerJinn-0.1.1.dev1/setup.py` & `primerJinn-0.1.2.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.14.0+/bin"))
 
 
 setup(
     name='primerJinn',
-    version='0.1.1.dev1',
+    version='0.1.2.dev1',
     url='https://github.com/SemiQuant/primerJinn',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
```

