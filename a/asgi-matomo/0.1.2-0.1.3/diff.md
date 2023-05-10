# Comparing `tmp/asgi_matomo-0.1.2.tar.gz` & `tmp/asgi_matomo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.1.2.tar", max compression
+gzip compressed data, was "asgi_matomo-0.1.3.tar", max compression
```

## Comparing `asgi_matomo-0.1.2.tar` & `asgi_matomo-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.2/LICENSE
--rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.2/README.md
--rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.2/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     6396 2023-05-10 07:33:38.644749 asgi_matomo-0.1.2/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      667 2023-05-10 07:36:28.429933 asgi_matomo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.3/README.md
+-rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.3/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     6749 2023-05-10 07:52:06.256706 asgi_matomo-0.1.3/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0      691 2023-05-10 08:00:57.551353 asgi_matomo-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.3/PKG-INFO
```

### Comparing `asgi_matomo-0.1.2/LICENSE` & `asgi_matomo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.2/README.md` & `asgi_matomo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.2/asgi_matomo/middleware.py` & `asgi_matomo-0.1.3/asgi_matomo/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,28 +116,41 @@
 
         if server is None:
             if scope["server"] is None:
                 logger.error("'server' is not set in scope, skip tracking...")
                 await self.app(scope, receive, send)
                 return
             host, port = scope["server"]
-            logger.debug("setting server from scope", extra={"host": host, "port": port})
+            logger.debug(
+                "setting server from scope", extra={"host": host, "port": port}
+            )
             server = f"{host}:{port}" if port else host
 
+        if ", " in server:
+            servers = server.split(", ")
+            logger.debug(
+                "splitting server addresses, using first",
+                extra={"server-orig": server, "servers": servers},
+            )
+            server = servers[0]
+
         path = scope["path"]
         if root_path := scope.get("root_path"):
             logger.debug("using root_path", extra={"root_path": root_path})
             path = f"{root_path}{path}"
 
-        logger.debug("building url", extra={
-            "server": server,
-            "path": path,
-            "user_agent": user_agent,
-            "accept_lang": accept_lang
-        })
+        logger.debug(
+            "building url",
+            extra={
+                "server": server,
+                "path": path,
+                "user_agent": user_agent,
+                "accept_lang": accept_lang,
+            },
+        )
         url = urllib.parse.urlunsplit(
             (
                 "https" if self.assume_https else str(scope["scheme"]),
                 server,
                 path,
                 "",
                 str(scope["query_string"]) if scope.get("query_string") else None,
```

### Comparing `asgi_matomo-0.1.2/pyproject.toml` & `asgi_matomo-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.1.2"
+version = "0.1.3"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asgi_matomo"}]
 
 [tool.poetry.dependencies]
@@ -16,14 +16,15 @@
 pytest = "^7.3.1"
 black = "^23.3.0"
 starlette = "^0.26.1"
 pytest-asyncio = "^0.21.0"
 asgi-lifespan = "^2.1.0"
 mypy = "^1.2.0"
 pytest-cov = "^4.0.0"
+bump2version = "^1.0.1"
 
 [tool.poetry.group.ci.dependencies]
 ruff = "0.0.263"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `asgi_matomo-0.1.2/PKG-INFO` & `asgi_matomo-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

