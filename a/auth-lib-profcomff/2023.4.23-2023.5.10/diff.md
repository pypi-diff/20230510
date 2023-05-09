# Comparing `tmp/auth_lib_profcomff-2023.4.23.tar.gz` & `tmp/auth_lib_profcomff-2023.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.4.23.tar", last modified: Sun Apr 23 12:30:17 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.5.10.tar", last modified: Tue May  9 23:27:50 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.4.23.tar` & `auth_lib_profcomff-2023.5.10.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:27:50.053726 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 23:27:50.000000 auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:27:50.057726 auth_lib_profcomff-2023.5.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 23:27:38.000000 auth_lib_profcomff-2023.5.10/setup.py
```

### Comparing `auth_lib_profcomff-2023.4.23/LICENSE` & `auth_lib_profcomff-2023.5.10/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.23/PKG-INFO` & `auth_lib_profcomff-2023.5.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2023.4.23
+Version: 2023.5.10
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.4.23/README.md` & `auth_lib_profcomff-2023.5.10/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.23/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.5.10/auth_lib/aiomethods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
+from urllib.parse import urljoin
 
 import aiohttp
 
-from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
+from .exceptions import AuthFailed, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AsyncAuthLib:
     url: str
 
@@ -19,38 +20,31 @@
             response = await session.post(url=f"{self.url}/email/login", json=json)
         match response.status:
             case 200:
                 return await response.json()
             case 401:
                 raise AuthFailed(response=await response.json())
 
-    async def check_token(self, token: str) -> dict[str, Any]:
+    async def check_token(self, token: str) -> dict[str, Any] | None:
         headers = {"Authorization": token}
-        async with aiohttp.ClientSession() as session:
-            response = await session.get(
-                url=f"{self.url}/me",
-                headers=headers,
-                params={
-                    "info": [
-                        "groups",
-                        "indirect_groups",
-                        "session_scopes",
-                        "user_scopes",
-                    ]
-                },
-            )
-        match response.status:
-            case 200:
-                return await response.json()
-            case 400:
-                raise IncorrectData(response=await response.json())
-            case 404:
-                raise NotFound(response=await response.json())
-            case 403:
-                raise SessionExpired(response=await response.json())
+        async with aiohttp.request(
+            "GET",
+            urljoin(self.url, "me"),
+            headers={"Authorization": token},
+            params={
+                "info": [
+                    "indirect_groups",
+                    "session_scopes",
+                ]
+            },
+        ) as r:
+            user_session = await r.json()
+        if r.ok:
+            return user_session
+        return None
 
     async def logout(self, token: str) -> bool:
         headers = {"Authorization": token}
         async with aiohttp.ClientSession() as session:
             response = await session.post(url=f"{self.url}/logout", headers=headers)
 
         match response.status:
```

### Comparing `auth_lib_profcomff-2023.4.23/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.5.10/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.23/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.5.10/auth_lib/fastapi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from urllib.parse import urljoin
+from typing import Any
 from warnings import warn
 
-import aiohttp
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.base import SecurityBase
 from pydantic import BaseSettings
 from starlette.requests import Request
 from starlette.status import HTTP_403_FORBIDDEN
+from starlette.websockets import WebSocket
+
+from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     AUTH_AUTO_ERROR: bool = True
     AUTH_ALLOW_NONE: bool = False
 
@@ -53,37 +55,31 @@
 
     def _except(self):
         if self.auto_error:
             raise HTTPException(
                 status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
             )
         else:
-            return {}
+            return None
 
-    async def __call__(
-        self,
-        request: Request,
-    ) -> dict[str, str] | None:
-        token = request.headers.get("Authorization")
+    async def _get_session(self, token: str | None) -> dict[str, Any] | None:
         if not token and self.allow_none:
             return None
         if not token:
             return self._except()
-        async with aiohttp.request(
-            "GET",
-            urljoin(self.auth_url, "me"),
-            headers={"Authorization": token},
-            params={
-                "info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]
-            },
-        ) as r:
-            status_code = r.status
-            user_session = await r.json()
-        if status_code != 200:
-            self._except()
+        return await AsyncAuthLib(url=self.auth_url).check_token(token)
+
+    async def __call__(
+        self,
+        request: Request | WebSocket,
+    ) -> dict[str, Any] | None:
+        token = request.headers.get("Authorization")
+        user_session = await self._get_session(token)
+        if user_session is None:
+            return self._except()
         session_scopes = set(
             [scope["name"].lower() for scope in user_session["session_scopes"]]
         )
         required_scopes = set([scope.lower() for scope in self.scopes])
         if required_scopes - session_scopes:
             self._except()
         return user_session
```

### Comparing `auth_lib_profcomff-2023.4.23/auth_lib/methods.py` & `auth_lib_profcomff-2023.5.10/auth_lib/methods.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
+from urllib.parse import urljoin
 
 import requests
 
-from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
+from .exceptions import AuthFailed, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AuthLib:
     url: str
 
@@ -18,32 +19,29 @@
         response = requests.post(url=f"{self.url}/email/login", json=json)
         match response.status_code:
             case 200:
                 return response.json()
             case 401:
                 raise AuthFailed(response=response.json()["body"])
 
-    def check_token(self, token: str) -> dict[str, Any]:
+    def check_token(self, token: str) -> dict[str, Any] | None:
         headers = {"Authorization": token}
         response = requests.get(
-            url=f"{self.url}/me",
+            url=urljoin(self.url, "me"),
             headers=headers,
             params={
-                "info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]
+                "info": [
+                    "indirect_groups",
+                    "session_scopes",
+                ]
             },
         )
-        match response.status_code:
-            case 200:
-                return response.json()
-            case 400:
-                raise IncorrectData(response=response.json()["body"])
-            case 404:
-                raise NotFound(response=response.json()["body"])
-            case 403:
-                raise SessionExpired(response=response.json()["body"])
+        if response.ok:
+            return response.json()
+        return None
 
     def logout(self, token: str) -> bool:
         headers = {"Authorization": token}
         response = requests.post(url=f"{self.url}/logout", headers=headers)
 
         match response.status_code:
             case 200:
```

### Comparing `auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.5.10/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.4.23
+Version: 2023.5.10
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.4.23/setup.py` & `auth_lib_profcomff-2023.5.10/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.04.23",
+    version="2023.05.10",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
```

