# Comparing `tmp/tuneflow-devkit-py-0.8.0.tar.gz` & `tmp/tuneflow-devkit-py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.0.tar", last modified: Mon May  8 19:37:43 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.1.tar", last modified: Wed May 10 04:54:39 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.0.tar` & `tuneflow-devkit-py-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-08 19:33:39.000000 tuneflow-devkit-py-0.8.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7077 2023-03-10 22:44:35.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8064 2023-04-01 02:37:00.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-08 19:37:43.000000 tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:37:43.486639 tuneflow-devkit-py-0.8.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.0/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.0/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.1/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.1/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-10 04:53:09.000000 tuneflow-devkit-py-0.8.1/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8042 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-10 04:54:39.000000 tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:54:39.089575 tuneflow-devkit-py-0.8.1/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.1/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.1/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.0/LICENSE` & `tuneflow-devkit-py-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.0/PKG-INFO` & `tuneflow-devkit-py-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.0/README.md` & `tuneflow-devkit-py-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.0/pyproject.toml` & `tuneflow-devkit-py-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.0"
+version = "0.8.1"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'python-socketio >= 5.7.2',
     'uvicorn[standard] >= 0.20.0',
-    'tuneflow-py >= 0.8.0',
+    'tuneflow-py >= 0.8.1',
     'msgpack == 1.0.4',
     'fastapi == 0.92.0',
     'msgpack-asgi == 1.1.0'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tuneflow/tuneflow-devkit-py"
```

### Comparing `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/debugger.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Creates a local debug server for a single plugin.
         '''
 
         if plugin_class is None or bundle_file_path is None:
             raise Exception("plugin_class and bundle_file must be provided")
         validate_plugin(plugin_class=plugin_class)
         self._plugin_class = plugin_class
-        with open(bundle_file_path, 'r') as bundle_file:
+        with open(bundle_file_path, 'rb') as bundle_file:
             bundle_info = json.load(bundle_file)
             # Validate plugin and bundle.
             plugin_info = find_match_plugin_info(
                 bundle_info=bundle_info, provider_id=plugin_class.provider_id(),
                 plugin_id=plugin_class.plugin_id())
             if plugin_info is None:
                 raise Exception(
```

### Comparing `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tuneflow_py import TuneflowPlugin, Song
 from typing import Type, List
 import json
 from msgpack import unpackb, packb
 from tuneflow_devkit.validation_utils import validate_plugin, find_match_plugin_info
 from collections import defaultdict
 from fastapi import FastAPI, Request, Response, Depends, BackgroundTasks
-from pathlib import PosixPath
+from pathlib import Path
 import asyncio
 import functools
 from fastapi.middleware.cors import CORSMiddleware
 import traceback
 from nanoid import generate as generate_nanoid
 
 
@@ -42,15 +42,15 @@
                 self._plugin_info_map[provider_id][plugin_id] = plugin_info
             # Ensure all entries in bundle.info have corresponding plugin code.
             for plugin_info in bundle_info["plugins"]:
                 if not any(
                         plugin_class.provider_id() == plugin_info["providerId"] and plugin_class.plugin_id() ==
                         plugin_info["pluginId"] for plugin_class in plugin_class_list):
                     raise Exception(
-                        f'Plugin {plugin_info["providerId"]} {plugin_info["pluginInfo"]} has no corresponding source code in the plugin list')
+                        f'Plugin {plugin_info["providerId"]} {plugin_info["pluginId"]} has no corresponding source code in the plugin list')
 
     def start(self, path_prefix='/', config=None):
         '''
         @param port Port to run the server
         '''
 
         app = FastAPI()
@@ -71,17 +71,17 @@
 
         @app.middleware("http")
         async def add_vary_origin_header(request: Request, call_next):
             response = await call_next(request)
             response.headers["Vary"] = 'Origin'
             return response
 
-        get_info_path = str(PosixPath(path_prefix).joinpath('plugin-bundle-info'))
-        init_plugin_path = str(PosixPath(path_prefix).joinpath('init-plugin-params'))
-        run_plugin_path = str(PosixPath(path_prefix).joinpath('jobs'))
+        get_info_path = str(Path(path_prefix).joinpath('plugin-bundle-info'))
+        init_plugin_path = str(Path(path_prefix).joinpath('init-plugin-params'))
+        run_plugin_path = str(Path(path_prefix).joinpath('jobs'))
 
         def init_plugin_task(plugin_class: Type[TuneflowPlugin], song: Song):
             try:
                 params_config = plugin_class.params(song)
                 return {"status": "OK",
                         "paramsConfig": params_config,
                         "params": plugin_class._get_default_params(param_config=params_config)
```

### Comparing `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.0/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.1/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.0/test/test_runner.py` & `tuneflow-devkit-py-0.8.1/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.0/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.1/test/test_validation_utils.py`

 * *Files identical despite different names*

