# Comparing `tmp/start_time_estimator-1.10.3.tar.gz` & `tmp/start_time_estimator-1.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_time_estimator-1.10.3.tar", max compression
+gzip compressed data, was "start_time_estimator-1.10.4.tar", max compression
```

## Comparing `start_time_estimator-1.10.3.tar` & `start_time_estimator-1.10.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11349 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/LICENSE
--rw-r--r--   0        0        0     7299 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/README.md
--rw-r--r--   0        0        0      552 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/pyproject.toml
--rw-r--r--   0        0        0       81 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/__init__.py
--rw-r--r--   0        0        0    15710 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/concurrency_oracle.py
--rw-r--r--   0        0        0     4429 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/config.py
--rw-r--r--   0        0        0     8683 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/estimator.py
--rw-r--r--   0        0        0     4846 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/resource_availability.py
--rw-r--r--   0        0        0      165 2023-05-10 10:43:41.808123 start_time_estimator-1.10.3/src/start_time_estimator/utils.py
--rw-r--r--   0        0        0     7949 1970-01-01 00:00:00.000000 start_time_estimator-1.10.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/LICENSE
+-rw-r--r--   0        0        0     7299 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/README.md
+-rw-r--r--   0        0        0      552 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/__init__.py
+-rw-r--r--   0        0        0    15710 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/concurrency_oracle.py
+-rw-r--r--   0        0        0     4429 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/config.py
+-rw-r--r--   0        0        0     8683 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/estimator.py
+-rw-r--r--   0        0        0     4846 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/resource_availability.py
+-rw-r--r--   0        0        0      165 2023-05-10 11:08:23.307549 start_time_estimator-1.10.4/src/start_time_estimator/utils.py
+-rw-r--r--   0        0        0     7949 1970-01-01 00:00:00.000000 start_time_estimator-1.10.4/PKG-INFO
```

### Comparing `start_time_estimator-1.10.3/LICENSE` & `start_time_estimator-1.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/README.md` & `start_time_estimator-1.10.4/README.md`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/pyproject.toml` & `start_time_estimator-1.10.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "start-time-estimator"
-version = "1.10.3"
+version = "1.10.4"
 description = "Python package to estimate the enabled time, enabling activity, and resource availability time of each activity instance in an event log."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0.0"
```

### Comparing `start_time_estimator-1.10.3/src/start_time_estimator/concurrency_oracle.py` & `start_time_estimator-1.10.4/src/start_time_estimator/concurrency_oracle.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/src/start_time_estimator/config.py` & `start_time_estimator-1.10.4/src/start_time_estimator/config.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/src/start_time_estimator/estimator.py` & `start_time_estimator-1.10.4/src/start_time_estimator/estimator.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/src/start_time_estimator/resource_availability.py` & `start_time_estimator-1.10.4/src/start_time_estimator/resource_availability.py`

 * *Files identical despite different names*

### Comparing `start_time_estimator-1.10.3/PKG-INFO` & `start_time_estimator-1.10.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-time-estimator
-Version: 1.10.3
+Version: 1.10.4
 Summary: Python package to estimate the enabled time, enabling activity, and resource availability time of each activity instance in an event log.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

