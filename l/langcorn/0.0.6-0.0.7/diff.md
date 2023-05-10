# Comparing `tmp/langcorn-0.0.6.tar.gz` & `tmp/langcorn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.6.tar", max compression
+gzip compressed data, was "langcorn-0.0.7.tar", max compression
```

## Comparing `langcorn-0.0.6.tar` & `langcorn-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-04-23 12:09:58.514611 langcorn-0.0.6/LICENSE
--rw-r--r--   0        0        0     4936 2023-04-23 12:09:58.514611 langcorn-0.0.6/Readme.md
--rw-r--r--   0        0        0       77 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/__init__.py
--rw-r--r--   0        0        0      417 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/__init__.py
--rw-r--r--   0        0        0     3156 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/api.py
--rw-r--r--   0        0        0      825 2023-04-23 12:09:58.514611 langcorn-0.0.6/langcorn/server/test_api.py
--rw-r--r--   0        0        0      944 2023-04-23 12:09:58.514611 langcorn-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 langcorn-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-10 16:00:05.898921 langcorn-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7377 2023-05-10 16:00:05.898921 langcorn-0.0.7/Readme.md
+-rw-r--r--   0        0        0       77 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     4447 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/api.py
+-rw-r--r--   0        0        0      999 2023-05-10 16:00:05.898921 langcorn-0.0.7/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      981 2023-05-10 16:00:05.898921 langcorn-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 langcorn-0.0.7/PKG-INFO
```

### Comparing `langcorn-0.0.6/LICENSE` & `langcorn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.6/langcorn/server/api.py` & `langcorn-0.0.7/langcorn/server/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import sys
+from typing import Any
 
-from fastapi import Depends, FastAPI, Header, HTTPException
+from fastapi import Depends, FastAPI, Header, HTTPException, Request
 from fastapi.security.utils import get_authorization_scheme_param
+from langchain.schema import messages_from_dict, messages_to_dict
 from loguru import logger
 from pydantic import BaseModel
 from uvicorn.importer import import_from_string
 
 # TODO: improve logging
 logger.remove(0)
 logger.add(
@@ -17,17 +19,28 @@
 )
 
 
 class LangRequest(BaseModel):
     prompt: str
 
 
+class MemoryData(BaseModel):
+    content: str
+    additional_kwargs: dict[str, Any]
+
+
+class Memory(BaseModel):
+    type: str
+    data: MemoryData
+
+
 class LangResponse(BaseModel):
     output: str
     error: str
+    memory: list[Memory]
 
 
 def authenticate_or_401(auth_token):
     if not auth_token:
         # Auth is not enabled.
         def dummy():
             return
@@ -48,48 +61,74 @@
     if hasattr(language_app, "input_variables"):
         return language_app.input_variables, language_app.output_variables
     elif hasattr(language_app, "prompt"):
         return language_app.prompt.input_variables, [language_app.output_key]
     return [language_app.input_key], ["output"]
 
 
-def derive_class(name, fields):
-    return type(
-        f"Lang{name}", (BaseModel,), {"__annotations__": {f: str for f in fields}}
-    )
+def derive_class(name, fields, add_memory=False):
+    annotations = {f: str for f in fields}
+    if add_memory:
+        annotations["memory"] = list[dict]
+    return type(f"Lang{name}", (BaseModel,), {"__annotations__": annotations})
+
+
+def set_openai_key(new_key: str) -> str:
+    if not new_key:
+        return
+    import openai
+
+    prev = openai.api_key
+    openai.api_key = new_key
+    return prev
 
 
 def make_handler(request_cls, chain):
-    async def handler(
-        request: request_cls,
-    ):
-        output = chain.run(request.dict())
-        # add error handling
-        return LangResponse(output=output, error="")
+    async def handler(request: request_cls, http_request: Request):
+        llm_api_key = http_request.headers.get("x-llm-api-key")
+        try:
+            api_key = set_openai_key(llm_api_key)
+            run_params = request.dict()
+            memory = run_params.pop("memory", [])
+            if chain.memory and memory and memory[0]:
+                chain.memory.chat_memory.messages = messages_from_dict(memory)
+            output = chain.run(run_params)
+
+            # add error handling
+            memory = (
+                []
+                if not chain.memory
+                else messages_to_dict(chain.memory.chat_memory.messages)
+            )
+        except Exception as e:
+            raise HTTPException(status_code=500, detail=dict(error=str(e)))
+        finally:
+            set_openai_key(api_key)
+        return LangResponse(output=output, error="", memory=memory)
 
     return handler
 
 
-def create_service(*lc_apps, auth_token: str = ""):
+def create_service(*lc_apps, auth_token: str = "", app: FastAPI = None):
     # Make local modules discoverable
     sys.path.append(os.path.dirname(__file__))
     logger.info("Creating service")
-    app = FastAPI()
+    app = app or FastAPI()
     endpoints = ["/docs"]
 
     _authenticate_or_401 = Depends(authenticate_or_401(auth_token=auth_token))
 
     for lang_app in lc_apps:
         chain = import_from_string(lang_app)
         inn, out = derive_fields(chain)
         logger.debug(f"inputs:{inn=}")
         logger.info(f"{lang_app=}:{chain.__class__.__name__}({inn})")
         endpoint_prefix = lang_app.split(":")[0]
         cls_name = "".join([c.capitalize() for c in endpoint_prefix.split(".")])
-        request_cls = derive_class(cls_name, inn)
+        request_cls = derive_class(cls_name, inn, add_memory=chain.memory)
         logger.debug(f"{request_cls=}")
 
         endpoints.append(f"/{endpoint_prefix}/run")
         # avoid hoisting issues with handler(request)
         app.post(
             f"/{endpoint_prefix}/run",
             response_model=LangResponse,
```

### Comparing `langcorn-0.0.6/langcorn/server/test_api.py` & `langcorn-0.0.7/langcorn/server/test_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import pytest
 from fastapi.testclient import TestClient
 
+from examples import app
+
 from .api import create_service
 
 client = TestClient(create_service("examples.ex1:chain"))
 
+example_app = TestClient(app.app)
+
 
 @pytest.fixture(
     scope="session",
 )
 def fn_executor():
     yield None
 
 
 class TestRoutes:
+    def test_examples(self):
+        response = example_app.get("/")
+        assert response.status_code == 404
+
     def test_read_main(self):
         response = client.get("/")
         assert response.status_code == 404
 
     def test_state(self):
         response = client.get("/ht")
         assert response.status_code == 200
```

### Comparing `langcorn-0.0.6/pyproject.toml` & `langcorn-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
@@ -15,19 +15,20 @@
 
 [tool.poetry.scripts]
 langcorn = "langcorn.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = "^0.95.0"
-uvicorn = "^0.21.1"
-langchain = "^0.0.139"
+uvicorn = "^0.22.0"
+langchain = "^0.0.163"
 openai = "^0.27.2"
 fire = "^0.5.0"
 loguru = "^0.7.0"
+bs4 = "0.0.1"  # required for ex4.py
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 httpx = "^0.23.3"
 pytest = "^7.2.2"
 types-requests = "^2.28.11"
```

### Comparing `langcorn-0.0.6/PKG-INFO` & `langcorn-0.0.7/Readme.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: langcorn
-Version: 0.0.6
-Summary: A Python package creating rest api interface for LangChain
-Home-page: https://github.com/msoedov/langcorn
-License: MIT
-Keywords: nlp,langchain,openai,gpt,fastapi
-Author: Alexander Miasoiedov
-Author-email: msoedov@gmail.com
-Maintainer: Alexander Miasoiedov
-Maintainer-email: msoedov@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: fire (>=0.5.0,<0.6.0)
-Requires-Dist: langchain (>=0.0.139,<0.0.140)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0)
-Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
-Project-URL: Repository, https://github.com/msoedov/langcorn
-Description-Content-Type: text/markdown
-
 # Langcorn
 
 LangCorn is an API server that enables you to serve LangChain models and pipelines with ease, leveraging the power of FastAPI for a robust and efficient experience.
 
 <p>
 <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/msoedov/langcorn" />
 <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/msoedov/langcorn" />
@@ -131,14 +105,31 @@
 
 from fastapi import FastAPI
 from langcorn import create_service
 
 app:FastAPI = create_service("examples.ex2:chain", "examples.ex1:chain")
 ```
 
+or
+
+```python
+from fastapi import FastAPI
+from langcorn import create_service
+
+app: FastAPI = create_service(
+    "examples.ex1:chain",
+    "examples.ex2:chain",
+    "examples.ex3:chain",
+    "examples.ex4:sequential_chain",
+    "examples.ex5:conversation",
+    "examples.ex6:conversation_with_summary",
+)
+
+```
+
 Run your LangCorn FastAPI server:
 
 ```shell
 
 uvicorn main:app --host 0.0.0.0 --port 8000
 ```
 
@@ -147,29 +138,101 @@
 ## Docs
 
 Automatically served FastAPI doc
 [Live example](https://langcorn-ift9ub8zg-msoedov.vercel.app/docs#/) hosted on vercel.
 
 ![](https://res.cloudinary.com/dq0w2rtm9/image/upload/c_pad,b_auto:predominant,fl_preserve_transparency/v1681817836/Screen_Shot_2023-04-18_at_14.36.00_ms2thb.jpg?_s=public-apps)
 
-
 ## Auth
 
 It possible to add a static api token auth by specifying `auth_token`
 
 ```shell
 python langcorn server examples.ex1:chain examples.ex2:chain --auth_token=api-secret-value
 ```
 
 or
 
 ```python
 app:FastAPI = create_service("examples.ex1:chain", auth_token="api-secret-value")
 ```
 
+## Custom API KEYs
+
+```shell
+POST http://0.0.0.0:3000/examples.ex6/run
+X-LLM-API-KEY: sk-******
+Content-Type: application/json
+```
+
+## Handling memory
+
+```json
+{
+  "history": "string",
+  "input": "What is brain?",
+  "memory": [
+    {
+      "type": "human",
+      "data": {
+        "content": "What is memory?",
+        "additional_kwargs": {}
+      }
+    },
+    {
+      "type": "ai",
+      "data": {
+        "content": " Memory is the ability of the brain to store, retain, and recall information. It is the capacity to remember past experiences, facts, and events. It is also the ability to learn and remember new information.",
+        "additional_kwargs": {}
+      }
+    }
+  ]
+}
+
+```
+
+Response:
+
+```json
+{
+  "output": " The brain is an organ in the human body that is responsible for controlling thought, memory, emotion, and behavior. It is composed of billions of neurons that communicate with each other through electrical and chemical signals. It is the most complex organ in the body and is responsible for all of our conscious and unconscious actions.",
+  "error": "",
+  "memory": [
+    {
+      "type": "human",
+      "data": {
+        "content": "What is memory?",
+        "additional_kwargs": {}
+      }
+    },
+    {
+      "type": "ai",
+      "data": {
+        "content": " Memory is the ability of the brain to store, retain, and recall information. It is the capacity to remember past experiences, facts, and events. It is also the ability to learn and remember new information.",
+        "additional_kwargs": {}
+      }
+    },
+    {
+      "type": "human",
+      "data": {
+        "content": "What is brain?",
+        "additional_kwargs": {}
+      }
+    },
+    {
+      "type": "ai",
+      "data": {
+        "content": " The brain is an organ in the human body that is responsible for controlling thought, memory, emotion, and behavior. It is composed of billions of neurons that communicate with each other through electrical and chemical signals. It is the most complex organ in the body and is responsible for all of our conscious and unconscious actions.",
+        "additional_kwargs": {}
+      }
+    }
+  ]
+}
+```
+
 ## Documentation
 
 For more detailed information on how to use LangCorn, including advanced features and customization options, please refer to the official documentation.
 
 ## 👋 Contributing
 
 Contributions to LangCorn are welcome! If you'd like to contribute, please follow these steps:
@@ -181,8 +244,7 @@
 - Open a pull request to the main LangCorn repository
 
 Before contributing, please read the contributing guidelines.
 
 ## License
 
 LangCorn is released under the MIT License.
-
```

