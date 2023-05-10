# Comparing `tmp/nudebomb-0.2.6.tar.gz` & `tmp/nudebomb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudebomb-0.2.6.tar", max compression
+gzip compressed data, was "nudebomb-0.3.0.tar", max compression
```

## Comparing `nudebomb-0.2.6.tar` & `nudebomb-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    35149 2022-12-29 22:58:10.856493 nudebomb-0.2.6/LICENSE
--rw-r--r--   0        0        0      814 2022-12-29 22:58:10.856493 nudebomb-0.2.6/NEWS.md
--rw-r--r--   0        0        0     2255 2022-12-29 22:58:10.856493 nudebomb-0.2.6/README.md
--rw-r--r--   0        0        0       16 2022-12-29 22:58:10.856493 nudebomb-0.2.6/nudebomb/__init__.py
--rw-r--r--   0        0        0     4224 2022-12-29 22:58:10.856493 nudebomb-0.2.6/nudebomb/cli.py
--rw-r--r--   0        0        0     3934 2022-12-29 22:58:10.856493 nudebomb-0.2.6/nudebomb/config.py
--rw-r--r--   0        0        0      258 2022-12-29 22:58:10.856493 nudebomb-0.2.6/nudebomb/config_default.yaml
--rw-r--r--   0        0        0     2560 2022-12-29 22:58:10.856493 nudebomb-0.2.6/nudebomb/langfiles.py
--rw-r--r--   0        0        0     6891 2022-12-29 22:58:10.860494 nudebomb-0.2.6/nudebomb/mkv.py
--rw-r--r--   0        0        0      442 2022-12-29 22:58:10.860494 nudebomb-0.2.6/nudebomb/track.py
--rw-r--r--   0        0        0      249 2022-12-29 22:58:10.860494 nudebomb-0.2.6/nudebomb/version.py
--rw-r--r--   0        0        0     4517 2022-12-29 22:58:10.860494 nudebomb-0.2.6/nudebomb/walk.py
--rw-r--r--   0        0        0     3545 2022-12-29 22:58:10.860494 nudebomb-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       13 2022-12-29 22:58:10.860494 nudebomb-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     2396 2022-12-29 22:58:10.860494 nudebomb-0.2.6/tests/mockdata/clean_tracks.json
--rw-r--r--   0        0        0  5100034 2022-12-29 22:58:10.868495 nudebomb-0.2.6/tests/test_files/test5.mkv
--rw-r--r--   0        0        0     1676 2022-12-29 22:58:10.868495 nudebomb-0.2.6/tests/test_integrated.py
--rw-r--r--   0        0        0     2050 2022-12-29 22:58:10.868495 nudebomb-0.2.6/tests/test_mkv.py
--rw-r--r--   0        0        0      688 2022-12-29 22:58:10.868495 nudebomb-0.2.6/tests/test_track.py
--rw-r--r--   0        0        0      580 2022-12-29 22:58:10.868495 nudebomb-0.2.6/tests/util.py
--rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 nudebomb-0.2.6/setup.py
--rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 nudebomb-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 01:44:50.249635 nudebomb-0.3.0/LICENSE
+-rw-r--r--   0        0        0      941 2023-05-10 01:44:50.249635 nudebomb-0.3.0/NEWS.md
+-rw-r--r--   0        0        0     2255 2023-05-10 01:44:50.249635 nudebomb-0.3.0/README.md
+-rw-r--r--   0        0        0       16 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/__init__.py
+-rw-r--r--   0        0        0     4479 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/cli.py
+-rw-r--r--   0        0        0     3950 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/config.py
+-rw-r--r--   0        0        0      290 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/config_default.yaml
+-rw-r--r--   0        0        0     2589 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/langfiles.py
+-rw-r--r--   0        0        0     7015 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/mkv.py
+-rw-r--r--   0        0        0      442 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/track.py
+-rw-r--r--   0        0        0      344 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/version.py
+-rw-r--r--   0        0        0     4526 2023-05-10 01:44:50.249635 nudebomb-0.3.0/nudebomb/walk.py
+-rw-r--r--   0        0        0     3853 2023-05-10 01:44:50.253635 nudebomb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 01:44:50.253635 nudebomb-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2396 2023-05-10 01:44:50.253635 nudebomb-0.3.0/tests/mockdata/clean_tracks.json
+-rw-r--r--   0        0        0  5100034 2023-05-10 01:44:50.257635 nudebomb-0.3.0/tests/test_files/test5.mkv
+-rw-r--r--   0        0        0     1908 2023-05-10 01:44:50.257635 nudebomb-0.3.0/tests/test_integrated.py
+-rw-r--r--   0        0        0     2335 2023-05-10 01:44:50.257635 nudebomb-0.3.0/tests/test_mkv.py
+-rw-r--r--   0        0        0      810 2023-05-10 01:44:50.257635 nudebomb-0.3.0/tests/test_track.py
+-rw-r--r--   0        0        0      622 2023-05-10 01:44:50.257635 nudebomb-0.3.0/tests/util.py
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 nudebomb-0.3.0/PKG-INFO
```

### Comparing `nudebomb-0.2.6/LICENSE` & `nudebomb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nudebomb-0.2.6/NEWS.md` & `nudebomb-0.3.0/NEWS.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # 📰 Nudebomb News
 
+## v0.3.0
+
+- Features
+
+  - New ignore timestamps for one run but write them option.
+  - Update deps including new treestamps.
+
 ## v0.2.6
 
 - Features
 
   - Update poetry lockfile & dev deps
 
 ## v0.2.5
```

### Comparing `nudebomb-0.2.6/README.md` & `nudebomb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nudebomb-0.2.6/nudebomb/cli.py` & `nudebomb-0.3.0/nudebomb/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,22 @@
         "-t",
         "--timestamps",
         action="store_true",
         help="Read and write timestamps to strip only files that have been "
         "modified since the last run.",
     )
     parser.add_argument(
+        "-C",
+        "--timestamps-no-check-config",
+        dest="timestamps_check_config",
+        action="store_false",
+        default=True,
+        help="Do not compare program config options with loaded timestamps.",
+    )
+    parser.add_argument(
         "-c", "--config", action="store", help="Alternate config file path"
     )
     parser.add_argument(
         "-A",
         "--after",
         action="store",
         dest="after",
```

### Comparing `nudebomb-0.2.6/nudebomb/config.py` & `nudebomb-0.3.0/nudebomb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Confuse config for comicbox."""
 import os
 import sys
 import typing
-
 from argparse import Namespace
 from platform import system
 from time import mktime
 
 from confuse import Configuration
 from confuse.templates import AttrDict, MappingTemplate, Optional, Sequence
 from dateutil.parser import parse
 from termcolor import cprint
 
 from nudebomb.version import PROGRAM_NAME
 
-
 TEMPLATE = MappingTemplate(
     {
         PROGRAM_NAME: MappingTemplate(
             {
                 "after": Optional(str),
                 "dry_run": bool,
                 "ignore": Sequence(str),
@@ -27,35 +25,34 @@
                 "paths": Sequence(str),
                 "recurse": bool,
                 "strip_und_language": bool,
                 "sub_languages": Optional(Sequence(str)),
                 "subtitles": bool,
                 "symlinks": bool,
                 "timestamps": bool,
+                "timestamps_check_config": bool,
                 "title": bool,
                 "verbose": bool,
             }
         )
     }
 )
-TIMESTAMPS_CONFIG_KEYS = set(
-    (
-        "languages",
-        "mkvmerge_bin",
-        "recurse",
-        "strip_und_language",
-        "sub_languages",
-        "subtitles",
-        "symlinks",
-        "title",
-    )
-)
+TIMESTAMPS_CONFIG_KEYS = {
+    "languages",
+    "mkvmerge_bin",
+    "recurse",
+    "strip_und_language",
+    "sub_languages",
+    "subtitles",
+    "symlinks",
+    "title",
+}
 
 if system() == "Windows":
-    os.system("color")
+    os.system("color")  # noqa S605, S607
 
 
 def _set_after(config) -> None:
     after = config[PROGRAM_NAME]["after"].get()
     if after is None:
         return
 
@@ -131,10 +128,10 @@
     _set_after(config)
     _set_default_mkvmerge_bin(config)
     _set_unique_lang_list(config, "sub_languages")
     _set_ignore(config)
     _set_timestamps(config)
     ad = config.get(TEMPLATE)
     if not isinstance(ad, AttrDict):
-        raise ValueError()
+        raise TypeError
     ad.paths = sorted(frozenset(ad.nudebomb.paths))
     return ad.nudebomb
```

### Comparing `nudebomb-0.2.6/nudebomb/langfiles.py` & `nudebomb-0.3.0/nudebomb/langfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Module for reading lang files."""
 import pycountry
-
 from termcolor import cprint
 
-
 LANGS_FNS = ("lang", "langs", ".lang", ".langs")
 
 
 def lang_to_alpha3(lang):
     """Convert languages to ISO-639-1 (alpha2) format."""
     if not lang:
         lang = "und"
-    elif len(lang) == 3:
+    elif len(lang) == 3:  # noqa PLR2004
         pass
-    elif len(lang) == 2:
+    elif len(lang) == 2:  # noqa PLR2004
         try:
             lo = pycountry.languages.get(alpha_2=lang)
             lang = lo.alpha_3
-        except Exception:
+        except Exception:  # noqa
             pass
     else:
         cprint(
             f"WARNING: Languages should be in two or three letter format: {lang}",
             "yellow",
         )
 
@@ -37,16 +35,15 @@
         self._lang_roots = {}
         langs = set()
         for lang in self._config.languages:
             langs.add(lang_to_alpha3(lang))
         self._languages = frozenset(langs)
 
     def read_lang_files(self, path):
-        """
-        Read the lang files and parse languages.
+        """Read the lang files and parse languages.
 
         lang_roots is a dictionary to cache paths and languages to avoid
         reparsing the same language files.
         """
         if path not in self._lang_roots:
             self._lang_roots[path] = set()
             for fn in LANGS_FNS:
```

### Comparing `nudebomb-0.2.6/nudebomb/mkv.py` & `nudebomb-0.3.0/nudebomb/mkv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """MKV file operations."""
 import json
 import subprocess
 import sys
 import time
-
 from pathlib import Path
 
 from termcolor import cprint
 
 from nudebomb.langfiles import lang_to_alpha3
 from nudebomb.track import Track
 
@@ -27,15 +26,17 @@
         self._init_track_map()
 
     def _init_track_map(self):
         self._track_map = {}
 
         # Ask mkvmerge for the json info
         command = (self._config.mkvmerge_bin, "-J", str(self.path))
-        proc = subprocess.run(command, capture_output=True, check=True, text=True)
+        proc = subprocess.run(
+            command, capture_output=True, check=True, text=True  # noqa S603
+        )
 
         # Process the json response
         json_data = json.loads(proc.stdout)
         tracks = json_data.get("tracks")
         if not tracks:
             cprint(
                 f"WARNING: No tracks for {self.path}. Might not be a valid movie.",
@@ -105,15 +106,16 @@
             prefix = track_type
             if track_type == self.SUBTITLE_TRACK_NAME:
                 prefix = prefix[:-1]
             command += [f"--{prefix}-tracks", ",".join(sorted(keep_ids))]
         elif track_type == self.SUBTITLE_TRACK_NAME:
             command += ["--no-subtitles"]
         else:
-            raise ValueError("Tried to remove all audio tracks.")
+            reason = "Tried to remove all audio tracks."
+            raise ValueError(reason)
 
         # Report what tracks will be removed
         output += f"Removing {track_type} track(s):\n"
         for track in remove:
             output += f"   {track}\n"
 
         output += "----------------------------\n"
@@ -125,15 +127,17 @@
     @staticmethod
     def _remux_file(command):
         """Remux a mkv file with the given parameters."""
         sys.stdout.write("Progress 0%")
         sys.stdout.flush()
 
         # Call subprocess command to remux file
-        process = subprocess.Popen(command, stdout=subprocess.PIPE, text=True)
+        process = subprocess.Popen(
+            command, stdout=subprocess.PIPE, text=True  # noqa S603
+        )
         # Display Percentage until subprocess has finished
         while process.poll() is None:
             # Sleep for a quarter second and then display progress
             # TODO replace with communicate timeout wait
             time.sleep(0.25)
             if process.stdout:
                 for line in iter(process.stdout.readline, ""):
@@ -183,16 +187,16 @@
             if self._config.verbose:
                 cprint(f"\tNot remuxing {self.path}", "green", attrs=["dark"])
             else:
                 cprint(".", "green", attrs=["bold"], end="")
             return
 
         try:
-            print(output, flush=True)
+            cprint(output, flush=True)
             if self._config.dry_run:
-                print("Dry run 100%")
+                cprint("Dry run 100%", "black", attrs=["bold"])
             else:
                 self._remux_file(command)
                 tmp_path.replace(self.path)
         except Exception as exc:
             cprint(str(exc), "red")
             tmp_path.unlink(missing_ok=True)
```

### Comparing `nudebomb-0.2.6/nudebomb/walk.py` & `nudebomb-0.3.0/nudebomb/walk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 """Walk directory trees and strip mkvs."""
 import os
-
 from copy import deepcopy
 from pathlib import Path
 
 from termcolor import cprint
-from treestamps import Treestamps
+from treestamps import Grovestamps, GrovestampsConfig
+from treestamps.tree import Treestamps
 
 from nudebomb.config import TIMESTAMPS_CONFIG_KEYS
 from nudebomb.langfiles import LangFiles
 from nudebomb.mkv import MKVFile
 from nudebomb.version import PROGRAM_NAME
 
 
 class Walk:
     """Directory traversal class."""
 
     def __init__(self, config):
         """Initialize."""
         self._config = config
         self._langfiles = LangFiles(config)
-        self._timestamps: dict[Path, Treestamps] = {}
 
     def _is_path_ignored(self, path: Path) -> bool:
         """Return if path should be ignored."""
-        for ignore_glob in self._config.ignore:
-            if path.match(ignore_glob):
-                return True
-        return False
+        return any(path.match(ignore_glob) for ignore_glob in self._config.ignore)
 
     def strip_path(self, top_path, path):
         """Strip a single mkv file."""
-        if not path.suffix == ".mkv":
+        if path.suffix != ".mkv":
             return
 
         mtime = None
         if self._config.after:
             mtime = self._config.after
         elif self._config.timestamps:
             mtime = self._timestamps.get(top_path, {}).get(path)
@@ -43,43 +39,43 @@
         if mtime is not None and mtime > path.stat().st_mtime:
             if self._config.verbose:
                 cprint(f"Skip unchanged {path}", "cyan", attrs=["dark"])
             else:
                 cprint(".", "cyan", end="")
             return
 
-        dirpath = Treestamps.dirpath(path)
+        dir_path = Treestamps.get_dir(path)
         config = deepcopy(self._config)
-        config.languages = self._langfiles.get_langs(top_path, dirpath)
+        config.languages = self._langfiles.get_langs(top_path, dir_path)
         mkv_obj = MKVFile(config, path)
         mkv_obj.remove_tracks()
 
         if self._config.timestamps:
-            self._timestamps[top_path].set(path)
+            self._timestamps[top_path.resolve()].set(path)
 
-    def walk_dir(self, top_path, dir):
+    def walk_dir(self, top_path, dir_path):
         """Walk a directory."""
         if not self._config.recurse:
             return
 
         filenames = []
 
-        for filename in sorted(os.listdir(dir)):
-            entry_path = dir / filename
+        for filename in sorted(os.listdir(dir_path)):
+            entry_path = dir_path / filename
             if entry_path.is_dir():
                 self.walk_file(top_path, entry_path)
             else:
                 filenames.append(entry_path)
 
         for path in filenames:
             self.walk_file(top_path, path)
 
         if self._config.timestamps:
-            timestamps = self._timestamps[top_path]
-            timestamps.set(dir, compact=True)
+            timestamps = self._timestamps[top_path.resolve()]
+            timestamps.set(dir_path, compact=True)
 
     def walk_file(self, top_path, path):
         """Walk a file."""
         if self._is_path_ignored(path):
             if self._config.verbose:
                 cprint(f"Skip ignored {path}", "white", attrs=["dark"])
             else:
@@ -95,45 +91,43 @@
             self.walk_dir(top_path, path)
         else:
             self.strip_path(top_path, path)
 
     def print_info(self):
         """Print intentions before we begin."""
         langs = ", ".join(sorted(self._config.languages))
-        if self._config.sub_languages:
-            audio = "audio "
-        else:
-            audio = ""
-        print(f"Stripping {audio}languages except {langs}.")
+        audio = "audio " if self._config.sub_languages else ""
+        cprint(f"Stripping {audio}languages except {langs}.")
         if self._config.sub_languages:
             sub_langs = ", ".join(sorted(self._config.sub_languages))
-            print(f"Stripping subtitle languages except {sub_langs}.")
+            cprint(f"Stripping subtitle languages except {sub_langs}.")
 
-        print("Searching for MKV files to process", end="")
+        cprint("Searching for MKV files to process", end="")
         if self._config.verbose:
-            print(":")
+            cprint(":")
 
     def run(self):
         """Run the stripper against all configured paths."""
         self.print_info()
 
         if self._config.timestamps:
-            self._timestamps = Treestamps.map_factory(
-                self._config.paths,
+            copse_config = GrovestampsConfig(
                 PROGRAM_NAME,
-                self._config.verbose,
-                self._config.symlinks,
-                self._config.ignore,
-                self._config,
-                TIMESTAMPS_CONFIG_KEYS,
+                paths=self._config.paths,
+                verbose=self._config.verbose,
+                symlinks=self._config.symlinks,
+                ignore=self._config.ignore,
+                check_config=self._config.timestamps_check_config,
+                program_config=self._config,
+                program_config_keys=TIMESTAMPS_CONFIG_KEYS,
             )
+            self._timestamps = Grovestamps(copse_config)
+
         for path_str in self._config.paths:
             path = Path(path_str)
-            top_path = Treestamps.dirpath(path)
+            top_path = Treestamps.get_dir(path)
             self.walk_file(top_path, path)
         if not self._config.verbose:
-            print("done.")
+            cprint("done.")
 
         if self._config.timestamps:
-            for top_path, timestamps in self._timestamps.items():
-                print(f"Saving timestamps for {top_path}")
-                timestamps.dump()
+            self._timestamps.dump()
```

### Comparing `nudebomb-0.2.6/pyproject.toml` & `nudebomb-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nudebomb"
-version = "0.2.6"
+version = "0.3.0"
 description = "Strip unused languages from mkv files en mass"
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/nudebomb"
 documentation = "https://github.com/ajslater/nudebomb"
 keywords = ["mkv", "movie", "video", "srt", "audio", "subtitles"]
@@ -26,52 +26,39 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 confuse = "^2.0.0"
 pycountry = "^22.3.5"
 python-dateutil = "^2.8.2"
 "ruamel.yaml" = "^0.17.21"
-treestamps = "^0.3.3"
+treestamps = "^0.4.0"
+termcolor = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
-bandit = "^1.7.4"
+black = "^23.3.0"
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
-flake8-black = "^0.3.2"
-flake8-bugbear = "^22.1"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.3.0"
-isort = "^5.10.1"
 neovim = "^0.3.1"
-pep8-naming = "^0.13.2"
-pip-review = "^1.1.0"
 pynvim = "^0.4"
 pyright = "^1.1.237"
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 pytest-gitignore = "^1.3"
-radon = "^5.1"
-tomli = "^2.0.1"
+radon = {version = "^6.0.1", extras = ["toml"]}
+ruff = "^0.0.265"
 types-python-dateutil = "^2.8.0"
 vulture = "^2.1"
 
 [tool.poetry.scripts]
 nudebomb = "nudebomb.cli:main"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/ajslater/nudebomb"
 "Issues" = "https://github.com/ajslater/nudebomb/issues"
 
-[tool.bandit]
-exclude = [
-  ".venv",
-  "node_modules",
-  "**/__pycache__",
-]
-
 [tool.black]
 exclude = "/(.git|.mypy_cache|.pytest_cache|.venv|__pycache__|dist|node_modules|test-results|typings)/"
 
 [tool.codespell]
 skip=".git,.mypy_cache,.pytest_cache,.venv,*~,./dist,./node_modules,./package-lock.json,./poetry.lock,./test-results"
 builtin="clear,rare,code"
 check-hidden=true
@@ -92,23 +79,14 @@
   "test-results/*",
   "typings/*"
 ]
 
 [tool.coverage.html]
 directory = "test-results/coverage"
 
-[tool.isort]
-profile="black"
-atomic=true
-lines_after_imports=2
-lines_between_types=1
-multi_line_output=3
-skip=".git,.mypy_cache,.pytest_cache,.venv,__pycache__,dist,node_modules,test-results,typings"
-color_output=true
-
 [tool.pytest.ini_options]
 junit_family = "xunit2"
 addopts = """
   --junitxml=test-results/pytest/junit.xml
   -ra
   --strict-markers
   --cov
@@ -123,19 +101,14 @@
   --ignore=node_modules
   --ignore=test-results
   --ignore=typings
   --ignore=vulture_whitelist.py
   --ignore-glob=*__pycache__*
 """
 
-[tool.vulture]
-exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*"]
-min_confidence = 61
-sort_by_size = true
-
 [tool.pyright]
 exclude = [
   "**/__pycache__",
   "**/node_modules",
   ".git",
   ".mypy_cache",
   ".pytest_cache",
@@ -146,7 +119,33 @@
   "test-results",
   "typings",
   "vulture_whitelist.py"
 ]
 useLibraryCodeForTypes = true
 reportMissingImports = true
 reportImportCycles = true
+
+[tool.radon]
+exclude = "*~,.git/*,.mypy_cache/*,.pytest_cache/*,.venv/*,__pycache__/*,dist/*,node_modules/*,test-results/*,typings/*"
+
+[tool.ruff]
+extend-exclude = ["cache", "typings"]
+extend-ignore = ["S101", "D203", "D213"]
+extend-select = ["A", "ARG", "B", "B9", "C", "C4", "C90", "D", "DJ",
+  "DTZ", "E", "EM", "EXE", "F", "I", "ICN", "INP", "ISC", "PIE", "PL",
+  "PT", "PTH", "PYI", "Q", "N", "RET", "RSE", "RUF", "S", "SIM", "SLF",
+  "T10", "T20", "TCH", "TID", "TRY", "UP", "W", "YTT"
+  # "ANN", "ERA", "COM"
+]
+external = ["V101"]
+# format = "grouped"
+# show-source = true
+target-version = "py39"
+task-tags = ["TODO", "FIXME", "XXX", "http", "HACK"]
+
+[tool.ruff.pycodestyle]
+ignore-overlong-task-comments = true
+
+[tool.vulture]
+exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*"]
+min_confidence = 61
+sort_by_size = true
```

### Comparing `nudebomb-0.2.6/tests/mockdata/clean_tracks.json` & `nudebomb-0.3.0/tests/mockdata/clean_tracks.json`

 * *Files identical despite different names*

### Comparing `nudebomb-0.2.6/tests/test_files/test5.mkv` & `nudebomb-0.3.0/tests/test_files/test5.mkv`

 * *Files identical despite different names*

### Comparing `nudebomb-0.2.6/tests/test_mkv.py` & `nudebomb-0.3.0/tests/test_mkv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,81 @@
 """Test MKVFile object."""
 import os
 import shutil
-
 from pathlib import Path
 
 from nudebomb.config import get_config
 from nudebomb.mkv import MKVFile
 
 from .util import SRC_PATH, TEST_FN, mkv_tracks
 
-
 __all__ = ()
 
-TEST_DIR = Path("/tmp/nudebomb.test_remux")
+TEST_DIR = Path("/tmp/nudebomb.test_remux")  # noqa
 TEST_MKV = TEST_DIR / TEST_FN
 
 
 def assert_eng_und_only(out_tracks):
+    """Asset english and undefined only tracks."""
     audio_count = 0
     subs_count = 0
     for track in out_tracks:
         track_type = track.get("type")
         if track_type not in MKVFile.REMOVABLE_TRACK_NAMES:
             continue
         lang = track["properties"]["language"]
-        print(track_type, lang)
+        print(track_type, lang)  # noqa T201
         assert lang in ["und", "eng"]
         if track_type == MKVFile.SUBTITLE_TRACK_NAME:
             subs_count += 1
         elif track_type == MKVFile.AUDIO_TRACK_NAME:
             audio_count += 1
         else:
-            raise AssertionError(f"Bad track type: {track_type}")
-    assert audio_count == 2
-    assert subs_count == 2
+            msg = f"Bad track type: {track_type}"
+            raise AssertionError(msg)
+    assert audio_count == 2  # noqa: PLR2004
+    assert subs_count == 2  # noqa: PLR2004
 
 
 class TestMkv:
+    """Test MKV."""
+
     def setup_method(self):
+        """Set up method."""
         shutil.rmtree(TEST_DIR, ignore_errors=True)
         TEST_DIR.mkdir()
         shutil.copy(SRC_PATH, TEST_MKV)
         self.src_tracks = mkv_tracks(TEST_MKV)
         os.environ["NUDEBOMB_NUDEBOMB__LANGUAGES__0"] = "und"
         os.environ["NUDEBOMB_NUDEBOMB__LANGUAGES__1"] = "eng"
 
     def teardown_method(self):
+        """Tear down method."""
         shutil.rmtree(TEST_DIR)
 
     def test_dry_run(self):
+        """Test dry run."""
         config = get_config()
         config.dry_run = True
         mkvfile = MKVFile(config, TEST_MKV)
         mkvfile.remove_tracks()
         out_tracks = mkv_tracks(TEST_MKV)
 
         assert out_tracks == self.src_tracks
 
     def test_run(self):
+        """Test run."""
         config = get_config()
         mkvfile = MKVFile(config, TEST_MKV)
         mkvfile.remove_tracks()
         out_tracks = mkv_tracks(TEST_MKV)
         assert_eng_und_only(out_tracks)
 
     def test_fail(self):
+        """Test fail."""
         config = get_config()
         config.languages = ["xxx"]
         mkvfile = MKVFile(config, TEST_MKV)
         mkvfile.remove_tracks()
         out_tracks = mkv_tracks(TEST_MKV)
 
         assert out_tracks == self.src_tracks
```

### Comparing `nudebomb-0.2.6/tests/test_track.py` & `nudebomb-0.3.0/tests/test_track.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Test Track class."""
 import json
 
 from nudebomb.track import Track
 
 from .util import read
 
-
 __all__ = ()
 
 
 class TestTrack:
+    """Test Track."""
+
     def test_video_track(self):
+        """Test video track."""
         data = json.loads(read("clean_tracks.json"))["tracks"][0]
         track = Track(data)
         assert str(track) == "Track #0: und - MPEG-4p10/AVC/h.264"
 
     def test_audio_track(self):
+        """Test audio track."""
         data = json.loads(read("clean_tracks.json"))["tracks"][1]
         track = Track(data)
         assert str(track) == "Track #2: eng - AC-3"
 
     def test_subtitle_track(self):
+        """Test subtitile track."""
         data = json.loads(read("clean_tracks.json"))["tracks"][2]
         track = Track(data)
         assert str(track) == "Track #5: eng - SubRip/SRT"
```

### Comparing `nudebomb-0.2.6/setup.py` & `nudebomb-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,104 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nudebomb
+Version: 0.3.0
+Summary: Strip unused languages from mkv files en mass
+Home-page: https://github.com/ajslater/nudebomb
+License: GPL-3.0-only
+Keywords: mkv,movie,video,srt,audio,subtitles
+Author: AJ Slater
+Author-email: aj@slater.net
+Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Multimedia :: Video :: Conversion
+Requires-Dist: confuse (>=2.0.0,<3.0.0)
+Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: termcolor (>=2.3.0,<3.0.0)
+Requires-Dist: treestamps (>=0.4.0,<0.5.0)
+Project-URL: Documentation, https://github.com/ajslater/nudebomb
+Project-URL: Issues, https://github.com/ajslater/nudebomb/issues
+Project-URL: Source, https://github.com/ajslater/nudebomb
+Description-Content-Type: text/markdown
 
-packages = \
-['nudebomb', 'tests']
+# Nudebomb
 
-package_data = \
-{'': ['*'], 'tests': ['mockdata/*', 'test_files/*']}
+The Nudebomb recursively strips matroska media files of unwanted audio and
+subtitle tracks.
 
-install_requires = \
-['confuse>=2.0.0,<3.0.0',
- 'pycountry>=22.3.5,<23.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'treestamps>=0.3.3,<0.4.0']
-
-entry_points = \
-{'console_scripts': ['nudebomb = nudebomb.cli:main']}
-
-setup_kwargs = {
-    'name': 'nudebomb',
-    'version': '0.2.6',
-    'description': 'Strip unused languages from mkv files en mass',
-    'long_description': "# Nudebomb\n\nThe Nudebomb recursively strips matroska media files of unwanted audio and\nsubtitle tracks.\n\n## News\n\nYou may find user focused nudebomb changes in the [NEWS file](https://github.com/ajslater/nudebomb/tree/NEWS.md).\n\n## Requirements\n\n- MKVToolNix\n- Python3\n\n## Install\n\n    pip install\n\n## Usage\n\n### Posix\n\n    nudebomb -rl eng,fre /mnt/movies\n\n### Windows\n\n    nudebomb -b C:\\\\Program/ Files\\MKVToolNix\\mkvmerge.exe -rl eng,jap \\\\nas\\movies\n\n## Config\n\nYou may configure Nudebomb options via the command, a yaml config file\nand environment variables.\n\n### Environment variable format\n\nPrefix environment variables with `NUDEBOMB_NUDEBOMB__` and enumerate lists elements:\n\n```sh\nNUDEBOMB_NUDEBOMB__RECURSE=True\nNUDEBOMB_NUDEBOMB__LANGUAGES__0=und\nNUDEBOMB_NUDEBOMB__LANGUAGES__1=eng\n```\n\n## Lang Files\n\nWhile you may have a primary language, you probably want videos from other countries to keep\ntheir native language as well. Lang files let you do this.\n\nLang files are persistent files on disk that nudebomb parses to keep to all languages in\nthem in the mkvs in the current directory and all mkvs in sub directories.\n\nValid lang file names are: 'lang', 'langs', '.lang', or '.langs'\nThey include comma separated list of languages to keep like the `-l` option.\n\ne.g. You may have an entire collecttion of different TV shows with a root lang file\ncontaining the `eng` language. Under that directory you may have a specific TV show directory\nwith lang file containing `jpn`. All mkvs in season directories under that would then\nkeep both the `eng` and `jpn` languages, while other TV shows would keep only `eng` languages.\n\nFor each mkv file, nudebomb looks up the directory tree for each parent lang file and uses the\nunion of all languages found to determine what languages to keep.\n\n### APIs\n\nLangfiles would be obsolete if nudebomb could deterimining native languages for mkv files by\npolling and caching results from major online media databases. It's the right thing to do, but I\ndon't care to implement it. Patches or forks welcome.\n\n## Inspiration\n\nNudebomb is a radical fork of [mkvstrip](https://github.com/willforde/mkvstrip). It adds recursion, lang files, timestamps and more configuration to mkvstrip and fixes some minor bugs.\n",
-    'author': 'AJ Slater',
-    'author_email': 'aj@slater.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ajslater/nudebomb',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+## News
 
+You may find user focused nudebomb changes in the [NEWS file](https://github.com/ajslater/nudebomb/tree/NEWS.md).
+
+## Requirements
+
+- MKVToolNix
+- Python3
+
+## Install
+
+    pip install
+
+## Usage
+
+### Posix
+
+    nudebomb -rl eng,fre /mnt/movies
+
+### Windows
+
+    nudebomb -b C:\\Program/ Files\MKVToolNix\mkvmerge.exe -rl eng,jap \\nas\movies
+
+## Config
+
+You may configure Nudebomb options via the command, a yaml config file
+and environment variables.
+
+### Environment variable format
+
+Prefix environment variables with `NUDEBOMB_NUDEBOMB__` and enumerate lists elements:
+
+```sh
+NUDEBOMB_NUDEBOMB__RECURSE=True
+NUDEBOMB_NUDEBOMB__LANGUAGES__0=und
+NUDEBOMB_NUDEBOMB__LANGUAGES__1=eng
+```
+
+## Lang Files
+
+While you may have a primary language, you probably want videos from other countries to keep
+their native language as well. Lang files let you do this.
+
+Lang files are persistent files on disk that nudebomb parses to keep to all languages in
+them in the mkvs in the current directory and all mkvs in sub directories.
+
+Valid lang file names are: 'lang', 'langs', '.lang', or '.langs'
+They include comma separated list of languages to keep like the `-l` option.
+
+e.g. You may have an entire collecttion of different TV shows with a root lang file
+containing the `eng` language. Under that directory you may have a specific TV show directory
+with lang file containing `jpn`. All mkvs in season directories under that would then
+keep both the `eng` and `jpn` languages, while other TV shows would keep only `eng` languages.
+
+For each mkv file, nudebomb looks up the directory tree for each parent lang file and uses the
+union of all languages found to determine what languages to keep.
+
+### APIs
+
+Langfiles would be obsolete if nudebomb could deterimining native languages for mkv files by
+polling and caching results from major online media databases. It's the right thing to do, but I
+don't care to implement it. Patches or forks welcome.
+
+## Inspiration
+
+Nudebomb is a radical fork of [mkvstrip](https://github.com/willforde/mkvstrip). It adds recursion, lang files, timestamps and more configuration to mkvstrip and fixes some minor bugs.
 
-setup(**setup_kwargs)
```

