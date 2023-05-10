# Comparing `tmp/silero_api_server-0.0.7.tar.gz` & `tmp/silero_api_server-0.1.0.tar.gz`

## Comparing `silero_api_server-0.0.7.tar` & `silero_api_server-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/run.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/run.sh
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/__init__.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/server.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.env
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/run.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/run.sh
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/__init__.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.0/PKG-INFO
```

### Comparing `silero_api_server-0.0.7/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.1.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.7/silero_api_server/server.py` & `silero_api_server-0.1.0/silero_api_server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 
 import dotenv, os
 from fastapi import FastAPI, Response, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
+import uvicorn
 from silero_api_server.tts import SileroTtsService
 from loguru import logger
 from typing import Optional
 
+
 dotenv.load_dotenv()
 HOSTNAME = os.getenv('TTS_SERVER_HOSTNAME')
 PORT = os.getenv('TTS_SERVER_PORT')
 LOCAL_URL = f"http://{HOSTNAME}:{PORT}"
-SAMPLE_PATH = os.path.join(os.path.dirname(__file__),'sample')
 
-tts_service = SileroTtsService(os.path.abspath(SAMPLE_PATH))
+os.chdir(os.getcwd())
+SAMPLE_PATH = "samples"
+
+tts_service = SileroTtsService(os.path.abspath(os.getcwd()))
 app = FastAPI()
 
 # Make sure the samples directory exists
 if not os.path.exists(SAMPLE_PATH):
     os.mkdir(SAMPLE_PATH)
 
 if len(os.listdir(SAMPLE_PATH)) == 0:
     logger.info("Samples empty, generating new samples.")
     tts_service.generate_samples()
 
-app.mount(f"/{SAMPLE_PATH}",StaticFiles(directory='samples'),name='samples')
+app.mount(f"/samples",StaticFiles(directory=SAMPLE_PATH),name='samples')
 origins = ["*"]
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
@@ -70,8 +74,11 @@
 def play_sample(speaker: str):
     return FileResponse(f"{SAMPLE_PATH}/{speaker}.wav")
 
 @app.post("/tts/generate-samples")
 def generate_samples(sample_text: Optional[str] = ""):
     tts_service.update_sample_text(sample_text)
     tts_service.generate_samples()
-    return Response("Generated samples",status_code=200)
+    return Response("Generated samples",status_code=200)
+
+if __name__ == "__main__":
+    uvicorn.run(app,host="0.0.0.0",port=8001)
```

### Comparing `silero_api_server-0.0.7/silero_api_server/tts.py` & `silero_api_server-0.1.0/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.7/LICENSE` & `silero_api_server-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.7/README.md` & `silero_api_server-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.0.7/pyproject.toml` & `silero_api_server-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-api-server"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Ouoertheo", email="ouoertheo@tomeofjamin.net" },
 ]
 description = "A simple FastAPI server to host Silero TTS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `silero_api_server-0.0.7/PKG-INFO` & `silero_api_server-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.0.7
+Version: 0.1.0
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

