# Comparing `tmp/texproject-0.8.7.tar.gz` & `tmp/texproject-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texproject-0.8.7.tar", last modified: Sun Apr 16 20:48:28 2023, max compression
+gzip compressed data, was "texproject-0.8.8.tar", last modified: Wed May 10 10:44:32 2023, max compression
```

## Comparing `texproject-0.8.7.tar` & `texproject-0.8.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.753260 texproject-0.8.7/
--rw-r--r--   0 alexrutar   (501) staff       (20)     1067 2023-04-16 20:46:26.000000 texproject-0.8.7/LICENSE
--rw-r--r--   0 alexrutar   (501) staff       (20)      108 2022-02-27 13:35:18.000000 texproject-0.8.7/MANIFEST.in
--rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-04-16 20:48:28.753380 texproject-0.8.7/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     5994 2023-04-16 20:46:26.000000 texproject-0.8.7/README.md
--rw-r--r--   0 alexrutar   (501) staff       (20)      359 2022-11-06 14:30:17.000000 texproject-0.8.7/pyproject.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      935 2023-04-16 20:48:28.753894 texproject-0.8.7/setup.cfg
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.740460 texproject-0.8.7/src/
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.746535 texproject-0.8.7/src/texproject/
--rw-r--r--   0 alexrutar   (501) staff       (20)      214 2023-04-16 20:47:02.000000 texproject-0.8.7/src/texproject/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       63 2021-12-14 22:57:13.000000 texproject-0.8.7/src/texproject/__main__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     3440 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/base.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    17277 2023-02-25 18:19:54.000000 texproject-0.8.7/src/texproject/command.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5653 2022-12-20 21:15:22.000000 texproject-0.8.7/src/texproject/control.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.749724 texproject-0.8.7/src/texproject/defaults/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2021-12-22 01:04:12.000000 texproject-0.8.7/src/texproject/defaults/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1186 2022-11-23 22:47:39.000000 texproject-0.8.7/src/texproject/defaults/config.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      115 2022-11-19 14:45:53.000000 texproject-0.8.7/src/texproject/defaults/template.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)      299 2022-01-13 12:30:10.000000 texproject-0.8.7/src/texproject/error.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    10385 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/filesystem.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5889 2023-04-16 20:46:17.000000 texproject-0.8.7/src/texproject/git.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    10908 2022-11-24 00:01:51.000000 texproject-0.8.7/src/texproject/output.py
--rw-r--r--   0 alexrutar   (501) staff       (20)    12788 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/template.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.752666 texproject-0.8.7/src/texproject/templates/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2022-01-05 23:14:40.000000 texproject-0.8.7/src/texproject/templates/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       61 2021-01-19 13:47:15.000000 texproject-0.8.7/src/texproject/templates/arxiv_autotex.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)      304 2021-12-16 13:57:44.000000 texproject-0.8.7/src/texproject/templates/base.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)      308 2022-11-19 23:06:18.000000 texproject-0.8.7/src/texproject/templates/bibinfo.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)       67 2020-07-09 06:18:10.000000 texproject-0.8.7/src/texproject/templates/bibliography.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)      520 2023-02-25 18:19:54.000000 texproject-0.8.7/src/texproject/templates/build.yaml
--rw-r--r--   0 alexrutar   (501) staff       (20)      842 2022-11-23 22:38:53.000000 texproject-0.8.7/src/texproject/templates/classinfo.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)       64 2021-12-21 16:46:46.000000 texproject-0.8.7/src/texproject/templates/gitignore
--rwxr-xr-x   0 alexrutar   (501) staff       (20)      559 2022-03-23 18:03:46.000000 texproject-0.8.7/src/texproject/templates/pre-commit
--rw-r--r--   0 alexrutar   (501) staff       (20)       17 2020-07-08 17:23:05.000000 texproject-0.8.7/src/texproject/templates/project_macro_file.tex
--rw-r--r--   0 alexrutar   (501) staff       (20)     4292 2023-04-16 20:46:26.000000 texproject-0.8.7/src/texproject/term.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     4992 2022-11-23 23:46:55.000000 texproject-0.8.7/src/texproject/utils.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.748847 texproject-0.8.7/src/texproject.egg-info/
--rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     1103 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/SOURCES.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/dependency_links.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       47 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/entry_points.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       53 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/requires.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       11 2023-04-16 20:48:28.000000 texproject-0.8.7/src/texproject.egg-info/top_level.txt
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-04-16 20:48:28.752986 texproject-0.8.7/test/
--rw-r--r--   0 alexrutar   (501) staff       (20)     7589 2023-02-25 18:19:54.000000 texproject-0.8.7/test/test_first.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.374362 texproject-0.8.8/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1067 2023-04-16 20:46:26.000000 texproject-0.8.8/LICENSE
+-rw-r--r--   0 alexrutar   (501) staff       (20)      108 2022-02-27 13:35:18.000000 texproject-0.8.8/MANIFEST.in
+-rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-05-10 10:44:32.374489 texproject-0.8.8/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5994 2023-04-16 20:46:26.000000 texproject-0.8.8/README.md
+-rw-r--r--   0 alexrutar   (501) staff       (20)      359 2022-11-06 14:30:17.000000 texproject-0.8.8/pyproject.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      945 2023-05-10 10:44:32.375229 texproject-0.8.8/setup.cfg
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.352212 texproject-0.8.8/src/
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.364047 texproject-0.8.8/src/texproject/
+-rw-r--r--   0 alexrutar   (501) staff       (20)      214 2023-05-10 10:43:00.000000 texproject-0.8.8/src/texproject/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       63 2021-12-14 22:57:13.000000 texproject-0.8.8/src/texproject/__main__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     3440 2023-04-16 20:46:26.000000 texproject-0.8.8/src/texproject/base.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    17277 2023-02-25 18:19:54.000000 texproject-0.8.8/src/texproject/command.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5653 2022-12-20 21:15:22.000000 texproject-0.8.8/src/texproject/control.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.366998 texproject-0.8.8/src/texproject/defaults/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2021-12-22 01:04:12.000000 texproject-0.8.8/src/texproject/defaults/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1186 2022-11-23 22:47:39.000000 texproject-0.8.8/src/texproject/defaults/config.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      115 2022-11-19 14:45:53.000000 texproject-0.8.8/src/texproject/defaults/template.toml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      299 2022-01-13 12:30:10.000000 texproject-0.8.8/src/texproject/error.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    10399 2023-05-10 10:39:53.000000 texproject-0.8.8/src/texproject/filesystem.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     5889 2023-04-16 20:46:17.000000 texproject-0.8.8/src/texproject/git.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    10908 2022-11-24 00:01:51.000000 texproject-0.8.8/src/texproject/output.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)    12788 2023-04-16 20:46:26.000000 texproject-0.8.8/src/texproject/template.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.373067 texproject-0.8.8/src/texproject/templates/
+-rw-r--r--   0 alexrutar   (501) staff       (20)        0 2022-01-05 23:14:40.000000 texproject-0.8.8/src/texproject/templates/__init__.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)       61 2021-01-19 13:47:15.000000 texproject-0.8.8/src/texproject/templates/arxiv_autotex.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)      304 2021-12-16 13:57:44.000000 texproject-0.8.8/src/texproject/templates/base.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)      308 2022-11-19 23:06:18.000000 texproject-0.8.8/src/texproject/templates/bibinfo.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)       67 2020-07-09 06:18:10.000000 texproject-0.8.8/src/texproject/templates/bibliography.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)      520 2023-02-25 18:19:54.000000 texproject-0.8.8/src/texproject/templates/build.yaml
+-rw-r--r--   0 alexrutar   (501) staff       (20)      842 2022-11-23 22:38:53.000000 texproject-0.8.8/src/texproject/templates/classinfo.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)       64 2021-12-21 16:46:46.000000 texproject-0.8.8/src/texproject/templates/gitignore
+-rwxr-xr-x   0 alexrutar   (501) staff       (20)      559 2022-03-23 18:03:46.000000 texproject-0.8.8/src/texproject/templates/pre-commit
+-rw-r--r--   0 alexrutar   (501) staff       (20)       17 2020-07-08 17:23:05.000000 texproject-0.8.8/src/texproject/templates/project_macro_file.tex
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4292 2023-04-16 20:46:26.000000 texproject-0.8.8/src/texproject/term.py
+-rw-r--r--   0 alexrutar   (501) staff       (20)     4992 2022-11-23 23:46:55.000000 texproject-0.8.8/src/texproject/utils.py
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.366161 texproject-0.8.8/src/texproject.egg-info/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     6471 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/PKG-INFO
+-rw-r--r--   0 alexrutar   (501) staff       (20)     1103 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/SOURCES.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/dependency_links.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       47 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/entry_points.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/requires.txt
+-rw-r--r--   0 alexrutar   (501) staff       (20)       11 2023-05-10 10:44:32.000000 texproject-0.8.8/src/texproject.egg-info/top_level.txt
+drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-10 10:44:32.374007 texproject-0.8.8/test/
+-rw-r--r--   0 alexrutar   (501) staff       (20)     7589 2023-02-25 18:19:54.000000 texproject-0.8.8/test/test_first.py
```

### Comparing `texproject-0.8.7/LICENSE` & `texproject-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/PKG-INFO` & `texproject-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texproject
-Version: 0.8.7
+Version: 0.8.8
 Summary: An automatic LaTeX project manager.
 Home-page: https://github.com/alexrutar/texproject
 Author: Alex Rutar
 Author-email: a@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `texproject-0.8.7/README.md` & `texproject-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/setup.cfg` & `texproject-0.8.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11.0
 install_requires = 
 	tomli-w >= 1.0.0
 	Jinja2 >= 3.1.2
-	xdg >= 5.1.1
+	xdg-base-dirs >= 6.0.0
 	click >= 8.1.3
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	tpr = texproject.command:cli
```

### Comparing `texproject-0.8.7/src/texproject/base.py` & `texproject-0.8.8/src/texproject/base.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/command.py` & `texproject-0.8.8/src/texproject/command.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/control.py` & `texproject-0.8.8/src/texproject/control.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/defaults/config.toml` & `texproject-0.8.8/src/texproject/defaults/config.toml`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/filesystem.py` & `texproject-0.8.8/src/texproject/filesystem.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from importlib.resources import files
 
 from . import defaults
 from pathlib import Path
 from tomllib import loads
 from tomli_w import dumps
-from xdg import XDG_DATA_HOME, XDG_CONFIG_HOME
+from xdg_base_dirs import xdg_data_home, xdg_config_home
 
 from .base import (
     NAMES,
     constant,
     LinkMode,
     ModCommand,
     RemoveCommand,
@@ -123,15 +123,15 @@
         self.process = self._dct["process"]
         self.github = self._dct["github"]
         self.metadata = self._dct["metadata"]
 
     @constant
     def global_path(self) -> Path:
         """TODO: write"""
-        return XDG_CONFIG_HOME / "texproject" / "config.toml"
+        return xdg_config_home() / "texproject" / "config.toml"
 
     @constant
     def local_path(self) -> Path:
         """TODO: write"""
         return self.working_dir / "config.toml"
 
 
@@ -140,15 +140,15 @@
 
     Data location constants
     """
 
     @constant
     def data_dir(self) -> Path:
         """TODO: write"""
-        return XDG_DATA_HOME / "texproject"
+        return xdg_data_home() / "texproject"
 
     @constant
     def template_dir(self) -> Path:
         """TODO: write"""
         return self.data_dir / "templates"
```

### Comparing `texproject-0.8.7/src/texproject/git.py` & `texproject-0.8.8/src/texproject/git.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/output.py` & `texproject-0.8.8/src/texproject/output.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/template.py` & `texproject-0.8.8/src/texproject/template.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/templates/build.yaml` & `texproject-0.8.8/src/texproject/templates/build.yaml`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/templates/classinfo.tex` & `texproject-0.8.8/src/texproject/templates/classinfo.tex`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/templates/pre-commit` & `texproject-0.8.8/src/texproject/templates/pre-commit`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/term.py` & `texproject-0.8.8/src/texproject/term.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject/utils.py` & `texproject-0.8.8/src/texproject/utils.py`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/src/texproject.egg-info/PKG-INFO` & `texproject-0.8.8/src/texproject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texproject
-Version: 0.8.7
+Version: 0.8.8
 Summary: An automatic LaTeX project manager.
 Home-page: https://github.com/alexrutar/texproject
 Author: Alex Rutar
 Author-email: a@rutar.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `texproject-0.8.7/src/texproject.egg-info/SOURCES.txt` & `texproject-0.8.8/src/texproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `texproject-0.8.7/test/test_first.py` & `texproject-0.8.8/test/test_first.py`

 * *Files identical despite different names*

