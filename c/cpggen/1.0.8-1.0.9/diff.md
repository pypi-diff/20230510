# Comparing `tmp/cpggen-1.0.8.tar.gz` & `tmp/cpggen-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.8.tar", max compression
+gzip compressed data, was "cpggen-1.0.9.tar", max compression
```

## Comparing `cpggen-1.0.8.tar` & `cpggen-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-09 14:27:37.705963 cpggen-1.0.8/LICENSE
--rw-r--r--   0        0        0     9252 2023-05-09 14:27:37.709963 cpggen-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/__init__.py
--rw-r--r--   0        0        0    17123 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/cli.py
--rw-r--r--   0        0        0    35546 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/logger.py
--rw-r--r--   0        0        0    11547 2023-05-09 14:27:37.709963 cpggen-1.0.8/cpggen/utils.py
--rw-r--r--   0        0        0     1278 2023-05-09 14:27:37.709963 cpggen-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    10532 1970-01-01 00:00:00.000000 cpggen-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 22:43:22.074547 cpggen-1.0.9/LICENSE
+-rw-r--r--   0        0        0    11158 2023-05-09 22:43:22.074547 cpggen-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/__init__.py
+-rw-r--r--   0        0        0    18985 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/cli.py
+-rw-r--r--   0        0        0    37138 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-09 22:43:22.074547 cpggen-1.0.9/cpggen/utils.py
+-rw-r--r--   0        0        0     1278 2023-05-09 22:43:22.074547 cpggen-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12438 1970-01-01 00:00:00.000000 cpggen-1.0.9/PKG-INFO
```

### Comparing `cpggen-1.0.8/LICENSE` & `cpggen-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.8/README.md` & `cpggen-1.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.8/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.9/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.8/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.9/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -158,18 +158,18 @@
 
 Example to export `cpg14` graphs in `dot` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export
 ```
 
-To export `pdg` in `neo4jcsv` format
+To export `cpg` in `neo4jcsv` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr cpg --export-format neo4jcsv
 ```
 
 ### Slicing graphs
 
 Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
 
 ```bash
@@ -219,14 +219,54 @@
 | Php         | No             | Low      |
 | Python      | No             | Low      |
 | C# / dotnet | Yes            | High     |
 | Go          | Yes            | High     |
 
 (\*) - Precision could be improved with dependencies
 
+## Full list of options
+
+```
+cpggen --help
+usage: cpggen [-h] [-i SRC] [-o CPG_OUT_DIR] [-l LANGUAGE] [--use-container] [--build] [--joern-home JOERN_HOME] [--server] [--server-host SERVER_HOST] [--server-port SERVER_PORT] [--export]
+              [--export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}] [--export-format {neo4jcsv,graphml,graphson,dot}] [--export-out-dir EXPORT_OUT_DIR] [--verbose] [--skip-sbom] [--slice] [--slice-mode {Usages,DataFlow}] [--use-parse]
+
+CPG Generator
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i SRC, --src SRC     Source directory or url
+  -o CPG_OUT_DIR, --out-dir CPG_OUT_DIR
+                        CPG output directory
+  -l LANGUAGE, --lang LANGUAGE
+                        Optional. CPG language frontend to use. Auto-detects by default.
+  --use-container       Use cpggen docker image
+  --build               Attempt to build the project automatically
+  --joern-home JOERN_HOME
+                        Joern installation directory
+  --server              Run cpggen as a server
+  --server-host SERVER_HOST
+                        cpggen server host
+  --server-port SERVER_PORT
+                        cpggen server port
+  --export              Export CPG as a graph
+  --export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}
+                        Graph representation to export
+  --export-format {neo4jcsv,graphml,graphson,dot}
+                        Export format
+  --export-out-dir EXPORT_OUT_DIR
+                        Export output directory
+  --verbose             Run cpggen in verbose mode
+  --skip-sbom           Do not generate SBoM
+  --slice               Extract intra-procedural slices from the CPG
+  --slice-mode {Usages,DataFlow}
+                        Mode used for CPG slicing
+  --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+```
+
 ## Environment variables
 
 | Name                    | Purpose                                                           |
 | ----------------------- | ----------------------------------------------------------------- |
 | JOERN_HOME              | Joern installation directory                                      |
 | CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
 | CPGGEN_PORT             | cpggen server port. Default 7072                                  |
```

### Comparing `cpggen-1.0.8/cpggen/cli.py` & `cpggen-1.0.9/cpggen/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,21 @@
     parser.add_argument(
         "--slice-mode",
         default=os.getenv("CPG_SLICE_MODE", "Usages"),
         dest="slice_mode",
         choices=["Usages", "DataFlow"],
         help="Mode used for CPG slicing",
     )
+    parser.add_argument(
+        "--use-parse",
+        dest="use_parse",
+        help="Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important",
+        action="store_true",
+        default=False,
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -179,28 +186,32 @@
     url = ""
     src = ""
     languages = ""
     cpg_out_dir = None
     is_temp_dir = False
     auto_build = True
     skip_sbom = True
+    export = False
     slice = False
+    use_parse = False
     slice_mode = "Usages"
     app_manifest_list = []
     errors_warnings = []
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
     if q.get("lang"):
         languages = q.get("lang")
+    if q.get("export", "") in ("true", "1"):
+        export = True
     if q.get("slice", "") in ("true", "1"):
         slice = True
     if q.get("slice_mode"):
         slice_mode = q.get("slice_mode")
     if q.get("auto_build", "") in ("false", "0"):
         auto_build = False
     if q.get("skip_sbom", "") in ("false", "0"):
@@ -213,14 +224,16 @@
         languages = params.get("lang")
     if not cpg_out_dir and params.get("out_dir"):
         cpg_out_dir = params.get("out_dir")
     if params.get("auto_build", "") in ("false", "0"):
         auto_build = False
     if params.get("skip_sbom", "") in ("false", "0"):
         skip_sbom = False
+    if params.get("export", "") in ("true", "1"):
+        export = True
     if params.get("slice", "") in ("true", "1"):
         slice = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
@@ -245,37 +258,47 @@
             src,
             cpg_out_dir,
             src,
             joern_home=os.getenv(
                 "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
             ),
             use_container=False,
+            use_parse=use_parse,
             auto_build=auto_build,
-            extra_args={"skip_sbom": skip_sbom, "slice_mode": slice_mode},
+            extra_args={
+                "skip_sbom": skip_sbom,
+                "slice_mode": slice_mode,
+                "for_export": export,
+                "for_slice": slice,
+            },
         )
         if mlist:
             app_manifest_list += mlist
         if slice and mlist:
             for ml in mlist:
                 if not os.path.exists(ml.get("cpg")):
                     errors_warnings.append(
                         f"""CPG file was not found at {ml.get("cpg")}"""
                     )
                     continue
                 executor.exec_tool(
                     "slice",
-                    src,
+                    ml.get("cpg"),
                     cpg_out_dir,
                     src,
                     joern_home=os.getenv(
                         "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
                     ),
                     use_container=False,
+                    use_parse=use_parse,
                     auto_build=False,
-                    extra_args={"slice_mode": slice_mode},
+                    extra_args={
+                        "slice_mode": slice_mode,
+                        "slice_out": ml.get("slice_out"),
+                    },
                 )
                 if not os.path.exists(ml.get("slice_out")):
                     errors_warnings.append(
                         f"""CPG slice file was not found at {ml.get("slice_out")}"""
                     )
     if is_temp_dir:
         try:
@@ -302,16 +325,20 @@
 
 def cpg(
     src,
     cpg_out_dir,
     languages,
     joern_home,
     use_container=False,
+    use_parse=False,
     auto_build=False,
     skip_sbom=False,
+    export=False,
+    slice=False,
+    slice_mode=None,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 for lang in languages:
                     LOG.debug(f"Generating CPG for the language {lang} at {src}")
                     pool.apply_async(
@@ -319,33 +346,50 @@
                         (
                             lang,
                             src,
                             cpg_out_dir,
                             src,
                             joern_home,
                             use_container,
+                            use_parse,
                             auto_build,
-                            {"skip_sbom": skip_sbom},
+                            {
+                                "skip_sbom": skip_sbom,
+                                "slice_mode": slice_mode,
+                                "for_export": export,
+                                "for_slice": slice,
+                            },
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
 def collect_cpg_manifests(cpg_out_dir):
     return utils.find_files(cpg_out_dir, ".manifest.json")
 
 
+def fix_export_repr(export_repr, export_format):
+    if export_format == "neo4jcsv":
+        if export_repr != "cpg":
+            LOG.warn(
+                "cpg is the only supported export representation for neo4jcsv format"
+            )
+        return "cpg"
+    return export_repr
+
+
 def export_slice_cpg(
     src,
     cpg_out_dir,
     joern_home,
     use_container,
+    use_parse,
     export,
     export_repr,
     export_format,
     export_out_dir,
     slice,
     slice_mode,
 ):
@@ -387,24 +431,30 @@
                             LOG.debug(
                                 f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
                             )
                         pool.apply_async(
                             executor.exec_tool,
                             (
                                 "export" if export else "slice",
-                                cpg_path if export else src,
+                                cpg_path,
                                 app_export_out_dir,
                                 cpg_out_dir,
                                 joern_home,
                                 use_container,
+                                use_parse,
                                 False,
                                 {
-                                    "export_repr": export_repr if export else None,
+                                    "export_repr": fix_export_repr(
+                                        export_repr, export_format
+                                    )
+                                    if export
+                                    else None,
                                     "export_format": export_format if export else None,
                                     "slice_mode": slice_mode if slice else None,
+                                    "slice_out": manifest_obj.get("slice_out"),
                                 },
                             ),
                         )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
@@ -433,14 +483,15 @@
     if cpg_out_dir:
         cpg_out_dir = str(PurePath(cpg_out_dir))
     if export_out_dir:
         export_out_dir = str(PurePath(export_out_dir))
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
+    use_parse = args.use_parse
     is_bundled_exe = False
     try:
         if getattr(sys, "_MEIPASS"):
             is_bundled_exe = True
             # Reset joern_home for bundled exe
             if not os.path.exists(joern_home):
                 joern_home = ""
@@ -477,23 +528,28 @@
 
     cpg(
         src,
         cpg_out_dir,
         languages,
         joern_home=joern_home,
         use_container=use_container,
+        use_parse=use_parse,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
+        export=args.export,
+        slice=args.slice,
+        slice_mode=args.slice_mode,
     )
     if args.export or args.slice:
         export_slice_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
+            use_parse=use_parse,
             export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
             slice=args.slice,
             slice_mode=args.slice_mode,
         )
```

### Comparing `cpggen-1.0.8/cpggen/executor.py` & `cpggen-1.0.9/cpggen/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,30 +123,33 @@
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "java-with-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
     "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "binary": "%(joern_home)sghidra2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "javascript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
+    "typescript": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg%(only_bat_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "csharp": "%(joern_home)sbin%(os_path_sep)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "dotnet": "%(joern_home)sbin%(os_path_sep)scsharp2cpg%(exe_ext)s -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-errors --no-log-file --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg%(exe_ext)s generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s%(exe_ext)s%(cdxgen_args)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
-    "export": "%(joern_home)sjoern-export%(only_bat_ext)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
-    "slice": "%(joern_home)sjoern-slice%(only_bat_ext)s -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
+    "parse": "%(joern_home)sjoern-parse%(only_bat_ext)s -J-Xmx%(memory)s --language %(parse_lang)s --output %(cpg_out)s %(src)s",
+    "export": "%(joern_home)sjoern-export%(only_bat_ext)s -J-Xmx%(memory)s --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "slice": "%(joern_home)sjoern-slice%(only_bat_ext)s -J-Xmx%(memory)s --dummy-types true --exclude-operators true -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
     "qwiet": "sl%(exe_ext)s analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "jar": {
@@ -196,14 +199,33 @@
     "typescript": "js",
     "go": "go",
     "csharp": "csharp",
     "dotnet": "csharp",
     "cpp": "c",
 }
 
+joern_parse_lang_map = {
+    "jar": "javasrc",
+    "jsp": "javasrc",
+    "scala": "javasrc",
+    "java": "javasrc",
+    "python": "pythonsrc",
+    "js": "jssrc",
+    "ts": "jssrc",
+    "javascript": "jssrc",
+    "typescript": "jssrc",
+    "go": "golang",
+    "csharp": "csharp",
+    "dotnet": "csharp",
+    "cpp": "newc",
+    "c": "newc",
+    "binary": "ghidra",
+    "ruby": "rubysrc",
+}
+
 
 def qwiet_analysis(app_manifest, src, cwd, env):
     try:
         relative_path = os.path.relpath(cwd, src)
         if relative_path and not relative_path.startswith(".."):
             os.environ["SL_VCS_RELATIVE_PATH"] = relative_path
             env["SL_VCS_RELATIVE_PATH"] = relative_path
@@ -395,14 +417,15 @@
 def exec_tool(
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
     joern_home=None,
     use_container=False,
+    use_parse=False,
     auto_build=False,
     extra_args={},
     env=os.environ.copy(),
     stdout=subprocess.DEVNULL,
 ):
     with Progress(
         console=console,
@@ -441,15 +464,22 @@
             elif tool_lang == "slice":
                 tool_verb = "Slicing CPG with joern-slice"
             task = progress.add_task(
                 "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
-            cmd_with_args = cpg_tools_map.get(tool_lang)
+            cpg_cmd_lang = tool_lang
+            # If the intention is to export or slice then use joern-parse
+            if use_parse or (
+                extra_args
+                and (extra_args.get("for_export") or extra_args.get("for_slice"))
+            ):
+                cpg_cmd_lang = "parse"
+            cmd_with_args = cpg_tools_map.get(cpg_cmd_lang)
             if not cmd_with_args:
                 return
             # Perform build first
             if auto_build or build_tools_map.get(tool_lang):
                 if os.getenv("CI"):
                     LOG.info(
                         f"Automatically building {src} for {tool_lang}. To speed up this step, cache the build dependencies using the CI cache settings."
@@ -479,71 +509,75 @@
             modules = [src]
             # For go, the modules are based on the presence of go.mod files
             if tool_lang == "go":
                 go_mods = find_go_mods(src)
                 if go_mods:
                     modules = [os.path.dirname(gmod) for gmod in go_mods]
             for amodule in modules:
-                cmd_with_args = cpg_tools_map.get(tool_lang)
+                cmd_with_args = cpg_tools_map.get(cpg_cmd_lang)
                 if use_container:
                     # We need to make src an absolute path since relative paths wouldn't work in container mode
                     amodule = os.path.abspath(amodule)
                     container_cli = "docker"
                     if check_command("podman"):
                         container_cli = "podman"
                     cmd_with_args = f"""{container_cli} run --rm -w {amodule} -v {tempfile.gettempdir()}:/tmp -v {amodule}:{amodule}:rw -v {os.path.abspath(cpg_out_dir)}:{os.path.abspath(cpg_out_dir)}:rw -t {os.getenv("CPGGEN_IMAGE", "ghcr.io/appthreat/cpggen")} {cmd_with_args}"""
                     # We need to fix joern_home to the directory inside the container
                     joern_home = ""
                 sbom_cmd_with_args = cpg_tools_map.get("sbom")
                 sbom_out = ""
                 manifest_out = ""
-                slice_out = ""
+                slice_out = extra_args.get("slice_out", "")
+                cpg_out = (
+                    cpg_out_dir
+                    if cpg_out_dir.endswith(".bin.zip")
+                    or cpg_out_dir.endswith(".bin")
+                    or cpg_out_dir.endswith(".cpg")
+                    else os.path.abspath(
+                        os.path.join(
+                            cpg_out_dir,
+                            f"{os.path.basename(amodule)}-{tool_lang_simple}-cpg.bin.zip",
+                        )
+                    )
+                )
                 if tool_lang == "export":
                     cpg_out = os.path.abspath(cpg_out_dir)
                 elif tool_lang == "slice":
+                    if not slice_out:
+                        slice_out = cpg_out.replace(".bin.zip", ".slices")
                     cpg_out = src
                 else:
-                    cpg_out = (
-                        cpg_out_dir
-                        if cpg_out_dir.endswith(".bin.zip")
-                        or cpg_out_dir.endswith(".bin")
-                        or cpg_out_dir.endswith(".cpg")
-                        else os.path.abspath(
-                            os.path.join(
-                                cpg_out_dir,
-                                f"{os.path.basename(amodule)}-{tool_lang_simple}-cpg.bin.zip",
-                            )
-                        )
-                    )
                     sbom_out = (
                         cpg_out.replace(".bin.zip", ".bom.xml")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.bom.xml"
                     )
                     manifest_out = (
                         cpg_out.replace(".bin.zip", ".manifest.json")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.manifest.json"
                     )
                     LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
-                slice_out = cpg_out.replace(".bin.zip", ".slices")
-                slice_out = slice_out + (
-                    ".json" if extra_args.get("slice_mode") == "Usages" else ".cpg"
-                )
+                if not slice_out:
+                    slice_out = cpg_out.replace(".bin.zip", ".slices")
+                    slice_out = slice_out + (
+                        ".json" if extra_args.get("slice_mode") == "Usages" else ".cpg"
+                    )
+                    extra_args["slice_out"] = slice_out
                 cmd_with_args = cmd_with_args % dict(
                     src=os.path.abspath(amodule),
                     cpg_out=cpg_out,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
+                    parse_lang=joern_parse_lang_map.get(tool_lang, tool_lang),
                     sbom_out=sbom_out,
-                    slice_out=slice_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
                     only_bat_ext=only_bat_ext,
                     os_path_sep=os.path.sep,
                     **extra_args,
                 )
@@ -572,15 +606,19 @@
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd) and not os.path.exists(lang_cmd):
                     if not use_container:
                         LOG.warn(
-                            f"{lang_cmd} is not found. Try running cpggen with --use-container argument"
+                            f"{lang_cmd} is not found. Try running cpggen with --use-container argument."
+                        )
+                    elif not use_parse:
+                        LOG.warn(
+                            "Try running cpggen with --use-parse argument to use joern-parse command instead of language frontends."
                         )
                     else:
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
                         )
                     return
                 # Is this an Export or Slice task?
```

### Comparing `cpggen-1.0.8/cpggen/logger.py` & `cpggen-1.0.9/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.8/cpggen/utils.py` & `cpggen-1.0.9/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.8/pyproject.toml` & `cpggen-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.8"
+version = "1.0.9"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.8/PKG-INFO` & `cpggen-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.8
+Version: 1.0.9
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
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.8/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.9/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.8/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.9/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -189,18 +189,18 @@
 
 Example to export `cpg14` graphs in `dot` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export
 ```
 
-To export `pdg` in `neo4jcsv` format
+To export `cpg` in `neo4jcsv` format
 
 ```bash
-cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr cpg --export-format neo4jcsv
 ```
 
 ### Slicing graphs
 
 Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
 
 ```bash
@@ -250,14 +250,54 @@
 | Php         | No             | Low      |
 | Python      | No             | Low      |
 | C# / dotnet | Yes            | High     |
 | Go          | Yes            | High     |
 
 (\*) - Precision could be improved with dependencies
 
+## Full list of options
+
+```
+cpggen --help
+usage: cpggen [-h] [-i SRC] [-o CPG_OUT_DIR] [-l LANGUAGE] [--use-container] [--build] [--joern-home JOERN_HOME] [--server] [--server-host SERVER_HOST] [--server-port SERVER_PORT] [--export]
+              [--export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}] [--export-format {neo4jcsv,graphml,graphson,dot}] [--export-out-dir EXPORT_OUT_DIR] [--verbose] [--skip-sbom] [--slice] [--slice-mode {Usages,DataFlow}] [--use-parse]
+
+CPG Generator
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i SRC, --src SRC     Source directory or url
+  -o CPG_OUT_DIR, --out-dir CPG_OUT_DIR
+                        CPG output directory
+  -l LANGUAGE, --lang LANGUAGE
+                        Optional. CPG language frontend to use. Auto-detects by default.
+  --use-container       Use cpggen docker image
+  --build               Attempt to build the project automatically
+  --joern-home JOERN_HOME
+                        Joern installation directory
+  --server              Run cpggen as a server
+  --server-host SERVER_HOST
+                        cpggen server host
+  --server-port SERVER_PORT
+                        cpggen server port
+  --export              Export CPG as a graph
+  --export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}
+                        Graph representation to export
+  --export-format {neo4jcsv,graphml,graphson,dot}
+                        Export format
+  --export-out-dir EXPORT_OUT_DIR
+                        Export output directory
+  --verbose             Run cpggen in verbose mode
+  --skip-sbom           Do not generate SBoM
+  --slice               Extract intra-procedural slices from the CPG
+  --slice-mode {Usages,DataFlow}
+                        Mode used for CPG slicing
+  --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+```
+
 ## Environment variables
 
 | Name                    | Purpose                                                           |
 | ----------------------- | ----------------------------------------------------------------- |
 | JOERN_HOME              | Joern installation directory                                      |
 | CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
 | CPGGEN_PORT             | cpggen server port. Default 7072                                  |
```

