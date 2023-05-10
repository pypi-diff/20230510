# Comparing `tmp/exaroton-0.0.4.tar.gz` & `tmp/exaroton-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exaroton-0.0.4.tar", max compression
+gzip compressed data, was "exaroton-0.0.5.tar", max compression
```

## Comparing `exaroton-0.0.4.tar` & `exaroton-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      101 2023-03-01 14:10:48.209243 exaroton-0.0.4/exaroton/__init__.py
--rw-r--r--   0        0        0     8431 2023-03-01 15:30:58.400615 exaroton-0.0.4/exaroton/exaroton.py
--rw-r--r--   0        0        0     3019 2023-03-01 14:10:48.209743 exaroton-0.0.4/exaroton/types.py
--rw-r--r--   0        0        0     1089 2023-03-01 14:10:48.208243 exaroton-0.0.4/LICENSE
--rw-r--r--   0        0        0      979 2023-03-01 15:32:28.803266 exaroton-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2731 2023-03-01 14:10:48.208743 exaroton-0.0.4/README.md
--rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 exaroton-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      101 2023-05-10 11:59:45.350220 exaroton-0.0.5/exaroton/__init__.py
+-rw-r--r--   0        0        0     8671 2023-05-10 11:58:57.972318 exaroton-0.0.5/exaroton/exaroton.py
+-rw-r--r--   0        0        0     3019 2023-03-01 14:10:48.209743 exaroton-0.0.5/exaroton/types.py
+-rw-r--r--   0        0        0     1089 2023-03-01 14:10:48.208243 exaroton-0.0.5/LICENSE
+-rw-r--r--   0        0        0      979 2023-05-10 11:59:39.190238 exaroton-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2731 2023-03-01 14:10:48.208743 exaroton-0.0.5/README.md
+-rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 exaroton-0.0.5/PKG-INFO
```

### Comparing `exaroton-0.0.4/exaroton/exaroton.py` & `exaroton-0.0.5/exaroton/exaroton.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 
         elif content_type == "text/plain;charset=UTF-8":
             return bytes.decode(req.content, "utf8")
 
         elif content_type == "application/octet-stream":
             return req.content
 
+        elif content_type == "image/png":
+            # In case returned data is an image (for example the server-icon.png)
+            # This type isn't actually documentated by the API Docs :thumbsup:
+            return req.content
+
     def get_account(self) -> types.Account:
         """Get information about the authenticated Account
 
         Returns:
             ``types.Account``: Your Account
         """
         _data = self._make_request("account")["data"]
```

### Comparing `exaroton-0.0.4/exaroton/types.py` & `exaroton-0.0.5/exaroton/types.py`

 * *Files identical despite different names*

### Comparing `exaroton-0.0.4/LICENSE` & `exaroton-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exaroton-0.0.4/pyproject.toml` & `exaroton-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exaroton"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python API wrapper for exaroton"
 authors = ["Colin <colin@colinshark.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ColinShark/exaroton"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `exaroton-0.0.4/README.md` & `exaroton-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `exaroton-0.0.4/PKG-INFO` & `exaroton-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exaroton
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python API wrapper for exaroton
 Home-page: https://github.com/ColinShark/exaroton
 License: MIT
 Author: Colin
 Author-email: colin@colinshark.de
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

