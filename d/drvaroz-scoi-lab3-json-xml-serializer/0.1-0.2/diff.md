# Comparing `tmp/drvaroz_scoi_lab3_json_xml_serializer-0.1.tar.gz` & `tmp/drvaroz_scoi_lab3_json_xml_serializer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drvaroz_scoi_lab3_json_xml_serializer-0.1.tar", last modified: Wed May 10 14:30:55 2023, max compression
+gzip compressed data, was "drvaroz_scoi_lab3_json_xml_serializer-0.2.tar", last modified: Wed May 10 14:41:42 2023, max compression
```

## Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1.tar` & `drvaroz_scoi_lab3_json_xml_serializer-0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      398 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/PKG-INFO
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      398 2023-05-10 14:30:55.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/PKG-INFO
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      641 2023-05-10 14:30:55.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/SOURCES.txt
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        1 2023-05-10 14:30:55.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/dependency_links.txt
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       64 2023-05-10 14:30:55.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/top_level.txt
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 16:37:22.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      322 2023-05-08 08:54:46.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/factory.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 14:49:50.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1741 2023-05-08 08:45:06.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/json_parser.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      523 2023-05-08 07:17:50.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/json_serializer.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 10:05:02.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1004 2023-05-08 10:34:14.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/constants.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     6682 2023-05-08 10:44:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/serializer.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-08 07:41:47.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/__init__.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      682 2023-05-09 09:48:58.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_constants.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2332 2023-05-09 09:48:58.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_parser.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      549 2023-05-08 20:08:32.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_serializer.py
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       38 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/setup.cfg
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      591 2023-05-10 14:27:50.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/setup.py
-drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:30:55.553873 drvaroz_scoi_lab3_json_xml_serializer-0.1/tests/
--rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2440 2023-05-09 10:21:43.000000 drvaroz_scoi_lab3_json_xml_serializer-0.1/tests/test_variables.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.120267 drvaroz_scoi_lab3_json_xml_serializer-0.2/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      398 2023-05-10 14:41:42.120267 drvaroz_scoi_lab3_json_xml_serializer-0.2/PKG-INFO
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.116269 drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      398 2023-05-10 14:41:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/PKG-INFO
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      641 2023-05-10 14:41:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        1 2023-05-10 14:41:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       64 2023-05-10 14:41:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/top_level.txt
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.116269 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       26 2023-05-10 14:37:22.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      322 2023-05-08 08:54:46.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/factory.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.116269 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 14:49:50.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1741 2023-05-08 08:45:06.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/json_parser.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      523 2023-05-08 07:17:50.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/json_serializer.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.116269 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-04 10:05:02.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     1004 2023-05-08 10:34:14.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/constants.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     6682 2023-05-08 10:44:42.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/serializer.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.120267 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-08 07:41:47.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/__init__.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      682 2023-05-09 09:48:58.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_constants.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2332 2023-05-09 09:48:58.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_parser.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      549 2023-05-08 20:08:32.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_serializer.py
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)       38 2023-05-10 14:41:42.120267 drvaroz_scoi_lab3_json_xml_serializer-0.2/setup.cfg
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)      591 2023-05-10 14:41:18.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/setup.py
+drwxrwxr-x   0 vadim_zhur  (1000) vadim_zhur  (1000)        0 2023-05-10 14:41:42.120267 drvaroz_scoi_lab3_json_xml_serializer-0.2/tests/
+-rw-rw-r--   0 vadim_zhur  (1000) vadim_zhur  (1000)     2440 2023-05-09 10:21:43.000000 drvaroz_scoi_lab3_json_xml_serializer-0.2/tests/test_variables.py
```

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/drvaroz_scoi_lab3_json_xml_serializer.egg-info/SOURCES.txt` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/drvaroz_scoi_lab3_json_xml_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/json_parser.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/json_parser.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/json/json_serializer.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/json/json_serializer.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/constants.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/constants.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/source/serializer.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/source/serializer.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_constants.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_constants.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_parser.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/serializers/xml/xml_serializer.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/serializers/xml/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/setup.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="drvaroz_scoi_lab3_json_xml_serializer",
-    version="0.1",
+    version="0.2",
     description="package for python (de)serialization in .json and .xml",
     url="https://github.com/DrVaroZ/SCoL_labs/tree/lab3",
     author="Vadim Zhur",
     author_email="vadim10zhur@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```

### Comparing `drvaroz_scoi_lab3_json_xml_serializer-0.1/tests/test_variables.py` & `drvaroz_scoi_lab3_json_xml_serializer-0.2/tests/test_variables.py`

 * *Files identical despite different names*

