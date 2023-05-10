# Comparing `tmp/redlines-0.2.2.tar.gz` & `tmp/redlines-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redlines-0.2.2.tar", max compression
+gzip compressed data, was "redlines-0.3.0.tar", max compression
```

## Comparing `redlines-0.2.2.tar` & `redlines-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1067 2022-02-12 16:02:49.948179 redlines-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2275 2022-02-13 09:06:02.982480 redlines-0.2.2/README.md
--rw-r--r--   0        0        0      611 2022-02-15 16:01:59.241354 redlines-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       31 2022-02-13 09:03:05.789101 redlines-0.2.2/redlines/__init__.py
--rw-r--r--   0        0        0     4100 2022-02-15 15:46:52.154972 redlines-0.2.2/redlines/redlines.py
--rw-r--r--   0        0        0     2990 2022-02-16 14:20:51.861513 redlines-0.2.2/setup.py
--rw-r--r--   0        0        0     2937 2022-02-16 14:20:51.861765 redlines-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-10 14:46:40.787757 redlines-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2679 2023-05-10 14:46:40.787757 redlines-0.3.0/README.md
+-rw-r--r--   0        0        0      611 2023-05-10 14:46:40.787757 redlines-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-05-10 14:46:40.787757 redlines-0.3.0/redlines/__init__.py
+-rw-r--r--   0        0        0     7824 2023-05-10 14:46:40.787757 redlines-0.3.0/redlines/redlines.py
+-rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 redlines-0.3.0/PKG-INFO
```

### Comparing `redlines-0.2.2/LICENSE.txt` & `redlines-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redlines-0.2.2/README.md` & `redlines-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Redlines
+![Repository banner image](repository-open-graph.png)
 
 `Redlines` produces a Markdown text showing the differences between two strings/text. The changes are represented with
 strike-throughs and underlines, which looks similar to Microsoft Word's track changes. This method of showing changes is
 more familiar to lawyers and is more compact for long series of characters.
 
 Redlines uses [SequenceMatcher](https://docs.python.org/3/library/difflib.html#difflib.SequenceMatcher)
 to find differences between words used.
 
 ## Example
 
 Given an original string:
 
-    The quick brown fox jumps over the lazy dog.`
+    The quick brown fox jumps over the lazy dog.
 
 And the string to be tested with:
 
     The quick brown fox walks past the lazy dog.
 
 The library gives a result of:
 
@@ -34,32 +35,48 @@
 ## Usage
 
 The library contains one class: `Redlines`, which is used to compare text.
 
 ```python
 from redlines import Redlines
 
-test = Redlines("The quick brown fox jumps over the lazy dog.",
-                "The quick brown fox walks past the lazy dog.")
-assert test.output_markdown == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+test = Redlines(
+    "The quick brown fox jumps over the lazy dog.",
+    "The quick brown fox walks past the lazy dog.",
+)
+assert (
+        test.output_markdown
+        == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+)
 ```
 
 Alternatively, you can create Redline with the text to be tested, and compare several times to see the results.
 
 ```python
 from redlines import Redlines
 
 test = Redlines("The quick brown fox jumps over the lazy dog.")
-assert test.compare(
-    'The quick brown fox walks past the lazy dog.') == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
-
-assert test.compare(
-    'The quick brown fox jumps over the dog.') == 'The quick brown fox jumps over the <del>lazy </del>dog.'
+assert (
+        test.compare("The quick brown fox walks past the lazy dog.")
+        == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+)
+
+assert (
+        test.compare("The quick brown fox jumps over the dog.")
+        == "The quick brown fox jumps over the <del>lazy </del>dog."
+)
 ```
 
+## Uses
+
+* View and mark changes in legislation: [PLUS Explorer](https://houfu-plus-explorer.streamlit.app/)
+* Visualise changes after ChatGPT transforms a
+  text: [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
+  Lesson 6
+
 ## Roadmap / Contributing
 
 Please feel free to post issues and comments. I work on this in my free time, so please excuse lack of activity.
 
 ### Nice things to do
 
 * Style the way changes are presented
```

### Comparing `redlines-0.2.2/pyproject.toml` & `redlines-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redlines"
-version = "0.2.2"
+version = "0.3.0"
 description = "Compare text, and produce human-readable differences or deltas which look like track changes in Microsoft Word."
 authors = ["houfu <houfu@lovelawrobots.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/houfu/redlines"
 repository = "https://github.com/houfu/redlines"
```

### Comparing `redlines-0.2.2/PKG-INFO` & `redlines-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: redlines
-Version: 0.2.2
+Version: 0.3.0
 Summary: Compare text, and produce human-readable differences or deltas which look like track changes in Microsoft Word.
 Home-page: https://github.com/houfu/redlines
 License: MIT
 Author: houfu
 Author-email: houfu@lovelawrobots.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/houfu/redlines
 Description-Content-Type: text/markdown
 
 # Redlines
+![Repository banner image](repository-open-graph.png)
 
 `Redlines` produces a Markdown text showing the differences between two strings/text. The changes are represented with
 strike-throughs and underlines, which looks similar to Microsoft Word's track changes. This method of showing changes is
 more familiar to lawyers and is more compact for long series of characters.
 
 Redlines uses [SequenceMatcher](https://docs.python.org/3/library/difflib.html#difflib.SequenceMatcher)
 to find differences between words used.
 
 ## Example
 
 Given an original string:
 
-    The quick brown fox jumps over the lazy dog.`
+    The quick brown fox jumps over the lazy dog.
 
 And the string to be tested with:
 
     The quick brown fox walks past the lazy dog.
 
 The library gives a result of:
 
@@ -51,32 +53,48 @@
 ## Usage
 
 The library contains one class: `Redlines`, which is used to compare text.
 
 ```python
 from redlines import Redlines
 
-test = Redlines("The quick brown fox jumps over the lazy dog.",
-                "The quick brown fox walks past the lazy dog.")
-assert test.output_markdown == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+test = Redlines(
+    "The quick brown fox jumps over the lazy dog.",
+    "The quick brown fox walks past the lazy dog.",
+)
+assert (
+        test.output_markdown
+        == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+)
 ```
 
 Alternatively, you can create Redline with the text to be tested, and compare several times to see the results.
 
 ```python
 from redlines import Redlines
 
 test = Redlines("The quick brown fox jumps over the lazy dog.")
-assert test.compare(
-    'The quick brown fox walks past the lazy dog.') == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
-
-assert test.compare(
-    'The quick brown fox jumps over the dog.') == 'The quick brown fox jumps over the <del>lazy </del>dog.'
+assert (
+        test.compare("The quick brown fox walks past the lazy dog.")
+        == "The quick brown fox <del>jumps over </del><ins>walks past </ins>the lazy dog."
+)
+
+assert (
+        test.compare("The quick brown fox jumps over the dog.")
+        == "The quick brown fox jumps over the <del>lazy </del>dog."
+)
 ```
 
+## Uses
+
+* View and mark changes in legislation: [PLUS Explorer](https://houfu-plus-explorer.streamlit.app/)
+* Visualise changes after ChatGPT transforms a
+  text: [ChatGPT Prompt Engineering for Developers](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)
+  Lesson 6
+
 ## Roadmap / Contributing
 
 Please feel free to post issues and comments. I work on this in my free time, so please excuse lack of activity.
 
 ### Nice things to do
 
 * Style the way changes are presented
```

