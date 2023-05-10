# Comparing `tmp/sample-git-diffs-0.3.0.tar.gz` & `tmp/sample-git-diffs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-git-diffs-0.3.0.tar", max compression
+gzip compressed data, was "sample-git-diffs-0.3.1.tar", max compression
```

## Comparing `sample-git-diffs-0.3.0.tar` & `sample-git-diffs-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      594 2023-05-10 12:18:37.061714 sample-git-diffs-0.3.0/README.md
--rw-r--r--   0        0        0      523 2023-05-10 12:56:41.321425 sample-git-diffs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.3.0/sample_git_diffs/__init__.py
--rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.3.0/sample_git_diffs/sample_git_diffs.py
--rw-r--r--   0        0        0     1818 2023-05-10 12:54:09.583903 sample-git-diffs-0.3.0/sample_git_diffs/to_md.py
--rw-r--r--   0        0        0     1453 2023-05-10 12:56:51.966426 sample-git-diffs-0.3.0/setup.py
--rw-r--r--   0        0        0     1189 2023-05-10 12:56:51.966778 sample-git-diffs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1367 2023-05-10 13:06:01.433668 sample-git-diffs-0.3.1/README.md
+-rw-r--r--   0        0        0      523 2023-05-10 13:06:17.126366 sample-git-diffs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.3.1/sample_git_diffs/__init__.py
+-rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.3.1/sample_git_diffs/sample_git_diffs.py
+-rw-r--r--   0        0        0     1818 2023-05-10 12:54:09.583903 sample-git-diffs-0.3.1/sample_git_diffs/to_md.py
+-rw-r--r--   0        0        0     2259 2023-05-10 13:06:24.739221 sample-git-diffs-0.3.1/setup.py
+-rw-r--r--   0        0        0     1962 2023-05-10 13:06:24.739409 sample-git-diffs-0.3.1/PKG-INFO
```

### Comparing `sample-git-diffs-0.3.0/pyproject.toml` & `sample-git-diffs-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sample-git-diffs"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["ninpnin <you@example.com>"]
 packages = [{include = "sample_git_diffs"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ninpnin/sample-git-diffs"
```

### Comparing `sample-git-diffs-0.3.0/sample_git_diffs/sample_git_diffs.py` & `sample-git-diffs-0.3.1/sample_git_diffs/sample_git_diffs.py`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.3.0/sample_git_diffs/to_md.py` & `sample-git-diffs-0.3.1/sample_git_diffs/to_md.py`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.3.0/PKG-INFO` & `sample-git-diffs-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-git-diffs
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Home-page: https://github.com/ninpnin/sample-git-diffs
 License: MIT
 Author: ninpnin
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,7 +30,32 @@
 ```
 
 For example, if you want to draw a sample of 25 diffs from the folder data/, you run
 
 ```
 sample-git-diffs --diffstat "git diff --stat data/" --n 25
 ```
+
+To save this to changes.diff, you run
+
+```
+sample-git-diffs --diffstat "git diff --stat data/" --n 25 > changes.diff
+```
+
+There's also a script that converts the generated .diff / .patch files into markdown.
+
+```
+usage: diff2markdown [-h] --path PATH [--username USERNAME] [--reponame REPONAME] [--branch BRANCH]
+
+optional arguments:
+  -h, --help           show this help message and exit
+  --path PATH
+  --username USERNAME
+  --reponame REPONAME
+  --branch BRANCH
+```
+
+For example, if you want to convert the changes.diff file into markdown, assuming that the repo is called 'sample-git-diffs', you're on branch 'main' and the github username is 'testuser', you run
+
+```
+diff2markdown --path changes.diff --username testuser --reponame sample-git-diffs --branch main
+```
```

