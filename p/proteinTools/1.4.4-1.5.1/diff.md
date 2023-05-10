# Comparing `tmp/proteinTools-1.4.4.tar.gz` & `tmp/proteinTools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.4.4.tar", last modified: Wed May  3 04:09:01 2023, max compression
+gzip compressed data, was "proteinTools-1.5.1.tar", last modified: Wed May 10 05:27:49 2023, max compression
```

## Comparing `proteinTools-1.4.4.tar` & `proteinTools-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:01.046785 proteinTools-1.4.4/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.4.4/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-03 04:09:01.038872 proteinTools-1.4.4/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.4.4/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:00.902194 proteinTools-1.4.4/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    53271 2023-05-03 03:59:01.000000 proteinTools-1.4.4/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.4.4/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:00.999945 proteinTools-1.4.4/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-03 04:09:01.083979 proteinTools-1.4.4/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-03 04:08:43.000000 proteinTools-1.4.4/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.243954 proteinTools-1.5.1/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.5.1/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:27:49.239238 proteinTools-1.5.1/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.5.1/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.102919 proteinTools-1.5.1/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53455 2023-05-10 05:27:12.000000 proteinTools-1.5.1/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.5.1/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-10 05:27:49.212034 proteinTools-1.5.1/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-10 05:27:48.000000 proteinTools-1.5.1/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-10 05:27:49.254575 proteinTools-1.5.1/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-10 05:27:38.000000 proteinTools-1.5.1/setup.py
```

### Comparing `proteinTools-1.4.4/LICENSE` & `proteinTools-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.4.4/proteinTools/PT.py` & `proteinTools-1.5.1/proteinTools/PT.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         self.z = z
         self.residue = residue
         self.data = data
         self.mass = atom_dict[self.element]
         self.radius = element_radii[self.element]
         self.number = number
         
+    @cached_property
+    def center(self):
+        return [self.x, self.y, self.z]
+        
 class residue:
     """
     Residue class
     
     This class contains the essential parameters of an individual residue in a protein structural file, including the child atoms, protein sidechain, residue index, and type of amino acid.
     """
     def __init__(self, amino_acid, index, chain):
@@ -70,21 +74,21 @@
         Returns
         -------
         list
             A list consisting of the x, y, and z coordinate in 3D space of the residue center of mass position for the protein structural file.
         """
         x, y, z, totmass = 0, 0, 0, 0
         for atom in self.atoms:
-            x += atom.x
-            y += atom.y 
-            z += atom.z
             totmass += atom.mass
-        x /= atom.mass
-        y /= atom.mass
-        z /= atom.mass
+        for atom in self.atoms:
+            modifier = atom.mass / totmass
+            x += atom.x * modifier
+            y += atom.y * modifier
+            z += atom.z * modifier
+        print([x, y, z])
         return [x, y, z]
         
     def __getitem__(self, key):
         """
         Residue Index
     
         This property returns the atom contained in the parent residue based on the index of the atom as it appears in the structural file.
@@ -652,21 +656,21 @@
         list
             A list consisting of the x, y, and z coordinate in 3D space of the protein center of mass position for the protein structural file.
         """
         try:
             x, y, z, totmass = 0, 0, 0, 0
             for res in self.residue_list:
                 for atom in res.atoms:
-                    x += atom.x
-                    y += atom.y
-                    z += atom.z
                     totmass += atom.mass
-            x /= totmass
-            y /= totmass
-            z /= totmass
+            for res in self.residue_list:
+                for atom in res.atoms:
+                    modifier = atom.mass / totmass
+                    x += atom.x * modifier
+                    y += atom.y * modifier
+                    z += atom.z * modifier
             return [x, y, z]
         except:
             print('Protein not downloaded yet or downloaded incorrectly!')
     
     @cached_property
     def sites(self):
         """
@@ -1167,14 +1171,12 @@
     TODO
     - Add more ID conversions
     '''
 
 '''
 #For unit testing    
 if __name__ == '__main__':
-    p = Protein('3akm')
+    p = Protein('1O3F')
     p.download()
-    for res in p.residue_list:
-        for atom in res.atoms:
-            print(atom.radius)
-            
-'''      
+    print(p[0].center)
+    print(p[0][0].data)
+'''
```

### Comparing `proteinTools-1.4.4/setup.py` & `proteinTools-1.5.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.4.4",
+    version = "1.5.1",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

