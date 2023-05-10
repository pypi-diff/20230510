# Comparing `tmp/hledger_args-0.0.1.tar.gz` & `tmp/hledger_args-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.1.tar", last modified: Tue May  9 22:13:23 2023, max compression
+gzip compressed data, was "hledger_args-0.0.2.tar", last modified: Tue May  9 22:17:41 2023, max compression
```

## Comparing `hledger_args-0.0.1.tar` & `hledger_args-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.611551 hledger_args-0.0.1/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      498 2023-05-09 22:13:23.610551 hledger_args-0.0.1/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3402 2023-05-09 22:09:08.000000 hledger_args-0.0.1/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.603551 hledger_args-0.0.1/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      158 2023-05-09 19:52:11.000000 hledger_args-0.0.1/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.605551 hledger_args-0.0.1/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.1/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.1/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.1/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.1/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3005 2023-05-09 20:06:49.000000 hledger_args-0.0.1/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2497 2023-05-09 18:45:24.000000 hledger_args-0.0.1/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.1/hledger_args/options.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.606551 hledger_args-0.0.1/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      498 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-09 22:13:23.000000 hledger_args-0.0.1/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-09 19:27:27.000000 hledger_args-0.0.1/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-09 22:13:23.611551 hledger_args-0.0.1/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.606551 hledger_args-0.0.1/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.1/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.603551 hledger_args-0.0.1/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:13:23.610551 hledger_args-0.0.1/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.134073 hledger_args-0.0.2/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3742 2023-05-09 22:17:41.134073 hledger_args-0.0.2/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3402 2023-05-09 22:09:08.000000 hledger_args-0.0.2/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.129073 hledger_args-0.0.2/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3402 2023-05-09 22:09:08.000000 hledger_args-0.0.2/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.130073 hledger_args-0.0.2/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.2/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.2/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.2/hledger_args/base_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.2/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3005 2023-05-09 20:06:49.000000 hledger_args-0.0.2/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2497 2023-05-09 18:45:24.000000 hledger_args-0.0.2/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.2/hledger_args/options.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.132073 hledger_args-0.0.2/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3742 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-09 22:17:41.000000 hledger_args-0.0.2/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-09 22:17:30.000000 hledger_args-0.0.2/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-09 22:17:41.134073 hledger_args-0.0.2/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.132073 hledger_args-0.0.2/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.2/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.128073 hledger_args-0.0.2/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 22:17:41.134073 hledger_args-0.0.2/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.2/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.1/README.md` & `hledger_args-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args/base_args.py` & `hledger_args-0.0.2/hledger_args/base_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args/batch_args.py` & `hledger_args-0.0.2/hledger_args/batch_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args/cli.py` & `hledger_args-0.0.2/hledger_args/cli.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args/inter_args.py` & `hledger_args-0.0.2/hledger_args/inter_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args/options.py` & `hledger_args-0.0.2/hledger_args/options.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.0.2/hledger_args.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/pyproject.toml` & `hledger_args-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.1"
+version = "0.0.2"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "questionary"
```

### Comparing `hledger_args-0.0.1/venv/bin/rst2html.py` & `hledger_args-0.0.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2html4.py` & `hledger_args-0.0.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2html5.py` & `hledger_args-0.0.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2latex.py` & `hledger_args-0.0.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2man.py` & `hledger_args-0.0.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2odt.py` & `hledger_args-0.0.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.0.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2pseudoxml.py` & `hledger_args-0.0.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2s5.py` & `hledger_args-0.0.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2xetex.py` & `hledger_args-0.0.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rst2xml.py` & `hledger_args-0.0.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.1/venv/bin/rstpep2html.py` & `hledger_args-0.0.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

