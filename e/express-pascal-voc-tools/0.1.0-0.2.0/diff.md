# Comparing `tmp/express-pascal-voc-tools-0.1.0.tar.gz` & `tmp/express-pascal-voc-tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "express-pascal-voc-tools-0.1.0.tar", last modified: Tue May  9 17:38:45 2023, max compression
+gzip compressed data, was "express-pascal-voc-tools-0.2.0.tar", last modified: Tue May  9 19:32:35 2023, max compression
```

## Comparing `express-pascal-voc-tools-0.1.0.tar` & `express-pascal-voc-tools-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 17:38:45.007046 express-pascal-voc-tools-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      798 2023-05-09 17:38:45.001040 express-pascal-voc-tools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-09 11:26:47.000000 express-pascal-voc-tools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.903297 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/
--rw-rw-rw-   0        0        0      798 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-09 17:38:44.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 17:38:43.000000 express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 17:38:45.008341 express-pascal-voc-tools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-09 12:11:51.000000 express-pascal-voc-tools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.967205 express-pascal-voc-tools-0.1.0/voc_tools/
--rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.1.0/voc_tools/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-05-09 13:23:59.000000 express-pascal-voc-tools-0.1.0/voc_tools/annotation.py
--rw-rw-rw-   0        0        0     2318 2023-05-09 17:37:01.000000 express-pascal-voc-tools-0.1.0/voc_tools/reader.py
-drwxrwxrwx   0        0        0        0 2023-05-09 17:38:44.987774 express-pascal-voc-tools-0.1.0/voc_tools/unittest/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.1.0/voc_tools/unittest/__init__.py
--rw-rw-rw-   0        0        0     1289 2023-05-09 13:54:53.000000 express-pascal-voc-tools-0.1.0/voc_tools/unittest/reader_test.py
--rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.1.0/voc_tools/visulizer.py
--rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.1.0/voc_tools/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:32:35.062446 express-pascal-voc-tools-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-09 09:49:08.000000 express-pascal-voc-tools-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      897 2023-05-09 19:32:35.058973 express-pascal-voc-tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-09 17:39:47.000000 express-pascal-voc-tools-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 19:32:35.017008 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/
+-rw-rw-rw-   0        0        0      897 2023-05-09 19:32:34.000000 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-09 19:32:34.000000 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:32:34.000000 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 19:32:34.000000 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 19:32:34.000000 express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:32:35.063465 express-pascal-voc-tools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      942 2023-05-09 18:48:05.000000 express-pascal-voc-tools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:32:35.043421 express-pascal-voc-tools-0.2.0/voc_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:14:59.000000 express-pascal-voc-tools-0.2.0/voc_tools/__init__.py
+-rw-rw-rw-   0        0        0     2942 2023-05-09 19:22:34.000000 express-pascal-voc-tools-0.2.0/voc_tools/annotation.py
+-rw-rw-rw-   0        0        0     2318 2023-05-09 17:37:01.000000 express-pascal-voc-tools-0.2.0/voc_tools/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:32:35.052963 express-pascal-voc-tools-0.2.0/voc_tools/unittest/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:15:29.000000 express-pascal-voc-tools-0.2.0/voc_tools/unittest/__init__.py
+-rw-rw-rw-   0        0        0     1381 2023-05-09 19:23:14.000000 express-pascal-voc-tools-0.2.0/voc_tools/unittest/reader_test.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 10:19:19.000000 express-pascal-voc-tools-0.2.0/voc_tools/visulizer.py
+-rw-rw-rw-   0        0        0        2 2023-05-09 13:20:51.000000 express-pascal-voc-tools-0.2.0/voc_tools/writer.py
```

### Comparing `express-pascal-voc-tools-0.1.0/LICENSE` & `express-pascal-voc-tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.1.0/PKG-INFO` & `express-pascal-voc-tools-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Pascal Voc Tools
- A tool for creating, reading and visualizing Pascal VOC annotations
+
+A tool for creating, reading and visualizing Pascal VOC annotations
 
 # Getting Started
 
 ## Install
+
 `pip install express-pascal-voc-tools`
 
 ## VOC Reading
 
-
 # Collaborate
+
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
+
+## Build and Publish
+
+`python setup.py sdist bdist_wheel`
+`python -m twine upload dist/*`
```

### Comparing `express-pascal-voc-tools-0.1.0/express_pascal_voc_tools.egg-info/PKG-INFO` & `express-pascal-voc-tools-0.2.0/express_pascal_voc_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: express-pascal-voc-tools
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool for creating, reading and visualizing Pascal VOC annotations
 Author: Soumen Sardar
 Author-email: soumensardarintmain@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Express Pascal Voc Tools
- A tool for creating, reading and visualizing Pascal VOC annotations
+
+A tool for creating, reading and visualizing Pascal VOC annotations
 
 # Getting Started
 
 ## Install
+
 `pip install express-pascal-voc-tools`
 
 ## VOC Reading
 
-
 # Collaborate
+
 GitHub: [https://github.com/Redcof/pascal_voc_tools.git](https://github.com/Redcof/pascal_voc_tools.git)
+
+## Build and Publish
+
+`python setup.py sdist bdist_wheel`
+`python -m twine upload dist/*`
```

### Comparing `express-pascal-voc-tools-0.1.0/setup.py` & `express-pascal-voc-tools-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['lxml'],
+    install_requires=['lxml', 'numpy'],
     version_config=True,
-    version="0.1.0"
+    version="0.2.0"
     # setup_requires=["setuptools-git-versioning"]
 )
```

### Comparing `express-pascal-voc-tools-0.1.0/voc_tools/annotation.py` & `express-pascal-voc-tools-0.2.0/voc_tools/annotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import os
+
+import numpy as np
+
+
 class Annotation:
     def __init__(self, filename, xmin, ymin, xmax, ymax, center_x, center_y, class_name):
         self._xmin, self._ymin, self._xmax, self._ymax, self._center_x, self._center_y, self._class_name = (
             xmin, ymin, xmax,
             ymax, center_x,
             center_y,
             class_name)
@@ -36,36 +41,65 @@
         return self._center_y
 
     @property
     def class_name(self):
         return self._class_name
 
     def __str__(self):
-        return "file:{},xmin:{},ymin:{},xmax:{},ymax:{},center_x:{},center_y:{},class_name:{}".format(
-            self._filename, self._xmin, self._ymin, self._xmax, self._ymax, self._center_x, self._center_y,
-            self._class_name
-        )
-
-    @classmethod
-    def csv_header(cls):
-        return "file,xmin,ymin,xmax,ymax,center_x,center_y,class_name"
+        s = ""
+        for k, v in zip(self.raw_attributes(), self.raw()):
+            s = "{}{}:{},".format(s, k, v)
+        return s.strip(",")
+
+    @staticmethod
+    def csv_header():
+        return ",".join(Annotation.raw_attributes())
 
     def csv(self):
-        return "{},{},{},{},{},{},{},{}".format(
-            self._filename, self._xmin, self._ymin, self._xmax, self._ymax, self._center_x, self._center_y,
-            self._class_name
-        )
+        return "{},{},{},{},{},{},{},{}".format(*self.raw())
 
+    @staticmethod
+    def raw_attributes():
+        return "file", "xmin", "ymin", "xmax", "ymax", "center_x", "center_y", "class_name"
 
-class VOCDataset:
+    def raw(self):
+        return (self._filename, self._xmin, self._ymin, self._xmax, self._ymax, self._center_x, self._center_y,
+                self._class_name
+                )
+
+
+class ABCDataset:
     def __init__(self, dataset_path):
         self.dataset_path = dataset_path
+        self.meta = np.array([], dtype='object')
+
+    def load(self):
+        from voc_tools.reader import from_dir
+        self.meta = np.array([anno.raw() for anno in from_dir(self.dataset_path)], dtype='object')
+        return self
+
+    def unload(self):
+        del self.meta
+        self.meta = np.array([], dtype='object')
+        return self
+
+    def class_names(self):
+        class_name_idx = Annotation.raw_attributes().index('class_name')
+        return set(self.meta[:, class_name_idx])
 
     def to_csv(self, path_to_csv, write_mode="w"):
         """
         Generate csv file for given VOC dataset
         """
         from voc_tools.reader import from_dir
         with open(path_to_csv, write_mode) as csv_fp:
             csv_fp.write("{}\n".format(Annotation.csv_header()))
             for anno in from_dir(self.dataset_path):
                 csv_fp.write("{}\n".format(anno.csv()))
+        return self
+
+
+class VOCDataset:
+    def __init__(self, dataset_path):
+        self.dataset_path = dataset_path
+        self.train = ABCDataset(os.path.join(self.dataset_path, "train"))
+        self.test = ABCDataset(os.path.join(self.dataset_path, "test"))
```

### Comparing `express-pascal-voc-tools-0.1.0/voc_tools/reader.py` & `express-pascal-voc-tools-0.2.0/voc_tools/reader.py`

 * *Files identical despite different names*

### Comparing `express-pascal-voc-tools-0.1.0/voc_tools/unittest/reader_test.py` & `express-pascal-voc-tools-0.2.0/voc_tools/unittest/reader_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 from voc_tools import reader as voc_reader
 
 from voc_tools.annotation import Annotation, VOCDataset
 
 
 class MyTestCase(unittest.TestCase):
     def test_something(self):
-        dataset_path = pathlib.Path(r"sixray_data/train")
+        dataset_path = pathlib.Path(r"sixray_data")
 
-        self.assertEqual(list(voc_reader.list_dir(str(dataset_path), fullpath=False)),
+        self.assertEqual(list(voc_reader.list_dir(str(dataset_path / "train"), fullpath=False)),
                          ["P00002.xml", "P00003.xml", "P00004.xml"], msg="XML files not matched.")
-        self.assertEqual(list(voc_reader.list_dir(str(dataset_path), fullpath=False, images=True)),
+        self.assertEqual(list(voc_reader.list_dir(str(dataset_path / "train"), fullpath=False, images=True)),
                          ["P00002.jpg", "P00003.jpg", "P00004.jpg"], msg="JPEG files not matched.")
         self.assertEqual(Annotation.csv_header(), "file,xmin,ymin,xmax,ymax,center_x,center_y,class_name",
                          msg="CSV header mismatch")
 
         for anno in voc_reader.from_file(r"sixray_data\train\JPEGImages\P00002.jpeg"):
-            print(anno.csv())
+            print(anno)
         for anno in voc_reader.from_file(r"sixray_data\train\Annotations\P00002.xml"):
             print(anno.csv())
-        for anno in voc_reader.from_dir(str(dataset_path)):
+        for anno in voc_reader.from_dir(str(dataset_path / "train")):
             print(anno.csv())
+        print(Annotation.csv_header())
 
-        VOCDataset(str(dataset_path)).to_csv(str(dataset_path / "train.csv"))
+        print(VOCDataset(str(dataset_path)).train.load().to_csv(str(dataset_path / "train.csv")).class_names())
 
 
 if __name__ == '__main__':
     unittest.main()
```

