# Comparing `tmp/wyoming_faster_whisper-0.0.2.tar.gz` & `tmp/wyoming_faster_whisper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_faster_whisper-0.0.2.tar", last modified: Tue May  9 19:41:26 2023, max compression
+gzip compressed data, was "wyoming_faster_whisper-0.0.3.tar", last modified: Wed May 10 14:43:47 2023, max compression
```

## Comparing `wyoming_faster_whisper-0.0.2.tar` & `wyoming_faster_whisper-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-05-03 14:29:10.000000 wyoming_faster_whisper-0.0.2/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3837 2023-05-03 17:15:52.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/download.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/feature_extractor.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/transcribe.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2199 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-09 19:41:26.123894 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-09 19:41:26.000000 wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-05-10 14:43:21.000000 wyoming_faster_whisper-0.0.3/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3837 2023-05-10 14:42:35.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/download.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/feature_extractor.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/transcribe.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2199 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/handler.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/top_level.txt
```

### Comparing `wyoming_faster_whisper-0.0.2/PKG-INFO` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wyoming_faster_whisper
-Version: 0.0.2
+Name: wyoming-faster-whisper
+Version: 0.0.3
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.2/setup.py` & `wyoming_faster_whisper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_faster_whisper",
-    version="0.0.2",
+    version="0.0.3",
     description="Wyoming Server for Faster Whisper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/__main__.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -73,19 +73,19 @@
     if model_dir is None:
         _LOGGER.info("Downloading %s to %s", model, args.download_dir)
         model_dir = download_model(model, args.download_dir)
 
     if args.language and (args.language != "auto"):
         _LOGGER.debug("Language: %s", args.language)
         languages = [args.language]
+    else:
+        languages = WHISPER_LANGUAGES
 
         # Whisper does not understand "auto"
         args.language = None
-    else:
-        languages = WHISPER_LANGUAGES
 
     wyoming_info = Info(
         asr=[
             AsrProgram(
                 name="faster-whisper",
                 attribution=Attribution(
                     name="Guillaume Klein",
```

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/const.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/download.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/feature_extractor.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/faster_whisper/transcribe.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/file_hash.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper/handler.py` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/handler.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/PKG-INFO` & `wyoming_faster_whisper-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wyoming-faster-whisper
-Version: 0.0.2
+Name: wyoming_faster_whisper
+Version: 0.0.3
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.2/wyoming_faster_whisper.egg-info/SOURCES.txt` & `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

