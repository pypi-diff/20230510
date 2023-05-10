# Comparing `tmp/m3u8-3.3.0.tar.gz` & `tmp/m3u8-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3u8-3.3.0.tar", last modified: Sat Aug 20 12:30:23 2022, max compression
+gzip compressed data, was "m3u8-3.4.0.tar", last modified: Thu Dec 29 01:51:28 2022, max compression
```

## Comparing `m3u8-3.3.0.tar` & `m3u8-3.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-08-20 12:30:23.107871 m3u8-3.3.0/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-04-10 23:49:58.000000 m3u8-3.3.0/LICENSE
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2022-04-10 23:49:58.000000 m3u8-3.3.0/MANIFEST.in
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    14627 2022-08-20 12:30:23.107673 m3u8-3.3.0/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    14410 2022-07-25 00:06:47.000000 m3u8-3.3.0/README.rst
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-08-20 12:30:23.106096 m3u8-3.3.0/m3u8/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2419 2022-08-20 12:25:17.000000 m3u8-3.3.0/m3u8/__init__.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1075 2022-04-10 23:49:58.000000 m3u8-3.3.0/m3u8/httpclient.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1590 2022-04-10 23:49:58.000000 m3u8-3.3.0/m3u8/mixins.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    48103 2022-08-20 12:25:17.000000 m3u8-3.3.0/m3u8/model.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    21487 2022-08-20 12:25:17.000000 m3u8-3.3.0/m3u8/parser.py
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1645 2022-08-20 12:25:17.000000 m3u8-3.3.0/m3u8/protocol.py
-drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-08-20 12:30:23.107476 m3u8-3.3.0/m3u8.egg-info/
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)    14627 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/PKG-INFO
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      319 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/SOURCES.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/dependency_links.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/not-zip-safe
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        8 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/requires.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2022-08-20 12:30:23.000000 m3u8-3.3.0/m3u8.egg-info/top_level.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)        8 2022-04-10 23:49:58.000000 m3u8-3.3.0/requirements.txt
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2022-08-20 12:30:23.107917 m3u8-3.3.0/setup.cfg
--rw-r--r--   0 mauricio.antunes   (501) staff       (20)      648 2022-08-20 12:29:43.000000 m3u8-3.3.0/setup.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-12-29 01:51:28.446334 m3u8-3.4.0/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1135 2022-12-29 01:47:32.000000 m3u8-3.4.0/LICENSE
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       59 2022-12-29 01:47:32.000000 m3u8-3.4.0/MANIFEST.in
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15259 2022-12-29 01:51:28.445947 m3u8-3.4.0/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15062 2022-12-29 01:47:32.000000 m3u8-3.4.0/README.rst
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-12-29 01:51:28.431607 m3u8-3.4.0/m3u8/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     2419 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/__init__.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1075 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/httpclient.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1590 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/mixins.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    48287 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/model.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    21487 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/parser.py
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)     1645 2022-12-29 01:47:32.000000 m3u8-3.4.0/m3u8/protocol.py
+drwxr-xr-x   0 mauricio.antunes   (501) staff       (20)        0 2022-12-29 01:51:28.445718 m3u8-3.4.0/m3u8.egg-info/
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)    15259 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/PKG-INFO
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      319 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/SOURCES.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/dependency_links.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        1 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/not-zip-safe
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        8 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/requires.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        5 2022-12-29 01:51:28.000000 m3u8-3.4.0/m3u8.egg-info/top_level.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)        8 2022-12-29 01:47:32.000000 m3u8-3.4.0/requirements.txt
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)       38 2022-12-29 01:51:28.446382 m3u8-3.4.0/setup.cfg
+-rw-r--r--   0 mauricio.antunes   (501) staff       (20)      648 2022-12-29 01:50:10.000000 m3u8-3.4.0/setup.py
```

### Comparing `m3u8-3.3.0/LICENSE` & `m3u8-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/PKG-INFO` & `m3u8-3.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: m3u8
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python m3u8 parser
 Home-page: https://github.com/globocom/m3u8
 Author: Globo.com
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6
 License-File: LICENSE
 
 .. image:: https://github.com/globocom/m3u8/actions/workflows/main.yml/badge.svg
 
 .. image:: https://badge.fury.io/py/m3u8.svg
     :target: https://badge.fury.io/py/m3u8
@@ -64,15 +63,15 @@
 * `#EXT-X-DISCONTINUITY-SEQUENCE`_
 * `#EXT-X-PROGRAM-DATE-TIME`_
 * `#EXT-X-MEDIA`_
 * `#EXT-X-PLAYLIST-TYPE`_
 * `#EXT-X-KEY`_
 * `#EXT-X-STREAM-INF`_
 * `#EXT-X-VERSION`_
-* #EXT-X-ALLOW-CACHE
+* `#EXT-X-ALLOW-CACHE`_
 * `#EXT-X-ENDLIST`_
 * `#EXTINF`_
 * `#EXT-X-I-FRAMES-ONLY`_
 * `#EXT-X-BITRATE`_
 * `#EXT-X-BYTERANGE`_
 * `#EXT-X-I-FRAME-STREAM-INF`_
 * `#EXT-X-DISCONTINUITY`_
@@ -80,19 +79,19 @@
 * #EXT-X-CUE-OUT-CONT
 * #EXT-X-CUE-IN
 * #EXT-X-CUE-SPAN
 * #EXT-OATCLS-SCTE35
 * `#EXT-X-INDEPENDENT-SEGMENTS`_
 * `#EXT-X-MAP`_
 * `#EXT-X-START`_
-* #EXT-X-SERVER-CONTROL
-* #EXT-X-PART-INF
-* #EXT-X-PART
-* #EXT-X-RENDITION-REPORT
-* #EXT-X-SKIP
+* `#EXT-X-SERVER-CONTROL`_
+* `#EXT-X-PART-INF`_
+* `#EXT-X-PART`_
+* `#EXT-X-RENDITION-REPORT`_
+* `#EXT-X-SKIP`_
 * `#EXT-X-SESSION-DATA`_
 * `#EXT-X-PRELOAD-HINT`_
 * `#EXT-X-SESSION-KEY`_
 * `#EXT-X-DATERANGE`_
 * `#EXT-X-GAP`_
 * `#EXT-X-CONTENT-STEERING`_
 
@@ -366,14 +365,15 @@
 If you plan to implement a new feature or something that will take more
 than a few minutes, please open an issue to make sure we don't work on
 the same thing.
 
 .. _m3u8: https://tools.ietf.org/html/rfc8216
 .. _#EXT-X-VERSION: https://tools.ietf.org/html/rfc8216#section-4.3.1.2
 .. _#EXTINF: https://tools.ietf.org/html/rfc8216#section-4.3.2.1
+.. _#EXT-X-ALLOW-CACHE: https://datatracker.ietf.org/doc/html/draft-pantos-http-live-streaming-07#section-3.3.6
 .. _#EXT-X-BITRATE: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.8
 .. _#EXT-X-BYTERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.2
 .. _#EXT-X-DISCONTINUITY: https://tools.ietf.org/html/rfc8216#section-4.3.2.3
 .. _#EXT-X-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.2.4
 .. _#EXT-X-MAP: https://tools.ietf.org/html/rfc8216#section-4.3.2.5
 .. _#EXT-X-PROGRAM-DATE-TIME: https://tools.ietf.org/html/rfc8216#section-4.3.2.6
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
@@ -389,19 +389,22 @@
 .. _#EXT-X-SESSION-DATA: https://tools.ietf.org/html/rfc8216#section-4.3.4.4
 .. _#EXT-X-SESSION-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.4.5
 .. _#EXT-X-INDEPENDENT-SEGMENTS: https://tools.ietf.org/html/rfc8216#section-4.3.5.1
 .. _#EXT-X-START: https://tools.ietf.org/html/rfc8216#section-4.3.5.2
 .. _#EXT-X-PRELOAD-HINT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis-09#section-4.4.5.3
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
 .. _#EXT-X-GAP: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-05#section-4.4.2.7
-.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.6
+.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.64
+.. _#EXT-X-SKIP: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.2
+.. _#EXT-X-RENDITION-REPORT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.4
+.. _#EXT-X-PART: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.9
+.. _#EXT-X-PART-INF: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.7
+.. _#EXT-X-SERVER-CONTROL: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.8
 .. _issue 1: https://github.com/globocom/m3u8/issues/1
 .. _variant streams: https://tools.ietf.org/html/rfc8216#section-6.2.4
 .. _example here: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.5
 .. _issue 4: https://github.com/globocom/m3u8/issues/4
 .. _I-frame playlists: https://tools.ietf.org/html/rfc8216#section-4.3.4.3
 .. _Apple's documentation: https://developer.apple.com/library/ios/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-I_FRAME_PLAYLIST
 .. _Alternative audio: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.7
 .. _VOD: https://developer.apple.com/library/mac/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-TNTAG2
 .. _EVENT: https://developer.apple.com/library/mac/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-EVENT_PLAYLIST
-
-
```

### Comparing `m3u8-3.3.0/README.rst` & `m3u8-3.4.0/m3u8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: m3u8
+Version: 3.4.0
+Summary: Python m3u8 parser
+Home-page: https://github.com/globocom/m3u8
+Author: Globo.com
+License: MIT
+Requires-Python: >=3.6
+License-File: LICENSE
+
 .. image:: https://github.com/globocom/m3u8/actions/workflows/main.yml/badge.svg
 
 .. image:: https://badge.fury.io/py/m3u8.svg
     :target: https://badge.fury.io/py/m3u8
 
 m3u8
 ====
@@ -53,15 +63,15 @@
 * `#EXT-X-DISCONTINUITY-SEQUENCE`_
 * `#EXT-X-PROGRAM-DATE-TIME`_
 * `#EXT-X-MEDIA`_
 * `#EXT-X-PLAYLIST-TYPE`_
 * `#EXT-X-KEY`_
 * `#EXT-X-STREAM-INF`_
 * `#EXT-X-VERSION`_
-* #EXT-X-ALLOW-CACHE
+* `#EXT-X-ALLOW-CACHE`_
 * `#EXT-X-ENDLIST`_
 * `#EXTINF`_
 * `#EXT-X-I-FRAMES-ONLY`_
 * `#EXT-X-BITRATE`_
 * `#EXT-X-BYTERANGE`_
 * `#EXT-X-I-FRAME-STREAM-INF`_
 * `#EXT-X-DISCONTINUITY`_
@@ -69,19 +79,19 @@
 * #EXT-X-CUE-OUT-CONT
 * #EXT-X-CUE-IN
 * #EXT-X-CUE-SPAN
 * #EXT-OATCLS-SCTE35
 * `#EXT-X-INDEPENDENT-SEGMENTS`_
 * `#EXT-X-MAP`_
 * `#EXT-X-START`_
-* #EXT-X-SERVER-CONTROL
-* #EXT-X-PART-INF
-* #EXT-X-PART
-* #EXT-X-RENDITION-REPORT
-* #EXT-X-SKIP
+* `#EXT-X-SERVER-CONTROL`_
+* `#EXT-X-PART-INF`_
+* `#EXT-X-PART`_
+* `#EXT-X-RENDITION-REPORT`_
+* `#EXT-X-SKIP`_
 * `#EXT-X-SESSION-DATA`_
 * `#EXT-X-PRELOAD-HINT`_
 * `#EXT-X-SESSION-KEY`_
 * `#EXT-X-DATERANGE`_
 * `#EXT-X-GAP`_
 * `#EXT-X-CONTENT-STEERING`_
 
@@ -355,14 +365,15 @@
 If you plan to implement a new feature or something that will take more
 than a few minutes, please open an issue to make sure we don't work on
 the same thing.
 
 .. _m3u8: https://tools.ietf.org/html/rfc8216
 .. _#EXT-X-VERSION: https://tools.ietf.org/html/rfc8216#section-4.3.1.2
 .. _#EXTINF: https://tools.ietf.org/html/rfc8216#section-4.3.2.1
+.. _#EXT-X-ALLOW-CACHE: https://datatracker.ietf.org/doc/html/draft-pantos-http-live-streaming-07#section-3.3.6
 .. _#EXT-X-BITRATE: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.8
 .. _#EXT-X-BYTERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.2
 .. _#EXT-X-DISCONTINUITY: https://tools.ietf.org/html/rfc8216#section-4.3.2.3
 .. _#EXT-X-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.2.4
 .. _#EXT-X-MAP: https://tools.ietf.org/html/rfc8216#section-4.3.2.5
 .. _#EXT-X-PROGRAM-DATE-TIME: https://tools.ietf.org/html/rfc8216#section-4.3.2.6
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
@@ -378,15 +389,20 @@
 .. _#EXT-X-SESSION-DATA: https://tools.ietf.org/html/rfc8216#section-4.3.4.4
 .. _#EXT-X-SESSION-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.4.5
 .. _#EXT-X-INDEPENDENT-SEGMENTS: https://tools.ietf.org/html/rfc8216#section-4.3.5.1
 .. _#EXT-X-START: https://tools.ietf.org/html/rfc8216#section-4.3.5.2
 .. _#EXT-X-PRELOAD-HINT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis-09#section-4.4.5.3
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
 .. _#EXT-X-GAP: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-05#section-4.4.2.7
-.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.6
+.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.64
+.. _#EXT-X-SKIP: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.2
+.. _#EXT-X-RENDITION-REPORT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.4
+.. _#EXT-X-PART: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.9
+.. _#EXT-X-PART-INF: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.7
+.. _#EXT-X-SERVER-CONTROL: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.8
 .. _issue 1: https://github.com/globocom/m3u8/issues/1
 .. _variant streams: https://tools.ietf.org/html/rfc8216#section-6.2.4
 .. _example here: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.5
 .. _issue 4: https://github.com/globocom/m3u8/issues/4
 .. _I-frame playlists: https://tools.ietf.org/html/rfc8216#section-4.3.4.3
 .. _Apple's documentation: https://developer.apple.com/library/ios/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-I_FRAME_PLAYLIST
 .. _Alternative audio: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.7
```

### Comparing `m3u8-3.3.0/m3u8/__init__.py` & `m3u8-3.4.0/m3u8/__init__.py`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/m3u8/httpclient.py` & `m3u8-3.4.0/m3u8/httpclient.py`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/m3u8/mixins.py` & `m3u8-3.4.0/m3u8/mixins.py`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/m3u8/model.py` & `m3u8-3.4.0/m3u8/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,17 @@
             Segment(base_uri=self.base_uri, keyobject=find_key(segment.get('key', {}), self.keys), **segment)
             for segment in self.data.get('segments', [])
         ])
 
         for attr, param in self.simple_attributes:
             setattr(self, attr, self.data.get(param))
 
+        for i, segment in enumerate(self.segments, self.media_sequence or 0):
+            segment.media_sequence = i
+
         self.files = []
         for key in self.keys:
             # Avoid None key, it could be the first one, don't repeat them
             if key and key.uri not in self.files:
                 self.files.append(key.uri)
         self.files.extend(self.segments.uri)
 
@@ -444,15 +447,16 @@
     '''
 
     def __init__(self, uri=None, base_uri=None, program_date_time=None, current_program_date_time=None,
                  duration=None, title=None, bitrate=None, byterange=None, cue_out=False,
                  cue_out_start=False, cue_in=False, discontinuity=False, key=None, scte35=None,
                  oatcls_scte35=None, scte35_duration=None, scte35_elapsedtime=None, asset_metadata=None,
                  keyobject=None, parts=None, init_section=None, dateranges=None, gap_tag=None,
-                 custom_parser_values=None):
+                 media_sequence=None, custom_parser_values=None):
+        self.media_sequence = media_sequence
         self.uri = uri
         self.duration = duration
         self.title = title
         self._base_uri = base_uri
         self.bitrate = bitrate
         self.byterange = byterange
         self.program_date_time = program_date_time
```

### Comparing `m3u8-3.3.0/m3u8/parser.py` & `m3u8-3.4.0/m3u8/parser.py`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/m3u8/protocol.py` & `m3u8-3.4.0/m3u8/protocol.py`

 * *Files identical despite different names*

### Comparing `m3u8-3.3.0/m3u8.egg-info/PKG-INFO` & `m3u8-3.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: m3u8
-Version: 3.3.0
-Summary: Python m3u8 parser
-Home-page: https://github.com/globocom/m3u8
-Author: Globo.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6
-License-File: LICENSE
-
 .. image:: https://github.com/globocom/m3u8/actions/workflows/main.yml/badge.svg
 
 .. image:: https://badge.fury.io/py/m3u8.svg
     :target: https://badge.fury.io/py/m3u8
 
 m3u8
 ====
@@ -64,15 +53,15 @@
 * `#EXT-X-DISCONTINUITY-SEQUENCE`_
 * `#EXT-X-PROGRAM-DATE-TIME`_
 * `#EXT-X-MEDIA`_
 * `#EXT-X-PLAYLIST-TYPE`_
 * `#EXT-X-KEY`_
 * `#EXT-X-STREAM-INF`_
 * `#EXT-X-VERSION`_
-* #EXT-X-ALLOW-CACHE
+* `#EXT-X-ALLOW-CACHE`_
 * `#EXT-X-ENDLIST`_
 * `#EXTINF`_
 * `#EXT-X-I-FRAMES-ONLY`_
 * `#EXT-X-BITRATE`_
 * `#EXT-X-BYTERANGE`_
 * `#EXT-X-I-FRAME-STREAM-INF`_
 * `#EXT-X-DISCONTINUITY`_
@@ -80,19 +69,19 @@
 * #EXT-X-CUE-OUT-CONT
 * #EXT-X-CUE-IN
 * #EXT-X-CUE-SPAN
 * #EXT-OATCLS-SCTE35
 * `#EXT-X-INDEPENDENT-SEGMENTS`_
 * `#EXT-X-MAP`_
 * `#EXT-X-START`_
-* #EXT-X-SERVER-CONTROL
-* #EXT-X-PART-INF
-* #EXT-X-PART
-* #EXT-X-RENDITION-REPORT
-* #EXT-X-SKIP
+* `#EXT-X-SERVER-CONTROL`_
+* `#EXT-X-PART-INF`_
+* `#EXT-X-PART`_
+* `#EXT-X-RENDITION-REPORT`_
+* `#EXT-X-SKIP`_
 * `#EXT-X-SESSION-DATA`_
 * `#EXT-X-PRELOAD-HINT`_
 * `#EXT-X-SESSION-KEY`_
 * `#EXT-X-DATERANGE`_
 * `#EXT-X-GAP`_
 * `#EXT-X-CONTENT-STEERING`_
 
@@ -366,14 +355,15 @@
 If you plan to implement a new feature or something that will take more
 than a few minutes, please open an issue to make sure we don't work on
 the same thing.
 
 .. _m3u8: https://tools.ietf.org/html/rfc8216
 .. _#EXT-X-VERSION: https://tools.ietf.org/html/rfc8216#section-4.3.1.2
 .. _#EXTINF: https://tools.ietf.org/html/rfc8216#section-4.3.2.1
+.. _#EXT-X-ALLOW-CACHE: https://datatracker.ietf.org/doc/html/draft-pantos-http-live-streaming-07#section-3.3.6
 .. _#EXT-X-BITRATE: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.8
 .. _#EXT-X-BYTERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.2
 .. _#EXT-X-DISCONTINUITY: https://tools.ietf.org/html/rfc8216#section-4.3.2.3
 .. _#EXT-X-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.2.4
 .. _#EXT-X-MAP: https://tools.ietf.org/html/rfc8216#section-4.3.2.5
 .. _#EXT-X-PROGRAM-DATE-TIME: https://tools.ietf.org/html/rfc8216#section-4.3.2.6
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
@@ -389,19 +379,22 @@
 .. _#EXT-X-SESSION-DATA: https://tools.ietf.org/html/rfc8216#section-4.3.4.4
 .. _#EXT-X-SESSION-KEY: https://tools.ietf.org/html/rfc8216#section-4.3.4.5
 .. _#EXT-X-INDEPENDENT-SEGMENTS: https://tools.ietf.org/html/rfc8216#section-4.3.5.1
 .. _#EXT-X-START: https://tools.ietf.org/html/rfc8216#section-4.3.5.2
 .. _#EXT-X-PRELOAD-HINT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis-09#section-4.4.5.3
 .. _#EXT-X-DATERANGE: https://tools.ietf.org/html/rfc8216#section-4.3.2.7
 .. _#EXT-X-GAP: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-05#section-4.4.2.7
-.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.6
+.. _#EXT-X-CONTENT-STEERING: https://tools.ietf.org/html/draft-pantos-hls-rfc8216bis-10#section-4.4.6.64
+.. _#EXT-X-SKIP: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.2
+.. _#EXT-X-RENDITION-REPORT: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.5.4
+.. _#EXT-X-PART: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.4.9
+.. _#EXT-X-PART-INF: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.7
+.. _#EXT-X-SERVER-CONTROL: https://datatracker.ietf.org/doc/html/draft-pantos-hls-rfc8216bis#section-4.4.3.8
 .. _issue 1: https://github.com/globocom/m3u8/issues/1
 .. _variant streams: https://tools.ietf.org/html/rfc8216#section-6.2.4
 .. _example here: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.5
 .. _issue 4: https://github.com/globocom/m3u8/issues/4
 .. _I-frame playlists: https://tools.ietf.org/html/rfc8216#section-4.3.4.3
 .. _Apple's documentation: https://developer.apple.com/library/ios/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-I_FRAME_PLAYLIST
 .. _Alternative audio: http://tools.ietf.org/html/draft-pantos-http-live-streaming-08#section-8.7
 .. _VOD: https://developer.apple.com/library/mac/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-TNTAG2
 .. _EVENT: https://developer.apple.com/library/mac/technotes/tn2288/_index.html#//apple_ref/doc/uid/DTS40012238-CH1-EVENT_PLAYLIST
-
-
```

### Comparing `m3u8-3.3.0/setup.py` & `m3u8-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_description = file.read()
 
 install_reqs = [req for req in open(abspath(join(dirname(__file__), 'requirements.txt')))]
 
 setup(
     name="m3u8",
     author='Globo.com',
-    version="3.3.0",
+    version="3.4.0",
     license='MIT',
     zip_safe=False,
     include_package_data=True,
     install_requires=install_reqs,
     packages=["m3u8"],
     url="https://github.com/globocom/m3u8",
     description="Python m3u8 parser",
```

