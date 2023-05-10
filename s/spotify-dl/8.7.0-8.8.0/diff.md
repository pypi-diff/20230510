# Comparing `tmp/spotify_dl-8.7.0.tar.gz` & `tmp/spotify_dl-8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_dl-8.7.0.tar", last modified: Sun Apr 16 08:58:03 2023, max compression
+gzip compressed data, was "spotify_dl-8.8.0.tar", last modified: Wed May 10 08:18:09 2023, max compression
```

## Comparing `spotify_dl-8.7.0.tar` & `spotify_dl-8.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/spotify_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/spotify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6196 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/spotify_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-16 08:57:48.000000 spotify_dl-8.7.0/spotify_dl/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:58:03.095536 spotify_dl-8.7.0/spotify_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 08:58:03.000000 spotify_dl-8.7.0/spotify_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/spotify_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/spotify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6709 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/spotify_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-05-10 08:17:57.000000 spotify_dl-8.8.0/spotify_dl/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:18:09.125866 spotify_dl-8.8.0/spotify_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:18:09.000000 spotify_dl-8.8.0/spotify_dl.egg-info/top_level.txt
```

### Comparing `spotify_dl-8.7.0/LICENSE` & `spotify_dl-8.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.7.0/PKG-INFO` & `spotify_dl-8.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_dl
-Version: 8.7.0
+Version: 8.8.0
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spotify_dl-8.7.0/README.md` & `spotify_dl-8.8.0/README.md`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.7.0/setup.py` & `spotify_dl-8.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_dl-8.7.0/spotify_dl/scaffold.py` & `spotify_dl-8.8.0/spotify_dl/scaffold.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import logging
 from os import getenv
 import sentry_sdk
 from rich.logging import RichHandler
 from rich.console import Console
 
-__all__ = ["log", "get_tokens", "console"]
+__all__ = ["log", "setLogLevel", "get_tokens", "console"]
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(message)s",
     datefmt="[%X]",
     handlers=[RichHandler(show_level=False, show_time=False)],
 )
 console = Console()
 log = logging.getLogger("sdl")
 sentry_sdk.init(
     "https://fc66a23d79634b9bba1690ea13e289f0@o321064.ingest.sentry.io/2383261"
 )
 
 
+def setLogLevel(level):
+    """
+    Sets the log level of the global logger to the passed level
+    :param level: the log level
+    """
+    logging.getLogger().setLevel(level)
+
+
 def get_tokens():
     """
     Checks if the required API keys for Spotify has been set.
     :param name: Name to be cleaned up
     :return string containing the cleaned name
     """
     log.debug("Checking for tokens")
```

### Comparing `spotify_dl-8.7.0/spotify_dl/spotify.py` & `spotify_dl-8.8.0/spotify_dl/spotify.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                     if track_info is None:
                         offset += 1
                         continue
                     track_album_info = track_info.get("album")
                     track_num = track_info.get("track_number")
                     spotify_id = track_info.get("id")
                     track_name = track_info.get("name")
-                    track_artist = ",".join(
+                    track_artist = ", ".join(
                         [artist["name"] for artist in track_info.get("artists")]
                     )
                     if track_album_info:
                         track_album = track_album_info.get("name")
                         track_year = (
                             track_album_info.get("release_date")[:4]
                             if track_album_info.get("release_date")
```

### Comparing `spotify_dl-8.7.0/spotify_dl/spotify_dl.py` & `spotify_dl-8.8.0/spotify_dl/spotify_dl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python3
 import argparse
 import time
 import json
 import os
 import sys
-from logging import DEBUG
+from logging import DEBUG, ERROR
 from pathlib import Path, PurePath
 import spotipy
 from spotipy.oauth2 import SpotifyClientCredentials
 
 from spotify_dl.constants import VERSION
-from spotify_dl.scaffold import log, console, get_tokens
+from spotify_dl.scaffold import log, setLogLevel, console, get_tokens
 from spotify_dl.spotify import (
     fetch_tracks,
     parse_spotify_url,
     validate_spotify_urls,
     get_item_name,
 )
 
-from spotify_dl.youtube import download_songs, default_filename, playlist_num_filename
+from spotify_dl.youtube import download_songs, default_filename, playlist_num_filename, dump_json
 
 
 def spotify_dl():
     """Main entry point of the script."""
     parser = argparse.ArgumentParser(prog="spotify_dl")
     parser.add_argument(
         "-l",
@@ -46,14 +46,21 @@
         "-d",
         "--download",
         action="store_true",
         help="Download using youtube-dl",
         default=True,
     )
     parser.add_argument(
+        "-j",
+        "--dump-json",
+        action="store_true",
+        help="Dump info-json using youtube-dl",
+        default=False
+    )
+    parser.add_argument(
         "-f",
         "--format_str",
         type=str,
         action="store",
         help="Specify youtube-dl format string.",
         default="bestaudio/best",
     )
@@ -81,14 +88,21 @@
         "-w",
         "--no-overwrites",
         action="store_true",
         help="Whether we should avoid overwriting the target audio file if it already exists",
         default=False,
     )
     parser.add_argument(
+        "-r",
+        "--remove-trailing-tracks",
+        default="no",
+        action="store_true",
+        help="Whether we should delete tracks that were previously downloaded but are not longer in the playlist"
+    )
+    parser.add_argument(
         "-V",
         "--verbose",
         action="store_true",
         help="Show more information on what" "s happening.",
     )
     parser.add_argument(
         "-v",
@@ -111,22 +125,29 @@
         type=str,
         default="",
         help="Download through a proxy. Support HTTP & SOCKS5. Use 'http://username:password@hostname:port' or 'http://hostname:port'",
     )
     args = parser.parse_args()
     num_cores = os.cpu_count()
     args.multi_core = int(args.multi_core)
-    console.log(f"Starting spotify_dl [bold green]v{VERSION}[/bold green]")
+
+    if args.dump_json:
+        setLogLevel(ERROR)
     if args.verbose:
-        log.setLevel(DEBUG)
+        setLogLevel(DEBUG)
+
+    log.info("Starting spotify_dl v%s", VERSION)
     log.debug("Setting debug mode on spotify_dl")
 
     if args.multi_core > (num_cores - 1):
-        console.log(
-            f"Requested cores [bold red]{args.multi_core}[/bold red] exceeds available [bold green]{num_cores}[/bold green], using [bold green]{num_cores - 1}[/bold green] cores."
+        log.info(
+            "Requested cores %d exceeds available %d, using %d cores.",
+            args.multi_core,
+            num_cores,
+            num_cores - 1
         )
         args.multi_core = num_cores - 1
     if args.version:
         console.print(f"spotify_dl [bold green]v{VERSION}[/bold green]")
         sys.exit(0)
 
     if os.path.isfile(os.path.expanduser("~/.spotify_dl_settings")):
@@ -152,16 +173,17 @@
 
     sp = spotipy.Spotify(
         auth_manager=SpotifyClientCredentials(
             client_id=client_id, client_secret=client_secret
         )
     )
     log.debug("Arguments: %s ", args)
-    console.print(
-        f"Sponsorblock enabled?: [bold green]{args.use_sponsorblock}[/bold green]"
+    log.info(
+        "Sponsorblock enabled?: %s",
+        args.use_sponsorblock
     )
     valid_urls = validate_spotify_urls(args.url)
     if not valid_urls:
         sys.exit(1)
 
     url_data = {"urls": []}
 
@@ -169,37 +191,42 @@
         url_dict = {}
         item_type, item_id = parse_spotify_url(url)
         directory_name = get_item_name(sp, item_type, item_id)
         url_dict["save_path"] = Path(
             PurePath.joinpath(Path(args.output), Path(directory_name))
         )
         url_dict["save_path"].mkdir(parents=True, exist_ok=True)
-        console.print(
-            f"Saving songs to [bold green]{directory_name}[/bold green] directory"
+        log.info(
+            "Saving songs to %s directory",
+            directory_name
         )
         url_dict["songs"] = fetch_tracks(sp, item_type, url)
         url_data["urls"].append(url_dict.copy())
-    if args.download is True:
+    if args.dump_json is True:
+        dump_json(url_dict["songs"])
+    elif args.download is True:
         file_name_f = default_filename
         if args.keep_playlist_order:
             file_name_f = playlist_num_filename
 
         download_songs(
             songs=url_data,
             output_dir=args.output,
             format_str=args.format_str,
             skip_mp3=args.skip_mp3,
             keep_playlist_order=args.keep_playlist_order,
             no_overwrites=args.no_overwrites,
+            remove_trailing_tracks=args.remove_trailing_tracks,
             use_sponsorblock=args.use_sponsorblock,
             file_name_f=file_name_f,
             multi_core=args.multi_core,
             proxy=args.proxy,
         )
 
 
 if __name__ == "__main__":
     start_time = time.time()
     spotify_dl()
-    console.log(
-        f"Download completed in [bold green]{time.time() - start_time} seconds.[/bold green]"
+    log.info(
+        "Download completed in %f seconds.", 
+        time.time() - start_time
     )
```

### Comparing `spotify_dl-8.7.0/spotify_dl/youtube.py` & `spotify_dl-8.8.0/spotify_dl/youtube.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import urllib.request
 from os import path
 import os
 import multiprocessing
+
+import json
 import mutagen
 import csv
 import yt_dlp
 from mutagen.easyid3 import EasyID3
 from mutagen.id3 import APIC, ID3
 from mutagen.mp3 import MP3
 from spotify_dl.scaffold import log
@@ -21,14 +23,36 @@
 
 
 def playlist_num_filename(**kwargs):
     """name with track number"""
     return f"{kwargs['track_num']} - {default_filename(**kwargs)}"
 
 
+def dump_json(songs):
+    """
+    Outputs the JSON response of ydl.extract_info to stdout
+    :param songs: the songs for which the JSON should be output
+    """
+    for song in songs:
+        query = f"{song.get('artist')} - {song.get('name')} Lyrics".replace(":", "").replace("\"", "")
+
+        ydl_opts = {
+            'quiet': True
+        }
+
+        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
+            try:
+                ytJson = ydl.extract_info('ytsearch:' + query, False)
+                print(json.dumps(ytJson.get('entries')))
+            except Exception as e:  # skipcq: PYL-W0703
+                log.debug(e)
+                print(f"Failed to download {song.get('name')}, make sure yt_dlp is up to date")
+                continue
+
+
 def write_tracks(tracks_file, song_dict):
     """
     Writes the information of all tracks in the playlist[s] to a text file in csv kind of format
     This includins the name, artist, and spotify URL. Each is delimited by a comma.
     :param tracks_file: name of file towhich the songs are to be written
     :param song_dict: the songs to be written to tracks_file
     """
@@ -116,14 +140,15 @@
     """
     function handles actual download of the songs
     the youtube_search lib is used to search for songs and get best url
     :param kwargs: dictionary of key value arguments to be used in download
     """
     sponsorblock_postprocessor = []
     reference_file = kwargs["reference_file"]
+    files = {}
     with open(reference_file, "r", encoding="utf-8") as file:
         for line in file:
             temp = line.split(";")
             name, artist, album, i = (
                 temp[0],
                 temp[1],
                 temp[4],
@@ -146,22 +171,29 @@
                     },
                     {
                         "key": "ModifyChapters",
                         "remove_sponsor_segments": ["music_offtopic"],
                         "force_keyframes": True,
                     },
                 ]
+            save_path = kwargs["track_db"][i]["save_path"]
+            file_path = path.join(save_path, file_name)
+
+            mp3file_path = f"{file_path}.mp3"
 
-            file_path = path.join(kwargs["track_db"][i]["save_path"], file_name)
+            if save_path not in files:
+                path_files = set()
+                files[save_path] = path_files
+            else:
+                path_files = files[save_path]
 
-            mp3filename = f"{file_path}.mp3"
-            mp3file_path = path.join(mp3filename)
+            path_files.add(f"{file_name}.mp3")
 
             if kwargs["no_overwrites"] and not kwargs["skip_mp3"] and path.exists(mp3file_path):
-                print(f'File {mp3filename} already exists, we do not overwrite it ')
+                print(f'File {mp3file_path} already exists, we do not overwrite it ')
                 continue
 
             outtmpl = f"{file_path}.%(ext)s"
             ydl_opts = {
                 "proxy": kwargs.get('proxy'),
                 "default_search": "ytsearch",
                 "format": "bestaudio/best",
@@ -188,15 +220,21 @@
             with yt_dlp.YoutubeDL(ydl_opts) as ydl:
                 try:
                     ydl.download([query])
                 except Exception as e:  # skipcq: PYL-W0703
                     log.debug(e)
                     print(f"Failed to download {name}, make sure yt_dlp is up to date")
             if not kwargs["skip_mp3"]:
-                set_tags(temp, mp3filename, kwargs)
+                set_tags(temp, mp3file_path, kwargs)
+        if kwargs["remove_trailing_tracks"]:
+            for save_path in files:
+                for f in os.listdir(save_path):
+                    if f not in files[save_path]:
+                        print(f"File {f} is not in the playlist anymore, we delete it")
+                        os.remove(path.join(save_path, f))
 
 
 def multicore_find_and_download_songs(kwargs):
     """
     function handles divinding songs to be downloaded among the specified number of CPU's
     extra songs are shared among the CPU's
     each cpu then handles its own batch through the multihandler fn
```

### Comparing `spotify_dl-8.7.0/spotify_dl.egg-info/PKG-INFO` & `spotify_dl-8.8.0/spotify_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-dl
-Version: 8.7.0
+Version: 8.8.0
 Summary: Downloads songs from a Spotify Playlist/Track/Album that you provide
 Home-page: https://github.com/SathyaBhat/spotify-dl/
 Author: Sathya Bhat
 Author-email: sathya@sathyasays.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

