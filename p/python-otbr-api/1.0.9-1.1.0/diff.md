# Comparing `tmp/python-otbr-api-1.0.9.tar.gz` & `tmp/python-otbr-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-1.0.9.tar", last modified: Mon Mar 13 14:07:31 2023, max compression
+gzip compressed data, was "python-otbr-api-1.1.0.tar", last modified: Wed May 10 18:04:51 2023, max compression
```

## Comparing `python-otbr-api-1.0.9.tar` & `python-otbr-api-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:07:31.609941 python-otbr-api-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-13 14:07:31.609941 python-otbr-api-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:07:31.605940 python-otbr-api-1.0.9/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-13 14:07:11.000000 python-otbr-api-1.0.9/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:07:31.609941 python-otbr-api-1.0.9/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 14:07:31.000000 python-otbr-api-1.0.9/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-13 14:07:31.609941 python-otbr-api-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 18:04:30.000000 python-otbr-api-1.1.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:04:51.000000 python-otbr-api-1.1.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 18:04:51.804274 python-otbr-api-1.1.0/setup.cfg
```

### Comparing `python-otbr-api-1.0.9/LICENSE` & `python-otbr-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.0.9/pyproject.toml` & `python-otbr-api-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "1.0.9"
+version      = "1.1.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-1.0.9/python_otbr_api/mdns.py` & `python-otbr-api-1.1.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.0.9/python_otbr_api/models.py` & `python-otbr-api-1.1.0/python_otbr_api/models.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.0.9/python_otbr_api/pskc.py` & `python-otbr-api-1.1.0/python_otbr_api/pskc.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.0.9/python_otbr_api/tlv_parser.py` & `python-otbr-api-1.1.0/python_otbr_api/tlv_parser.py`

 * *Files identical despite different names*

