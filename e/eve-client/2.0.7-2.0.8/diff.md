# Comparing `tmp/eve_client-2.0.7.tar.gz` & `tmp/eve_client-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eve_client-2.0.7.tar", max compression
+gzip compressed data, was "eve_client-2.0.8.tar", max compression
```

## Comparing `eve_client-2.0.7.tar` & `eve_client-2.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1468 2023-02-13 03:57:40.402408 eve_client-2.0.7/LICENSE.md
--rw-r--r--   0        0        0     6038 2023-01-26 22:55:48.518308 eve_client-2.0.7/README.md
--rw-r--r--   0        0        0        0 2023-01-26 19:08:28.307262 eve_client-2.0.7/eve_client/__init__.py
--rw-r--r--   0        0        0    14670 2023-02-09 20:02:40.933161 eve_client-2.0.7/eve_client/eve.py
--rw-r--r--   0        0        0      632 2022-06-01 02:54:44.000000 eve_client-2.0.7/eve_client/helper.py
--rw-r--r--   0        0        0      772 2023-02-13 03:59:41.680908 eve_client-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     6956 1970-01-01 00:00:00.000000 eve_client-2.0.7/setup.py
--rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 eve_client-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1468 2023-04-18 12:43:35.900999 eve_client-2.0.8/LICENSE.md
+-rw-r--r--   0        0        0     6038 2023-01-26 22:55:48.000000 eve_client-2.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-01-26 19:08:28.000000 eve_client-2.0.8/eve_client/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-10 01:22:55.842200 eve_client-2.0.8/eve_client/__version__.py
+-rw-r--r--   0        0        0    23781 2023-05-02 13:16:15.720415 eve_client-2.0.8/eve_client/eve.py
+-rw-r--r--   0        0        0      632 2022-06-01 02:54:44.000000 eve_client-2.0.8/eve_client/helper.py
+-rw-r--r--   0        0        0      798 2023-05-10 01:22:59.743162 eve_client-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 eve_client-2.0.8/PKG-INFO
```

### Comparing `eve_client-2.0.7/LICENSE.md` & `eve_client-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.7/README.md` & `eve_client-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.7/eve_client/helper.py` & `eve_client-2.0.8/eve_client/helper.py`

 * *Files identical despite different names*

### Comparing `eve_client-2.0.7/pyproject.toml` & `eve_client-2.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eve_client"
-version = "2.0.7"
+version = "2.0.8"
 description = "EVE Client API Library from Exodus Intelligence LLC."
 authors = ["DevTeam <dev@exodusintel.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 packages = [{include = "eve_client"}]
 
 [tool.poetry.dependencies]
@@ -14,14 +14,15 @@
 requests = "^2.26.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.1.3"
+requests-mock = "^1.10.0"
 
 [tool.black]
 line-length = 79
 exclude = '''
 /(
     \.git
   | \.mypy_cache
```

### Comparing `eve_client-2.0.7/PKG-INFO` & `eve_client-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eve-client
-Version: 2.0.7
+Version: 2.0.8
 Summary: EVE Client API Library from Exodus Intelligence LLC.
 License: BSD-3-Clause
 Author: DevTeam
 Author-email: dev@exodusintel.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

