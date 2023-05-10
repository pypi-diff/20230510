# Comparing `tmp/lumaapi-0.0.1.tar.gz` & `tmp/lumaapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumaapi-0.0.1.tar", last modified: Fri May  5 02:17:32 2023, max compression
+gzip compressed data, was "lumaapi-0.0.2.tar", last modified: Wed May 10 17:21:31 2023, max compression
```

## Comparing `lumaapi-0.0.1.tar` & `lumaapi-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 02:17:32.257935 lumaapi-0.0.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)      138 2023-05-05 01:32:56.000000 lumaapi-0.0.1/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)      960 2023-05-05 02:17:32.257935 lumaapi-0.0.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      567 2023-05-05 01:32:07.000000 lumaapi-0.0.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 02:17:32.257935 lumaapi-0.0.1/lumaapi/
--rw-rw-r--   0 alex      (1000) alex      (1000)    14078 2023-05-05 02:10:19.000000 lumaapi-0.0.1/lumaapi/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 02:17:32.257935 lumaapi-0.0.1/lumaapi.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      960 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      277 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       56 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-05-05 02:17:32.000000 lumaapi-0.0.1/lumaapi.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      719 2023-05-05 02:15:41.000000 lumaapi-0.0.1/pyproject.toml
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 02:17:32.257935 lumaapi-0.0.1/scripts/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1192 2023-05-05 02:05:29.000000 lumaapi-0.0.1/scripts/run_lumaapi.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      116 2023-05-05 02:17:32.257935 lumaapi-0.0.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 17:21:31.808676 lumaapi-0.0.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      138 2023-05-05 01:32:56.000000 lumaapi-0.0.2/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-05-10 17:21:31.808676 lumaapi-0.0.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      829 2023-05-10 17:21:01.000000 lumaapi-0.0.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 17:21:31.808676 lumaapi-0.0.2/lumaapi/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15402 2023-05-10 17:19:43.000000 lumaapi-0.0.2/lumaapi/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 17:21:31.808676 lumaapi-0.0.2/lumaapi.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      277 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       56 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       16 2023-05-10 17:21:31.000000 lumaapi-0.0.2/lumaapi.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      702 2023-05-10 17:21:18.000000 lumaapi-0.0.2/pyproject.toml
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-10 17:21:31.808676 lumaapi-0.0.2/scripts/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1192 2023-05-05 02:05:29.000000 lumaapi-0.0.2/scripts/run_lumaapi.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      116 2023-05-10 17:21:31.808676 lumaapi-0.0.2/setup.cfg
```

### Comparing `lumaapi-0.0.1/lumaapi/__init__.py` & `lumaapi-0.0.2/lumaapi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import shutil
 from typing import Optional, List, Dict
 import uuid
 import urllib.parse
 from enum import Enum
 from dataclasses import dataclass
 from datetime import datetime
+import enum_tools.documentation
 import time
 import json
 import requests
 
 import platformdirs
 
 
@@ -41,82 +42,103 @@
 
 @dataclass
 class LumaCreditInfo:
     """
     Response of credits query
     """
     remaining: int
-    """ Number of remaining credits """
+    """
+    Number of remaining credits
+    """
 
     used: int
-    """ Number of used credits """
+    """
+    Number of used credits
+    """
 
     total: int
-    """ Number of remaining+used credits """
+    """
+    Number of remaining+used credits
+    """
 
+@enum_tools.documentation.document_enum
 class CaptureType(Enum):
     """
     Capture types.
     Current API version always has RECONSTRUCTION type
-    (generation API not yet available for public)
     """
-    RECONSTRUCTION = 0
-    GENERATION = 1
+    RECONSTRUCTION = 0  # doc: This is the only option
 
     @classmethod
     def parse(cls, name: str) -> "CaptureType":
         return getattr(cls, name.upper(), None)
 
+@enum_tools.documentation.document_enum
 class CameraType(Enum):
     """
     Camera types
     """
-    NORMAL = "normal"
-    """ Perspective camera """
-    FISHEYE = "fisheye"
-    """ Fisheye camera """
-    EQUIRECTANGULAR = "equirectangular"
-    """ Equirectangular 360 camera """
+    NORMAL = "normal" # doc: Perspective camera
+    FISHEYE = "fisheye"  # doc: Fisheye camera
+    EQUIRECTANGULAR = "equirectangular"  # doc: Equirectangular 360 camera
 
     @classmethod
     def parse(cls, name: str) -> "CameraType":
         return getattr(cls, name.upper(), None)
 
 
+@enum_tools.documentation.document_enum
 class PrivacyLevel(Enum):
     """
     Privacy levels for capture
     """
-    PRIVATE = "private"
-    UNLISTED = "unlisted"
-    PUBLIC = "public"
-    OPEN = "open"
+    PRIVATE = "private"  # doc: Fully private (default)
+    UNLISTED = "unlisted" # doc: Unlisted. Sharable by link
+    PUBLIC = "public"  # doc: Shows up in feeds and can be featured
+    OPEN = "open"  # doc: Can be remixed by other users
 
     @classmethod
     def parse(cls, name: str) -> "PrivacyLevel":
         return getattr(cls, name.upper(), None)
 
+@enum_tools.documentation.document_enum
 class CaptureStatus(Enum):
     """
-    Run status
+    Capture upload status. Not to be confused with :class:`.RunStatus`
     """
-    NEW = 0
-    UPLOADING = 0
-    COMPLETE = 1
+    NEW = 0  # doc: New capture, not uploaded
+    UPLOADING = 0  # doc: Capture is uploading
+    COMPLETE = 1 # doc: Capture has finished uploading
 
     @classmethod
     def parse(cls, name: str) -> "CaptureStatus":
         return getattr(cls, name.upper(), None)
 
 @dataclass
 class CaptureLocation:
+    """
+    Capture location information.
+    Current API uploads will not have this information.
+    """
     latitude: float = 0.0
+    """
+    Latitude in deg
+    """
     longitude: float = 0.0
-    name: str = ""
+    """
+    Longitude in deg
+    """
+    name: str = "" 
+    """
+    Name of location if available
+    """
     is_visible: bool = True
+    """
+    Whether location is visible to other users
+    """
 
     @classmethod
     def from_dict(cls, data: Dict) -> "CaptureLocation":
         return cls(
                 latitude=data.get("latitude", 0.0),
                 longitude=data.get("longitude", 0.0),
                 name=data.get("name", ""),
@@ -129,37 +151,47 @@
             "name": self.name,
             "isVisible": self.is_visible
         }
 
 
 class RunStatus(Enum):
     """
-    Run status
+    Capture run status
     """
-    NEW = 0
-    DISPATCHED = 1
-    FAILED = 2
-    FINISHED = 3
+    NEW = 0  # doc: New run in queue
+    DISPATCHED = 1  # doc: Run dispatched to worker
+    FAILED = 2  # doc: Run failed
+    FINISHED = 3  # doc: Run finished
 
     @classmethod
     def parse(cls, name: str) -> "RunStatus":
         return getattr(cls, name.upper(), None)
 
 
 @dataclass
 class LumaRunInfo:
     status: RunStatus
+    """
+    Status of run
+    """
 
     progress: int
-    """ Percentage progress (0-100) """
+    """
+    Percentage progress (0-100)
+    """
 
     current_stage: str
-    """ Current stage of reconstruction for information. Examples are sfm and nerf """
+    """
+    Current stage of reconstruction for information. Examples are sfm and nerf
+    """
 
     artifacts: List[Dict[str, str]]
+    """
+    List of output artifacts (each entry has keys type and url)
+    """
 
 @dataclass
 class LumaCaptureInfo:
     title: str
     """ Capture title """
     type: CaptureType
     """ Capture type. This will currently be reconstruction """
@@ -193,38 +225,59 @@
                     artifacts=lrun["artifacts"],
                 ) if lrun is not None else None
         )
 
 
 class LumaClient:
     """
-    Luma API Python Client.
-    Currently limited to basic video/zip/folder uploads
-    and status checking.
+    Luma API Python Client. Currently limited to basic video/zip/folder uploads and status checking.
+
+    **Library usage:**
 
-    Library usage: :code:`from lumaapi import LumaClient`
+    .. code-block:: python
 
-    CLI usage:
+         from lumaapi import LumaClient
+         client = LumaClient(api_key)
+         slug = client.submit(video_path, title)
+         print(client.status(slug))
 
+    **CLI usage:**
     To submit a video
-    :code:`luma submit <video> <title>`
+
+    .. code-block:: shell
+
+        luma submit <path> <title>
+
+    where path can be a video, zip, or directory.
     This outputs a slug.
 
     To check status of the capture
-    :code:`luma status <slug>`
+
+    .. code-block:: shell
+
+        luma status <slug>
 
     To search user's captures
-    :code:`luma get <title>`
+
+    .. code-block:: shell
+
+        luma get <title>
 
     To manually authenticate
     (the CLI automatically prompts for api-key when running anything else)
-    :code:`luma auth`
+
+    .. code-block:: shell
+
+        luma auth
 
     To check for credits
-    :code:`luma credits`
+
+    .. code-block:: shell
+
+        luma credits
     """
     def __init__(self,
                  api_key: Optional[str] = None,
                  is_cli: bool = False):
         self.auth_header = None
         self.is_cli = is_cli
         if api_key is not None:
@@ -255,15 +308,15 @@
         Update the api_key to the provided api_key.
         Alternatively, if api_key is not given, load the cached API key,
         or ask the user to enter it
         If api_key is updated, runs client.credits() to check its validity.
 
         :param api_key: str, optional, API key to use instead of prompting user
 
-        :return: dict, headers to use for authenticated requests (:code:`Authorization: luma-pai-key=<api_key>`)
+        :return: dict, headers to use for authenticated requests (:code:`Authorization: luma-api-key=<api_key>`)
         """
         os.makedirs(CACHE_DIR, exist_ok=True)
         if api_key is None and self.auth_header is not None:
             result = self.auth_header
         elif api_key is None and os.path.isfile(AUTH_FILE):
             with open(AUTH_FILE, "r") as f:
                 result = json.load(f)
```

### Comparing `lumaapi-0.0.1/pyproject.toml` & `lumaapi-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lumaapi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Luma AI", email = "hello@lumalabs.ai"},
 ]
 description = "Luma AI API wrapper library and CLI"
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["one", "two"]
-license = {text = "BSD-3-Clause"}
+license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "requests",
     "fire",
+    "enum-tools",
     "platformdirs",
 ]
 
 [project.urls]
 Homepage = "https://lumalabs.ai/luma-api"
 
 [tool.setuptools.packages.find]
```

### Comparing `lumaapi-0.0.1/scripts/run_lumaapi.py` & `lumaapi-0.0.2/scripts/run_lumaapi.py`

 * *Files identical despite different names*

