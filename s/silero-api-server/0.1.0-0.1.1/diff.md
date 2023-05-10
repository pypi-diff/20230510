# Comparing `tmp/silero_api_server-0.1.0.tar.gz` & `tmp/silero_api_server-0.1.1.tar.gz`

## Comparing `silero_api_server-0.1.0.tar` & `silero_api_server-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/run.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/run.sh
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/__init__.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/server.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.env
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/run.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/run.sh
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/PKG-INFO
```

### Comparing `silero_api_server-0.1.0/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.1.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.0/silero_api_server/server.py` & `silero_api_server-0.1.1/silero_api_server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+import pathlib
 import dotenv, os
 from fastapi import FastAPI, Response, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 import uvicorn
@@ -12,18 +13,19 @@
 
 
 dotenv.load_dotenv()
 HOSTNAME = os.getenv('TTS_SERVER_HOSTNAME')
 PORT = os.getenv('TTS_SERVER_PORT')
 LOCAL_URL = f"http://{HOSTNAME}:{PORT}"
 
-os.chdir(os.getcwd())
+module_path = pathlib.Path(__file__).resolve().parent
+os.chdir(module_path)
 SAMPLE_PATH = "samples"
 
-tts_service = SileroTtsService(os.path.abspath(os.getcwd()))
+tts_service = SileroTtsService(f"{module_path}//{SAMPLE_PATH}")
 app = FastAPI()
 
 # Make sure the samples directory exists
 if not os.path.exists(SAMPLE_PATH):
     os.mkdir(SAMPLE_PATH)
 
 if len(os.listdir(SAMPLE_PATH)) == 0:
```

### Comparing `silero_api_server-0.1.0/silero_api_server/tts.py` & `silero_api_server-0.1.1/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.0/LICENSE` & `silero_api_server-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.0/README.md` & `silero_api_server-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.0/pyproject.toml` & `silero_api_server-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-api-server"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Ouoertheo", email="ouoertheo@tomeofjamin.net" },
 ]
 description = "A simple FastAPI server to host Silero TTS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `silero_api_server-0.1.0/PKG-INFO` & `silero_api_server-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

