# Comparing `tmp/cpggen-1.0.9.tar.gz` & `tmp/cpggen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.9.tar", max compression
+gzip compressed data, was "cpggen-1.1.0.tar", max compression
```

## Comparing `cpggen-1.0.9.tar` & `cpggen-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-09 22:43:22.074547 cpggen-1.0.9/LICENSE
--rw-r--r--   0        0        0    11158 2023-05-09 22:43:22.074547 cpggen-1.0.9/README.md
--rw-r--r--   0        0        0        0 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/__init__.py
--rw-r--r--   0        0        0    18985 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/cli.py
--rw-r--r--   0        0        0    37138 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/utils.py
--rw-r--r--   0        0        0     1278 2023-05-09 22:43:22.074547 cpggen-1.0.9/pyproject.toml
--rw-r--r--   0        0        0    12438 1970-01-01 00:00:00.000000 cpggen-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 01:06:37.905057 cpggen-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11604 2023-05-10 01:06:37.905057 cpggen-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/__init__.py
+-rw-r--r--   0        0        0    19518 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/cli.py
+-rw-r--r--   0        0        0    37417 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/logger.py
+-rw-r--r--   0        0        0    14143 2023-05-10 01:06:37.909057 cpggen-1.1.0/cpggen/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-10 01:06:37.909057 cpggen-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12976 1970-01-01 00:00:00.000000 cpggen-1.1.0/PKG-INFO
```

### Comparing `cpggen-1.0.9/LICENSE` & `cpggen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.9/README.md` & `cpggen-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.9/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.9/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -127,20 +127,24 @@
 
 To specify input and output directory.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
-You can even pass a git url as source
+You can even pass a git or a package url as source
 
 ```
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
+```
+cpggen -i "pkg:maven/org.apache.commons/commons-io@1.3.2" -o /tmp/cpg
+```
+
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
 
 # Comma separated values are accepted for multiple languages
 cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
@@ -261,30 +265,32 @@
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
   --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
 ```
 
 ## Environment variables
 
-| Name                    | Purpose                                                           |
-| ----------------------- | ----------------------------------------------------------------- |
-| JOERN_HOME              | Joern installation directory                                      |
-| CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
-| CPGGEN_PORT             | cpggen server port. Default 7072                                  |
-| CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
-| CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
-| CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
-| AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
-| CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
-| CPG_EXPORT_REPR         | Graph to export. Default all                                      |
-| CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
-| CPG_SLICE               | Set to true to slice CPG                                          |
-| CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
-| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
-| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                 |
+| Name                    | Purpose                                                                    |
+| ----------------------- | -------------------------------------------------------------------------- |
+| JOERN_HOME              | Joern installation directory                                               |
+| CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                                      |
+| CPGGEN_PORT             | cpggen server port. Default 7072                                           |
+| CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed             |
+| CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed          |
+| CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                         |
+| AT_DEBUG_MODE           | Set to debug to enable debug logging                                       |
+| CPG_EXPORT              | Set to true to export CPG graphs in dot format                             |
+| CPG_EXPORT_REPR         | Graph to export. Default all                                               |
+| CPG_EXPORT_FORMAT       | Export format. Default dot                                                 |
+| CPG_SLICE               | Set to true to slice CPG                                                   |
+| CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
+| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
+| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
+| ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
+| JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-1.0.9/cpggen/cli.py` & `cpggen-1.1.0/cpggen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,17 @@
         default=False,
         dest="verbose_mode",
         help="Run cpggen in verbose mode",
     )
     parser.add_argument(
         "--skip-sbom",
         action="store_true",
-        default=True if not os.getenv("SHIFTLEFT_ACCESS_TOKEN") else False,
+        default=True
+        if not os.getenv("SHIFTLEFT_ACCESS_TOKEN") and not os.getenv("ENABLE_SBOM")
+        else False,
         dest="skip_sbom",
         help="Do not generate SBoM",
     )
     parser.add_argument(
         "--slice",
         action="store_true",
         default=True if os.getenv("CPG_SLICE") in ("true", "1") else False,
@@ -235,17 +237,22 @@
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
     if not url and (src.startswith("http") or src.startswith("git")):
         url = src
-    if url.startswith("http") or url.startswith("git"):
+    if url.startswith("http") or url.startswith("git") or url.startswith("pkg:"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
-        src = utils.clone_repo(url, clone_dir)
+        if src.startswith("pkg:"):
+            download_file = utils.download_package(src, clone_dir)
+            if download_file and os.path.exists(download_file):
+                src = clone_dir
+        else:
+            src = utils.clone_repo(url, clone_dir)
         is_temp_dir = True
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
@@ -507,17 +514,22 @@
             console.print(
                 "Alternatively, ensure docker or podman is available to use cpggen container image"
             )
     # GitHub action is very weird
     if os.getenv("GITHUB_PATH") and utils.check_command("joern"):
         joern_home = ""
     is_temp_dir = False
-    if src.startswith("http") or src.startswith("git://"):
+    if src.startswith("http") or src.startswith("git://") or src.startswith("pkg:"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
-        src = utils.clone_repo(src, clone_dir)
+        if src.startswith("pkg:"):
+            download_file = utils.download_package(src, clone_dir)
+            if download_file and os.path.exists(download_file):
+                src = clone_dir
+        else:
+            src = utils.clone_repo(src, clone_dir)
         is_temp_dir = True
         if not cpg_out_dir:
             cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
         if not export_out_dir:
             export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
```

### Comparing `cpggen-1.0.9/cpggen/executor.py` & `cpggen-1.1.0/cpggen/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "java-with-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
+    "jimple": "%(joern_home)sjimple2cpg%(only_bat_ext)s%(android_jar)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "binary": "%(joern_home)sghidra2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "javascript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "typescript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
@@ -574,14 +575,17 @@
                     tool_lang=tool_lang,
                     parse_lang=joern_parse_lang_map.get(tool_lang, tool_lang),
                     sbom_out=sbom_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
                     only_bat_ext=only_bat_ext,
+                    android_jar=f' {os.getenv("JIMPLE_ANDROID_JAR", "").strip()}'
+                    if os.getenv("JIMPLE_ANDROID_JAR")
+                    else "",
                     os_path_sep=os.path.sep,
                     **extra_args,
                 )
                 sbom_lang = tool_lang_simple
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
```

### Comparing `cpggen-1.0.9/cpggen/logger.py` & `cpggen-1.1.0/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.9/cpggen/utils.py` & `cpggen-1.1.0/cpggen/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import re
 import shutil
 import tempfile
 import zipfile
 from pathlib import Path
 from sys import platform
 
+import httpx
+import rich.progress
+from packageurl import PackageURL
+from packageurl.contrib import purl2url
+from rich.progress import Progress
+
 GIT_AVAILABLE = False
 try:
     import git
 
     GIT_AVAILABLE = True
 except Exception:
     pass
@@ -314,14 +320,15 @@
 
 
 def detect_project_type(src_dir):
     """Detect project type by looking for certain files
     :param src_dir: Source directory
     :return List of detected types
     """
+    is_java_like = False
     home_dir = str(Path.home())
     maven_cache = os.path.join(home_dir, ".m2")
     gradle_cache = os.path.join(home_dir, ".gradle", "caches", "modules-2", "files-2.1")
     maven_cache_exists = os.path.exists(maven_cache)
     gradle_cache_exists = os.path.exists(gradle_cache)
     project_types = []
     if find_python_reqfiles(src_dir) or find_files(src_dir, ".py", False, True):
@@ -340,14 +347,15 @@
         else:
             project_types.append("kotlin")
     if (
         find_files(src_dir, "pom.xml", False, True)
         or find_files(src_dir, ".gradle", False, True)
         or find_files(src_dir, ".java", False, True)
     ):
+        is_java_like = True
         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
             project_types.append("jar")
         else:
             if os.path.exists(str(Path.home() / ".m2")):
                 project_types.append("java-with-deps")
             elif os.path.exists(
                 str(Path.home() / ".gradle" / "caches" / "modules-2" / "files-2.1")
@@ -391,15 +399,82 @@
         project_types.append("c")
     if find_files(src_dir, ".bc", False, True) or find_files(
         src_dir, ".ll", False, True
     ):
         project_types.append("llvm")
     if is_exe(src_dir):
         project_types.append("binary")
+    # Directory contains just a bunch of jar then try jimple
+    if not is_java_like:
+        if find_files(src_dir, ".jar", False, True):
+            if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
+                project_types.append("jar")
+            else:
+                project_types.append("jimple")
+        elif (
+            find_files(src_dir, ".apk", False, True)
+            or find_files(src_dir, ".zip", False, True)
+            or find_files(src_dir, ".dex", False, True)
+            or find_files(src_dir, ".class", False, True)
+            or find_files(src_dir, ".jimple", False, True)
+        ):
+            project_types.append("jimple")
     return project_types
 
 
 def clone_repo(repo_url, clone_dir, depth=1):
     if not GIT_AVAILABLE:
         return None
     git.Repo.clone_from(repo_url, clone_dir, depth=depth)
     return clone_dir
+
+
+def build_maven_download_url(purl):
+    """
+    Return a maven download URL from the `purl` string.
+    """
+    MAVEN_CENTRAL_URL = "https://repo1.maven.org/maven2/"
+    ANDROID_MAVEN = "https://maven.google.com/"
+    url_prefix = MAVEN_CENTRAL_URL
+
+    purl_data = PackageURL.from_string(purl)
+    group = purl_data.namespace.replace(".", "/")
+    name = purl_data.name
+    version = purl_data.version
+
+    if "android" in group:
+        url_prefix = ANDROID_MAVEN
+
+    if name and version:
+        return f"{url_prefix}{group}/{name}/{version}/{name}-{version}.jar"
+
+
+def get_download_url(purl_str):
+    if purl_str.startswith("pkg:maven"):
+        return build_maven_download_url(purl_str)
+    return purl2url.get_download_url(purl_str)
+
+
+def download_package(purl_str, download_dir):
+    if not purl_str:
+        return
+    durl = get_download_url(purl_str)
+    if not durl:
+        return
+    with open(
+        os.path.join(download_dir, os.path.basename(durl)), mode="wb"
+    ) as download_file:
+        with httpx.stream("GET", durl) as response:
+            total = int(response.headers["Content-Length"])
+            with Progress(
+                "[progress.percentage]{task.percentage:>3.0f}%",
+                rich.progress.BarColumn(bar_width=None),
+                rich.progress.DownloadColumn(),
+                rich.progress.TransferSpeedColumn(),
+            ) as progress:
+                download_task = progress.add_task("Download", total=total)
+                for chunk in response.iter_bytes():
+                    download_file.write(chunk)
+                    progress.update(
+                        download_task, completed=response.num_bytes_downloaded
+                    )
+                return download_file.name
```

### Comparing `cpggen-1.0.9/pyproject.toml` & `cpggen-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.9"
+version = "1.1.0"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
@@ -28,14 +28,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 rich = "^13.3.5"
 gitpython = "^3.1.31"
 quart = "^0.18.4"
 psutil = "^5.9.5"
+packageurl-python = "^0.11.1"
+httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
 pyinstaller = "^5.10.1"
```

### Comparing `cpggen-1.0.9/PKG-INFO` & `cpggen-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.9
+Version: 1.1.0
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -19,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: packageurl-python (>=0.11.1,<0.12.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: quart (>=0.18.4,<0.19.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Project-URL: Repository, https://github.com/AppThreat/cpggen
 Description-Content-Type: text/markdown
 
 # CPG Generator
@@ -58,23 +60,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.9/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.9/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -158,20 +160,24 @@
 
 To specify input and output directory.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
-You can even pass a git url as source
+You can even pass a git or a package url as source
 
 ```
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
+```
+cpggen -i "pkg:maven/org.apache.commons/commons-io@1.3.2" -o /tmp/cpg
+```
+
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
 
 # Comma separated values are accepted for multiple languages
 cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
@@ -292,30 +298,32 @@
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
   --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
 ```
 
 ## Environment variables
 
-| Name                    | Purpose                                                           |
-| ----------------------- | ----------------------------------------------------------------- |
-| JOERN_HOME              | Joern installation directory                                      |
-| CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
-| CPGGEN_PORT             | cpggen server port. Default 7072                                  |
-| CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
-| CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
-| CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
-| AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
-| CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
-| CPG_EXPORT_REPR         | Graph to export. Default all                                      |
-| CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
-| CPG_SLICE               | Set to true to slice CPG                                          |
-| CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
-| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
-| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                 |
+| Name                    | Purpose                                                                    |
+| ----------------------- | -------------------------------------------------------------------------- |
+| JOERN_HOME              | Joern installation directory                                               |
+| CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                                      |
+| CPGGEN_PORT             | cpggen server port. Default 7072                                           |
+| CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed             |
+| CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed          |
+| CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                         |
+| AT_DEBUG_MODE           | Set to debug to enable debug logging                                       |
+| CPG_EXPORT              | Set to true to export CPG graphs in dot format                             |
+| CPG_EXPORT_REPR         | Graph to export. Default all                                               |
+| CPG_EXPORT_FORMAT       | Export format. Default dot                                                 |
+| CPG_SLICE               | Set to true to slice CPG                                                   |
+| CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
+| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
+| CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
+| ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
+| JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

