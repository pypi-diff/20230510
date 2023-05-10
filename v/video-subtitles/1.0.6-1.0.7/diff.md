# Comparing `tmp/video-subtitles-1.0.6.tar.gz` & `tmp/video-subtitles-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.6.tar", last modified: Wed May 10 05:27:05 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.7.tar", last modified: Wed May 10 06:17:59 2023, max compression
```

## Comparing `video-subtitles-1.0.6.tar` & `video-subtitles-1.0.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.221699 video-subtitles-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.166702 video-subtitles-1.0.6/.github/
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.187700 video-subtitles-1.0.6/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.6/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.6/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.6/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.6/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.190699 video-subtitles-1.0.6/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5489 2023-05-10 05:27:05.220703 video-subtitles-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4680 2023-05-10 05:23:03.000000 video-subtitles-1.0.6/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.6/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/make_venv.py
--rw-rw-rw-   0        0        0      828 2023-05-10 03:33:33.000000 video-subtitles-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.6/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 05:27:05.221699 video-subtitles-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.167702 video-subtitles-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.200703 video-subtitles-1.0.6/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-10 05:22:41.000000 video-subtitles-1.0.6/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.212700 video-subtitles-1.0.6/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     3731 2023-05-10 05:21:04.000000 video-subtitles-1.0.6/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.6/src/video_subtitles/convert_to_webvtt.py
--rw-rw-rw-   0        0        0     8942 2023-05-10 05:21:52.000000 video-subtitles-1.0.6/src/video_subtitles/gui.py
--rw-rw-rw-   0        0        0     3648 2023-05-10 05:06:12.000000 video-subtitles-1.0.6/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.6/src/video_subtitles/say.py
--rw-rw-rw-   0        0        0     2050 2023-05-10 03:57:36.000000 video-subtitles-1.0.6/src/video_subtitles/settings.py
--rw-rw-rw-   0        0        0     1354 2023-05-10 03:17:40.000000 video-subtitles-1.0.6/src/video_subtitles/thread_processor.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.6/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     3855 2023-05-10 04:55:21.000000 video-subtitles-1.0.6/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.211701 video-subtitles-1.0.6/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     5489 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.219703 video-subtitles-1.0.6/tests/
--rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.6/tests/test.srt
--rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.6/tests/test_cli.py
--rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.6/tests/test_full.py
--rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.6/tests/test_srt_to_webvtt.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.6/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.6/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/tox.ini
--rw-rw-rw-   0        0        0      953 2023-05-10 01:01:08.000000 video-subtitles-1.0.6/upload_package.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.446422 video-subtitles-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.388423 video-subtitles-1.0.7/.github/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.411421 video-subtitles-1.0.7/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.7/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.7/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.7/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.7/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.414423 video-subtitles-1.0.7/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5536 2023-05-10 06:17:59.445424 video-subtitles-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4726 2023-05-10 06:17:26.000000 video-subtitles-1.0.7/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.7/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/make_venv.py
+-rw-rw-rw-   0        0        0      828 2023-05-10 03:33:33.000000 video-subtitles-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.7/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 06:17:59.446422 video-subtitles-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.390422 video-subtitles-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.424421 video-subtitles-1.0.7/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-10 06:17:07.000000 video-subtitles-1.0.7/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.438424 video-subtitles-1.0.7/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     3728 2023-05-10 05:42:46.000000 video-subtitles-1.0.7/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.7/src/video_subtitles/convert_to_webvtt.py
+-rw-rw-rw-   0        0        0    10449 2023-05-10 06:16:18.000000 video-subtitles-1.0.7/src/video_subtitles/gui.py
+-rw-rw-rw-   0        0        0     3648 2023-05-10 05:06:12.000000 video-subtitles-1.0.7/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.7/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0     2050 2023-05-10 03:57:36.000000 video-subtitles-1.0.7/src/video_subtitles/settings.py
+-rw-rw-rw-   0        0        0     1622 2023-05-10 06:00:11.000000 video-subtitles-1.0.7/src/video_subtitles/thread_processor.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.7/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     3855 2023-05-10 04:55:21.000000 video-subtitles-1.0.7/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.437424 video-subtitles-1.0.7/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     5536 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       95 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 06:17:59.000000 video-subtitles-1.0.7/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 06:17:59.444423 video-subtitles-1.0.7/tests/
+-rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.7/tests/test.srt
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.7/tests/test_cli.py
+-rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.7/tests/test_full.py
+-rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.7/tests/test_srt_to_webvtt.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.7/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.7/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.7/tox.ini
+-rw-rw-rw-   0        0        0      953 2023-05-10 01:01:08.000000 video-subtitles-1.0.7/upload_package.py
```

### Comparing `video-subtitles-1.0.6/.github/workflows/lint.yml` & `video-subtitles-1.0.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.github/workflows/push_macos.yml` & `video-subtitles-1.0.7/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.7/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.github/workflows/push_win.yml` & `video-subtitles-1.0.7/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.gitignore` & `video-subtitles-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.vscode/launch.json` & `video-subtitles-1.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.vscode/settings.json` & `video-subtitles-1.0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/.vscode/tasks.json` & `video-subtitles-1.0.7/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/LICENSE` & `video-subtitles-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/PKG-INFO` & `video-subtitles-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.6
+Version: 1.0.7
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -131,14 +131,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
   * 1.0.1: Adds retry to translation step. Also alerts when the video is done.
   * 1.0.0: Initial release.
```

### Comparing `video-subtitles-1.0.6/README.md` & `video-subtitles-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
   * 1.0.1: Adds retry to translation step. Also alerts when the video is done.
   * 1.0.0: Initial release.
```

### Comparing `video-subtitles-1.0.6/make_venv.py` & `video-subtitles-1.0.7/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/pyproject.toml` & `video-subtitles-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/setup.py` & `video-subtitles-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles/cli.py` & `video-subtitles-1.0.7/src/video_subtitles/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     parser = argparse.ArgumentParser(description="Video Subtitles")
     parser.add_argument("--version", action="version", version=f"{__version__}")
     parser.add_argument("file", type=str, help="File or URL to process.")
     parser.add_argument(
         "--languages",
         type=parse_languages,
         help="Output languages as a comma-separated list.",
-        metavar="{en,es,fr,de,it,pt,ru,zh}",
+        metavar="{en,es,fr,de,it,ru,zh}",
         required=True,
     )
     parser.add_argument(
         "--model",
         type=str,
         help="Model to use.",
         default="large",
```

### Comparing `video-subtitles-1.0.6/src/video_subtitles/gui.py` & `video-subtitles-1.0.7/src/video_subtitles/gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 import os
 import platform
 import subprocess
 import sys
 from threading import Thread
 
 from PyQt6 import QtCore  # type: ignore
+from PyQt6.QtCore import pyqtSignal  # type: ignore
 from PyQt6.QtWidgets import (  # type: ignore
     QApplication,
     QComboBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMainWindow,
     QMessageBox,
+    QProgressBar,
     QPushButton,
     QVBoxLayout,
     QWidget,
 )
 
 from video_subtitles.run import run
 from video_subtitles.say import say
@@ -42,19 +44,23 @@
     else:
         subprocess.Popen(["xdg-open", path])  # pylint: disable=consider-using-with
 
 
 class MainWidget(QMainWindow):  # pylint: disable=too-many-instance-attributes
     """Main widget."""
 
+    progress_signal = pyqtSignal(bool)
+
     def __init__(self, on_drop_callback):  # pylint: disable=too-many-statements
         super().__init__()
+
         self.setWindowTitle("Video Subtitle Generator")
         self.resize(720, 480)
         self.setAcceptDrops(True)
+        self.on_destroy = None
 
         deepl_api_key = settings.deepl_key()
 
         # Creating a QWidget instance
         central_widget = QWidget()
         self.setCentralWidget(central_widget)
 
@@ -121,32 +127,54 @@
         header_layout.addLayout(output_layout)
 
         # Add a label to the window on top of everything else
         self.label = QLabel(self)
         self.label.setText("Drag and drop video file here for subtitles")
         self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
+        progress_bar_layout = QHBoxLayout()
+        # Create a progress bar
+        self.progress_bar = self.create_progress_bar()
+        self.progress_signal.connect(self.progress_bar.setVisible)
+        progress_bar_layout.addWidget(self.progress_bar)
+
         # Add the header pane and label widget to the main layout
         main_layout.addWidget(header_pane)
         main_layout.addWidget(self.label)
+        main_layout.addLayout(progress_bar_layout)
 
         # Setting the alignment of the header pane to the top
         main_layout.setAlignment(header_pane, QtCore.Qt.AlignmentFlag.AlignTop)
         self.on_drop_callback = on_drop_callback
 
+    def closeEvent(self, event):
+        """Called when the window is closed."""
+        if self.on_destroy:
+            self.on_destroy()
+        super().closeEvent(event)
+
     def show_help_dialog(self):
         """Shows a dialog with the language codes."""
         dialog = QMessageBox()
         dialog.setWindowTitle("Language Help")
         text = "Use the following language codes to specify the languages you want to translate to:\n\n"
         for key, val in LANGUAGE_CODES.items():
             text += f"{key}: {val}\n"
         dialog.setText(text)
         dialog.exec()
 
+    def create_progress_bar(self):
+        """Creates a progress bar."""
+        progress_bar = QProgressBar(self)
+        progress_bar.setMinimum(0)  # Set minimum value of the progress bar
+        progress_bar.setMaximum(0)  # Set maximum value of the progress bar
+        progress_bar.setValue(0)  # Set the current value of the progress bar
+        progress_bar.setVisible(False)  # Hide the progress bar by default
+        return progress_bar
+
     def dragEnterEvent(self, event):
         """Drag and drop handler."""
         if event.mimeData().hasUrls():
             event.accept()
         else:
             event.ignore()
 
@@ -238,8 +266,21 @@
             args=(videofile, deepl_api_key, languages, model, convert_to_webvtt),
             daemon=True,
         )
         thread_processor.add(thread)
 
     gui = MainWidget(callback)
     gui.show()
+
+    def update_function(val: bool):
+        """Updates the progress bar."""
+        data = update_function.__dict__
+        data["last_value"] = data.get("last_value", False)
+        if val == data["last_value"]:
+            return
+        data["last_value"] = val
+        gui.progress_signal.emit(val)
+
+    gui.on_destroy = thread_processor.stop
+    thread_processor.set_status_callback(update_function)
+    thread_processor.start()
     sys.exit(app.exec())
```

### Comparing `video-subtitles-1.0.6/src/video_subtitles/run.py` & `video-subtitles-1.0.7/src/video_subtitles/run.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles/say.py` & `video-subtitles-1.0.7/src/video_subtitles/say.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles/settings.py` & `video-subtitles-1.0.7/src/video_subtitles/settings.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles/thread_processor.py` & `video-subtitles-1.0.7/src/video_subtitles/thread_processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,23 +12,30 @@
     """Thread processor."""
 
     def __init__(self) -> None:
         super().__init__(daemon=True)
         self.pending_tasks: queue.Queue = queue.Queue()
         self.processing_task: threading.Thread | None = None
         self.event = threading.Event()
-        self.start()
+        self.update_status_cb = lambda _: None
+
+    def set_status_callback(self, callback) -> None:
+        """Sets the status callback."""
+        self.update_status_cb = callback
 
     def run(self) -> None:
         """Process each thread in the queue."""
         while not self.event.wait(0.1):
             if self.processing_task is not None:
+                self.update_status_cb(True)
                 if not self.processing_task.is_alive():
                     self.processing_task.join()
                     self.processing_task = None
+            else:
+                self.update_status_cb(False)
             if self.processing_task is not None:
                 continue
             if self.pending_tasks.empty():
                 continue
             self.processing_task = self.pending_tasks.get()
             self.processing_task.start()
```

### Comparing `video-subtitles-1.0.6/src/video_subtitles/translate.py` & `video-subtitles-1.0.7/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles/util.py` & `video-subtitles-1.0.7/src/video_subtitles/util.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/src/video_subtitles.egg-info/PKG-INFO` & `video-subtitles-1.0.7/src/video_subtitles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-subtitles
-Version: 1.0.6
+Version: 1.0.7
 Summary: Creates Video Subtitles
 Home-page: https://github.com/zackees/video-subtitles
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -131,14 +131,15 @@
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `ruff`, `pylint`, `flake8` and `mypy`.
 
 # Releases
 
+  * 1.0.7: Adds progress bar when doing work.
   * 1.0.6: Adds gui language help for language codes.
   * 1.0.5: Adds webvtt format option.
   * 1.0.4: Adds thread processor so that multiple files can be done one at a time.
   * 1.0.3: Adds gui.
   * 1.0.2: Fix bug.
   * 1.0.1: Adds retry to translation step. Also alerts when the video is done.
   * 1.0.0: Initial release.
```

### Comparing `video-subtitles-1.0.6/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.7/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/test.srt` & `video-subtitles-1.0.7/tests/test.srt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/test_cli.py` & `video-subtitles-1.0.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/test_full.py` & `video-subtitles-1.0.7/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/test_srt_to_webvtt.py` & `video-subtitles-1.0.7/tests/test_srt_to_webvtt.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/test_srt_translator.py` & `video-subtitles-1.0.7/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/tests/video.mp4` & `video-subtitles-1.0.7/tests/video.mp4`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.6/upload_package.py` & `video-subtitles-1.0.7/upload_package.py`

 * *Files identical despite different names*

