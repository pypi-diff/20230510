# Comparing `tmp/video-subtitles-1.0.5.tar.gz` & `tmp/video-subtitles-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.5.tar", last modified: Wed May 10 04:08:12 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.6.tar", last modified: Wed May 10 05:27:05 2023, max compression
```

## Comparing `video-subtitles-1.0.5.tar` & `video-subtitles-1.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.378723 video-subtitles-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.281725 video-subtitles-1.0.5/.github/
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.328724 video-subtitles-1.0.5/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.5/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.5/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.5/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.5/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.332723 video-subtitles-1.0.5/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     7677 2023-05-10 04:08:12.378723 video-subtitles-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6776 2023-05-10 04:06:01.000000 video-subtitles-1.0.5/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.5/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/make_venv.py
--rw-rw-rw-   0        0        0      828 2023-05-10 03:33:33.000000 video-subtitles-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.5/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 04:08:12.379724 video-subtitles-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.283726 video-subtitles-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.342723 video-subtitles-1.0.5/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-10 04:06:24.000000 video-subtitles-1.0.5/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.369723 video-subtitles-1.0.5/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     4094 2023-05-10 03:39:48.000000 video-subtitles-1.0.5/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.5/src/video_subtitles/convert_to_webvtt.py
--rw-rw-rw-   0        0        0     8119 2023-05-10 04:04:59.000000 video-subtitles-1.0.5/src/video_subtitles/gui.py
--rw-rw-rw-   0        0        0     3648 2023-05-10 03:45:37.000000 video-subtitles-1.0.5/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.5/src/video_subtitles/say.py
--rw-rw-rw-   0        0        0     2050 2023-05-10 03:57:36.000000 video-subtitles-1.0.5/src/video_subtitles/settings.py
--rw-rw-rw-   0        0        0     1354 2023-05-10 03:17:40.000000 video-subtitles-1.0.5/src/video_subtitles/thread_processor.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.5/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     2681 2023-05-10 01:39:56.000000 video-subtitles-1.0.5/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.368723 video-subtitles-1.0.5/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     7677 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 04:08:12.000000 video-subtitles-1.0.5/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 04:08:12.376723 video-subtitles-1.0.5/tests/
--rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.5/tests/test.srt
--rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.5/tests/test_cli.py
--rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.5/tests/test_full.py
--rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.5/tests/test_srt_to_webvtt.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.5/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.5/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.5/tox.ini
--rw-rw-rw-   0        0        0      953 2023-05-10 01:01:08.000000 video-subtitles-1.0.5/upload_package.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.221699 video-subtitles-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.166702 video-subtitles-1.0.6/.github/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.187700 video-subtitles-1.0.6/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.6/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.6/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.6/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2094 2023-05-10 02:09:59.000000 video-subtitles-1.0.6/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.190699 video-subtitles-1.0.6/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5489 2023-05-10 05:27:05.220703 video-subtitles-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4680 2023-05-10 05:23:03.000000 video-subtitles-1.0.6/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.6/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/make_venv.py
+-rw-rw-rw-   0        0        0      828 2023-05-10 03:33:33.000000 video-subtitles-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.6/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 05:27:05.221699 video-subtitles-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.167702 video-subtitles-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.200703 video-subtitles-1.0.6/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-10 05:22:41.000000 video-subtitles-1.0.6/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.212700 video-subtitles-1.0.6/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     3731 2023-05-10 05:21:04.000000 video-subtitles-1.0.6/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0      332 2023-05-10 03:44:22.000000 video-subtitles-1.0.6/src/video_subtitles/convert_to_webvtt.py
+-rw-rw-rw-   0        0        0     8942 2023-05-10 05:21:52.000000 video-subtitles-1.0.6/src/video_subtitles/gui.py
+-rw-rw-rw-   0        0        0     3648 2023-05-10 05:06:12.000000 video-subtitles-1.0.6/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.6/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0     2050 2023-05-10 03:57:36.000000 video-subtitles-1.0.6/src/video_subtitles/settings.py
+-rw-rw-rw-   0        0        0     1354 2023-05-10 03:17:40.000000 video-subtitles-1.0.6/src/video_subtitles/thread_processor.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.6/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     3855 2023-05-10 04:55:21.000000 video-subtitles-1.0.6/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.211701 video-subtitles-1.0.6/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     5489 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       95 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 05:27:05.000000 video-subtitles-1.0.6/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 05:27:05.219703 video-subtitles-1.0.6/tests/
+-rw-rw-rw-   0        0        0     2704 2023-05-10 03:34:47.000000 video-subtitles-1.0.6/tests/test.srt
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.6/tests/test_cli.py
+-rw-rw-rw-   0        0        0      988 2023-05-10 03:40:25.000000 video-subtitles-1.0.6/tests/test_full.py
+-rw-rw-rw-   0        0        0      656 2023-05-10 03:46:07.000000 video-subtitles-1.0.6/tests/test_srt_to_webvtt.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.6/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.6/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.6/tox.ini
+-rw-rw-rw-   0        0        0      953 2023-05-10 01:01:08.000000 video-subtitles-1.0.6/upload_package.py
```

### Comparing `video-subtitles-1.0.5/.github/workflows/lint.yml` & `video-subtitles-1.0.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.github/workflows/push_macos.yml` & `video-subtitles-1.0.6/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.6/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.github/workflows/push_win.yml` & `video-subtitles-1.0.6/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.gitignore` & `video-subtitles-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.vscode/launch.json` & `video-subtitles-1.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.vscode/settings.json` & `video-subtitles-1.0.6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/.vscode/tasks.json` & `video-subtitles-1.0.6/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/LICENSE` & `video-subtitles-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/make_venv.py` & `video-subtitles-1.0.6/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/pyproject.toml` & `video-subtitles-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/setup.py` & `video-subtitles-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/cli.py` & `video-subtitles-1.0.6/src/video_subtitles/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,26 @@
 import warnings
 
 from video_subtitles import __version__
 from video_subtitles.run import run
 from video_subtitles.say import say
 from video_subtitles.settings import Settings
 from video_subtitles.util import (
-    LANGUAGE_CODES,
     MODELS,
     GraphicsInfo,
     ensure_transcribe_anything_installed,
+    parse_languages,
     query_cuda_video_cards,
 )
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 settings = Settings()
 
 
-def parse_languages(languages_str: str) -> list[str]:
-    """Parse a comma-separated list of languages and return a list of language codes."""
-    languages = languages_str.split(",")
-    for language in languages:
-        if language not in LANGUAGE_CODES:
-            raise argparse.ArgumentTypeError(f"Invalid language code: {language}")
-    return languages
-
-
 def ensure_dependencies() -> list[GraphicsInfo]:
     """Ensure that dependencies are installed."""
     cuda_cards = query_cuda_video_cards()
     if not cuda_cards:
         raise RuntimeError("No Nvidia/CUDA video cards found.")
     ensure_transcribe_anything_installed()
     return cuda_cards
```

### Comparing `video-subtitles-1.0.5/src/video_subtitles/gui.py` & `video-subtitles-1.0.6/src/video_subtitles/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Gui for the video_subtitles package
 """
 
-# pylint: disable=no-name-in-module,c-extension-no-member,invalid-name
+# pylint: disable=no-name-in-module,c-extension-no-member,invalid-name,line-too-long
 
 import os
 import platform
 import subprocess
 import sys
 from threading import Thread
 
@@ -14,23 +14,25 @@
 from PyQt6.QtWidgets import (  # type: ignore
     QApplication,
     QComboBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMainWindow,
+    QMessageBox,
+    QPushButton,
     QVBoxLayout,
     QWidget,
 )
 
 from video_subtitles.run import run
 from video_subtitles.say import say
 from video_subtitles.settings import Settings
 from video_subtitles.thread_processor import ThreadProcessor
-from video_subtitles.util import MODELS
+from video_subtitles.util import LANGUAGE_CODES, MODELS, parse_languages
 
 settings = Settings()
 
 
 def open_folder(path):
     """Opens a folder in the OS."""
     if platform.system() == "Windows":
@@ -89,47 +91,62 @@
         # Add the convert_to_webvtt dropdown menu
         webvtt_layout = QHBoxLayout()
         self.subtitle_format = QLabel(self)
         self.subtitle_format.setText("Subtitle Format:")
         self.webvtt_select = QComboBox(self)
         self.webvtt_select.addItems(["WEBVTT", "SRT"])
         self.webvtt_select.setCurrentText(settings.subtitle_format())
+
         webvtt_layout.addWidget(self.subtitle_format)
         webvtt_layout.addWidget(self.webvtt_select)
         webvtt_layout.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft)
 
         header_layout.addLayout(deepl_layout)
         header_layout.addLayout(model_layout)
         header_layout.addLayout(webvtt_layout)
 
         # Add translation output label and text field
         output_layout = QHBoxLayout()
         self.output_label = QLabel(self)
         self.output_label.setText("Translation Outputs:")
         self.output_text = QLineEdit(self)
         self.output_text.setText(",".join(settings.languages()))
+
+        # Add the Language Help button
+        self.help_button = QPushButton("Language Help")
+        self.help_button.clicked.connect(self.show_help_dialog)
         output_layout.addWidget(self.output_label)
         output_layout.addWidget(self.output_text)
         output_layout.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeft)
+        output_layout.addWidget(self.help_button)
         header_layout.addLayout(output_layout)
 
         # Add a label to the window on top of everything else
         self.label = QLabel(self)
         self.label.setText("Drag and drop video file here for subtitles")
         self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
         # Add the header pane and label widget to the main layout
         main_layout.addWidget(header_pane)
         main_layout.addWidget(self.label)
 
         # Setting the alignment of the header pane to the top
         main_layout.setAlignment(header_pane, QtCore.Qt.AlignmentFlag.AlignTop)
-
         self.on_drop_callback = on_drop_callback
 
+    def show_help_dialog(self):
+        """Shows a dialog with the language codes."""
+        dialog = QMessageBox()
+        dialog.setWindowTitle("Language Help")
+        text = "Use the following language codes to specify the languages you want to translate to:\n\n"
+        for key, val in LANGUAGE_CODES.items():
+            text += f"{key}: {val}\n"
+        dialog.setText(text)
+        dialog.exec()
+
     def dragEnterEvent(self, event):
         """Drag and drop handler."""
         if event.mimeData().hasUrls():
             event.accept()
         else:
             event.ignore()
 
@@ -148,15 +165,20 @@
 
     def dropEvent(self, event):
         """Drag and drop handler."""
         self.save_settings()
         files = [u.toLocalFile() for u in event.mimeData().urls()]
         deepl_api_key = self.deepl_input.text().strip()  # get api key from input field
         model = self.model_select.currentText().strip()
-        languages = self.output_text.text().strip().split(",")
+        try:
+            languages = parse_languages(self.output_text.text())
+        except ValueError as ve:
+            QMessageBox.critical(self, "Error", str(ve))
+            return
+
         languages = [lang.strip() for lang in languages]
         convert_to_webvtt = self.webvtt_select.currentText().strip() == "WEBVTT"
         for f in files:
             self.on_drop_callback(
                 f, deepl_api_key, languages, model, convert_to_webvtt
             )  # pass api key to callback
```

### Comparing `video-subtitles-1.0.5/src/video_subtitles/run.py` & `video-subtitles-1.0.6/src/video_subtitles/run.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/say.py` & `video-subtitles-1.0.6/src/video_subtitles/say.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/settings.py` & `video-subtitles-1.0.6/src/video_subtitles/settings.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/thread_processor.py` & `video-subtitles-1.0.6/src/video_subtitles/thread_processor.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/translate.py` & `video-subtitles-1.0.6/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/src/video_subtitles/util.py` & `video-subtitles-1.0.6/src/video_subtitles/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Utilities for video_subtitles."""
 
+# pylint: disable=line-too-long
+
 import os
 import subprocess
 import tempfile
 from dataclasses import dataclass
 from shutil import which
 
 from download import download  # type: ignore
@@ -67,23 +69,57 @@
             rtn = subprocess.call(["python", os.path.join(tempdir, "install_cuda.py")])
             if rtn != 0:
                 raise RuntimeError(  # pylint: disable=raise-missing-from
                     "install_cuda.py failed."
                 )
 
 
+def parse_languages(languages_str: str) -> list[str]:
+    """Parse a comma-separated list of languages and return a list of language codes."""
+    languages = languages_str.split(",")
+    languages = [language.strip().lower() for language in languages]
+    for language in languages:
+        if language not in LANGUAGE_CODES:
+            raise ValueError(f"Unknown language: {language}")
+    return languages
+
+
 LANGUAGE_CODES = {
-    "en": "English",
+    "bg": "Bulgarian",
+    "cs": "Czech",
+    "da": "Danish",
+    "de": "German",
+    "el": "Greek",
+    "en": "English (unspecified variant for backward compatibility; please select EN-GB or EN-US instead)",
+    "en-gb": "English (British)",
+    "en-us": "English (American)",
     "es": "Spanish",
+    "et": "Estonian",
+    "fi": "Finnish",
     "fr": "French",
-    "de": "German",
+    "hu": "Hungarian",
+    "id": "Indonesian",
     "it": "Italian",
-    "pt": "Portuguese",
+    "ja": "Japanese",
+    "ko": "Korean",
+    "lt": "Lithuanian",
+    "lv": "Latvian",
+    "nb": "Norwegian (Bokmål)",
+    "nl": "Dutch",
+    "pl": "Polish",
+    "pt-br": "Portuguese (Brazilian)",
+    "pt-pt": "Portuguese (all Portuguese varieties excluding Brazilian Portuguese)",
+    "ro": "Romanian",
     "ru": "Russian",
-    "zh": "Chinese",
+    "sk": "Slovak",
+    "sl": "Slovenian",
+    "sv": "Swedish",
+    "tr": "Turkish",
+    "uk": "Ukrainian",
+    "zh": "Chinese (simplified)",
 }
 
 MODELS = {
     # Maps model name to number of GPU memory (in gigabytes) required.
     "tiny": 1.0,
     "base": 1.0,
     "small": 2.0,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `video-subtitles-1.0.5/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.6/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/test.srt` & `video-subtitles-1.0.6/tests/test.srt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/test_cli.py` & `video-subtitles-1.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/test_full.py` & `video-subtitles-1.0.6/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/test_srt_to_webvtt.py` & `video-subtitles-1.0.6/tests/test_srt_to_webvtt.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/test_srt_translator.py` & `video-subtitles-1.0.6/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/tests/video.mp4` & `video-subtitles-1.0.6/tests/video.mp4`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.5/upload_package.py` & `video-subtitles-1.0.6/upload_package.py`

 * *Files identical despite different names*

