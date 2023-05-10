# Comparing `tmp/OnloadTable-0.3.1.tar.gz` & `tmp/OnloadTable-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnloadTable-0.3.1.tar", last modified: Sat May  6 02:35:46 2023, max compression
+gzip compressed data, was "OnloadTable-0.3.2.tar", last modified: Wed May 10 03:42:19 2023, max compression
```

## Comparing `OnloadTable-0.3.1.tar` & `OnloadTable-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.071701 OnloadTable-0.3.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.044693 OnloadTable-0.3.1/OnloadTable/
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.059695 OnloadTable-0.3.1/OnloadTable/Function/
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.060693 OnloadTable-0.3.1/OnloadTable/Function/Function/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.065693 OnloadTable-0.3.1/OnloadTable/Function/Ui/
--rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/ExcelUi.pyd
--rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/MaskWin.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/__init__.py
--rw-rw-rw-   0        0        0   290816 2023-05-05 11:08:53.000000 OnloadTable-0.3.1/OnloadTable/Function/mysqlexcel.pyd
--rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:23.000000 OnloadTable-0.3.1/OnloadTable/Function/optionDb.pyd
--rw-rw-rw-   0        0        0       36 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Function/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.068693 OnloadTable-0.3.1/OnloadTable/Ui/
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/Ui/__init__.py
--rw-rw-rw-   0        0        0    90112 2023-05-05 10:30:39.000000 OnloadTable-0.3.1/OnloadTable/Ui/onloadUi.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 03:36:33.000000 OnloadTable-0.3.1/OnloadTable/__init__.py
--rw-rw-rw-   0        0        0   244224 2023-05-06 02:29:25.000000 OnloadTable-0.3.1/OnloadTable/onload.pyd
-drwxrwxrwx   0        0        0        0 2023-05-06 02:35:46.050693 OnloadTable-0.3.1/OnloadTable.egg-info/
--rw-rw-rw-   0        0        0      400 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-05-06 02:35:46.000000 OnloadTable-0.3.1/OnloadTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 02:35:45.000000 OnloadTable-0.3.1/OnloadTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      400 2023-05-06 02:35:46.072693 OnloadTable-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.1/README.md
--rw-rw-rw-   0        0        0      135 2023-05-06 02:35:46.073590 OnloadTable-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-05-06 02:35:27.000000 OnloadTable-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.916357 OnloadTable-0.3.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 OnloadTable-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 OnloadTable-0.3.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.883355 OnloadTable-0.3.2/OnloadTable/
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.900357 OnloadTable-0.3.2/OnloadTable/Function/
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.902361 OnloadTable-0.3.2/OnloadTable/Function/Function/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/Function/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.909358 OnloadTable-0.3.2/OnloadTable/Function/Ui/
+-rw-rw-rw-   0        0        0    46080 2023-04-28 06:34:36.000000 OnloadTable-0.3.2/OnloadTable/Function/Ui/ExcelUi.pyd
+-rw-rw-rw-   0        0        0    40448 2023-04-28 06:34:44.000000 OnloadTable-0.3.2/OnloadTable/Function/Ui/MaskWin.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/Function/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/Function/__init__.py
+-rw-rw-rw-   0        0        0   290816 2023-05-05 13:21:34.000000 OnloadTable-0.3.2/OnloadTable/Function/mysqlexcel.pyd
+-rw-rw-rw-   0        0        0    69632 2023-04-28 06:24:22.000000 OnloadTable-0.3.2/OnloadTable/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0       36 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/Function/settings.py
+-rw-rw-rw-   0        0        0   244224 2023-05-10 03:39:05.000000 OnloadTable-0.3.2/OnloadTable/OnloadTable.pyd
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.912356 OnloadTable-0.3.2/OnloadTable/Ui/
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/Ui/__init__.py
+-rw-rw-rw-   0        0        0    90112 2023-04-28 06:24:14.000000 OnloadTable-0.3.2/OnloadTable/Ui/onloadUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-03-01 03:36:32.000000 OnloadTable-0.3.2/OnloadTable/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:42:19.891355 OnloadTable-0.3.2/OnloadTable.egg-info/
+-rw-rw-rw-   0        0        0      394 2023-05-10 03:42:19.000000 OnloadTable-0.3.2/OnloadTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-05-10 03:42:19.000000 OnloadTable-0.3.2/OnloadTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:42:19.000000 OnloadTable-0.3.2/OnloadTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 03:42:19.000000 OnloadTable-0.3.2/OnloadTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      394 2023-05-10 03:42:19.916357 OnloadTable-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 OnloadTable-0.3.2/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-10 03:42:19.918355 OnloadTable-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-05-10 03:40:41.000000 OnloadTable-0.3.2/setup.py
```

### Comparing `OnloadTable-0.3.1/LICENSE.txt` & `OnloadTable-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnloadTable-0.3.1/OnloadTable.egg-info/SOURCES.txt` & `OnloadTable-0.3.2/OnloadTable.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+OnloadTable/OnloadTable.pyd
 OnloadTable/__init__.py
-OnloadTable/onload.pyd
 OnloadTable.egg-info/PKG-INFO
 OnloadTable.egg-info/SOURCES.txt
 OnloadTable.egg-info/dependency_links.txt
 OnloadTable.egg-info/top_level.txt
 OnloadTable/Function/__init__.py
 OnloadTable/Function/mysqlexcel.pyd
 OnloadTable/Function/optionDb.pyd
```

### Comparing `OnloadTable-0.3.1/setup.py` & `OnloadTable-0.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "OnloadTable",
-	version = VERSION,
-    author ="wangweidong",
-    author_email = "17891967090@163.com",
-    description='上传底稿目录功能',
+    version=VERSION,
+    author="wangweidong",
+    author_email="17891967090@163.com",
+    description='加载底稿目录',
     long_description_content_type="text/markdown",
-	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
-	long_description = open('README.md',encoding="utf-8").read(),
+    url='https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
+    long_description=open('README.md', encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
-	packages = find_packages(),
- 	# license = '',
-   	classifiers = [
-       'Programming Language :: Python',
+    packages=find_packages(),
+    # license = '',
+    classifiers=[
+        'Programming Language :: Python',
 
     ],
-    #包含的类型
-    package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
-    include_package_data=True #也选上
+    # 包含的类型
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db']},  # 这个很重要
+    include_package_data=True  # 也选上
 
 )
```

