# Comparing `tmp/proteinTools-1.5.1.tar.gz` & `tmp/proteinTools-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.5.1.tar", last modified: Wed May 10 05:27:49 2023, max compression
+gzip compressed data, was "proteinTools-1.5.2.tar", last modified: Wed May 10 05:32:10 2023, max compression
```

## Comparing `proteinTools-1.5.1.tar` & `proteinTools-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.243954 proteinTools-1.5.1/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.5.1/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:27:49.239238 proteinTools-1.5.1/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.5.1/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.102919 proteinTools-1.5.1/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    53455 2023-05-10 05:27:12.000000 proteinTools-1.5.1/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.5.1/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.212034 proteinTools-1.5.1/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-10 05:27:49.254575 proteinTools-1.5.1/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-10 05:27:38.000000 proteinTools-1.5.1/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.105996 proteinTools-1.5.2/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.5.2/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:32:10.103589 proteinTools-1.5.2/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.5.2/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.001361 proteinTools-1.5.2/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53429 2023-05-10 05:31:56.000000 proteinTools-1.5.2/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.5.2/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:32:10.082657 proteinTools-1.5.2/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-10 05:32:09.000000 proteinTools-1.5.2/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-10 05:32:10.111572 proteinTools-1.5.2/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-10 05:31:29.000000 proteinTools-1.5.2/setup.py
```

### Comparing `proteinTools-1.5.1/LICENSE` & `proteinTools-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.5.1/proteinTools/PT.py` & `proteinTools-1.5.2/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         for atom in self.atoms:
             totmass += atom.mass
         for atom in self.atoms:
             modifier = atom.mass / totmass
             x += atom.x * modifier
             y += atom.y * modifier
             z += atom.z * modifier
-        print([x, y, z])
         return [x, y, z]
         
     def __getitem__(self, key):
         """
         Residue Index
     
         This property returns the atom contained in the parent residue based on the index of the atom as it appears in the structural file.
```

### Comparing `proteinTools-1.5.1/setup.py` & `proteinTools-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.5.1",
+    version = "1.5.2",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

