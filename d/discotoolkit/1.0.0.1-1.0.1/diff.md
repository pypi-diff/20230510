# Comparing `tmp/discotoolkit-1.0.0.1.tar.gz` & `tmp/discotoolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.0.1.tar", last modified: Fri Apr 21 05:57:44 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.1.tar", last modified: Wed May 10 16:28:50 2023, max compression
```

## Comparing `discotoolkit-1.0.0.1.tar` & `discotoolkit-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.659289 discotoolkit-1.0.0.1/
--rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-04-21 05:48:20.000000 discotoolkit-1.0.0.1/MANIFEST.in
--rw-rw-r--   0 rom       (1013) rom       (1027)      911 2023-04-21 05:57:34.655289 discotoolkit-1.0.0.1/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      812 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.619289 discotoolkit-1.0.0.1/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:44.000000 discotoolkit-1.0.0.1/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.0.1/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     1373 2023-04-17 05:08:54.000000 discotoolkit-1.0.0.1/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     4489 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     8380 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      556 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)       85 2023-04-14 07:12:49.000000 discotoolkit-1.0.0.1/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.651289 discotoolkit-1.0.0.1/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      911 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-04-21 05:57:34.659289 discotoolkit-1.0.0.1/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)     1061 2023-04-21 05:57:31.000000 discotoolkit-1.0.0.1/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.538223 discotoolkit-1.0.1/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-05-03 17:04:15.000000 discotoolkit-1.0.1/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-10 16:28:39.534222 discotoolkit-1.0.1/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1163 2023-05-10 16:28:04.000000 discotoolkit-1.0.1/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.494223 discotoolkit-1.0.1/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)    16691 2023-05-10 16:21:34.000000 discotoolkit-1.0.1/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.1/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     2479 2023-05-03 17:04:16.000000 discotoolkit-1.0.1/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     6958 2023-05-05 07:03:35.000000 discotoolkit-1.0.1/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)    12940 2023-05-03 17:04:16.000000 discotoolkit-1.0.1/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      631 2023-05-10 07:17:57.000000 discotoolkit-1.0.1/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      107 2023-05-10 06:00:24.000000 discotoolkit-1.0.1/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-05-10 16:28:39.526223 discotoolkit-1.0.1/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      848 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-05-10 16:28:39.000000 discotoolkit-1.0.1/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       89 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-05-10 16:28:38.000000 discotoolkit-1.0.1/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-05-10 16:28:39.538223 discotoolkit-1.0.1/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1115 2023-05-10 16:28:17.000000 discotoolkit-1.0.1/setup.py
```

### Comparing `discotoolkit-1.0.0.1/PKG-INFO` & `discotoolkit-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.0.1
+Version: 1.0.1
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
-            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
+            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
             
         
             Filter and download DISCO data based on sample metadata and cell type information
             
         CELLiD: cell type annotation
             
         scEnrichment: geneset enrichment using DISCO DEGs
             
-        CellMapper: project data into DISCO atlas
-            
 Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
```

### Comparing `discotoolkit-1.0.0.1/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.1/discotoolkit/GlobalVariable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""
+Global variable file to import for the subsequent script.
+
+Main purpose is for the logging to be imported to other script and getting the url
+"""
+
 import requests
 import json
 import logging
 # import random
 
 # setting the logging level
 # logger = logging.StreamHandler()
 # logger.setLevel(0)
 logging.basicConfig(level = logging.INFO)
 
-# testing for import
-# dummy = random.randint(0,100)
+timeout = 600
 
 # Define package-level variable
 response = requests.get("http://www.immunesinglecell.org/api/vishuo/getToolkitUrl")
 
-# response = requests.get(disco_url)
 if response.status_code == 200:
     prefix_disco_url = json.loads(response.text)["url"]
 else:
     prefix_disco_url = "http://www.immunesinglecell.org/toolkitapi"
```

### Comparing `discotoolkit-1.0.0.1/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.1/discotoolkit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0.0.1
+Version: 1.0.1
 Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
 Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
 Description: 
-            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
+            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
             
         
             Filter and download DISCO data based on sample metadata and cell type information
             
         CELLiD: cell type annotation
             
         scEnrichment: geneset enrichment using DISCO DEGs
             
-        CellMapper: project data into DISCO atlas
-            
 Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
```

### Comparing `discotoolkit-1.0.0.1/setup.py` & `discotoolkit-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
+# Read the contents of the requirements.txt file
+with open("requirements.txt", "r") as f:
+    requirements = f.read().splitlines()
+
 setup(
     name='discotoolkit',
-    version='1.0.0.1',
+    version='1.0.1',
     url='http://www.immunesinglecell.org/',
     author='Li Mengwei, Rom Uddamvathanak',
     author_email='uddamvathanak_rom@immunol.a-star.edu.sg',
     description='DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.',
     packages=find_packages(include=["discotoolkit", "discotoolkit.*"]),
-    install_requires=[
-        'numpy',
-        'pandas',
-    ],
-    python_requires = '>=3.8',
+    install_requires=requirements,
+    python_requires = '>=3.8.10',
     include_package_data=True,
     long_description="""
-    DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
+    DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions
     \n
     Filter and download DISCO data based on sample metadata and cell type information
     \nCELLiD: cell type annotation
     \nscEnrichment: geneset enrichment using DISCO DEGs
-    \nCellMapper: project data into DISCO atlas
     """,
     long_description_content_type = 'text/markdown',
 )
```

