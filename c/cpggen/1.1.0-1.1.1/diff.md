# Comparing `tmp/cpggen-1.1.0.tar.gz` & `tmp/cpggen-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.0.tar", max compression
+gzip compressed data, was "cpggen-1.1.1.tar", max compression
```

## Comparing `cpggen-1.1.0.tar` & `cpggen-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-10 01:06:37.905057 cpggen-1.1.0/LICENSE
--rw-r--r--   0        0        0    11604 2023-05-10 01:06:37.905057 cpggen-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/__init__.py
--rw-r--r--   0        0        0    19518 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/cli.py
--rw-r--r--   0        0        0    37417 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/logger.py
--rw-r--r--   0        0        0    14143 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/utils.py
--rw-r--r--   0        0        0     1326 2023-05-10 01:06:37.909057 cpggen-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12976 1970-01-01 00:00:00.000000 cpggen-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 01:53:37.866433 cpggen-1.1.1/LICENSE
+-rw-r--r--   0        0        0    11604 2023-05-10 01:53:37.866433 cpggen-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 01:53:37.866433 cpggen-1.1.1/cpggen/__init__.py
+-rw-r--r--   0        0        0    19564 2023-05-10 01:53:37.866433 cpggen-1.1.1/cpggen/cli.py
+-rw-r--r--   0        0        0    37417 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/logger.py
+-rw-r--r--   0        0        0    14143 2023-05-10 01:53:37.870433 cpggen-1.1.1/cpggen/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-10 01:53:37.870433 cpggen-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12976 1970-01-01 00:00:00.000000 cpggen-1.1.1/PKG-INFO
```

### Comparing `cpggen-1.1.0/LICENSE` & `cpggen-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.0/README.md` & `cpggen-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.1.0/cpggen/cli.py` & `cpggen-1.1.1/cpggen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,17 +235,19 @@
     if params.get("slice", "") in ("true", "1"):
         slice = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
-    if not url and (src.startswith("http") or src.startswith("git")):
+    if not url and (
+        src.startswith("http") or src.startswith("git://") or src.startswith("pkg:")
+    ):
         url = src
-    if url.startswith("http") or url.startswith("git") or url.startswith("pkg:"):
+    if url.startswith("http") or url.startswith("git://") or url.startswith("pkg:"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
         if src.startswith("pkg:"):
             download_file = utils.download_package(src, clone_dir)
             if download_file and os.path.exists(download_file):
                 src = clone_dir
         else:
             src = utils.clone_repo(url, clone_dir)
```

### Comparing `cpggen-1.1.0/cpggen/executor.py` & `cpggen-1.1.1/cpggen/executor.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.0/cpggen/logger.py` & `cpggen-1.1.1/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.0/cpggen/utils.py` & `cpggen-1.1.1/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.0/pyproject.toml` & `cpggen-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.0"
+version = "1.1.1"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.0/PKG-INFO` & `cpggen-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.0
+Version: 1.1.1
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -60,23 +60,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

