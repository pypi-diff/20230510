# Comparing `tmp/digimat.units-0.0.2.tar.gz` & `tmp/digimat.units-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.units-0.0.2.tar", last modified: Sun Apr 25 11:38:16 2021, max compression
+gzip compressed data, was "digimat.units-0.0.3.tar", last modified: Wed May 10 21:12:59 2023, max compression
```

## Comparing `digimat.units-0.0.2.tar` & `digimat.units-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2021-04-25 11:38:16.105817 digimat.units-0.0.2/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      307 2021-04-25 11:38:16.105350 digimat.units-0.0.2/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2021-04-25 11:38:16.105918 digimat.units-0.0.2/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      911 2021-04-25 11:38:11.000000 digimat.units-0.0.2/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2021-04-25 11:38:16.099479 digimat.units-0.0.2/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2021-04-25 11:38:16.100232 digimat.units-0.0.2/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.units-0.0.2/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2021-04-25 11:38:16.104578 digimat.units-0.0.2/src/digimat/units/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       26 2021-04-25 11:11:58.000000 digimat.units-0.0.2/src/digimat/units/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1854 2021-04-25 11:37:10.000000 digimat.units-0.0.2/src/digimat/units/units.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2021-04-25 11:38:16.103603 digimat.units-0.0.2/src/digimat.units.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      307 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      383 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2021-04-25 11:07:24.000000 digimat.units-0.0.2/src/digimat.units.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       18 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2021-04-25 11:38:16.000000 digimat.units-0.0.2/src/digimat.units.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-05-10 21:12:59.355970 digimat.units-0.0.3/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      268 2023-05-10 21:12:59.355615 digimat.units-0.0.3/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-05-10 21:12:59.356102 digimat.units-0.0.3/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      911 2023-05-10 21:12:48.000000 digimat.units-0.0.3/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-05-10 21:12:59.346502 digimat.units-0.0.3/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-05-10 21:12:59.347800 digimat.units-0.0.3/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.units-0.0.3/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-05-10 21:12:59.355010 digimat.units-0.0.3/src/digimat/units/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       26 2021-04-25 11:11:58.000000 digimat.units-0.0.3/src/digimat/units/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     2088 2023-05-10 21:12:36.000000 digimat.units-0.0.3/src/digimat/units/units.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-05-10 21:12:59.353251 digimat.units-0.0.3/src/digimat.units.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      268 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      383 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2021-04-25 11:07:24.000000 digimat.units-0.0.3/src/digimat.units.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       18 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-05-10 21:12:59.000000 digimat.units-0.0.3/src/digimat.units.egg-info/top_level.txt
```

### Comparing `digimat.units-0.0.2/setup.py` & `digimat.units-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.units',
-    version='0.0.2',
+    version='0.0.3',
     description='Digimat Units',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.units-0.0.2/src/digimat/units/units.py` & `digimat.units-0.0.3/src/digimat/units/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,32 +41,43 @@
 
     def __len__(self):
         return len(self.UNIT_STR)
 
     def __getitem__(self, key):
         return self.get(key)
 
+    def __iter__(self):
+        return iter(self._units.values())
+
     def isDigital(self, unit):
         try:
             if int(unit)==self.UNIT_DIGITAL:
                 return True
         except:
             pass
         return False
 
     def digital(self):
         return self.UNIT_DIGITAL
 
+    def none(self):
+        return 0xFF
+
     def table(self, key=None):
         t=PrettyTable()
         t.field_names = ['#', 'unit']
         t.align['#']='l'
         t.align['unit']='l'
         for unit in range(len(self)):
             name=self.UNIT_STR[unit]
             if not key or key.lower() in name.lower():
                 t.add_row([unit, name])
         print(t)
 
+    def dump(self):
+        for unit in range(len(self)):
+            name=self.UNIT_STR[unit]
+            print(unit, name)
+
 
 if __name__=='__main__':
     pass
```

