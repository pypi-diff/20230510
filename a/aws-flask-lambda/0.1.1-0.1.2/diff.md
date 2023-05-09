# Comparing `tmp/aws_flask_lambda-0.1.1.tar.gz` & `tmp/aws_flask_lambda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_flask_lambda-0.1.1.tar", last modified: Tue May  9 23:11:09 2023, max compression
+gzip compressed data, was "aws_flask_lambda-0.1.2.tar", last modified: Tue May  9 23:22:00 2023, max compression
```

## Comparing `aws_flask_lambda-0.1.1.tar` & `aws_flask_lambda-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 23:11:09.029543 aws_flask_lambda-0.1.1/
--rw-rw-rw-   0        0        0     1332 2023-05-09 23:11:09.029044 aws_flask_lambda-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-05-09 21:27:54.000000 aws_flask_lambda-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 23:11:09.022825 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/
--rw-rw-rw-   0        0        0     1332 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 23:11:09.030333 aws_flask_lambda-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-09 23:10:42.000000 aws_flask_lambda-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:22:00.776336 aws_flask_lambda-0.1.2/
+-rw-rw-rw-   0        0        0     1332 2023-05-09 23:22:00.771130 aws_flask_lambda-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-05-09 21:27:54.000000 aws_flask_lambda-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 23:22:00.717898 aws_flask_lambda-0.1.2/aws_flask_lambda/
+-rw-rw-rw-   0        0        0     3713 2023-03-03 22:19:32.000000 aws_flask_lambda-0.1.2/aws_flask_lambda/aws_flask_lambda.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:22:00.760946 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/
+-rw-rw-rw-   0        0        0     1332 2023-05-09 23:22:00.000000 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-05-09 23:22:00.000000 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:22:00.000000 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-09 23:22:00.000000 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 23:22:00.000000 aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:22:00.777070 aws_flask_lambda-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      771 2023-05-09 23:21:51.000000 aws_flask_lambda-0.1.2/setup.py
```

### Comparing `aws_flask_lambda-0.1.1/PKG-INFO` & `aws_flask_lambda-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_flask_lambda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to run applications on AWS Lambda Function using Flask
 Home-page: UNKNOWN
 Author: Seven Clouds Technologies
 Author-email: admin@seventechnologies.cloud
 License: UNKNOWN
 Description: # aws_flask_lambda
```

### Comparing `aws_flask_lambda-0.1.1/README.md` & `aws_flask_lambda-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/PKG-INFO` & `aws_flask_lambda-0.1.2/aws_flask_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-flask-lambda
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to run applications on AWS Lambda Function using Flask
 Home-page: UNKNOWN
 Author: Seven Clouds Technologies
 Author-email: admin@seventechnologies.cloud
 License: UNKNOWN
 Description: # aws_flask_lambda
```

### Comparing `aws_flask_lambda-0.1.1/setup.py` & `aws_flask_lambda-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aws_flask_lambda',
-    version='0.1.1',
+    version='0.1.2',
     description='Library to run applications on AWS Lambda Function using Flask',
     author='Seven Clouds Technologies',
     author_email='admin@seventechnologies.cloud',
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
-    packages=find_packages(),
+    packages=["aws_flask_lambda"],
+    package_dir={"aws_flask_lambda": "aws_flask_lambda"},
     include_package_data=True,
     install_requires=[
         'Flask==2.0.2',
         'werkzeug==2.0.2'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.8',
```

