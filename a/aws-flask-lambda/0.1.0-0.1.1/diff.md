# Comparing `tmp/aws_flask_lambda-0.1.0.tar.gz` & `tmp/aws_flask_lambda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_flask_lambda-0.1.0.tar", last modified: Tue May  9 20:45:54 2023, max compression
+gzip compressed data, was "aws_flask_lambda-0.1.1.tar", last modified: Tue May  9 23:11:09 2023, max compression
```

## Comparing `aws_flask_lambda-0.1.0.tar` & `aws_flask_lambda-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 20:45:54.381427 aws_flask_lambda-0.1.0/
--rw-rw-rw-   0        0        0      446 2023-05-09 20:45:54.381427 aws_flask_lambda-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 20:45:54.379618 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/
--rw-rw-rw-   0        0        0      446 2023-05-09 20:45:54.000000 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-09 20:45:54.000000 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:45:54.000000 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-09 20:45:54.000000 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:45:54.000000 aws_flask_lambda-0.1.0/aws_flask_lambda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 20:45:54.382730 aws_flask_lambda-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-05-09 20:45:33.000000 aws_flask_lambda-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:11:09.029543 aws_flask_lambda-0.1.1/
+-rw-rw-rw-   0        0        0     1332 2023-05-09 23:11:09.029044 aws_flask_lambda-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-05-09 21:27:54.000000 aws_flask_lambda-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 23:11:09.022825 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/
+-rw-rw-rw-   0        0        0     1332 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:11:08.000000 aws_flask_lambda-0.1.1/aws_flask_lambda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:11:09.030333 aws_flask_lambda-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-09 23:10:42.000000 aws_flask_lambda-0.1.1/setup.py
```

