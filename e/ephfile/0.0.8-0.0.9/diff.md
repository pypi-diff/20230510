# Comparing `tmp/ephfile-0.0.8.tar.gz` & `tmp/ephfile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephfile-0.0.8.tar", last modified: Wed May 10 13:50:08 2023, max compression
+gzip compressed data, was "ephfile-0.0.9.tar", last modified: Wed May 10 13:53:07 2023, max compression
```

## Comparing `ephfile-0.0.8.tar` & `ephfile-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:50:08.490382 ephfile-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 13:50:04.000000 ephfile-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:50:08.490382 ephfile-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 13:50:04.000000 ephfile-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:50:08.486382 ephfile-0.0.8/ephfile/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2908 2023-05-10 13:50:04.000000 ephfile-0.0.8/ephfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:50:08.486382 ephfile-0.0.8/ephfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:50:08.000000 ephfile-0.0.8/ephfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 13:50:08.000000 ephfile-0.0.8/ephfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:50:08.000000 ephfile-0.0.8/ephfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:50:08.000000 ephfile-0.0.8/ephfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:50:08.490382 ephfile-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3149 2023-05-10 13:50:04.000000 ephfile-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:53:07.069291 ephfile-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 13:53:02.000000 ephfile-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:53:07.069291 ephfile-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 13:53:02.000000 ephfile-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:53:07.069291 ephfile-0.0.9/ephfile/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-05-10 13:53:02.000000 ephfile-0.0.9/ephfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:53:07.069291 ephfile-0.0.9/ephfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:53:07.000000 ephfile-0.0.9/ephfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 13:53:07.000000 ephfile-0.0.9/ephfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:53:07.000000 ephfile-0.0.9/ephfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:53:07.000000 ephfile-0.0.9/ephfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:53:07.069291 ephfile-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3149 2023-05-10 13:53:02.000000 ephfile-0.0.9/setup.py
```

### Comparing `ephfile-0.0.8/LICENSE` & `ephfile-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ephfile-0.0.8/ephfile/__init__.py` & `ephfile-0.0.9/ephfile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os,sys,shutil
 
 class ephfile(object):
 	def __init__(self,foil=None,contents=None,create=True, contents_lambda=None, delete=True):
 		self.delete=delete
-		to_str = lambda x:str(x)
+		to_str = lambda x:str(x) + "\n"
 		if foil is None:
 			import tempfile
 			self.named = tempfile.NamedTemporaryFile()
 			self.foil = self.named.name
 		else:
 			self.named = None
 			if not os.path.exists(foil) and create:
```

### Comparing `ephfile-0.0.8/setup.py` & `ephfile-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

