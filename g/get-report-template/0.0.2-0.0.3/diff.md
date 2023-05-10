# Comparing `tmp/get-report-template-0.0.2.tar.gz` & `tmp/get-report-template-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-report-template-0.0.2.tar", last modified: Wed May 10 08:55:18 2023, max compression
+gzip compressed data, was "get-report-template-0.0.3.tar", last modified: Wed May 10 08:58:51 2023, max compression
```

## Comparing `get-report-template-0.0.2.tar` & `get-report-template-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:55:18.264933 get-report-template-0.0.2/
--rw-rw-rw-   0        0        0      469 2023-05-10 08:55:18.264434 get-report-template-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-10 08:35:12.000000 get-report-template-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:55:18.261430 get-report-template-0.0.2/get_report_template.egg-info/
--rw-rw-rw-   0        0        0      469 2023-05-10 08:55:18.000000 get-report-template-0.0.2/get_report_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-10 08:55:18.000000 get-report-template-0.0.2/get_report_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:55:18.000000 get-report-template-0.0.2/get_report_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-10 08:55:18.000000 get-report-template-0.0.2/get_report_template.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-05-10 08:55:18.000000 get-report-template-0.0.2/get_report_template.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 08:55:18.265433 get-report-template-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-05-10 08:52:51.000000 get-report-template-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:55:18.263430 get-report-template-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:19:17.000000 get-report-template-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0      291 2023-05-10 08:41:00.000000 get-report-template-0.0.2/src/get_report_template.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:58:51.350527 get-report-template-0.0.3/
+-rw-rw-rw-   0        0        0      469 2023-05-10 08:58:51.350028 get-report-template-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-10 08:35:12.000000 get-report-template-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:58:51.346527 get-report-template-0.0.3/get_report_template.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-05-10 08:58:51.000000 get-report-template-0.0.3/get_report_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-10 08:58:51.000000 get-report-template-0.0.3/get_report_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:58:51.000000 get-report-template-0.0.3/get_report_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-10 08:58:51.000000 get-report-template-0.0.3/get_report_template.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-05-10 08:58:51.000000 get-report-template-0.0.3/get_report_template.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:58:51.350527 get-report-template-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-05-10 08:58:35.000000 get-report-template-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:58:51.349027 get-report-template-0.0.3/src/
+-rw-rw-rw-   0        0        0        0 2023-05-10 08:19:17.000000 get-report-template-0.0.3/src/__init__.py
+-rw-rw-rw-   0        0        0      291 2023-05-10 08:41:00.000000 get-report-template-0.0.3/src/get_report_template.py
```

### Comparing `get-report-template-0.0.2/setup.py` & `get-report-template-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='get-report-template',
-    version='0.0.2',
+    version='0.0.3',
     description='',
     author='JayTrairat',
     author_email='jaytrairat@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/jaytrairat/python-get-report-template',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'get-report-template = src.get_report_template:main'
         ]
     },
     package_data={
-        'get-report-template':['mobile_case_template.docx']
+        'get-report-template':['src/*.docx']
     }
 )
```

