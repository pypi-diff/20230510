# Comparing `tmp/mafic-2.3.0.tar.gz` & `tmp/mafic-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.3.0.tar", max compression
+gzip compressed data, was "mafic-2.3.1.tar", max compression
```

## Comparing `mafic-2.3.0.tar` & `mafic-2.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-05-03 21:28:02.914935 mafic-2.3.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-05-03 21:28:02.914935 mafic-2.3.0/README.md
--rw-r--r--   0        0        0      886 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/ip.py
--rw-r--r--   0        0        0    39072 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/node.py
--rw-r--r--   0        0        0    24313 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/plugin.py
--rw-r--r--   0        0        0     8715 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-05-03 21:28:02.914935 mafic-2.3.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-05-03 21:28:02.914935 mafic-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-09 22:38:17.961736 mafic-2.3.1/LICENSE
+-rw-r--r--   0        0        0     3315 2023-05-09 22:38:17.961736 mafic-2.3.1/README.md
+-rw-r--r--   0        0        0      886 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/ip.py
+-rw-r--r--   0        0        0    39072 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/node.py
+-rw-r--r--   0        0        0    24952 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/plugin.py
+-rw-r--r--   0        0        0     8715 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-05-09 22:38:17.961736 mafic-2.3.1/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-05-09 22:38:17.965736 mafic-2.3.1/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-05-09 22:38:17.965736 mafic-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.3.1/PKG-INFO
```

### Comparing `mafic-2.3.0/LICENSE` & `mafic-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/README.md` & `mafic-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/__init__.py` & `mafic-2.3.1/mafic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.3.0/mafic/__libraries.py` & `mafic-2.3.1/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/__main__.py` & `mafic-2.3.1/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/errors.py` & `mafic-2.3.1/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/events.py` & `mafic-2.3.1/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/filter.py` & `mafic-2.3.1/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/ip.py` & `mafic-2.3.1/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/node.py` & `mafic-2.3.1/mafic/node.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/player.py` & `mafic-2.3.1/mafic/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """A Player is used to connect to a channel."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
+import asyncio
+from asyncio import Event
 from collections import OrderedDict
 from functools import reduce
 from logging import getLogger
 from operator import or_
 from time import time
 from typing import TYPE_CHECKING, Generic, cast
 
@@ -98,14 +100,17 @@
         self._ping = -1
         self._current: Track | None = None
         self._filters: OrderedDict[str, Filter] = OrderedDict()
         # Used to get the last track for TrackEndEvent.
         self._last_track: Track | None = None
         self._paused: bool = False
 
+        self._voice_server_update_event: Event = Event()
+        self._voice_state_update_event: Event = Event()
+
     def set_state(self, state: PlayerPayload) -> None:
         """Set the state of the player.
 
         .. note::
 
             This is used internally to set the state of the player.
             You should not need to use this.
@@ -330,25 +335,28 @@
         self._session_id = data["session_id"]
 
         channel_id = data["channel_id"]
 
         if channel_id is None:  # pyright: ignore[reportUnnecessaryComparison]
             # This can happen and is on disconnect.
             # Not sure why this is typed as always Snowflake.
-            return self.cleanup()
+            await self.disconnect(force=True)
+            return
 
         channel = self.guild.get_channel(int(channel_id))
         if not isinstance(channel, (VoiceChannel, StageChannel)):
             msg = "Channel was not a connectable channel that was recognised."
             raise TypeError(msg)
 
         self.channel = channel
 
-        if self._session_id != before_session_id:  # noqa: RET503
-            await self._dispatch_player_update()  # noqa: RET503
+        if self._session_id != before_session_id:
+            await self._dispatch_player_update()
+
+        self._voice_state_update_event.set()
 
     async def on_voice_server_update(self, data: VoiceServerUpdatePayload) -> None:
         """Handle a voice server update.
 
         This is called by the library and usually should not be called by the user.
 
         Parameters
@@ -376,18 +384,20 @@
         self._node.add_player(self._guild_id, self)
 
         self._guild_id = int(data["guild_id"])
         self._server_state = data
 
         await self._dispatch_player_update()
 
+        self._voice_server_update_event.set()
+
     async def connect(
         self,
         *,
-        timeout: float,  # noqa: ARG002
+        timeout: float,
         reconnect: bool,  # noqa: ARG002
         self_mute: bool = False,
         self_deaf: bool = False,
     ) -> None:
         """Connect to a voice channel.
 
         This is called by your Discord library when using ``Connectable.connect``.
@@ -411,15 +421,27 @@
             raise NoNodesAvailable
 
         _log.debug("Connecting to voice channel %s", self.channel.id)
 
         await self.channel.guild.change_voice_state(
             channel=self.channel, self_mute=self_mute, self_deaf=self_deaf
         )
-        self._connected = True
+        futures = [
+            self._voice_state_update_event.wait(),
+            self._voice_server_update_event.wait(),
+        ]
+
+        ensured = [asyncio.ensure_future(fut) for fut in futures]
+        _, pending = await asyncio.wait(
+            ensured, timeout=timeout, return_when=asyncio.ALL_COMPLETED
+        )
+
+        if len(pending) != 0:
+            await self.disconnect(force=True)
+            raise asyncio.TimeoutError
 
     async def disconnect(self, *, force: bool = False) -> None:
         """Disconnect from the voice channel.
 
         Parameters
         ----------
         force:
```

### Comparing `mafic-2.3.0/mafic/playlist.py` & `mafic-2.3.1/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/plugin.py` & `mafic-2.3.1/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/pool.py` & `mafic-2.3.1/mafic/pool.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/region.py` & `mafic-2.3.1/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/search_type.py` & `mafic-2.3.1/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/stats.py` & `mafic-2.3.1/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/strategy.py` & `mafic-2.3.1/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/track.py` & `mafic-2.3.1/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/type_variables.py` & `mafic-2.3.1/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/typings/common.py` & `mafic-2.3.1/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/typings/http.py` & `mafic-2.3.1/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/typings/incoming.py` & `mafic-2.3.1/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/typings/misc.py` & `mafic-2.3.1/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/typings/outgoing.py` & `mafic-2.3.1/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/utils/classproperty.py` & `mafic-2.3.1/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/mafic/warnings.py` & `mafic-2.3.1/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.3.0/pyproject.toml` & `mafic-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.3.0"
+version = "2.3.1"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.3.0/PKG-INFO` & `mafic-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.3.0
+Version: 2.3.1
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

