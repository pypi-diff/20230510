# Comparing `tmp/silero_api_server-0.1.1.tar.gz` & `tmp/silero_api_server-0.1.4.tar.gz`

## Comparing `silero_api_server-0.1.1.tar` & `silero_api_server-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.env
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/run.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/run.sh
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/server.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/silero_api_server/tts.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.env
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/requirements.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/run.ps1
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/run.sh
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/__main__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/server.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/silero_api_server/tts.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/README.md
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 silero_api_server-0.1.4/PKG-INFO
```

### Comparing `silero_api_server-0.1.1/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.1.4/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.1/silero_api_server/server.py` & `silero_api_server-0.1.4/silero_api_server/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import pathlib
 import dotenv, os
-from fastapi import FastAPI, Response, HTTPException
+from fastapi import FastAPI, Response, HTTPException, Request
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 import uvicorn
 from silero_api_server.tts import SileroTtsService
 from loguru import logger
@@ -28,15 +28,15 @@
 if not os.path.exists(SAMPLE_PATH):
     os.mkdir(SAMPLE_PATH)
 
 if len(os.listdir(SAMPLE_PATH)) == 0:
     logger.info("Samples empty, generating new samples.")
     tts_service.generate_samples()
 
-app.mount(f"/samples",StaticFiles(directory=SAMPLE_PATH),name='samples')
+app.mount(f"/samples",StaticFiles(directory=f"{module_path}//{SAMPLE_PATH}"),name='samples')
 origins = ["*"]
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
@@ -47,20 +47,20 @@
     speaker: str
     text: str
 
 class SampleText(BaseModel):
     text: str | None
 
 @app.get("/tts/speakers")
-def speakers():
+def speakers(request: Request):
     voices = [
         {
             "name":speaker,
             "voice_id":speaker,
-            "preview_url": f"{LOCAL_URL}/{SAMPLE_PATH}/{speaker}.wav"
+            "preview_url": f"{str(request.base_url)}{SAMPLE_PATH}/{speaker}.wav"
         } for speaker in tts_service.get_speakers()
     ]
     return voices
 
 @app.post("/tts/generate")
 def generate(voice: Voice):
     # Clean elipses
```

### Comparing `silero_api_server-0.1.1/silero_api_server/tts.py` & `silero_api_server-0.1.4/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.1/LICENSE` & `silero_api_server-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.1/README.md` & `silero_api_server-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.1.1/pyproject.toml` & `silero_api_server-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-api-server"
-version = "0.1.1"
 authors = [
   { name="Ouoertheo", email="ouoertheo@tomeofjamin.net" },
 ]
 description = "A simple FastAPI server to host Silero TTS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,15 +22,18 @@
   "python-dotenv==1.0.0",
   "torch==2.0.0",
   "torchaudio==2.0.1",
   "uvicorn",
   "soundfile",
   "numpy"
 ]
+dynamic=["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ouoertheo/silero-api-server"
 "Bug Tracker" = "https://github.com/ouoertheo/silero-api-server/issues"
 
+[tool.hatch.version]
+source = "vcs"
 
 [tool.hatch.build.targets.wheel]
 only-include = ["silero_api_server"]
```

### Comparing `silero_api_server-0.1.1/PKG-INFO` & `silero_api_server-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.1.1
+Version: 0.1.4
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

