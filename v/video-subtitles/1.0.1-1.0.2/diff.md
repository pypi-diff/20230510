# Comparing `tmp/video-subtitles-1.0.1.tar.gz` & `tmp/video-subtitles-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-subtitles-1.0.1.tar", last modified: Mon May  8 23:54:02 2023, max compression
+gzip compressed data, was "video-subtitles-1.0.2.tar", last modified: Tue May  9 01:55:03 2023, max compression
```

## Comparing `video-subtitles-1.0.1.tar` & `video-subtitles-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.527949 video-subtitles-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.449946 video-subtitles-1.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.485947 video-subtitles-1.0.1/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.1/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.1/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.1/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.489945 video-subtitles-1.0.1/.vscode/
--rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/launch.json
--rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5450 2023-05-08 23:54:02.527949 video-subtitles-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4660 2023-05-08 23:48:34.000000 video-subtitles-1.0.1/README.md
--rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.1/activate.sh
--rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/lint.sh
--rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/make_venv.py
--rw-rw-rw-   0        0        0      755 2023-05-08 23:34:23.000000 video-subtitles-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       66 2023-05-08 22:45:19.000000 video-subtitles-1.0.1/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 23:54:02.528947 video-subtitles-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.451947 video-subtitles-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.495946 video-subtitles-1.0.1/src/video_subtitles/
--rw-rw-rw-   0        0        0       34 2023-05-08 23:47:55.000000 video-subtitles-1.0.1/src/video_subtitles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.519946 video-subtitles-1.0.1/src/video_subtitles/assets/
--rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/src/video_subtitles/assets/example.txt
--rw-rw-rw-   0        0        0     4199 2023-05-08 23:46:45.000000 video-subtitles-1.0.1/src/video_subtitles/cli.py
--rw-rw-rw-   0        0        0     3071 2023-05-08 23:47:31.000000 video-subtitles-1.0.1/src/video_subtitles/run.py
--rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.1/src/video_subtitles/say.py
--rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.1/src/video_subtitles/translate.py
--rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.1/src/video_subtitles/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.518947 video-subtitles-1.0.1/src/video_subtitles.egg-info/
--rw-rw-rw-   0        0        0     5450 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 23:54:02.000000 video-subtitles-1.0.1/src/video_subtitles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 23:54:02.525947 video-subtitles-1.0.1/tests/
--rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.1/tests/test_cli.py
--rw-rw-rw-   0        0        0      951 2023-05-08 23:21:31.000000 video-subtitles-1.0.1/tests/test_full.py
--rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.1/tests/test_srt_translator.py
--rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.1/tests/video.mp4
--rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/tox.ini
--rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.1/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.495816 video-subtitles-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.380745 video-subtitles-1.0.2/.github/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.427290 video-subtitles-1.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      859 2023-05-08 22:48:26.000000 video-subtitles-1.0.2/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      861 2023-05-08 22:48:30.000000 video-subtitles-1.0.2/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      858 2023-05-08 22:48:34.000000 video-subtitles-1.0.2/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     2059 2023-05-08 22:03:27.000000 video-subtitles-1.0.2/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.431827 video-subtitles-1.0.2/.vscode/
+-rw-rw-rw-   0        0        0     1354 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/launch.json
+-rw-rw-rw-   0        0        0      818 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      104 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7527 2023-05-09 01:55:03.494816 video-subtitles-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6629 2023-05-09 01:53:15.000000 video-subtitles-1.0.2/README.md
+-rw-rw-rw-   0        0        0      415 2023-05-08 03:15:26.000000 video-subtitles-1.0.2/activate.sh
+-rw-rw-rw-   0        0        0      435 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/lint.sh
+-rw-rw-rw-   0        0        0     2138 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/make_venv.py
+-rw-rw-rw-   0        0        0      755 2023-05-08 23:34:23.000000 video-subtitles-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-09 01:29:01.000000 video-subtitles-1.0.2/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 01:55:03.495816 video-subtitles-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-05-08 04:34:00.000000 video-subtitles-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.382746 video-subtitles-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.440816 video-subtitles-1.0.2/src/video_subtitles/
+-rw-rw-rw-   0        0        0       34 2023-05-09 01:38:00.000000 video-subtitles-1.0.2/src/video_subtitles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.485814 video-subtitles-1.0.2/src/video_subtitles/assets/
+-rw-rw-rw-   0        0        0       54 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/src/video_subtitles/assets/example.txt
+-rw-rw-rw-   0        0        0     4199 2023-05-08 23:46:45.000000 video-subtitles-1.0.2/src/video_subtitles/cli.py
+-rw-rw-rw-   0        0        0     3061 2023-05-09 01:36:13.000000 video-subtitles-1.0.2/src/video_subtitles/run.py
+-rw-rw-rw-   0        0        0      772 2023-05-08 23:50:20.000000 video-subtitles-1.0.2/src/video_subtitles/say.py
+-rw-rw-rw-   0        0        0      841 2023-05-08 22:35:30.000000 video-subtitles-1.0.2/src/video_subtitles/translate.py
+-rw-rw-rw-   0        0        0     2373 2023-05-08 10:07:09.000000 video-subtitles-1.0.2/src/video_subtitles/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.483814 video-subtitles-1.0.2/src/video_subtitles.egg-info/
+-rw-rw-rw-   0        0        0     7527 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 01:55:03.000000 video-subtitles-1.0.2/src/video_subtitles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 01:55:03.491816 video-subtitles-1.0.2/tests/
+-rw-rw-rw-   0        0        0      622 2023-05-08 23:21:22.000000 video-subtitles-1.0.2/tests/test_cli.py
+-rw-rw-rw-   0        0        0      951 2023-05-08 23:21:31.000000 video-subtitles-1.0.2/tests/test_full.py
+-rw-rw-rw-   0        0        0     1433 2023-05-08 22:35:30.000000 video-subtitles-1.0.2/tests/test_srt_translator.py
+-rw-rw-rw-   0        0        0   313618 2023-05-08 04:41:54.000000 video-subtitles-1.0.2/tests/video.mp4
+-rw-rw-rw-   0        0        0      498 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/tox.ini
+-rw-rw-rw-   0        0        0      291 2023-05-08 03:14:30.000000 video-subtitles-1.0.2/upload_package.sh
```

### Comparing `video-subtitles-1.0.1/.github/workflows/lint.yml` & `video-subtitles-1.0.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.github/workflows/push_macos.yml` & `video-subtitles-1.0.2/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.github/workflows/push_ubuntu.yml` & `video-subtitles-1.0.2/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.github/workflows/push_win.yml` & `video-subtitles-1.0.2/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.gitignore` & `video-subtitles-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.vscode/launch.json` & `video-subtitles-1.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.vscode/settings.json` & `video-subtitles-1.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/.vscode/tasks.json` & `video-subtitles-1.0.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/LICENSE` & `video-subtitles-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/make_venv.py` & `video-subtitles-1.0.2/make_venv.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/pyproject.toml` & `video-subtitles-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/setup.py` & `video-subtitles-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/src/video_subtitles/cli.py` & `video-subtitles-1.0.2/src/video_subtitles/cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/src/video_subtitles/run.py` & `video-subtitles-1.0.2/src/video_subtitles/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """Run the program."""
     print("Running transcription")
     out_languages = out_languages.copy()
     print(f"Output languages: {out_languages}")
     print(f"Model: {model}")
     print(f"File: {file}")
     print("Done running transcription")
-    device = "cpu" if IS_GITHUB else "cuda"
+    device = "cuda" if not IS_GITHUB else "cpu"
     out_en_dir = transcribe(url_or_file=file, device=device, model=model, language="en")
     print(f"Output directory: {out_en_dir}")
     if not os.path.exists(out_en_dir):
         raise RuntimeError(f"Error - folder does not exist: {out_en_dir}")
     if "en" in out_languages:
         out_languages.remove("en")
     src_srt_file = os.path.join(out_en_dir, "out.srt")
@@ -79,9 +79,8 @@
     for srt_file in srt_files:
         language_name = os.path.basename(os.path.dirname(srt_file))
         out_file = os.path.join(outdir, f"{language_name}.srt")
         if os.path.exists(out_file):
             os.remove(out_file)
         shutil.move(srt_file, out_file)
         shutil.rmtree(os.path.dirname(srt_file))
-        break
     print("Done translating")
```

### Comparing `video-subtitles-1.0.1/src/video_subtitles/say.py` & `video-subtitles-1.0.2/src/video_subtitles/say.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/src/video_subtitles/translate.py` & `video-subtitles-1.0.2/src/video_subtitles/translate.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/src/video_subtitles/util.py` & `video-subtitles-1.0.2/src/video_subtitles/util.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/src/video_subtitles.egg-info/SOURCES.txt` & `video-subtitles-1.0.2/src/video_subtitles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/tests/test_cli.py` & `video-subtitles-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/tests/test_full.py` & `video-subtitles-1.0.2/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/tests/test_srt_translator.py` & `video-subtitles-1.0.2/tests/test_srt_translator.py`

 * *Files identical despite different names*

### Comparing `video-subtitles-1.0.1/tests/video.mp4` & `video-subtitles-1.0.2/tests/video.mp4`

 * *Files identical despite different names*

