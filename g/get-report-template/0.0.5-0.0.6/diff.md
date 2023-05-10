# Comparing `tmp/get-report-template-0.0.5.tar.gz` & `tmp/get-report-template-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-report-template-0.0.5.tar", last modified: Wed May 10 09:08:27 2023, max compression
+gzip compressed data, was "get-report-template-0.0.6.tar", last modified: Wed May 10 09:13:47 2023, max compression
```

## Comparing `get-report-template-0.0.5.tar` & `get-report-template-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 09:08:27.297879 get-report-template-0.0.5/
--rw-rw-rw-   0        0        0      469 2023-05-10 09:08:27.297380 get-report-template-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-10 08:35:12.000000 get-report-template-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 09:08:27.285378 get-report-template-0.0.5/get_report_template/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:19:17.000000 get-report-template-0.0.5/get_report_template/__init__.py
--rw-rw-rw-   0        0        0      291 2023-05-10 08:41:00.000000 get-report-template-0.0.5/get_report_template/get_report_template.py
-drwxrwxrwx   0        0        0        0 2023-05-10 09:08:27.296378 get-report-template-0.0.5/get_report_template.egg-info/
--rw-rw-rw-   0        0        0      469 2023-05-10 09:08:27.000000 get-report-template-0.0.5/get_report_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-05-10 09:08:27.000000 get-report-template-0.0.5/get_report_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 09:08:27.000000 get-report-template-0.0.5/get_report_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-05-10 09:08:27.000000 get-report-template-0.0.5/get_report_template.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-10 09:08:27.000000 get-report-template-0.0.5/get_report_template.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 09:08:27.297879 get-report-template-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      684 2023-05-10 09:08:25.000000 get-report-template-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:13:47.420776 get-report-template-0.0.6/
+-rw-rw-rw-   0        0        0       46 2023-05-10 09:13:39.000000 get-report-template-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      469 2023-05-10 09:13:47.420274 get-report-template-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-10 08:35:12.000000 get-report-template-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 09:13:47.403777 get-report-template-0.0.6/get_report_template/
+-rw-rw-rw-   0        0        0        0 2023-05-10 08:19:17.000000 get-report-template-0.0.6/get_report_template/__init__.py
+-rw-rw-rw-   0        0        0      291 2023-05-10 08:41:00.000000 get-report-template-0.0.6/get_report_template/get_report_template.py
+-rw-rw-rw-   0        0        0    42055 2023-05-10 08:04:50.000000 get-report-template-0.0.6/get_report_template/mobile_case_template.docx
+drwxrwxrwx   0        0        0        0 2023-05-10 09:13:47.419273 get-report-template-0.0.6/get_report_template.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-05-10 09:13:47.000000 get-report-template-0.0.6/get_report_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-10 09:13:47.000000 get-report-template-0.0.6/get_report_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:13:47.000000 get-report-template-0.0.6/get_report_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-10 09:13:47.000000 get-report-template-0.0.6/get_report_template.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-05-10 09:13:47.000000 get-report-template-0.0.6/get_report_template.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:13:47.421282 get-report-template-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-10 09:13:43.000000 get-report-template-0.0.6/setup.py
```

### Comparing `get-report-template-0.0.5/setup.py` & `get-report-template-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='get-report-template',
-    version='0.0.5',
+    version='0.0.6',
     description='',
     author='JayTrairat',
     author_email='jaytrairat@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/jaytrairat/python-get-report-template',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'get-report-template = get_report_template.get_report_template:main'
         ]
     },
-    package_data={
-        'get-report-template':['*.docx']
-    }
+    include_package_data=True
 )
```

