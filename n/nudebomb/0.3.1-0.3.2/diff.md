# Comparing `tmp/nudebomb-0.3.1.tar.gz` & `tmp/nudebomb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nudebomb-0.3.1.tar", max compression
+gzip compressed data, was "nudebomb-0.3.2.tar", max compression
```

## Comparing `nudebomb-0.3.1.tar` & `nudebomb-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2023-05-10 04:20:46.541169 nudebomb-0.3.1/LICENSE
--rw-r--r--   0        0        0     1014 2023-05-10 04:20:46.541169 nudebomb-0.3.1/NEWS.md
--rw-r--r--   0        0        0     2255 2023-05-10 04:20:46.541169 nudebomb-0.3.1/README.md
--rw-r--r--   0        0        0       16 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/__init__.py
--rw-r--r--   0        0        0     4479 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/cli.py
--rw-r--r--   0        0        0     3950 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/config.py
--rw-r--r--   0        0        0      290 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/config_default.yaml
--rw-r--r--   0        0        0     2589 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/langfiles.py
--rw-r--r--   0        0        0     7015 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/mkv.py
--rw-r--r--   0        0        0      442 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/track.py
--rw-r--r--   0        0        0      344 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/version.py
--rw-r--r--   0        0        0     4526 2023-05-10 04:20:46.541169 nudebomb-0.3.1/nudebomb/walk.py
--rw-r--r--   0        0        0     3853 2023-05-10 04:20:46.545165 nudebomb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-10 04:20:46.545165 nudebomb-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2396 2023-05-10 04:20:46.545165 nudebomb-0.3.1/tests/mockdata/clean_tracks.json
--rw-r--r--   0        0        0  5100034 2023-05-10 04:20:46.553158 nudebomb-0.3.1/tests/test_files/test5.mkv
--rw-r--r--   0        0        0     1908 2023-05-10 04:20:46.553158 nudebomb-0.3.1/tests/test_integrated.py
--rw-r--r--   0        0        0     2335 2023-05-10 04:20:46.553158 nudebomb-0.3.1/tests/test_mkv.py
--rw-r--r--   0        0        0      810 2023-05-10 04:20:46.553158 nudebomb-0.3.1/tests/test_track.py
--rw-r--r--   0        0        0      622 2023-05-10 04:20:46.553158 nudebomb-0.3.1/tests/util.py
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 nudebomb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 05:18:27.157465 nudebomb-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1097 2023-05-10 05:18:27.157465 nudebomb-0.3.2/NEWS.md
+-rw-r--r--   0        0        0     2255 2023-05-10 05:18:27.157465 nudebomb-0.3.2/README.md
+-rw-r--r--   0        0        0       16 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/__init__.py
+-rw-r--r--   0        0        0     4479 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/cli.py
+-rw-r--r--   0        0        0     3950 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/config.py
+-rw-r--r--   0        0        0      290 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/config_default.yaml
+-rw-r--r--   0        0        0     2589 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/langfiles.py
+-rw-r--r--   0        0        0     7015 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/mkv.py
+-rw-r--r--   0        0        0      442 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/track.py
+-rw-r--r--   0        0        0      344 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/version.py
+-rw-r--r--   0        0        0     4526 2023-05-10 05:18:27.157465 nudebomb-0.3.2/nudebomb/walk.py
+-rw-r--r--   0        0        0     3853 2023-05-10 05:18:27.161465 nudebomb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 05:18:27.161465 nudebomb-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     2396 2023-05-10 05:18:27.161465 nudebomb-0.3.2/tests/mockdata/clean_tracks.json
+-rw-r--r--   0        0        0  5100034 2023-05-10 05:18:27.169465 nudebomb-0.3.2/tests/test_files/test5.mkv
+-rw-r--r--   0        0        0     1908 2023-05-10 05:18:27.169465 nudebomb-0.3.2/tests/test_integrated.py
+-rw-r--r--   0        0        0     2335 2023-05-10 05:18:27.169465 nudebomb-0.3.2/tests/test_mkv.py
+-rw-r--r--   0        0        0      810 2023-05-10 05:18:27.169465 nudebomb-0.3.2/tests/test_track.py
+-rw-r--r--   0        0        0      622 2023-05-10 05:18:27.169465 nudebomb-0.3.2/tests/util.py
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 nudebomb-0.3.2/PKG-INFO
```

### Comparing `nudebomb-0.3.1/LICENSE` & `nudebomb-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/NEWS.md` & `nudebomb-0.3.2/NEWS.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # 📰 Nudebomb News
 
+## v0.3.2
+
+- Upstream treestamps returns to relative stamp paths for portability.
+
 ## v0.3.1
 
 - Upstream treestamps fixes crashes and check_config option.
 
 ## v0.3.0
 
 - Features
```

### Comparing `nudebomb-0.3.1/README.md` & `nudebomb-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/nudebomb/cli.py` & `nudebomb-0.3.2/nudebomb/cli.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/nudebomb/config.py` & `nudebomb-0.3.2/nudebomb/config.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/nudebomb/langfiles.py` & `nudebomb-0.3.2/nudebomb/langfiles.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/nudebomb/mkv.py` & `nudebomb-0.3.2/nudebomb/mkv.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/nudebomb/walk.py` & `nudebomb-0.3.2/nudebomb/walk.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/pyproject.toml` & `nudebomb-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nudebomb"
-version = "0.3.1"
+version = "0.3.2"
 description = "Strip unused languages from mkv files en mass"
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/nudebomb"
 documentation = "https://github.com/ajslater/nudebomb"
 keywords = ["mkv", "movie", "video", "srt", "audio", "subtitles"]
@@ -26,15 +26,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 confuse = "^2.0.0"
 pycountry = "^22.3.5"
 python-dateutil = "^2.8.2"
 "ruamel.yaml" = "^0.17.21"
-treestamps = "^0.4.1"
+treestamps = "^0.4.2"
 termcolor = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
 neovim = "^0.3.1"
```

### Comparing `nudebomb-0.3.1/tests/mockdata/clean_tracks.json` & `nudebomb-0.3.2/tests/mockdata/clean_tracks.json`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/tests/test_files/test5.mkv` & `nudebomb-0.3.2/tests/test_files/test5.mkv`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/tests/test_integrated.py` & `nudebomb-0.3.2/tests/test_integrated.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/tests/test_mkv.py` & `nudebomb-0.3.2/tests/test_mkv.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/tests/test_track.py` & `nudebomb-0.3.2/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/tests/util.py` & `nudebomb-0.3.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `nudebomb-0.3.1/PKG-INFO` & `nudebomb-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nudebomb
-Version: 0.3.1
+Version: 0.3.2
 Summary: Strip unused languages from mkv files en mass
 Home-page: https://github.com/ajslater/nudebomb
 License: GPL-3.0-only
 Keywords: mkv,movie,video,srt,audio,subtitles
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Requires-Dist: confuse (>=2.0.0,<3.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
-Requires-Dist: treestamps (>=0.4.1,<0.5.0)
+Requires-Dist: treestamps (>=0.4.2,<0.5.0)
 Project-URL: Documentation, https://github.com/ajslater/nudebomb
 Project-URL: Issues, https://github.com/ajslater/nudebomb/issues
 Project-URL: Source, https://github.com/ajslater/nudebomb
 Description-Content-Type: text/markdown
 
 # Nudebomb
```

