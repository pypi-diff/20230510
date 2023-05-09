# Comparing `tmp/aws_flask_lambda_swagger_ui-0.1.1.tar.gz` & `tmp/aws_flask_lambda_swagger_ui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_flask_lambda_swagger_ui-0.1.1.tar", last modified: Tue May  9 23:07:55 2023, max compression
+gzip compressed data, was "aws_flask_lambda_swagger_ui-0.1.2.tar", last modified: Tue May  9 23:30:06 2023, max compression
```

## Comparing `aws_flask_lambda_swagger_ui-0.1.1.tar` & `aws_flask_lambda_swagger_ui-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 23:07:55.864745 aws_flask_lambda_swagger_ui-0.1.1/
--rw-rw-rw-   0        0        0     1439 2023-05-09 23:07:55.863690 aws_flask_lambda_swagger_ui-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-09 23:03:33.000000 aws_flask_lambda_swagger_ui-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 23:07:55.861992 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/
--rw-rw-rw-   0        0        0     1439 2023-05-09 23:07:55.000000 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-09 23:07:55.000000 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:07:55.000000 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 23:07:55.000000 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:07:55.000000 aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 23:07:55.864908 aws_flask_lambda_swagger_ui-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-05-09 23:03:55.000000 aws_flask_lambda_swagger_ui-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:30:06.431386 aws_flask_lambda_swagger_ui-0.1.2/
+-rw-rw-rw-   0        0        0     1439 2023-05-09 23:30:06.431192 aws_flask_lambda_swagger_ui-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-09 23:03:33.000000 aws_flask_lambda_swagger_ui-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 23:30:06.385430 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui/
+-rw-rw-rw-   0        0        0     2255 2023-03-03 22:19:32.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui/aws_flask_lambda_swagger_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:30:06.429243 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/
+-rw-rw-rw-   0        0        0     1439 2023-05-09 23:30:06.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-09 23:30:06.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:30:06.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-09 23:30:06.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-09 23:30:06.000000 aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:30:06.431386 aws_flask_lambda_swagger_ui-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      794 2023-05-09 23:29:57.000000 aws_flask_lambda_swagger_ui-0.1.2/setup.py
```

### Comparing `aws_flask_lambda_swagger_ui-0.1.1/PKG-INFO` & `aws_flask_lambda_swagger_ui-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_flask_lambda_swagger_ui
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adding swagger ui on your AWS Lambda Function using a Flask blueprint
 Home-page: UNKNOWN
 Author: Seven Clouds Technologies
 Author-email: admin@seventechnologies.cloud
 License: UNKNOWN
 Description: # aws_flask_lambda_swagger_ui
```

### Comparing `aws_flask_lambda_swagger_ui-0.1.1/README.md` & `aws_flask_lambda_swagger_ui-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_flask_lambda_swagger_ui-0.1.1/aws_flask_lambda_swagger_ui.egg-info/PKG-INFO` & `aws_flask_lambda_swagger_ui-0.1.2/aws_flask_lambda_swagger_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-flask-lambda-swagger-ui
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adding swagger ui on your AWS Lambda Function using a Flask blueprint
 Home-page: UNKNOWN
 Author: Seven Clouds Technologies
 Author-email: admin@seventechnologies.cloud
 License: UNKNOWN
 Description: # aws_flask_lambda_swagger_ui
```

