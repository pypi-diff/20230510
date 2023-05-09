# Comparing `tmp/cpggen-1.0.7.tar.gz` & `tmp/cpggen-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.7.tar", max compression
+gzip compressed data, was "cpggen-1.0.8.tar", max compression
```

## Comparing `cpggen-1.0.7.tar` & `cpggen-1.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-09 02:51:25.070990 cpggen-1.0.7/LICENSE
--rw-r--r--   0        0        0     9252 2023-05-09 02:51:25.070990 cpggen-1.0.7/README.md
--rw-r--r--   0        0        0        0 2023-05-09 02:51:25.070990 cpggen-1.0.7/cpggen/__init__.py
--rw-r--r--   0        0        0    17207 2023-05-09 02:51:25.070990 cpggen-1.0.7/cpggen/cli.py
--rw-r--r--   0        0        0    35546 2023-05-09 02:51:25.070990 cpggen-1.0.7/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-09 02:51:25.074990 cpggen-1.0.7/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-09 02:51:25.074990 cpggen-1.0.7/cpggen/utils.py
--rw-r--r--   0        0        0     1278 2023-05-09 02:51:25.074990 cpggen-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 14:27:37.705963 cpggen-1.0.8/LICENSE
+-rw-r--r--   0        0        0     9252 2023-05-09 14:27:37.709963 cpggen-1.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/__init__.py
+-rw-r--r--   0        0        0    17123 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/cli.py
+-rw-r--r--   0        0        0    35546 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/utils.py
+-rw-r--r--   0        0        0     1278 2023-05-09 14:27:37.709963 cpggen-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.8/PKG-INFO
```

### Comparing `cpggen-1.0.7/LICENSE` & `cpggen-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.7/README.md` & `cpggen-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.7/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.8/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.7/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.8/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.0.7/cpggen/cli.py` & `cpggen-1.0.8/cpggen/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
                 if not os.path.exists(ml.get("cpg")):
                     errors_warnings.append(
                         f"""CPG file was not found at {ml.get("cpg")}"""
                     )
                     continue
                 executor.exec_tool(
                     "slice",
-                    ml.get("cpg"),
+                    src,
                     cpg_out_dir,
                     src,
                     joern_home=os.getenv(
                         "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
                     ),
                     use_container=False,
                     auto_build=False,
@@ -383,21 +383,19 @@
                             cpg_path = os.path.join(
                                 os.getenv("GITHUB_WORKSPACE"), cpg_path
                             )
                         if export:
                             LOG.debug(
                                 f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
                             )
-                        if slice:
-                            cpg_path = manifest_obj["cpg"]
                         pool.apply_async(
                             executor.exec_tool,
                             (
                                 "export" if export else "slice",
-                                cpg_path,
+                                cpg_path if export else src,
                                 app_export_out_dir,
                                 cpg_out_dir,
                                 joern_home,
                                 use_container,
                                 False,
                                 {
                                     "export_repr": export_repr if export else None,
```

### Comparing `cpggen-1.0.7/cpggen/executor.py` & `cpggen-1.0.8/cpggen/executor.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.7/cpggen/logger.py` & `cpggen-1.0.8/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.7/cpggen/utils.py` & `cpggen-1.0.8/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.7/pyproject.toml` & `cpggen-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.7"
+version = "1.0.8"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.7/PKG-INFO` & `cpggen-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -58,23 +58,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.7/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.8/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.7/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.8/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

