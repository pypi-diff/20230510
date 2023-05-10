# Comparing `tmp/tuneflow-py-0.8.0.tar.gz` & `tmp/tuneflow-py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.8.0.tar", last modified: Mon May  8 19:32:52 2023, max compression
+gzip compressed data, was "tuneflow-py-0.8.1.tar", last modified: Wed May 10 04:52:58 2023, max compression
```

## Comparing `tuneflow-py-0.8.0.tar` & `tuneflow-py-0.8.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.8.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.8.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-05-08 19:32:04.000000 tuneflow-py-0.8.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.476665 tuneflow-py-0.8.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.476665 tuneflow-py-0.8.0/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.8.0/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      839 2023-05-08 17:27:14.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4283 2023-05-07 06:46:25.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5088 2023-05-08 17:24:18.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5581 2023-05-07 06:47:53.000000 tuneflow-py-0.8.0/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.8.0/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-08 19:32:52.000000 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-05-08 19:32:52.000000 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-08 19:32:52.000000 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-05-08 19:32:52.000000 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-05-08 19:32:52.000000 tuneflow-py-0.8.0/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-08 19:32:52.486665 tuneflow-py-0.8.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.8.0/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.8.0/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/test/test_lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.8.0/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.8.0/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.8.0/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.8.0/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.8.0/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.8.0/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.8.1/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.8.1/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-05-10 04:51:15.000000 tuneflow-py-0.8.1/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.8.1/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      839 2023-05-08 17:27:14.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4283 2023-05-07 06:46:25.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5088 2023-05-08 17:24:18.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5581 2023-05-07 06:47:53.000000 tuneflow-py-0.8.1/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    34271 2023-05-10 04:28:18.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.8.1/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-10 04:52:58.000000 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-05-10 04:52:58.000000 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-10 04:52:58.000000 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-05-10 04:52:58.000000 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-05-10 04:52:58.000000 tuneflow-py-0.8.1/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-10 04:52:58.599577 tuneflow-py-0.8.1/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    30358 2023-05-10 04:29:39.000000 tuneflow-py-0.8.1/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.8.1/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/test/test_lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.8.1/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.8.1/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.8.1/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.8.1/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.8.1/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.8.1/test/test_utils.py
```

### Comparing `tuneflow-py-0.8.0/LICENSE` & `tuneflow-py-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/PKG-INFO` & `tuneflow-py-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.8.0/README.md` & `tuneflow-py-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/pyproject.toml` & `tuneflow-py-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.8.0"
+version = "0.8.1"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/__init__.py` & `tuneflow-py-0.8.1/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.8.1/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/common.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/common.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.8.1/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,14 +405,26 @@
         Sets a new audio file.
         '''
         self._proto.audio_clip_data.audio_file_path = file_path
         self._proto.audio_clip_data.start_tick = start_tick
         self._proto.audio_clip_data.duration = duration
         self._proto.audio_clip_data.speed_ratio = 1
         self._proto.audio_clip_data.pitch_offset = 0
+    
+    def set_audio_data(self, data: bytes, format: str, start_tick: int, duration: float):
+        '''
+        Sets to hole a new temporary audio data.
+        '''
+        self._proto.audio_clip_data.ClearField('audio_file_path')
+        self._proto.audio_clip_data.audio_data.data = data
+        self._proto.audio_clip_data.audio_data.format = format
+        self._proto.audio_clip_data.start_tick = start_tick
+        self._proto.audio_clip_data.duration = duration
+        self._proto.audio_clip_data.speed_ratio = 1
+        self._proto.audio_clip_data.pitch_offset = 0
 
     def clear_notes(self):
         del self._proto.notes[:]
 
     def delete_from_parent(self, delete_associated_track_automation: bool):
         if self.track is not None:
             self.track.delete_clip(self, delete_associated_track_automation)
```

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/lyric.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/note.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/song.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/models/track.py` & `tuneflow-py-0.8.1/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py/utils.py` & `tuneflow-py-0.8.1/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.8.1/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.8.0
+Version: 0.8.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.8.0/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.8.1/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_audio_clip.py` & `tuneflow-py-0.8.1/test/test_audio_clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,62 +79,73 @@
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=480,
             audio_clip_data=TEST_AUDIO_CLIP_DATA,
         )
         self.assertEqual(clip1.get_clip_end_tick(), 1440)
         self.assertEqual(clip1.get_audio_duration(), 1)
         self.assertEqual(clip1.get_audio_end_tick(), 1440)
-        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, TEST_AUDIO_CLIP_DATA["audio_file_path"])
-        self.assertEqual(clip1.get_audio_clip_data().start_tick, TEST_AUDIO_CLIP_DATA["start_tick"])
-        self.assertAlmostEqual(clip1.get_audio_clip_data().duration, TEST_AUDIO_CLIP_DATA["duration"])
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path,
+                         TEST_AUDIO_CLIP_DATA["audio_file_path"])
+        self.assertEqual(clip1.get_audio_clip_data().start_tick,
+                         TEST_AUDIO_CLIP_DATA["start_tick"])
+        self.assertAlmostEqual(clip1.get_audio_clip_data(
+        ).duration, TEST_AUDIO_CLIP_DATA["duration"])
 
     def test_get_audio_related_fields_with_audio_data(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=480,
             audio_clip_data=TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA,
         )
         self.assertEqual(clip1.get_clip_end_tick(), 1440)
         self.assertEqual(clip1.get_audio_duration(), 1)
         self.assertEqual(clip1.get_audio_end_tick(), 1440)
         self.assertEqual(clip1.get_audio_clip_data().audio_file_path, "")
         self.assertEqual(clip1.get_audio_clip_data().audio_data.format,
                          TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["audio_data"]["format"])
         self.assertEqual(clip1.get_audio_clip_data().audio_data.data,
                          TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["audio_data"]["data"])
-        self.assertEqual(clip1.get_audio_clip_data().start_tick, TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["start_tick"])
-        self.assertAlmostEqual(clip1.get_audio_clip_data().duration, TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["duration"])
+        self.assertEqual(clip1.get_audio_clip_data().start_tick,
+                         TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["start_tick"])
+        self.assertAlmostEqual(clip1.get_audio_clip_data(
+        ).duration, TEST_AUDIO_CLIP_DATA_WITH_AUDIO_DATA["duration"])
 
     def test_set_and_get_custom_clip_start_and_end_tick_out_of_audio_range(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=120,
             clip_end_tick=9000,
             audio_clip_data=TEST_AUDIO_CLIP_DATA,
         )
         self.assertEqual(clip1.get_clip_start_tick(), 480)
         self.assertEqual(clip1.get_clip_end_tick(), 1440)
         self.assertEqual(clip1.get_audio_duration(), 1)
         self.assertEqual(clip1.get_audio_end_tick(), 1440)
-        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, TEST_AUDIO_CLIP_DATA["audio_file_path"])
-        self.assertEqual(clip1.get_audio_clip_data().start_tick, TEST_AUDIO_CLIP_DATA["start_tick"])
-        self.assertAlmostEqual(clip1.get_audio_clip_data().duration, TEST_AUDIO_CLIP_DATA["duration"])
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path,
+                         TEST_AUDIO_CLIP_DATA["audio_file_path"])
+        self.assertEqual(clip1.get_audio_clip_data().start_tick,
+                         TEST_AUDIO_CLIP_DATA["start_tick"])
+        self.assertAlmostEqual(clip1.get_audio_clip_data(
+        ).duration, TEST_AUDIO_CLIP_DATA["duration"])
 
     def test_set_and_get_custom_clip_start_and_end_tick_within_audio_range(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=960,
             clip_end_tick=1000,
             audio_clip_data=TEST_AUDIO_CLIP_DATA,
         )
         self.assertEqual(clip1.get_clip_start_tick(), 960)
         self.assertEqual(clip1.get_clip_end_tick(), 1000)
         self.assertEqual(clip1.get_audio_duration(), 1)
         self.assertEqual(clip1.get_audio_end_tick(), 1440)
-        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, TEST_AUDIO_CLIP_DATA["audio_file_path"])
-        self.assertEqual(clip1.get_audio_clip_data().start_tick, TEST_AUDIO_CLIP_DATA["start_tick"])
-        self.assertAlmostEqual(clip1.get_audio_clip_data().duration, TEST_AUDIO_CLIP_DATA["duration"])
-    
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path,
+                         TEST_AUDIO_CLIP_DATA["audio_file_path"])
+        self.assertEqual(clip1.get_audio_clip_data().start_tick,
+                         TEST_AUDIO_CLIP_DATA["start_tick"])
+        self.assertAlmostEqual(clip1.get_audio_clip_data(
+        ).duration, TEST_AUDIO_CLIP_DATA["duration"])
+
     def test_get_optional_clip_audio_data_fields(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=960,
             clip_end_tick=1440,
             audio_clip_data={
                 "start_tick": 480,
                 "audio_file_path": 'file1',
@@ -249,14 +260,75 @@
         self.assertEqual(clip1.get_audio_duration(), 2)
         self.assertEqual(clip1.get_audio_start_tick(), 0)
         self.assertEqual(clip1.get_audio_end_tick(), 1680)
         self.assertEqual(clip1.get_clip_start_tick(), 960)
         self.assertEqual(clip1.get_clip_end_tick(), 1680)
         self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 0.5)
 
+    def test_set_audio_file(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1,
+            },
+        )
+        clip1.time_stretch_from_clip_right(1200)
+        clip1.set_audio_pitch_offset(1.0)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 2.0)
+        self.assertAlmostEqual(clip1.get_audio_pitch_offset(), 1.0)
+        self.assertAlmostEqual(clip1.get_audio_duration(), 0.5)
+        self.assertAlmostEqual(clip1.get_audio_start_tick(), 720)
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, 'file1')
+
+        clip1.set_audio_file(file_path='file2', start_tick=120, duration=2)
+
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 1.0)
+        self.assertAlmostEqual(clip1.get_audio_pitch_offset(), 0.0)
+        self.assertAlmostEqual(clip1.get_audio_duration(), 2.0)
+        self.assertAlmostEqual(clip1.get_audio_start_tick(), 120)
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, 'file2')
+
+    def test_set_audio_data(self):
+        clip1 = self.audio_track.create_audio_clip(
+            clip_start_tick=960,
+            clip_end_tick=1440,
+            audio_clip_data={
+                "start_tick": 480,
+                "audio_file_path": 'file1',
+                "duration": 1,
+            },
+        )
+        clip1.time_stretch_from_clip_right(1200)
+        clip1.set_audio_pitch_offset(1.0)
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 2.0)
+        self.assertAlmostEqual(clip1.get_audio_pitch_offset(), 1.0)
+        self.assertAlmostEqual(clip1.get_audio_duration(), 0.5)
+        self.assertAlmostEqual(clip1.get_audio_start_tick(), 720)
+        self.assertEqual(clip1.get_audio_clip_data().audio_file_path, 'file1') #type:ignore
+        self.assertTrue(
+            clip1.get_audio_clip_data().HasField('audio_file_path')) #type:ignore
+        self.assertFalse(
+            clip1.get_audio_clip_data().HasField('audio_data')) #type:ignore
+        
+        clip1.set_audio_data(data=bytes(), format='mp3',
+                             start_tick=120, duration=2)
+
+        self.assertAlmostEqual(clip1.get_audio_speed_ratio(), 1.0)
+        self.assertAlmostEqual(clip1.get_audio_pitch_offset(), 0.0)
+        self.assertAlmostEqual(clip1.get_audio_duration(), 2.0)
+        self.assertAlmostEqual(clip1.get_audio_start_tick(), 120)
+        self.assertFalse(
+            clip1.get_audio_clip_data().HasField('audio_file_path')) #type:ignore
+        self.assertTrue(
+            clip1.get_audio_clip_data().audio_data.HasField('data')) #type:ignore
+        self.assertEqual(clip1.get_audio_clip_data().audio_data.format, 'mp3') #type:ignore
+
 
 class TestTrimLeftAndTrimRight(BaseTestCase):
     def test_trim_left_within_audio_range(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=960,
             clip_end_tick=1000,
             audio_clip_data=TEST_AUDIO_CLIP_DATA,
@@ -441,29 +513,44 @@
             audio_clip_data={
                 "audio_file_path": 'file2',
                 "start_tick": 240,
                 "duration": 0.5,
             },
         )
         self.assertEqual(self.audio_track.get_clip_count(), 3)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_start_tick(), 0)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_end_tick(), 239)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().audio_file_path, 'file1')
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().duration, 1)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().start_tick, 0)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_start_tick(), 240)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_end_tick(), 720)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().audio_file_path, 'file2')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().duration, 0.5)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().start_tick, 240)
-        self.assertEqual(self.audio_track.get_clip_at(2).get_clip_start_tick(), 721)
-        self.assertEqual(self.audio_track.get_clip_at(2).get_clip_end_tick(), 960)
-        self.assertEqual(self.audio_track.get_clip_at(2).get_audio_clip_data().audio_file_path, 'file1')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(2).get_audio_clip_data().duration, 1)
-        self.assertEqual(self.audio_track.get_clip_at(2).get_audio_clip_data().start_tick, 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_start_tick(), 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_end_tick(), 239)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().audio_file_path, 'file1')
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().duration, 1)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().start_tick, 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_start_tick(), 240)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_end_tick(), 720)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().audio_file_path, 'file2')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().duration, 0.5)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().start_tick, 240)
+        self.assertEqual(self.audio_track.get_clip_at(
+            2).get_clip_start_tick(), 721)
+        self.assertEqual(self.audio_track.get_clip_at(
+            2).get_clip_end_tick(), 960)
+        self.assertEqual(self.audio_track.get_clip_at(
+            2).get_audio_clip_data().audio_file_path, 'file1')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            2).get_audio_clip_data().duration, 1)
+        self.assertEqual(self.audio_track.get_clip_at(
+            2).get_audio_clip_data().start_tick, 0)
 
     def test_create_clip_to_the_left_of_another_clip(self):
         self.audio_track.create_audio_clip(
             clip_start_tick=0,
             clip_end_tick=960,
             audio_clip_data={
                 "audio_file_path": 'file1',
@@ -477,24 +564,34 @@
             audio_clip_data={
                 "audio_file_path": 'file2',
                 "start_tick": 0,
                 "duration": 0.25,
             },
         )
         self.assertEqual(self.audio_track.get_clip_count(), 2)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_start_tick(), 0)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_end_tick(), 240)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().audio_file_path, 'file2')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().duration, 0.25)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().start_tick, 0)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_start_tick(), 241)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_end_tick(), 960)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().audio_file_path, 'file1')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().duration, 1)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().start_tick, 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_start_tick(), 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_end_tick(), 240)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().audio_file_path, 'file2')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().duration, 0.25)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().start_tick, 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_start_tick(), 241)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_end_tick(), 960)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().audio_file_path, 'file1')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().duration, 1)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().start_tick, 0)
 
     def test_create_clip_to_the_right_of_another_clip(self):
         self.audio_track.create_audio_clip(
             clip_start_tick=0,
             clip_end_tick=960,
             audio_clip_data={
                 "audio_file_path": 'file1',
@@ -508,25 +605,35 @@
             audio_clip_data={
                 "audio_file_path": 'file2',
                 "start_tick": 720,
                 "duration": 0.25,
             },
         )
         self.assertEqual(self.audio_track.get_clip_count(), 2)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_start_tick(), 0)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_clip_end_tick(), 719)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().audio_file_path, 'file1')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().duration, 1)
-        self.assertEqual(self.audio_track.get_clip_at(0).get_audio_clip_data().start_tick, 0)
-
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_start_tick(), 720)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_clip_end_tick(), 960)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().audio_file_path, 'file2')
-        self.assertAlmostEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().duration, 0.25)
-        self.assertEqual(self.audio_track.get_clip_at(1).get_audio_clip_data().start_tick, 720)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_start_tick(), 0)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_clip_end_tick(), 719)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().audio_file_path, 'file1')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().duration, 1)
+        self.assertEqual(self.audio_track.get_clip_at(
+            0).get_audio_clip_data().start_tick, 0)
+
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_start_tick(), 720)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_clip_end_tick(), 960)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().audio_file_path, 'file2')
+        self.assertAlmostEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().duration, 0.25)
+        self.assertEqual(self.audio_track.get_clip_at(
+            1).get_audio_clip_data().start_tick, 720)
 
     def test_trim_left_edge_overlaps_with_another_clip(self):
         clip1 = self.audio_track.create_audio_clip(
             clip_start_tick=0,
             clip_end_tick=480,
             audio_clip_data={
                 "audio_file_path": 'file1',
```

### Comparing `tuneflow-py-0.8.0/test/test_automation.py` & `tuneflow-py-0.8.1/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_lyric.py` & `tuneflow-py-0.8.1/test/test_lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_marker.py` & `tuneflow-py-0.8.1/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_midi_clip.py` & `tuneflow-py-0.8.1/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_note.py` & `tuneflow-py-0.8.1/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_song.py` & `tuneflow-py-0.8.1/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_track.py` & `tuneflow-py-0.8.1/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.8.0/test/test_utils.py` & `tuneflow-py-0.8.1/test/test_utils.py`

 * *Files identical despite different names*

