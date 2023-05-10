# Comparing `tmp/fastapi_async_langchain-0.4.3.tar.gz` & `tmp/fastapi_async_langchain-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.4.3.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.4.4.tar", max compression
```

## Comparing `fastapi_async_langchain-0.4.3.tar` & `fastapi_async_langchain-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-04 17:03:13.497625 fastapi_async_langchain-0.4.3/LICENSE
--rw-r--r--   0        0        0     1818 2023-05-04 17:03:13.497625 fastapi_async_langchain-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      502 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      934 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/base.py
--rw-r--r--   0        0        0      773 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/llm.py
--rw-r--r--   0        0        0     1964 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      171 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/__init__.py
--rw-r--r--   0        0        0     2605 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/base.py
--rw-r--r--   0        0        0      727 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/llm.py
--rw-r--r--   0        0        0      782 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/retrieval_qa.py
--rw-r--r--   0        0        0      536 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/schemas.py
--rw-r--r--   0        0        0       69 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/testing/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/testing/settings.py
--rw-r--r--   0        0        0      281 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/__init__.py
--rw-r--r--   0        0        0     2907 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/base.py
--rw-r--r--   0        0        0      928 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/llm.py
--rw-r--r--   0        0        0      985 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/retrieval_qa.py
--rw-r--r--   0        0        0      481 2023-05-04 17:03:13.701623 fastapi_async_langchain-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-10 20:30:39.676183 fastapi_async_langchain-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1818 2023-05-10 20:30:39.676183 fastapi_async_langchain-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/base.py
+-rw-r--r--   0        0        0      773 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/llm.py
+-rw-r--r--   0        0        0     1964 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      309 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     2605 2023-05-10 20:30:39.892185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0      819 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/conversational_retrieval.py
+-rw-r--r--   0        0        0      727 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0      782 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      536 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/testing/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/testing/settings.py
+-rw-r--r--   0        0        0      412 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/__init__.py
+-rw-r--r--   0        0        0     2907 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/base.py
+-rw-r--r--   0        0        0      928 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/llm.py
+-rw-r--r--   0        0        0      985 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/retrieval_qa.py
+-rw-r--r--   0        0        0      558 2023-05-10 20:30:39.896185 fastapi_async_langchain-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.4.4/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.4.3/LICENSE` & `fastapi_async_langchain-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/README.md` & `fastapi_async_langchain-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/base.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/llm.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/callbacks/retrieval_qa.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/base.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/llm.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/llm.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/responses/retrieval_qa.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/responses/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/schemas.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/testing/gradio.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/base.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/llm.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/llm.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/fastapi_async_langchain/websockets/retrieval_qa.py` & `fastapi_async_langchain-0.4.4/fastapi_async_langchain/websockets/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.4.3/PKG-INFO` & `fastapi_async_langchain-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.4.3
+Version: 0.4.4
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: langchain (>=0.0.157,<0.0.158)
+Requires-Dist: langchain (>=0.0.164,<0.0.165)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: urllib3 (<=1.26.15)
 Description-Content-Type: text/markdown
 
 # fastapi-async-langchain
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/fastapi-async-langchain/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/fastapi-async-langchain.svg)](https://pypi.org/project/fastapi-async-langchain/)
```

