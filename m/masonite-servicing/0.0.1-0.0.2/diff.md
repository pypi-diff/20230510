# Comparing `tmp/masonite-servicing-0.0.1.tar.gz` & `tmp/masonite-servicing-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masonite-servicing-0.0.1.tar", last modified: Tue May  9 09:00:16 2023, max compression
+gzip compressed data, was "masonite-servicing-0.0.2.tar", last modified: Wed May 10 09:04:08 2023, max compression
```

## Comparing `masonite-servicing-0.0.1.tar` & `masonite-servicing-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.1/LICENSE
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.1/MANIFEST.in
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4423 2023-05-09 08:15:50.000000 masonite-servicing-0.0.1/README.md
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.1/pyproject.toml
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/setup.cfg
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3616 2023-05-09 09:00:15.000000 masonite-servicing-0.0.1/setup.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.870821 masonite-servicing-0.0.1/src/
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.870821 masonite-servicing-0.0.1/src/masonite_servicing/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      674 2023-05-09 08:41:24.000000 masonite-servicing-0.0.1/src/masonite_servicing/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/src/masonite_servicing/config/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.1/src/masonite_servicing/config/masonite_servicing.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/src/masonite_servicing/providers/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.1/src/masonite_servicing/providers/ServicingProvider.py
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.1/src/masonite_servicing/providers/__init__.py
-drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 09:00:16.874821 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-09 09:00:16.000000 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/PKG-INFO
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      478 2023-05-09 09:00:16.000000 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/SOURCES.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-09 09:00:16.000000 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/dependency_links.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-09 09:00:16.000000 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/requires.txt
--rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-09 09:00:16.000000 masonite-servicing-0.0.1/src/masonite_servicing.egg-info/top_level.txt
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.265030 masonite-servicing-0.0.2/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     1066 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/LICENSE
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/MANIFEST.in
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-10 09:04:08.269030 masonite-servicing-0.0.2/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     4423 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/README.md
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      289 2023-05-09 08:15:50.000000 masonite-servicing-0.0.2/pyproject.toml
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      232 2023-05-10 09:04:08.269030 masonite-servicing-0.0.2/setup.cfg
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     3616 2023-05-10 09:04:04.000000 masonite-servicing-0.0.2/setup.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.245030 masonite-servicing-0.0.2/src/
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.245030 masonite-servicing-0.0.2/src/masonite_servicing/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      686 2023-05-10 09:03:21.000000 masonite-servicing-0.0.2/src/masonite_servicing/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.249030 masonite-servicing-0.0.2/src/masonite_servicing/config/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      282 2023-05-09 08:15:49.000000 masonite-servicing-0.0.2/src/masonite_servicing/config/masonite_servicing.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.265030 masonite-servicing-0.0.2/src/masonite_servicing/providers/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      520 2023-05-09 08:17:14.000000 masonite-servicing-0.0.2/src/masonite_servicing/providers/ServicingProvider.py
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       69 2023-05-09 08:15:49.000000 masonite-servicing-0.0.2/src/masonite_servicing/providers/__init__.py
+drwxrwxr-x   0 lvjhn     (1000) lvjhn     (1000)        0 2023-05-10 09:04:08.249030 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)     5644 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/PKG-INFO
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)      478 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)        1 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       80 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/requires.txt
+-rw-rw-r--   0 lvjhn     (1000) lvjhn     (1000)       19 2023-05-10 09:04:08.000000 masonite-servicing-0.0.2/src/masonite_servicing.egg-info/top_level.txt
```

### Comparing `masonite-servicing-0.0.1/LICENSE` & `masonite-servicing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.1/PKG-INFO` & `masonite-servicing-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-servicing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package description in one line displayed e.g. in README
 Home-page: https://github.com/lvjhn/masonite-servicing
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-servicing Version: 0.0.1 Summary: Package
+Metadata-Version: 2.1 Name: masonite-servicing Version: 0.0.2 Summary: Package
 description in one line displayed e.g. in README Home-page: https://github.com/
 lvjhn/masonite-servicing Author: LJ S.A. Author-email: lvjhn.mx@gmail.com
 License: MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

### Comparing `masonite-servicing-0.0.1/README.md` & `masonite-servicing-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.1/setup.py` & `masonite-servicing-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="masonite-servicing",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.1",
+    version="0.0.2",
     packages=[
         "masonite_servicing",
         "masonite_servicing.providers",
         "masonite_servicing.config",
     ],
     package_dir={"": "src"},
     description="Package description in one line displayed e.g. in README",
```

### Comparing `masonite-servicing-0.0.1/src/masonite_servicing/__init__.py` & `masonite-servicing-0.0.2/src/masonite_servicing/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         "message" : result.message, 
         "data" : result.data
     }
 
 def relay(result):
     return result[1]
 
-def fetch(cb): 
-    return cb()[1].data
+def fetch(cb, *args): 
+    return cb(*args)[1].data
 
 class SampleService:
     def add(self, x, y): 
         return result("ok", "added", x + y) 
     
 def main():
     sample_service = SampleService()
```

### Comparing `masonite-servicing-0.0.1/src/masonite_servicing/providers/ServicingProvider.py` & `masonite-servicing-0.0.2/src/masonite_servicing/providers/ServicingProvider.py`

 * *Files identical despite different names*

### Comparing `masonite-servicing-0.0.1/src/masonite_servicing.egg-info/PKG-INFO` & `masonite-servicing-0.0.2/src/masonite_servicing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masonite-servicing
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package description in one line displayed e.g. in README
 Home-page: https://github.com/lvjhn/masonite-servicing
 Author: LJ S.A.
 Author-email: lvjhn.mx@gmail.com
 License: MIT license
 Keywords: Masonite,Python,Development
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: masonite-servicing Version: 0.0.1 Summary: Package
+Metadata-Version: 2.1 Name: masonite-servicing Version: 0.0.2 Summary: Package
 description in one line displayed e.g. in README Home-page: https://github.com/
 lvjhn/masonite-servicing Author: LJ S.A. Author-email: lvjhn.mx@gmail.com
 License: MIT license Keywords: Masonite,Python,Development Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 Environment :: Web Environment Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

