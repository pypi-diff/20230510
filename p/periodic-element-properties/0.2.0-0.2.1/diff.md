# Comparing `tmp/periodic_element_properties-0.2.0.tar.gz` & `tmp/periodic_element_properties-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodic_element_properties-0.2.0.tar", max compression
+gzip compressed data, was "periodic_element_properties-0.2.1.tar", max compression
```

## Comparing `periodic_element_properties-0.2.0.tar` & `periodic_element_properties-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       83 2023-05-08 16:20:27.230424 periodic_element_properties-0.2.0/periodic_element_properties/__init__.py
--rw-r--r--   0        0        0     2927 2023-05-08 16:20:18.804444 periodic_element_properties-0.2.0/periodic_element_properties/elements.py
--rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.2.0/periodic_element_properties/properties_of_elements.json
--rw-r--r--   0        0        0      505 2023-05-08 16:21:04.860716 periodic_element_properties-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      957 2023-05-08 16:28:00.597231 periodic_element_properties-0.2.0/README.md
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 periodic_element_properties-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-05-10 16:15:13.323443 periodic_element_properties-0.2.1/periodic_element_properties/__init__.py
+-rw-r--r--   0        0        0     2927 2023-05-08 16:20:18.804444 periodic_element_properties-0.2.1/periodic_element_properties/elements.py
+-rw-r--r--   0        0        0    64278 2023-05-08 06:51:13.870866 periodic_element_properties-0.2.1/periodic_element_properties/properties_of_elements.json
+-rw-r--r--   0        0        0      505 2023-05-10 16:15:38.933833 periodic_element_properties-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      957 2023-05-08 16:28:00.597231 periodic_element_properties-0.2.1/README.md
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 periodic_element_properties-0.2.1/PKG-INFO
```

### Comparing `periodic_element_properties-0.2.0/periodic_element_properties/elements.py` & `periodic_element_properties-0.2.1/periodic_element_properties/elements.py`

 * *Files identical despite different names*

### Comparing `periodic_element_properties-0.2.0/periodic_element_properties/properties_of_elements.json` & `periodic_element_properties-0.2.1/periodic_element_properties/properties_of_elements.json`

 * *Files identical despite different names*

### Comparing `periodic_element_properties-0.2.0/README.md` & `periodic_element_properties-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `periodic_element_properties-0.2.0/PKG-INFO` & `periodic_element_properties-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodic-element-properties
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package contains information about periodic elements and their properties
 Author: Prithivee7
 Author-email: getprithivee@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

