# Comparing `tmp/braincube-aws-core-alpha-0.0.23.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.23.tar", last modified: Tue May  9 09:48:46 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.24.tar", last modified: Tue May  9 20:40:18 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.23.tar` & `braincube-aws-core-alpha-0.0.24.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.636150 braincube-aws-core-alpha-0.0.23/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.23/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 09:48:46.636482 braincube-aws-core-alpha-0.0.23/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.23/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.23/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-09 09:48:46.637814 braincube-aws-core-alpha-0.0.23/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.23/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.618811 braincube-aws-core-alpha-0.0.23/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.622977 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-09 09:48:46.000000 braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.623454 braincube-aws-core-alpha-0.0.23/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.626951 braincube-aws-core-alpha-0.0.23/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-08 14:04:48.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-08 13:56:23.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-09 09:28:51.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    30491 2023-05-09 08:33:33.000000 braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.629611 braincube-aws-core-alpha-0.0.23/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-08 13:58:47.000000 braincube-aws-core-alpha-0.0.23/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4178 2023-05-08 17:05:17.000000 braincube-aws-core-alpha-0.0.23/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.633000 braincube-aws-core-alpha-0.0.23/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3736 2023-05-08 16:38:53.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-08 14:02:55.000000 braincube-aws-core-alpha-0.0.23/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 09:48:46.635296 braincube-aws-core-alpha-0.0.23/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-08 14:03:54.000000 braincube-aws-core-alpha-0.0.23/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.822125 braincube-aws-core-alpha-0.0.24/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.24/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 20:40:18.822498 braincube-aws-core-alpha-0.0.24/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.24/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.24/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-09 20:40:18.825766 braincube-aws-core-alpha-0.0.24/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.24/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.803687 braincube-aws-core-alpha-0.0.24/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.808944 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-09 20:40:18.000000 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-09 20:40:18.000000 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-09 20:40:18.000000 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-09 20:40:18.000000 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-09 20:40:18.000000 braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.809377 braincube-aws-core-alpha-0.0.24/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.24/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.813175 braincube-aws-core-alpha-0.0.24/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.24/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-08 14:04:48.000000 braincube-aws-core-alpha-0.0.24/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-08 13:56:23.000000 braincube-aws-core-alpha-0.0.24/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-09 09:28:51.000000 braincube-aws-core-alpha-0.0.24/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    30491 2023-05-09 08:33:33.000000 braincube-aws-core-alpha-0.0.24/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.815855 braincube-aws-core-alpha-0.0.24/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.24/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-08 13:58:47.000000 braincube-aws-core-alpha-0.0.24/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4178 2023-05-08 17:05:17.000000 braincube-aws-core-alpha-0.0.24/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.819184 braincube-aws-core-alpha-0.0.24/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.24/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.24/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3736 2023-05-08 16:38:53.000000 braincube-aws-core-alpha-0.0.24/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-08 14:02:55.000000 braincube-aws-core-alpha-0.0.24/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-09 20:40:18.821341 braincube-aws-core-alpha-0.0.24/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.24/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      608 2023-05-09 18:15:31.000000 braincube-aws-core-alpha-0.0.24/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-08 14:03:54.000000 braincube-aws-core-alpha-0.0.24/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.23/LICENSE` & `braincube-aws-core-alpha-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/PKG-INFO` & `braincube-aws-core-alpha-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.23
+Version: 0.0.24
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.23/README.md` & `braincube-aws-core-alpha-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/setup.cfg` & `braincube-aws-core-alpha-0.0.24/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.23
+version = 0.0.24
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.23
+Version: 0.0.24
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.23/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.24/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.24/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.24/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.24/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.24/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.24/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.24/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.24/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.24/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.24/src/core/utils/convert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import json
+from uuid import UUID
+from enum import Enum
 from dataclasses import asdict, is_dataclass
 from datetime import date, datetime
 
 
 class JSONEncoder(json.JSONEncoder):
     def default(self, o):
+        if isinstance(o, Enum):
+            return o.value
+        if isinstance(o, UUID):
+            return str(o)
         if isinstance(o, (datetime, date)):
             return o.isoformat()
         if is_dataclass(o):
             return asdict(o)
         return super().default(o)
 
 
 def try_str_to_float(text: str) -> any:
     try:
         return float(text)
     except ValueError:
         return text
-
-
-def function_exists(cls, name: str) -> bool:
-    try:
-        return callable(getattr(cls, name))
-    except:
-        return False
```

### Comparing `braincube-aws-core-alpha-0.0.23/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.24/src/core/utils/data.py`

 * *Files identical despite different names*

