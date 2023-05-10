# Comparing `tmp/elevenlabslib-0.6.1.tar.gz` & `tmp/elevenlabslib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.6.1.tar", last modified: Sun May  7 11:13:14 2023, max compression
+gzip compressed data, was "elevenlabslib-0.7.0.tar", last modified: Wed May 10 20:41:45 2023, max compression
```

## Comparing `elevenlabslib-0.6.1.tar` & `elevenlabslib-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.184857 elevenlabslib-0.6.1/elevenlabslib/
--rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    14498 2023-05-06 21:48:53.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    33572 2023-05-05 17:09:22.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.6.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5592 2023-04-30 12:39:02.000000 elevenlabslib-0.6.1/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.199857 elevenlabslib-0.6.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-07 11:12:39.000000 elevenlabslib-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.597517 elevenlabslib-0.7.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-10 20:41:45.596521 elevenlabslib-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.581520 elevenlabslib-0.7.0/elevenlabslib/
+-rw-rw-rw-   0        0        0     4629 2023-05-10 20:06:36.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    15016 2023-05-10 20:10:15.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    36538 2023-05-10 20:40:35.000000 elevenlabslib-0.7.0/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.0/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-10 20:36:24.000000 elevenlabslib-0.7.0/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-10 20:41:45.595517 elevenlabslib-0.7.0/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 20:41:45.000000 elevenlabslib-0.7.0/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-10 20:38:23.000000 elevenlabslib-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 20:41:45.597517 elevenlabslib-0.7.0/setup.cfg
```

### Comparing `elevenlabslib-0.6.1/LICENSE` & `elevenlabslib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.1/PKG-INFO` & `elevenlabslib-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.6.1
+Version: 0.7.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.6.1/README.md` & `elevenlabslib-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from elevenlabslib.helpers import _api_json,_api_del,_api_get,_api_multipart
 
 
 class ElevenLabsHistoryItem:
     """
     Represents a previously generated audio.
 
-    Note:
-        There is no way to get an instance of ElevenLabsHistoryItem from a historyID, as there is no endpoint that returns that information.
-
     Tip:
         There is no method to get an ElevenLabsVoice object for the voice that was used to create the file as it may not exist anymore.
         You can use the voiceID for that.
     """
     def __init__(self, data:dict, parentUser:ElevenLabsUser):
         """
         Initializes a new instance of the ElevenLabsHistoryItem class.
@@ -27,25 +24,34 @@
         self._historyID = data["history_item_id"]
         self._voiceId = data["voice_id"]
         self._voiceName = data["voice_name"]
         self._text = data["text"]
         self._dateUnix = data["date_unix"]
         self._characterCountChangeFrom = data["character_count_change_from"]
         self._characterCountChangeTo = data["character_count_change_to"]
+        self._settingsUsed = data["settings"]
+        self._feedbackData = data["feedback"]
         self._fullMetadata = data
         self._audioData = None
 
     @property
     def metadata(self):
         """
         All the metadata associated with the item.
         """
         return self._fullMetadata
 
     @property
+    def settings_used(self):
+        """
+        The settings used for this generation.
+        """
+        return self._settingsUsed
+
+    @property
     def historyID(self):
         """
         The ID of the history item.
         """
         return self._historyID
 
     @property
```

### Comparing `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsUser.py`

 * *Files 4% similar despite different names*

```diff
@@ -212,14 +212,28 @@
         outputList = list()
         response = _api_get("/history", headers=self._headers)
         historyData = response.json()
         from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
         for value in historyData["history"]:
             outputList.append(ElevenLabsHistoryItem(value, self))
         return outputList
+
+    def get_history_item(self, historyItemID) -> ElevenLabsHistoryItem:
+        """
+        Args:
+            historyItemID: The HistoryItem ID.
+
+        Returns:
+            ElevenLabsHistoryItem: The corresponding ElevenLabsHistoryItem
+        """
+        response = _api_get(f"/history/{historyItemID}", headers=self._headers)
+        historyData = response.json()
+        from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
+        return ElevenLabsHistoryItem(historyData, self)
+
     def download_history_items(self, historyItems:list[str|ElevenLabsHistoryItem]) -> dict[str, bytes]:
         """
             Download multiple history items and return a dictionary where the key is the history ID
             and the value is the bytes of the mp3 file.
 
             Args:
                 historyItems (list[str|ElevenLabsHistoryItem]): List of history items (or their IDs) to download.
```

### Comparing `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.7.0/elevenlabslib/ElevenLabsVoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import os
 import queue
 
 import threading
 from typing import Optional, Tuple, Any
+from warnings import warn
 
 import soundfile as sf
 import sounddevice as sd
 
 from typing import TYPE_CHECKING
 
 
+
 if TYPE_CHECKING:
     from elevenlabslib.ElevenLabsSample import ElevenLabsSample
     from elevenlabslib.ElevenLabsUser import ElevenLabsUser
+    from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
 
 from elevenlabslib.helpers import *
 from elevenlabslib.helpers import _api_json,_api_del,_api_get,_api_multipart
 
 
 # These are hardcoded because they just plain work. If you really want to change them, please be careful.
 _playbackBlockSize = 2048
@@ -167,66 +170,97 @@
             if not (0 <= stability <= 1 and 0 <= similarity_boost <= 1):
                 raise ValueError("Please provide a value between 0 and 1.")
             payload["voice_settings"] = dict()
             payload["voice_settings"]["stability"] = stability
             payload["voice_settings"]["similarity_boost"] = similarity_boost
         return payload
 
-    def generate_audio_bytes(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None, model_id:str="eleven_monolingual_v1") -> bytes:
+    def generate_to_historyID(self, prompt: str, stability: Optional[float] = None, similarity_boost: Optional[float] = None, model_id: str = "eleven_monolingual_v1") -> str:
+        """
+        Generate audio bytes from the given prompt and returns the historyItemID corresponding to it.
+
+        Parameters:
+            prompt (str): The text prompt to generate audio from.
+            stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
+            similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
+            model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
+
+        Returns:
+            The ID for the new HistoryItem
         """
-        Generates speech for the given prompt and returns the audio data as bytes of an mp3 file.
+        payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
+        response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload, stream=True)
+
+        return response.headers["history-item-id"]
+
+    def generate_audio(self, prompt: str, stability: Optional[float] = None, similarity_boost: Optional[float] = None, model_id: str = "eleven_monolingual_v1") -> tuple[bytes,str]:
+        """
+        Generates speech for the given prompt and returns the audio data as bytes of an mp3 file alongside the new historyID.
 
         Tip:
             If you would like to save the audio to disk or otherwise, you can use helpers.save_audio_bytes().
 
         Args:
-        	prompt: The prompt to generate speech for.
-        	stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
-        	similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
-        	model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
+            prompt: The prompt to generate speech for.
+            stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
+            similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
+            model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
         Returns:
-        	The bytes of the audio file.
+            A tuple consisting of the bytes of the audio file and its historyID.
 
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
+        return response.content, response.headers["history-item-id"]
+    def generate_audio_bytes(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None, model_id:str="eleven_monolingual_v1") -> bytes:
+        warn("This function is deprecated. Please use generate_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
+        payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
+        response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
 
-        return response.content
 
-    def generate_and_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
+        return response.content
+    def generate_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
-                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1"):
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> tuple[bytes,str]:
         """
         Generate audio bytes from the given prompt and play them using sounddevice.
 
         Tip:
             This function downloads the entire file before playing it back, and even if playInBackground is set, it will halt execution until the file is downloaded.
             If you need faster response times and background downloading and playback, use generate_and_stream_audio.
 
         Parameters:
-        	prompt (str): The text prompt to generate audio from.
-        	playInBackground (bool): Whether to play audio in the background or wait for it to finish playing.
-        	portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
-        	stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
-        	similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
-        	onPlaybackStart: Function to call once the playback begins
-        	onPlaybackEnd: Function to call once the playback ends
-        	model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
+            prompt (str): The text prompt to generate audio from.
+            playInBackground (bool): Whether to play audio in the background or wait for it to finish playing.
+            portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
+            stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
+            similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
+            onPlaybackStart: Function to call once the playback begins
+            onPlaybackEnd: Function to call once the playback ends
+            model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
 
         Returns:
-            The audio bytes.
+           A tuple consisting of the bytes of the audio file and its historyID.
         """
+        audioData, historyID = self.generate_audio(prompt, stability, similarity_boost, model_id)
+        play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
+        return audioData, historyID
+
+    def generate_and_play_audio(self, prompt:str, playInBackground:bool, portaudioDeviceID:Optional[int] = None,
+                                stability:Optional[float]=None, similarity_boost:Optional[float]=None,
+                                onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> bytes:
+        warn("This function is deprecated. Please use generate_play_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
         audioData = self.generate_audio_bytes(prompt, stability, similarity_boost, model_id)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
         return audioData
 
     def generate_and_stream_audio(self, prompt:str, portaudioDeviceID:Optional[int] = None,
                                   stability:Optional[float]=None, similarity_boost:Optional[float]=None, streamInBackground=False,
-                                  onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0):
+                                  onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> str:
         """
 
         Note:
             The latencyOptimizationLevel ranges from 0 to 4. Each level trades off some more quality for speed.
 
             The levels are as follows:
                 - 0: Normal, no optimizations applied
@@ -246,29 +280,31 @@
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
             latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply.
 
+        Returns:
+            The historyID for the newly created item.
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         path = "/text-to-speech/" + self._voiceID + "/stream"
 
         streamedResponse = requests.post(api_endpoint + path, headers=self._linkedUser.headers, json=payload, stream=True, params={"optimize_streaming_latency":latencyOptimizationLevel})
 
         streamer = _AudioChunkStreamer(portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
         if streamInBackground:
             mainThread = threading.Thread(target=streamer.begin_streaming, args=(streamedResponse,))
             mainThread.start()
         else:
             streamer.begin_streaming(streamedResponse)
 
-        return
+        return streamedResponse.headers["history-item-id"]
 
 
     def get_preview_url(self) -> str|None:
         """
         Returns:
             str|None: The preview URL of the voice, or None if it hasn't been generated.
         """
```

### Comparing `elevenlabslib-0.6.1/elevenlabslib/__init__.py` & `elevenlabslib-0.7.0/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.1/elevenlabslib/helpers.py` & `elevenlabslib-0.7.0/elevenlabslib/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 import soundfile as sf
 import requests
 import os
 
 api_endpoint = "https://api.elevenlabs.io/v1"
 default_headers = {'accept': '*/*'}
 
-def _api_call(requestType, path, headers, jsonData=None, filesData=None) -> requests.Response:
+def _api_call(requestType, path, headers, jsonData=None, filesData=None, stream=False) -> requests.Response:
     if path[0] != "/":
         path = "/"+path
 
     if requestType == "get":
         response = requests.get(api_endpoint + path, headers=headers)
     elif requestType == "json":
-        response = requests.post(api_endpoint + path, headers=headers, json=jsonData)
+        response = requests.post(api_endpoint + path, headers=headers, json=jsonData, stream=stream)
     elif requestType == "del":
         response = requests.delete(api_endpoint + path, headers=headers)
     elif requestType == "multipart":
         if filesData is not None:
-            response = requests.post(api_endpoint + path, headers=headers, data=jsonData, files=filesData)
+            response = requests.post(api_endpoint + path, headers=headers, data=jsonData, files=filesData, stream=stream)
         else:
-            response = requests.post(api_endpoint + path, headers=headers, data=jsonData)
+            response = requests.post(api_endpoint + path, headers=headers, data=jsonData, stream=stream)
     else:
         raise ValueError("Unknown API call type!")
 
     try:
         response.raise_for_status()
         return response
     except requests.exceptions.RequestException as e:
@@ -39,18 +39,18 @@
 
 def _api_get(path, headers) -> requests.Response:
     return _api_call("get",path, headers)
 
 def _api_del(path, headers) -> requests.Response:
     return _api_call("del",path, headers)
 
-def _api_json(path, headers, jsonData) -> requests.Response:
-    return _api_call("json",path, headers, jsonData)
+def _api_json(path, headers, jsonData, stream=False) -> requests.Response:
+    return _api_call("json",path, headers, jsonData, stream)
 
-def _api_multipart(path, headers, data=None, filesData=None):
+def _api_multipart(path, headers, data=None, filesData=None, stream=False):
     return _api_call("multipart", path, headers, data, filesData)
 
 def _pretty_print_POST(res:requests.Response):
     req = res.request
     logging.debug(f"RESPONSE DATA: {res.text}")
     logging.debug('REQUEST THAT CAUSED THE ERROR:\n{}\n{}\r\n{}\r\n\r\n{}'.format(
         '-----------START-----------',
@@ -77,14 +77,19 @@
     Returns:
         None
     """
 
     if portaudioDeviceID is None:
         portaudioDeviceID = sd.default.device[1]
 
+    #Let's make sure the user didn't just forward the tuple from one of the generation functions...
+    if isinstance(audioData, tuple):
+        if isinstance(audioData[0], bytes):
+            audioData = audioData[0]
+
     playbackWrapper = _SDPlaybackWrapper(audioData, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
     if not playInBackground:
         with playbackWrapper.stream:
             playbackWrapper.endPlaybackEvent.wait()
     else:
         playbackWrapper.stream.start()
@@ -95,14 +100,18 @@
         soundfile is used for the conversion, so it supports any format it does.
 
         Parameters:
             audioData: The audio data.
             saveLocation: The path (or file-like object) where the data will be saved.
             outputFormat: The format in which the audio will be saved
         """
+    if isinstance(audioData, tuple):
+        if isinstance(audioData[0], bytes):
+            audioData = audioData[0]
+
     tempSoundFile = soundfile.SoundFile(io.BytesIO(audioData))
 
     if isinstance(saveLocation, str):
         with open(saveLocation, "wb") as fp:
             sf.write(fp, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
     else:
         sf.write(saveLocation, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
```

### Comparing `elevenlabslib-0.6.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.7.0/elevenlabslib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.6.1
+Version: 0.7.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.6.1/pyproject.toml` & `elevenlabslib-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.6.1"
+version = "0.7.0"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

