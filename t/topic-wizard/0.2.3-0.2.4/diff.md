# Comparing `tmp/topic_wizard-0.2.3.tar.gz` & `tmp/topic_wizard-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.2.3.tar", max compression
+gzip compressed data, was "topic_wizard-0.2.4.tar", max compression
```

## Comparing `topic_wizard-0.2.3.tar` & `topic_wizard-0.2.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.3/LICENSE
--rw-r--r--   0        0        0     2140 2023-03-13 12:27:09.710202 topic_wizard-0.2.3/README.md
--rw-r--r--   0        0        0      640 2023-04-25 07:41:20.946715 topic_wizard-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      129 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/__init__.py
--rw-r--r--   0        0        0     7178 2023-02-19 18:11:00.271490 topic_wizard-0.2.3/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.3/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4339 2023-04-24 14:06:16.382303 topic_wizard-0.2.3/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0     1355 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     5195 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3143 2023-04-24 14:37:23.038262 topic_wizard-0.2.3/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0        0 2023-04-24 14:55:26.304691 topic_wizard-0.2.3/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.3/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.3/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.3/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.3/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.3/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.3/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.3/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.3/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.3/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5178 2023-04-24 14:10:21.226703 topic_wizard-0.2.3/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.3/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.3/topicwizard/plots/words.py
--rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.3/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     3796 2023-04-24 13:29:24.942145 topic_wizard-0.2.3/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.3/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.3/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     3422 1970-01-01 00:00:00.000000 topic_wizard-0.2.3/setup.py
--rw-r--r--   0        0        0     3163 1970-01-01 00:00:00.000000 topic_wizard-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-29 12:25:42.522855 topic_wizard-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2142 2023-05-05 08:47:51.298632 topic_wizard-0.2.4/README.md
+-rw-r--r--   0        0        0      640 2023-05-10 13:43:20.671757 topic_wizard-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-05-10 13:39:02.256545 topic_wizard-0.2.4/topicwizard/__init__.py
+-rw-r--r--   0        0        0     7219 2023-05-06 10:19:10.654488 topic_wizard-0.2.4/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     5602 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4339 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     1355 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     5195 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3143 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3080 2023-05-10 12:08:24.294778 topic_wizard-0.2.4/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6652 2023-05-06 08:12:06.292221 topic_wizard-0.2.4/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1468 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0        0 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-06 08:17:16.043369 topic_wizard-0.2.4/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4257 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0     3503 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/plots/words.py
+-rw-r--r--   0        0        0     2708 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     4895 2023-05-10 13:42:17.894976 topic_wizard-0.2.4/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-29 12:25:42.566855 topic_wizard-0.2.4/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-05-05 08:47:51.306632 topic_wizard-0.2.4/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 topic_wizard-0.2.4/PKG-INFO
```

### Comparing `topic_wizard-0.2.3/LICENSE` & `topic_wizard-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/README.md` & `topic_wizard-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 [![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)
 [![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)
 [![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
-https://user-images.githubusercontent.com/13087737/219967955-1263c35b-4c5b-4ccc-adb9-23e073e099f0.mp4
+
+https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
+
 
 
 ## Features
 
 -   Investigate complex relations between topics, words and documents
 -   Highly interactive
 -   Name topics
```

### Comparing `topic_wizard-0.2.3/pyproject.toml` & `topic_wizard-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.2.3"
+version = "0.2.4"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.2.3/topicwizard/app.py` & `topic_wizard-0.2.4/topicwizard/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Iterable, List, Optional, Callable
-import sys
-import time
+import os
 import subprocess
+import sys
 import threading
-import os
-import joblib
+import time
+from typing import Any, Callable, Iterable, List, Optional
 
+import joblib
 from dash_extensions.enrich import Dash, DashBlueprint
 from sklearn.pipeline import Pipeline
 
-from topicwizard.blueprints.template import prepare_blueprint
 from topicwizard.blueprints.app import create_blueprint
+from topicwizard.blueprints.template import prepare_blueprint
 
 
 def is_notebook() -> bool:
     return "ipykernel" in sys.modules
 
 
 def is_colab() -> bool:
@@ -146,25 +146,27 @@
         from google.colab import output  # type: ignore
 
         thread = threading.Thread(target=run_silent(app, port))
         thread.start()
         time.sleep(4)
 
         print("Open in browser:")
-        output.serve_kernel_port_as_window(port, anchor_text="Click this link to open topicwizard.")
+        output.serve_kernel_port_as_window(
+            port, anchor_text="Click this link to open topicwizard."
+        )
         return thread
 
-    elif is_notebook():
-        from IPython.display import IFrame, display
-
-        thread = threading.Thread(target=run_silent(app, port))
-        thread.start()
-        time.sleep(4)
-        display(IFrame(src=url, width="1200", height="1000"))
-        return thread
+    # elif is_notebook():
+    #     from IPython.display import IFrame, display
+    #
+    #     thread = threading.Thread(target=run_silent(app, port))
+    #     thread.start()
+    #     time.sleep(4)
+    #     display(IFrame(src=url, width="1200", height="1000"))
+    #     return thread
     else:
         open_url(url)
         app.run_server(port=port)
 
 
 def load(
     filename: str,
```

### Comparing `topic_wizard-0.2.3/topicwizard/assets/favicon.ico` & `topic_wizard-0.2.4/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/blueprints/app.py` & `topic_wizard-0.2.4/topicwizard/blueprints/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/blueprints/documents.py` & `topic_wizard-0.2.4/topicwizard/blueprints/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/blueprints/template.py` & `topic_wizard-0.2.4/topicwizard/blueprints/template.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/blueprints/topics.py` & `topic_wizard-0.2.4/topicwizard/blueprints/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/blueprints/words.py` & `topic_wizard-0.2.4/topicwizard/blueprints/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/document_map.py` & `topic_wizard-0.2.4/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.2.4/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.2.4/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.2.4/topicwizard/components/documents/document_timeline.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.2.4/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.2.4/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.2.4/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.2.4/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.2.4/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.2.4/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/words/association_slider.py` & `topic_wizard-0.2.4/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.2.4/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/words/word_map.py` & `topic_wizard-0.2.4/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/components/words/word_selector.py` & `topic_wizard-0.2.4/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/plots/documents.py` & `topic_wizard-0.2.4/topicwizard/plots/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     )
     return fig
 
 
 def document_wordcloud(
     doc_id: int, document_term_matrix: np.ndarray, vocab: np.ndarray
 ) -> go.Figure:
-    coo = spr.coo_array(document_term_matrix[doc_id])
+    coo = spr.coo_array(document_term_matrix[[doc_id], :])
     term_dict = {vocab[column]: data for column, data in zip(coo.col, coo.data)}
     cloud = WordCloud(
         width=800,
         height=800,
         background_color="white",
         colormap="twilight",
         scale=4,
```

### Comparing `topic_wizard-0.2.3/topicwizard/plots/topics.py` & `topic_wizard-0.2.4/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/plots/words.py` & `topic_wizard-0.2.4/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/prepare/documents.py` & `topic_wizard-0.2.4/topicwizard/prepare/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/prepare/utils.py` & `topic_wizard-0.2.4/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/topicwizard/prepare/words.py` & `topic_wizard-0.2.4/topicwizard/prepare/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.3/PKG-INFO` & `topic_wizard-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,17 @@
 [![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)
 [![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)
 [![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)
 [![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)
 <br>
 
 
-https://user-images.githubusercontent.com/13087737/219967955-1263c35b-4c5b-4ccc-adb9-23e073e099f0.mp4
+
+https://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4
+
 
 
 ## Features
 
 -   Investigate complex relations between topics, words and documents
 -   Highly interactive
 -   Name topics
```

