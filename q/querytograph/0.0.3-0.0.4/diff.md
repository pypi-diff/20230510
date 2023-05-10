# Comparing `tmp/querytograph-0.0.3.tar.gz` & `tmp/querytograph-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querytograph-0.0.3.tar", last modified: Mon May  8 16:02:58 2023, max compression
+gzip compressed data, was "querytograph-0.0.4.tar", last modified: Tue May  9 15:41:25 2023, max compression
```

## Comparing `querytograph-0.0.3.tar` & `querytograph-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/
--rw-rw-r--   0 simk      (1000) simk      (1000)     1065 2023-05-07 16:29:46.000000 querytograph-0.0.3/LICENSE
--rw-rw-r--   0 simk      (1000) simk      (1000)     2083 2023-05-08 16:02:58.813732 querytograph-0.0.3/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)     1808 2023-05-08 16:00:20.000000 querytograph-0.0.3/README.md
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/querytograph/
--rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.3/querytograph/__init__.py
--rw-rw-r--   0 simk      (1000) simk      (1000)     7686 2023-05-08 15:47:14.000000 querytograph-0.0.3/querytograph/querytograph.py
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-08 16:02:58.813732 querytograph-0.0.3/querytograph.egg-info/
--rw-rw-r--   0 simk      (1000) simk      (1000)     2083 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)      259 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/SOURCES.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/dependency_links.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       71 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/requires.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-08 16:02:58.000000 querytograph-0.0.3/querytograph.egg-info/top_level.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-08 16:02:58.813732 querytograph-0.0.3/setup.cfg
--rw-rw-r--   0 simk      (1000) simk      (1000)      963 2023-05-08 16:02:21.000000 querytograph-0.0.3/setup.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-09 15:41:25.592411 querytograph-0.0.4/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1065 2023-05-07 16:29:46.000000 querytograph-0.0.4/LICENSE
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2092 2023-05-09 15:41:25.592411 querytograph-0.0.4/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1805 2023-05-08 16:04:34.000000 querytograph-0.0.4/README.md
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-09 15:41:25.592411 querytograph-0.0.4/querytograph/
+-rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.4/querytograph/__init__.py
+-rw-rw-r--   0 simk      (1000) simk      (1000)     7686 2023-05-08 15:47:14.000000 querytograph-0.0.4/querytograph/querytograph.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-09 15:41:25.592411 querytograph-0.0.4/querytograph.egg-info/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2092 2023-05-09 15:41:25.000000 querytograph-0.0.4/querytograph.egg-info/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)      259 2023-05-09 15:41:25.000000 querytograph-0.0.4/querytograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-09 15:41:25.000000 querytograph-0.0.4/querytograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       78 2023-05-09 15:41:25.000000 querytograph-0.0.4/querytograph.egg-info/requires.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-09 15:41:25.000000 querytograph-0.0.4/querytograph.egg-info/top_level.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-09 15:41:25.592411 querytograph-0.0.4/setup.cfg
+-rw-rw-r--   0 simk      (1000) simk      (1000)      993 2023-05-09 15:39:25.000000 querytograph-0.0.4/setup.py
```

### Comparing `querytograph-0.0.3/LICENSE` & `querytograph-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `querytograph-0.0.3/PKG-INFO` & `querytograph-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Using ChatGPT to convert your plain English queries into graphs
+Home-page: 
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +63,15 @@
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
 
 
 ## Contributing
 Contributions are welcome! Please contact me at franziss@gmail.com 
-This was a hack over my weekend and I am sure there are bounds to have bugs... sorry.. =)
+This was hack over a weekend and I am sure there are bounds to have bugs... sorry.. =)
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contact
 franziss@gmail.com
```

### Comparing `querytograph-0.0.3/README.md` & `querytograph-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,14 @@
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
 
 
 ## Contributing
 Contributions are welcome! Please contact me at franziss@gmail.com 
-This was a hack over my weekend and I am sure there are bounds to have bugs... sorry.. =)
+This was hack over a weekend and I am sure there are bounds to have bugs... sorry.. =)
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contact
 franziss@gmail.com
```

### Comparing `querytograph-0.0.3/querytograph/querytograph.py` & `querytograph-0.0.4/querytograph/querytograph.py`

 * *Files identical despite different names*

### Comparing `querytograph-0.0.3/querytograph.egg-info/PKG-INFO` & `querytograph-0.0.4/querytograph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Using ChatGPT to convert your plain English queries into graphs
+Home-page: 
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +63,15 @@
 3. Table Name  
    Filename of the dataframe that the user wants to query on.
    Do not require the exact name
 
 
 ## Contributing
 Contributions are welcome! Please contact me at franziss@gmail.com 
-This was a hack over my weekend and I am sure there are bounds to have bugs... sorry.. =)
+This was hack over a weekend and I am sure there are bounds to have bugs... sorry.. =)
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contact
 franziss@gmail.com
```

### Comparing `querytograph-0.0.3/setup.py` & `querytograph-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='querytograph',
     packages=find_packages(include=['querytograph']),
-    version='0.0.3',
+    version='0.0.4',
     description='Using ChatGPT to convert your plain English queries into graphs',
     long_description=long_description,
+    url='',
     long_description_content_type='text/markdown',
     author='franziss',
     author_email='franziss@gmail.com',
     license='MIT',
     install_requires=[
         'pandas',
         'openai',
         'langchain==0.0.160',
         'rapidfuzz==3.0.0',
         'gradio==3.26.0',
-        'numpy'
+        'numpy',
+        'plotly'
     ],
     setup_requires=[],
     tests_require=[]
 )
```

