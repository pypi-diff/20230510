# Comparing `tmp/fronius_solarweb-0.2.0.tar.gz` & `tmp/fronius_solarweb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fronius_solarweb-0.2.0.tar", max compression
+gzip compressed data, was "fronius_solarweb-0.2.1.tar", max compression
```

## Comparing `fronius_solarweb-0.2.0.tar` & `fronius_solarweb-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/LICENSE
--rw-r--r--   0        0        0      816 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/README.md
--rw-r--r--   0        0        0       34 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/__init__.py
--rw-r--r--   0        0        0     6032 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/api.py
--rw-r--r--   0        0        0      899 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/errors.py
--rw-r--r--   0        0        0        0 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/schema/__init__.py
--rw-r--r--   0        0        0     1774 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/schema/device.py
--rw-r--r--   0        0        0      136 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/schema/error.py
--rw-r--r--   0        0        0     1412 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/schema/pvsystem.py
--rw-r--r--   0        0        0      157 2023-02-17 02:58:00.318113 fronius_solarweb-0.2.0/fronius_solarweb/schema/service.py
--rw-r--r--   0        0        0      707 2023-02-17 02:58:09.738206 fronius_solarweb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 fronius_solarweb-0.2.0/setup.py
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 fronius_solarweb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/LICENSE
+-rw-r--r--   0        0        0      816 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/README.md
+-rw-r--r--   0        0        0       34 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/__init__.py
+-rw-r--r--   0        0        0     6032 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/api.py
+-rw-r--r--   0        0        0      899 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/errors.py
+-rw-r--r--   0        0        0        0 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/schema/__init__.py
+-rw-r--r--   0        0        0     1774 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/schema/device.py
+-rw-r--r--   0        0        0      136 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/schema/error.py
+-rw-r--r--   0        0        0     1412 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/schema/pvsystem.py
+-rw-r--r--   0        0        0      157 2023-05-10 19:27:02.334425 fronius_solarweb-0.2.1/fronius_solarweb/schema/service.py
+-rw-r--r--   0        0        0      716 2023-05-10 19:27:16.455255 fronius_solarweb-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 fronius_solarweb-0.2.1/PKG-INFO
```

### Comparing `fronius_solarweb-0.2.0/LICENSE` & `fronius_solarweb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/README.md` & `fronius_solarweb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/fronius_solarweb/api.py` & `fronius_solarweb-0.2.1/fronius_solarweb/api.py`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/fronius_solarweb/errors.py` & `fronius_solarweb-0.2.1/fronius_solarweb/errors.py`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/fronius_solarweb/schema/device.py` & `fronius_solarweb-0.2.1/fronius_solarweb/schema/device.py`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/fronius_solarweb/schema/pvsystem.py` & `fronius_solarweb-0.2.1/fronius_solarweb/schema/pvsystem.py`

 * *Files identical despite different names*

### Comparing `fronius_solarweb-0.2.0/pyproject.toml` & `fronius_solarweb-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "fronius_solarweb"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python wrapper for the Fronius Solar.web Cloud API"
 authors = ["Derek Caudwell <derek_caudwell@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/drc38/python-fronius-web"
 license = "MIT"
 
 [tool.poetry.urls]
 issues = "https://github.com/drc38/python-fronius-web/issues"
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
-httpx = "^0.23"
+python = ">=3.10"
+httpx = ">=0.23,<0.25"
 pydantic = "^1.10"
 tenacity = "^8.1"
 
 
 [tool.poetry.dev-dependencies]
 black = "^23.1"
 isort = "^5.10.1"
@@ -26,8 +26,8 @@
 pre-commit = "^3.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
-profile = "black"
+profile = "black"
```

### Comparing `fronius_solarweb-0.2.0/PKG-INFO` & `fronius_solarweb-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fronius-solarweb
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python wrapper for the Fronius Solar.web Cloud API
 Home-page: https://github.com/drc38/python-fronius-web
 License: MIT
 Author: Derek Caudwell
 Author-email: derek_caudwell@hotmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: tenacity (>=8.1,<9.0)
 Project-URL: Repository, https://github.com/drc38/python-fronius-web
 Project-URL: issues, https://github.com/drc38/python-fronius-web/issues
 Description-Content-Type: text/markdown
 
 # Fronius Solar.web
```

