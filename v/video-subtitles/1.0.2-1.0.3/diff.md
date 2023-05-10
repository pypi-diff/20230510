# Comparing `tmp/video-subtitles-1.0.2.tar.gz` & `tmp/video-subtitles-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.2.tar", last modified: Tue May  9 01:55:03 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.3.tar", last modified: Wed May 10 00:58:15 2023, max compression
```

## Comparing `video-subtitles-1.0.2.tar` & `video-subtitles-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.495816 video-subtitles-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.380745 video-subtitles-1.0.2/.github/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.427290 video-subtitles-1.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.2/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.2/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.2/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.2/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.431827 video-subtitles-1.0.2/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7527 2023-05-09 01:55:03.494816 video-subtitles-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6629 2023-05-09 01:53:15.000000 video-subtitles-1.0.2/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.2/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/make_venv.py
--rw-rw-rw-   0        0        0      755 2023-05-08 23:34:23.000000 video-subtitles-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.2/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 01:55:03.495816 video-subtitles-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.382746 video-subtitles-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.440816 video-subtitles-1.0.2/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-09 01:38:00.000000 video-subtitles-1.0.2/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.485814 video-subtitles-1.0.2/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     4199 2023-05-08 23:46:45.000000 video-subtitles-1.0.2/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0     3061 2023-05-09 01:36:13.000000 video-subtitles-1.0.2/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.2/src/video_subtitles/say.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.2/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.2/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.483814 video-subtitles-1.0.2/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     7527 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.491816 video-subtitles-1.0.2/tests/
--rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.2/tests/test_cli.py
--rw-rw-rw-   0        0        0      951 2023-05-08 23:21:31.000000 video-subtitles-1.0.2/tests/test_full.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.2/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.2/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/tox.ini
--rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.569476 video-subtitles-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.521474 video-subtitles-1.0.3/.github/
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.541473 video-subtitles-1.0.3/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.3/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.3/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.3/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.3/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.543473 video-subtitles-1.0.3/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7530 2023-05-10 00:58:15.568473 video-subtitles-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2023-05-09 01:55:43.000000 video-subtitles-1.0.3/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.3/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/make_venv.py
+-rw-rw-rw-   0        0        0      775 2023-05-09 23:58:29.000000 video-subtitles-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.3/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 00:58:15.569476 video-subtitles-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.522473 video-subtitles-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.550474 video-subtitles-1.0.3/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-10 00:50:57.000000 video-subtitles-1.0.3/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.563475 video-subtitles-1.0.3/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     4369 2023-05-10 00:48:17.000000 video-subtitles-1.0.3/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0     2991 2023-05-10 00:53:36.000000 video-subtitles-1.0.3/src/video_subtitles/gui.py
+-rw-rw-rw-   0        0        0     3203 2023-05-10 00:50:23.000000 video-subtitles-1.0.3/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.3/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.3/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.3/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.562473 video-subtitles-1.0.3/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     7530 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      916 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 00:58:15.000000 video-subtitles-1.0.3/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 00:58:15.567475 video-subtitles-1.0.3/tests/
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.3/tests/test_cli.py
+-rw-rw-rw-   0        0        0      951 2023-05-08 23:21:31.000000 video-subtitles-1.0.3/tests/test_full.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.3/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.3/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/tox.ini
+-rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.3/upload_package.sh
```

### Comparing `video-subtitles-1.0.2/.github/workflows/lint.yml` & `video-subtitles-1.0.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.github/workflows/push_macos.yml` & `video-subtitles-1.0.3/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.3/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.github/workflows/push_win.yml` & `video-subtitles-1.0.3/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.gitignore` & `video-subtitles-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.vscode/launch.json` & `video-subtitles-1.0.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.vscode/settings.json` & `video-subtitles-1.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/.vscode/tasks.json` & `video-subtitles-1.0.3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/LICENSE` & `video-subtitles-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/PKG-INFO` & `video-subtitles-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.2
+Version: 1.0.3
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -211,15 +211,15 @@
   "ur": "Urdu",
   "uz": "Uzbek",
   "vi": "Vietnamese",
   "yi": "Yiddish",
   "yo": "Yoruba",
   "zh": "Chinese",
 }
-
+```
 
 
 # Windows
 
 This environment requires you to use `git-bash`.
 
 # Linting
```

### Comparing `video-subtitles-1.0.2/README.md` & `video-subtitles-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
   "ur": "Urdu",
   "uz": "Uzbek",
   "vi": "Vietnamese",
   "yi": "Yiddish",
   "yo": "Yoruba",
   "zh": "Chinese",
 }
-
+```
 
 
 # Windows
 
 This environment requires you to use `git-bash`.
 
 # Linting
```

### Comparing `video-subtitles-1.0.2/make_venv.py` & `video-subtitles-1.0.3/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/pyproject.toml` & `video-subtitles-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "download",
     "srtranslator",
     "gTTS",
     "playaudio",
+    "PyQt6==6.3.1"
 ]
 
 dynamic = ["version"]
 
 [tool.ruff]
 line-length = 200
```

### Comparing `video-subtitles-1.0.2/setup.py` & `video-subtitles-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/src/video_subtitles/cli.py` & `video-subtitles-1.0.3/src/video_subtitles/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Command line front end interface.
 """
 
 import argparse
 import os
+import sys
 import warnings
 
 from video_subtitles import __version__
 from video_subtitles.run import run
 from video_subtitles.say import say
 from video_subtitles.util import (
     LANGUAGE_CODES,
@@ -100,25 +101,32 @@
         write_api_key(key)
         api_key = read_api_key()
     return api_key
 
 
 def main() -> int:
     """Main entry point for the template_python_cmd package."""
+    print(f"videosubtitles version: {__version__}")
+    cuda_cards = ensure_dependencies()
+    print("Found the following Nvidia/CUDA video cards:")
+    for card in cuda_cards:
+        print(f"  [{card.idx}]: {card.name}, {card.memory_gb} GB")
+    if len(sys.argv) == 1:
+        from video_subtitles.gui import (  # pylint: disable=import-outside-toplevel
+            run_gui,
+        )
+
+        run_gui()
+        return 0
     try:
         args = parse_args()
         file = args.file
         if not os.path.exists(file):
             print(f"Error - file does not exist: {file}")
             return 1
-        print(f"videosubtitles version: {__version__}")
-        cuda_cards = ensure_dependencies()
-        print("Found the following Nvidia/CUDA video cards:")
-        for card in cuda_cards:
-            print(f"  [{card.idx}]: {card.name}, {card.memory_gb} GB")
         api_key: None | str = None
         if args.api_key:
             api_key = args.api_key
             if api_key == "free":
                 api_key = None
         else:
             api_key = validate_api_key()
```

### Comparing `video-subtitles-1.0.2/src/video_subtitles/run.py` & `video-subtitles-1.0.3/src/video_subtitles/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Runs the program
 """
 import os
 import shutil
 
-from transcribe_anything.api import transcribe
-
 from video_subtitles.translate import srt_wrap, translate
 
 IS_GITHUB = os.environ.get("GITHUB_ACTIONS", False)
 
 
 def find_srt_files(folder: str) -> list[str]:
     """Find srt files in a folder."""
@@ -23,22 +21,28 @@
 
 
 def run(  # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     file: str,
     deepl_api_key: str | None,
     out_languages: list[str],
     model: str,
-) -> None:
+) -> str:
     """Run the program."""
+    from transcribe_anything.api import (  # pylint: disable=import-outside-toplevel
+        transcribe,
+    )
+
     print("Running transcription")
     out_languages = out_languages.copy()
     print(f"Output languages: {out_languages}")
     print(f"Model: {model}")
     print(f"File: {file}")
     print("Done running transcription")
+    if deepl_api_key == "free":
+        deepl_api_key = None
     device = "cuda" if not IS_GITHUB else "cpu"
     out_en_dir = transcribe(url_or_file=file, device=device, model=model, language="en")
     print(f"Output directory: {out_en_dir}")
     if not os.path.exists(out_en_dir):
         raise RuntimeError(f"Error - folder does not exist: {out_en_dir}")
     if "en" in out_languages:
         out_languages.remove("en")
@@ -80,7 +84,8 @@
         language_name = os.path.basename(os.path.dirname(srt_file))
         out_file = os.path.join(outdir, f"{language_name}.srt")
         if os.path.exists(out_file):
             os.remove(out_file)
         shutil.move(srt_file, out_file)
         shutil.rmtree(os.path.dirname(srt_file))
     print("Done translating")
+    return outdir
```

### Comparing `video-subtitles-1.0.2/src/video_subtitles/say.py` & `video-subtitles-1.0.3/src/video_subtitles/say.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/src/video_subtitles/translate.py` & `video-subtitles-1.0.3/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/src/video_subtitles/util.py` & `video-subtitles-1.0.3/src/video_subtitles/util.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/src/video_subtitles.egg-info/PKG-INFO` & `video-subtitles-1.0.3/src/video_subtitles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.2
+Version: 1.0.3
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -211,15 +211,15 @@
   "ur": "Urdu",
   "uz": "Uzbek",
   "vi": "Vietnamese",
   "yi": "Yiddish",
   "yo": "Yoruba",
   "zh": "Chinese",
 }
-
+```
 
 
 # Windows
 
 This environment requires you to use `git-bash`.
 
 # Linting
```

### Comparing `video-subtitles-1.0.2/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.3/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .github/workflows/push_ubuntu.yml
 .github/workflows/push_win.yml
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 src/video_subtitles/__init__.py
 src/video_subtitles/cli.py
+src/video_subtitles/gui.py
 src/video_subtitles/run.py
 src/video_subtitles/say.py
 src/video_subtitles/translate.py
 src/video_subtitles/util.py
 src/video_subtitles.egg-info/PKG-INFO
 src/video_subtitles.egg-info/SOURCES.txt
 src/video_subtitles.egg-info/dependency_links.txt
```

### Comparing `video-subtitles-1.0.2/tests/test_cli.py` & `video-subtitles-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/tests/test_full.py` & `video-subtitles-1.0.3/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/tests/test_srt_translator.py` & `video-subtitles-1.0.3/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.2/tests/video.mp4` & `video-subtitles-1.0.3/tests/video.mp4`

 * *Files identical despite different names*

