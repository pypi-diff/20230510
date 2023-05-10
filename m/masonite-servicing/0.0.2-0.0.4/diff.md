# Comparing `tmp/masonite-servicing-0.0.2.tar.gz` & `tmp/masonite-servicing-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-servicing-0.0.2.tar", last modified: Wed May 10 09:04:08 2023, max compression
+gzip compressed data, was "masonite-servicing-0.0.4.tar", last modified: Wed May 10 11:49:55 2023, max compression
```

## Comparing `masonite-servicing-0.0.2.tar` & `masonite-servicing-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.265030 masonite-servicing-0.0.2/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-10 09:04:08.269030 masonite-servicing-0.0.2/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4423 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-10 09:04:08.269030 masonite-servicing-0.0.2/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3616 2023-05-10 09:04:04.000000 masonite-servicing-0.0.2/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.245030 masonite-servicing-0.0.2/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.245030 masonite-servicing-0.0.2/src/masonite_servicing/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      686 2023-05-10 09:03:21.000000 masonite-servicing-0.0.2/src/masonite_servicing/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.249030 masonite-servicing-0.0.2/src/masonite_servicing/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.2/src/masonite_servicing/config/masonite_servicing.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.265030 masonite-servicing-0.0.2/src/masonite_servicing/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.2/src/masonite_servicing/providers/ServicingProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.2/src/masonite_servicing/providers/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.249030 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      478 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.4/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.4/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      360 2023-05-10 10:46:59.000000 masonite-servicing-0.0.4/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.4/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3651 2023-05-10 11:49:53.000000 masonite-servicing-0.0.4/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.543701 masonite-servicing-0.0.4/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/src/masonite_servicing/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      950 2023-05-10 11:46:03.000000 masonite-servicing-0.0.4/src/masonite_servicing/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/src/masonite_servicing/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.4/src/masonite_servicing/config/servicing.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/src/masonite_servicing/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.4/src/masonite_servicing/providers/ServicingProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.4/src/masonite_servicing/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 11:49:55.547701 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1616 2023-05-10 11:49:55.000000 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      469 2023-05-10 11:49:55.000000 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-10 11:49:55.000000 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-10 11:49:55.000000 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-10 11:49:55.000000 masonite-servicing-0.0.4/src/masonite_servicing.egg-info/top_level.txt
```

### Comparing `masonite-servicing-0.0.2/LICENSE` & `masonite-servicing-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.2/setup.py` & `masonite-servicing-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     long_description = fh.read()
 
 setup(
     name="masonite-servicing",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.2",
+    version="0.0.4",
     packages=[
         "masonite_servicing",
         "masonite_servicing.providers",
         "masonite_servicing.config",
     ],
     package_dir={"": "src"},
-    description="Package description in one line displayed e.g. in README",
+    description="A simple and small utility library that aids in constructing service feature in Masonite 4.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/lvjhn/masonite-servicing",
     # Author details
     author="LJ S.A.",
     author_email="lvjhn.mx@gmail.com",
```

### Comparing `masonite-servicing-0.0.2/src/masonite_servicing/__init__.py` & `masonite-servicing-0.0.4/src/masonite_servicing/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # flake8: noqa F401
 from .providers.ServicingProvider import ServicingProvider
+from masonite.validation import Validator
 
 class ServiceResult:
     def __init__(self, *args): 
         self.status = args[0]
         self.message = args[1]
         self.data = args[2]
 
 def result(*args):
    return ServiceResult(*args)
 
+def respond(request, validators, result):
+    errors = request.validate(*validators)
+
+    if errors: 
+        return {
+            "status"  : "not-ok", 
+            "message" : "VALIDATION_ERROR", 
+            "errors"  : errors.all()
+        }
 
-def respond(result):
     return {
         "status" : result.status, 
         "message" : result.message, 
         "data" : result.data
     }
 
 def relay(result):
     return result[1]
 
 def fetch(cb, *args): 
-    return cb(*args)[1].data
+    return cb(*args).data
 
 class SampleService:
     def add(self, x, y): 
         return result("ok", "added", x + y) 
     
 def main():
     sample_service = SampleService()
```

### Comparing `masonite-servicing-0.0.2/src/masonite_servicing/providers/ServicingProvider.py` & `masonite-servicing-0.0.4/src/masonite_servicing/providers/ServicingProvider.py`

 * *Files identical despite different names*

