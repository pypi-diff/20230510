# Comparing `tmp/JupyterQuiz-2.5.1.tar.gz` & `tmp/JupyterQuiz-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterQuiz-2.5.1.tar", last modified: Mon May  8 23:11:43 2023, max compression
+gzip compressed data, was "JupyterQuiz-2.5.2.tar", last modified: Wed May 10 09:46:57 2023, max compression
```

## Comparing `JupyterQuiz-2.5.1.tar` & `JupyterQuiz-2.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.5.1/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.5.1/CITATION.cff
--rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.5.1/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.5.1/LICENSE
--rw-r--r--   0        0        0    11048 2023-04-28 15:48:44.041844 JupyterQuiz-2.5.1/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.5.1/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.5.1/examples/num-example.gif
--rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.5.1/examples/questions.json
--rw-r--r--   0        0        0      661 2023-05-08 22:19:01.666330 JupyterQuiz-2.5.1/jupyterquiz/__init__.py
--rw-r--r--   0        0        0     9836 2023-04-28 15:36:48.745920 JupyterQuiz-2.5.1/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.5.1/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.5.1/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.5.1/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 JupyterQuiz-2.5.1/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     6192 2023-04-28 14:31:14.576981 JupyterQuiz-2.5.1/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2935 2023-04-28 15:09:47.356037 JupyterQuiz-2.5.1/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.5.1/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.5.1/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.5.1/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.5.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.5.1/schema/README
--rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.5.1/schema/mc_schema.json
--rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.5.1/schema/mc_schema.png
--rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.5.1/schema/mc_schema.svg
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.5.1/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.5.1/schema/num_schema.png
--rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.5.1/schema/schema.ipynb
--rw-r--r--   0        0        0   349141 2023-04-28 15:41:36.693358 JupyterQuiz-2.5.1/test.ipynb
--rw-r--r--   0        0        0    11362 1970-01-01 00:00:00.000000 JupyterQuiz-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.5.2/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.5.2/CITATION.cff
+-rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.5.2/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.5.2/LICENSE
+-rw-r--r--   0        0        0    11048 2023-04-28 15:48:44.041844 JupyterQuiz-2.5.2/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.5.2/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.5.2/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.5.2/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-05-10 09:46:19.315209 JupyterQuiz-2.5.2/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0     9836 2023-04-28 15:36:48.745920 JupyterQuiz-2.5.2/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.5.2/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.5.2/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.5.2/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 JupyterQuiz-2.5.2/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     6192 2023-04-28 14:31:14.576981 JupyterQuiz-2.5.2/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2935 2023-04-28 15:09:47.356037 JupyterQuiz-2.5.2/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.5.2/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.5.2/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.5.2/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.5.2/schema/README
+-rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.5.2/schema/mc_schema.json
+-rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.5.2/schema/mc_schema.png
+-rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.5.2/schema/mc_schema.svg
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.5.2/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.5.2/schema/num_schema.png
+-rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.5.2/schema/schema.ipynb
+-rw-r--r--   0        0        0   349141 2023-04-28 15:41:36.693358 JupyterQuiz-2.5.2/test.ipynb
+-rw-r--r--   0        0        0    11362 1970-01-01 00:00:00.000000 JupyterQuiz-2.5.2/PKG-INFO
```

### Comparing `JupyterQuiz-2.5.1/.gitignore` & `JupyterQuiz-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/HideQuiz.ipynb` & `JupyterQuiz-2.5.2/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/LICENSE` & `JupyterQuiz-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/README.md` & `JupyterQuiz-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/examples/mc-example.gif` & `JupyterQuiz-2.5.2/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/examples/num-example.gif` & `JupyterQuiz-2.5.2/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/examples/questions.json` & `JupyterQuiz-2.5.2/examples/questions.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/__init__.py` & `JupyterQuiz-2.5.2/jupyterquiz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.5.1'
+__version__ = '2.5.2'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/dynamic.py` & `JupyterQuiz-2.5.2/jupyterquiz/dynamic.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/helpers.js` & `JupyterQuiz-2.5.2/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/multiple_choice.js` & `JupyterQuiz-2.5.2/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/multiple_choice.py` & `JupyterQuiz-2.5.2/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/numeric.js` & `JupyterQuiz-2.5.2/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/show_questions.js` & `JupyterQuiz-2.5.2/jupyterquiz/show_questions.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/jupyterquiz/styles.css` & `JupyterQuiz-2.5.2/jupyterquiz/styles.css`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/preserve-responses.ipynb` & `JupyterQuiz-2.5.2/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/previews/github-preview.png` & `JupyterQuiz-2.5.2/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/previews/github-preview.psd` & `JupyterQuiz-2.5.2/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/mc_schema.json` & `JupyterQuiz-2.5.2/schema/mc_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/mc_schema.png` & `JupyterQuiz-2.5.2/schema/mc_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/mc_schema.svg` & `JupyterQuiz-2.5.2/schema/mc_schema.svg`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/num_schema.json` & `JupyterQuiz-2.5.2/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/num_schema.png` & `JupyterQuiz-2.5.2/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/schema/schema.ipynb` & `JupyterQuiz-2.5.2/schema/schema.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/test.ipynb` & `JupyterQuiz-2.5.2/test.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.5.1/PKG-INFO` & `JupyterQuiz-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.5.1
+Version: 2.5.2
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
```

