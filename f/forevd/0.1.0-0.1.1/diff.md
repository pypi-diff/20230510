# Comparing `tmp/forevd-0.1.0.tar.gz` & `tmp/forevd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.0.tar", max compression
+gzip compressed data, was "forevd-0.1.1.tar", max compression
```

## Comparing `forevd-0.1.0.tar` & `forevd-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-09 23:17:02.895404 forevd-0.1.0/LICENSE
--rw-r--r--   0        0        0      486 2023-05-09 23:17:02.895404 forevd-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/__init__.py
--rw-r--r--   0        0        0     4390 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/__main__.py
--rw-r--r--   0        0        0     1498 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/apache/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/apache/httpd.conf
--rw-r--r--   0        0        0        0 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-05-09 23:17:02.895404 forevd-0.1.0/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      844 2023-05-09 23:17:02.895404 forevd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 forevd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 03:19:40.654211 forevd-0.1.1/LICENSE
+-rw-r--r--   0        0        0      486 2023-05-10 03:19:40.654211 forevd-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/__init__.py
+-rw-r--r--   0        0        0     4390 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/__main__.py
+-rw-r--r--   0        0        0     1498 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     3370 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0        0 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 03:19:40.658211 forevd-0.1.1/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-10 03:19:40.658211 forevd-0.1.1/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      844 2023-05-10 03:19:40.658211 forevd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 forevd-0.1.1/PKG-INFO
```

### Comparing `forevd-0.1.0/LICENSE` & `forevd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.0/forevd/__main__.py` & `forevd-0.1.1/forevd/__main__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.0/forevd/apache/__init__.py` & `forevd-0.1.1/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.0/forevd/apache/httpd.conf` & `forevd-0.1.1/forevd/apache/httpd.conf`

 * *Files identical despite different names*

### Comparing `forevd-0.1.0/pyproject.toml` & `forevd-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.0"
+version = "0.1.1"
 description = "Forward and reverse proxy using nginx or apache"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `forevd-0.1.0/PKG-INFO` & `forevd-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Forward and reverse proxy using nginx or apache
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

