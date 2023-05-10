# Comparing `tmp/asgi_matomo-0.1.3.tar.gz` & `tmp/asgi_matomo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.1.3.tar", max compression
+gzip compressed data, was "asgi_matomo-0.1.4.tar", max compression
```

## Comparing `asgi_matomo-0.1.3.tar` & `asgi_matomo-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.3/LICENSE
--rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.3/README.md
--rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.3/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     6749 2023-05-10 07:52:06.256706 asgi_matomo-0.1.3/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      691 2023-05-10 08:00:57.551353 asgi_matomo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.4/README.md
+-rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.4/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     6776 2023-05-10 08:15:11.684805 asgi_matomo-0.1.4/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0      691 2023-05-10 08:15:40.778584 asgi_matomo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.4/PKG-INFO
```

### Comparing `asgi_matomo-0.1.3/LICENSE` & `asgi_matomo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.3/README.md` & `asgi_matomo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.3/asgi_matomo/middleware.py` & `asgi_matomo-0.1.4/asgi_matomo/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,22 +155,22 @@
                 "",
                 str(scope["query_string"]) if scope.get("query_string") else None,
             )
         )
 
         cip = scope["client"][0] if scope["client"] else None
 
-        start_time = time.perf_counter()
+        start_time_ns = time.perf_counter_ns()
 
         try:
             await self.app(scope, receive, send)
         except Exception:
             raise
         finally:
-            end_time = time.perf_counter()
+            end_time_ns = time.perf_counter_ns()
 
             params_that_require_token = {}
 
             if self.access_token:
                 if cip is None:
                     logger.error("'client' is not set in scope")
                 else:
@@ -182,15 +182,15 @@
             tracking_dict = {
                 "idsite": self.idsite,
                 "url": url,
                 "rec": 1,
                 "rand": random.getrandbits(32),
                 "apiv": 1,
                 "ua": user_agent,
-                "gt_ms": end_time - start_time,
+                "gt_ms": (end_time_ns - start_time_ns) / 1000,
                 # "lang": accept_lang,
                 **params_that_require_token,
             }
 
             if accept_lang:
                 tracking_dict["lang"] = accept_lang
```

### Comparing `asgi_matomo-0.1.3/pyproject.toml` & `asgi_matomo-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.1.3"
+version = "0.1.4"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asgi_matomo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `asgi_matomo-0.1.3/PKG-INFO` & `asgi_matomo-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

