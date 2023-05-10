# Comparing `tmp/zep_python-0.2.tar.gz` & `tmp/zep_python-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.2.tar", max compression
+gzip compressed data, was "zep_python-0.21.tar", max compression
```

## Comparing `zep_python-0.2.tar` & `zep_python-0.21.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-10 02:08:40.024333 zep_python-0.2/LICENSE
--rw-r--r--   0        0        0    10553 2023-05-10 02:08:40.024333 zep_python-0.2/README.md
--rw-r--r--   0        0        0      620 2023-05-10 02:08:40.024333 zep_python-0.2/pyproject.toml
--rw-r--r--   0        0        0      282 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/exceptions.py
--rw-r--r--   0        0        0     6823 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/models.py
--rw-r--r--   0        0        0      670 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/utils.py
--rw-r--r--   0        0        0    10971 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/zep_client.py
--rw-r--r--   0        0        0    11180 1970-01-01 00:00:00.000000 zep_python-0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 03:55:56.053819 zep_python-0.21/LICENSE
+-rw-r--r--   0        0        0    10560 2023-05-10 03:55:56.053819 zep_python-0.21/README.md
+-rw-r--r--   0        0        0      621 2023-05-10 03:55:56.053819 zep_python-0.21/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/exceptions.py
+-rw-r--r--   0        0        0     6823 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/models.py
+-rw-r--r--   0        0        0      670 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/utils.py
+-rw-r--r--   0        0        0    10971 2023-05-10 03:55:56.053819 zep_python-0.21/zep_python/zep_client.py
+-rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 zep_python-0.21/PKG-INFO
```

### Comparing `zep_python-0.2/LICENSE` & `zep_python-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.2/README.md` & `zep_python-0.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ## Quick Start
 
 Ensure that you have a Zep server running. See https://github.com/getzep/zep.
 
 ```python
 import asyncio
 
-from zep import Memory, Message, SearchPayload, ZepClient
+from zep_python import Memory, Message, SearchPayload, ZepClient
 
 base_url = "http://localhost:8000"  # TODO: Replace with Zep API URL
 session_id = "2a2a2a" # an identifier for your user's session.
 
 async with ZepClient(base_url) as client:
 
     role = "user"
```

### Comparing `zep_python-0.2/pyproject.toml` & `zep_python-0.21/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.2"
+version = "0.21"
 description = "Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.24.1"
+httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.265"
 mypy = "^1.2.0"
 pre-commit = "^3.3.1"
 sphinxawesome-theme = "^4.0.3"
```

### Comparing `zep_python-0.2/zep_python/exceptions.py` & `zep_python-0.21/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.2/zep_python/models.py` & `zep_python-0.21/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.2/zep_python/utils.py` & `zep_python-0.21/zep_python/utils.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.2/zep_python/zep_client.py` & `zep_python-0.21/zep_python/zep_client.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.2/PKG-INFO` & `zep_python-0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.2
+Version: 0.21
 Summary: Zep stores, manages, enriches, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
 [![Release to PyPI](https://github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://github.com/getzep/zep-python/actions/workflows/release.yml)
 
 # Zep: A long-term memory store for conversational AI applications
 
 This is the Python client package for the Zep service. For more information about Zep, see https://github.com/getzep/zep.
@@ -34,15 +34,15 @@
 ## Quick Start
 
 Ensure that you have a Zep server running. See https://github.com/getzep/zep.
 
 ```python
 import asyncio
 
-from zep import Memory, Message, SearchPayload, ZepClient
+from zep_python import Memory, Message, SearchPayload, ZepClient
 
 base_url = "http://localhost:8000"  # TODO: Replace with Zep API URL
 session_id = "2a2a2a" # an identifier for your user's session.
 
 async with ZepClient(base_url) as client:
 
     role = "user"
```

