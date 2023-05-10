# Comparing `tmp/hledger_args-0.0.3.tar.gz` & `tmp/hledger_args-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.3.tar", last modified: Wed May 10 18:03:14 2023, max compression
+gzip compressed data, was "hledger_args-0.0.4.tar", last modified: Wed May 10 18:06:18 2023, max compression
```

## Comparing `hledger_args-0.0.3.tar` & `hledger_args-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.567464 hledger_args-0.0.3/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4227 2023-05-10 18:03:14.566464 hledger_args-0.0.3/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3887 2023-05-10 17:51:31.000000 hledger_args-0.0.3/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.555464 hledger_args-0.0.3/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3887 2023-05-10 17:51:31.000000 hledger_args-0.0.3/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.556464 hledger_args-0.0.3/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.3/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.3/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.3/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.3/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3016 2023-05-10 17:51:43.000000 hledger_args-0.0.3/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3425 2023-05-10 18:03:07.000000 hledger_args-0.0.3/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.3/hledger_args/options.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.557464 hledger_args-0.0.3/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4227 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-10 18:03:14.000000 hledger_args-0.0.3/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-10 18:02:06.000000 hledger_args-0.0.3/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-10 18:03:14.567464 hledger_args-0.0.3/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.557464 hledger_args-0.0.3/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.3/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.554464 hledger_args-0.0.3/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:03:14.566464 hledger_args-0.0.3/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.090762 hledger_args-0.0.4/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4210 2023-05-10 18:06:18.090762 hledger_args-0.0.4/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3870 2023-05-10 18:04:25.000000 hledger_args-0.0.4/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.086763 hledger_args-0.0.4/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3870 2023-05-10 18:04:25.000000 hledger_args-0.0.4/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.087762 hledger_args-0.0.4/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.4/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.4/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-09 16:59:35.000000 hledger_args-0.0.4/hledger_args/base_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1199 2023-05-09 16:57:24.000000 hledger_args-0.0.4/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3016 2023-05-10 17:51:43.000000 hledger_args-0.0.4/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3425 2023-05-10 18:03:07.000000 hledger_args-0.0.4/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.4/hledger_args/options.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.088763 hledger_args-0.0.4/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4210 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-10 18:06:18.000000 hledger_args-0.0.4/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-10 18:04:42.000000 hledger_args-0.0.4/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-10 18:06:18.090762 hledger_args-0.0.4/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.088763 hledger_args-0.0.4/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.4/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.083763 hledger_args-0.0.4/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-10 18:06:18.090762 hledger_args-0.0.4/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.4/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.3/PKG-INFO` & `hledger_args-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_args
-Version: 0.0.3
+Version: 0.0.4
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -18,20 +18,21 @@
 
 ### Interactive Mode
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
-| Placeholders | Description                                                                       |
-|--------------|-----------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                             |
-| {payee}      | fuzzy search existing payee or new                                                |
-| {tag}        | fuzzy search existing tags or values or new                                       |
-| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger-args |
+| Placeholders | Description                                                                    |
+|--------------|--------------------------------------------------------------------------------|
+| {account}    | fuzzy search existing accounts or new                                          |
+| {payee}      | fuzzy search existing payee or new                                             |
+| {tag}        | fuzzy search existing tags and values or new                                   |
+| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
 - hledger
```

### Comparing `hledger_args-0.0.3/README.md` & `hledger_args-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 ### Interactive Mode
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
-| Placeholders | Description                                                                       |
-|--------------|-----------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                             |
-| {payee}      | fuzzy search existing payee or new                                                |
-| {tag}        | fuzzy search existing tags or values or new                                       |
-| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger-args |
+| Placeholders | Description                                                                    |
+|--------------|--------------------------------------------------------------------------------|
+| {account}    | fuzzy search existing accounts or new                                          |
+| {payee}      | fuzzy search existing payee or new                                             |
+| {tag}        | fuzzy search existing tags and values or new                                   |
+| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
 - hledger
```

### Comparing `hledger_args-0.0.3/docs/README.md` & `hledger_args-0.0.4/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 ### Interactive Mode
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
-| Placeholders | Description                                                                       |
-|--------------|-----------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                             |
-| {payee}      | fuzzy search existing payee or new                                                |
-| {tag}        | fuzzy search existing tags or values or new                                       |
-| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger-args |
+| Placeholders | Description                                                                    |
+|--------------|--------------------------------------------------------------------------------|
+| {account}    | fuzzy search existing accounts or new                                          |
+| {payee}      | fuzzy search existing payee or new                                             |
+| {tag}        | fuzzy search existing tags and values or new                                   |
+| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
 - hledger
```

### Comparing `hledger_args-0.0.3/hledger_args/base_args.py` & `hledger_args-0.0.4/hledger_args/base_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/hledger_args/batch_args.py` & `hledger_args-0.0.4/hledger_args/batch_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/hledger_args/cli.py` & `hledger_args-0.0.4/hledger_args/cli.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/hledger_args/inter_args.py` & `hledger_args-0.0.4/hledger_args/inter_args.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/hledger_args/options.py` & `hledger_args-0.0.4/hledger_args/options.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/hledger_args.egg-info/PKG-INFO` & `hledger_args-0.0.4/hledger_args.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-args
-Version: 0.0.3
+Version: 0.0.4
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -18,20 +18,21 @@
 
 ### Interactive Mode
 
 Instead of giving the the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
 
 ### Special placeholders
 
-| Placeholders | Description                                                                       |
-|--------------|-----------------------------------------------------------------------------------|
-| {account}    | fuzzy search existing accounts or new                                             |
-| {payee}      | fuzzy search existing payee or new                                                |
-| {tag}        | fuzzy search existing tags or values or new                                       |
-| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger-args |
+| Placeholders | Description                                                                    |
+|--------------|--------------------------------------------------------------------------------|
+| {account}    | fuzzy search existing accounts or new                                          |
+| {payee}      | fuzzy search existing payee or new                                             |
+| {tag}        | fuzzy search existing tags and values or new                                   |
+| {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
+
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
 - hledger
```

### Comparing `hledger_args-0.0.3/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.0.4/hledger_args.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/pyproject.toml` & `hledger_args-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.3"
+version = "0.0.4"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "questionary"
```

### Comparing `hledger_args-0.0.3/venv/bin/rst2html.py` & `hledger_args-0.0.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2html4.py` & `hledger_args-0.0.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2html5.py` & `hledger_args-0.0.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2latex.py` & `hledger_args-0.0.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2man.py` & `hledger_args-0.0.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2odt.py` & `hledger_args-0.0.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.0.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2pseudoxml.py` & `hledger_args-0.0.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2s5.py` & `hledger_args-0.0.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2xetex.py` & `hledger_args-0.0.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rst2xml.py` & `hledger_args-0.0.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.3/venv/bin/rstpep2html.py` & `hledger_args-0.0.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

