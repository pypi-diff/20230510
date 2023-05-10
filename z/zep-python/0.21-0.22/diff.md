# Comparing `tmp/zep_python-0.21.tar.gz` & `tmp/zep_python-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.21.tar", max compression
+gzip compressed data, was "zep_python-0.22.tar", max compression
```

## Comparing `zep_python-0.21.tar` & `zep_python-0.22.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-05-10 03:55:56.053819 zep_python-0.21/LICENSE
--rw-r--r--   0        0        0    10560 2023-05-10 03:55:56.053819 zep_python-0.21/README.md
--rw-r--r--   0        0        0      621 2023-05-10 03:55:56.053819 zep_python-0.21/pyproject.toml
--rw-r--r--   0        0        0      282 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/exceptions.py
--rw-r--r--   0        0        0     6823 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/models.py
--rw-r--r--   0        0        0      670 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/utils.py
--rw-r--r--   0        0        0    10971 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/zep_client.py
--rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 zep_python-0.21/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 04:23:10.066776 zep_python-0.22/LICENSE
+-rw-r--r--   0        0        0    10560 2023-05-10 04:23:10.066776 zep_python-0.22/README.md
+-rw-r--r--   0        0        0      621 2023-05-10 04:23:10.066776 zep_python-0.22/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/exceptions.py
+-rw-r--r--   0        0        0     6823 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/py.typed
+-rw-r--r--   0        0        0      670 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/utils.py
+-rw-r--r--   0        0        0    10971 2023-05-10 04:23:10.066776 zep_python-0.22/zep_python/zep_client.py
+-rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 zep_python-0.22/PKG-INFO
```

### Comparing `zep_python-0.21/LICENSE` & `zep_python-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/README.md` & `zep_python-0.22/README.md`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/pyproject.toml` & `zep_python-0.22/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.21"
+version = "0.22"
 description = "Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.21/zep_python/exceptions.py` & `zep_python-0.22/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/zep_python/models.py` & `zep_python-0.22/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/zep_python/utils.py` & `zep_python-0.22/zep_python/utils.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/zep_python/zep_client.py` & `zep_python-0.22/zep_python/zep_client.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.21/PKG-INFO` & `zep_python-0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.21
+Version: 0.22
 Summary: Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

