# Comparing `tmp/chatplayground-1.1.0.tar.gz` & `tmp/chatplayground-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatplayground-1.1.0.tar", max compression
+gzip compressed data, was "chatplayground-1.1.1.tar", max compression
```

## Comparing `chatplayground-1.1.0.tar` & `chatplayground-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-09 22:48:34.566951 chatplayground-1.1.0/LICENSE
--rw-r--r--   0        0        0     4471 2023-05-09 22:48:34.566951 chatplayground-1.1.0/README.md
--rw-r--r--   0        0        0       17 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/.gitignore
--rw-r--r--   0        0        0       22 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/app/__init__.py
--rw-r--r--   0        0        0   108083 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/app/app.py
--rw-r--r--   0        0        0    15406 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/assets/favicon.ico
--rw-r--r--   0        0        0     1281 2023-05-09 22:48:34.566951 chatplayground-1.1.0/chatplayground/assets/react-json-view-lite.css
--rw-r--r--   0        0        0   178190 2023-05-09 22:48:34.570951 chatplayground-1.1.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
--rw-r--r--   0        0        0      846 2023-05-09 22:48:34.570951 chatplayground-1.1.0/chatplayground/pcconfig.py
--rw-r--r--   0        0        0     3081 2023-05-09 22:48:34.594951 chatplayground-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6838 1970-01-01 00:00:00.000000 chatplayground-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 09:42:40.414148 chatplayground-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4574 2023-05-10 09:42:40.414148 chatplayground-1.1.1/README.md
+-rw-r--r--   0        0        0       17 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/.gitignore
+-rw-r--r--   0        0        0       22 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/app/__init__.py
+-rw-r--r--   0        0        0   108121 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/app/app.py
+-rw-r--r--   0        0        0    15406 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/assets/favicon.ico
+-rw-r--r--   0        0        0     1281 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/assets/react-json-view-lite.css
+-rw-r--r--   0        0        0   178190 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
+-rw-r--r--   0        0        0      921 2023-05-10 09:42:40.418148 chatplayground-1.1.1/chatplayground/pcconfig.py
+-rw-r--r--   0        0        0     3081 2023-05-10 09:42:40.442148 chatplayground-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6941 1970-01-01 00:00:00.000000 chatplayground-1.1.1/PKG-INFO
```

### Comparing `chatplayground-1.1.0/LICENSE` & `chatplayground-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.0/README.md` & `chatplayground-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,45 +16,44 @@
 - It's not possible to edit messages without deleting everything below.
 - It's hard to see what the explored alternatives are for a given message.
 - It's hard to see what the explored alternatives are for a given message thread.
 - It's not possible to change the model settings or the model type (GPT3.5/4) later on.
 
 ## Installation
 
+### Node.JS
+
 To install Chat Playground, first, make sure you have Node.js installed. You can use `conda` to install Node.js as follows:
 
 ```
 conda install -c conda-forge nodejs
 ```
 
-Or, to install a specific version of Node.js (this one worked for me):
+Or, to install a specific version of Node.js (this one worked for me on my MacBook---so this will not work on Linux):
 
 ```
 conda install -c conda-forge nodejs=18.15.0=h26a3f6d_0
 ```
 
+### Chat Playground
+
 Once Node.js is installed, you can install Chat Playground using `pip` or `pipx` (if you have nodejs available in your base environment):
 
 ```
 pipx install chatplayground
 ```
 
+### OpenAI Key :key:
+
 Ensure that your OpenAI key is set in an OPENAI_API_KEY environment variable. You then can run the playground with
 
 ```
 chatplayground
 ```
 
-## Documentation
-
-* Official Documentation: <https://blackhc.github.io/chatplayground>
-* Source Code: <https://github.com/blackhc/chatplayground>
-* PyPI Package: <https://pypi.org/project/chatplayground/>
-* License: GPL-3.0-only
-
 ## Features
 
 * Preview of possible alternative message threads as an exposee view.
 * Preview of possible alternatives at the message level.
 * Editing messages within a message thread without deleting everything below.
 * Forking message threads (similar to the ChatGPT web app).
 * Messages stored as JSON files in a local directory.
@@ -79,14 +78,21 @@
 - No tests currently.
 - Calling event functions in State classes requires passing self, even though it shouldn't: `self.state_event_function(self)`.
 - Issues with streaming events from the OpenAI request to the UI, requiring a hacky workaround for updates to propagate to the UI correctly.
 - Known Pynecone issues, as mentioned in the code.
 
 Despite these issues, the project came together very quickly with PyneCone and works quite well.
 
+## Documentation
+
+* License: GPL-3.0-only
+* Source Code: <https://github.com/blackhc/chatplayground>
+* PyPI Package: <https://pypi.org/project/chatplayground/>
+* Official Documentation: <https://blackhc.github.io/chatplayground>
+
 ## Contributing
 
 Bug fixes, feature requests, and pull requests are welcome! If you have any questions or suggestions, please open an issue on GitHub.
 
 ## License
 
 Chat Playground is licensed under AGPL3.0. If you require a commercial license for any part of the project, please contact the author.
```

### Comparing `chatplayground-1.1.0/chatplayground/app/app.py` & `chatplayground-1.1.1/chatplayground/app/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,17 @@
     auto_focus: Var[typing.Union[str, int, bool]]
 
 
 auto_focus_text_area = AutoFocusTextArea.create
 
 
 def render_tooltip(*args, **kwargs):
+    """
+    Render a tooltip.
+    """
     return pc.tooltip(*args, **kwargs, open_delay=500)
 
 
 class UID:
     """A unique ID generator that uses the current time and a counter to generate unique IDs.
 
     TODO: this is not thread safe, but that should not be a problem for now.
```

### Comparing `chatplayground-1.1.0/chatplayground/assets/favicon.ico` & `chatplayground-1.1.1/chatplayground/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.0/chatplayground/assets/react-json-view-lite.css` & `chatplayground-1.1.1/chatplayground/assets/react-json-view-lite.css`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.0/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json` & `chatplayground-1.1.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json`

 * *Files identical despite different names*

### Comparing `chatplayground-1.1.0/chatplayground/pcconfig.py` & `chatplayground-1.1.1/chatplayground/pcconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 import pynecone as pc
 import pynecone.pc as cli
 
 config = pc.Config(
     app_name="app",
     db_url="sqlite:///pynecone.db",
+    port=3111,
+    backend_port=8111,
+    api_url="http://localhost:8111",
     env=pc.Env.PROD,
     frontend_packages=[
         "react-object-view",
         "react-json-view-lite",
         "react-icons",
     ],
 )
```

### Comparing `chatplayground-1.1.0/pyproject.toml` & `chatplayground-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatplayground"
-version = "1.1.0"
+version = "1.1.1"
 homepage = "https://github.com/blackhc/chatplayground"
 description = "ChatPlayground for LLMs"
 authors = ["Andreas Kirsch <blackhc@gmail.com>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `chatplayground-1.1.0/PKG-INFO` & `chatplayground-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatplayground
-Version: 1.1.0
+Version: 1.1.1
 Summary: ChatPlayground for LLMs
 Home-page: https://github.com/blackhc/chatplayground
 License: GPL-3.0-only
 Author: Andreas Kirsch
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -68,45 +68,44 @@
 - It's not possible to edit messages without deleting everything below.
 - It's hard to see what the explored alternatives are for a given message.
 - It's hard to see what the explored alternatives are for a given message thread.
 - It's not possible to change the model settings or the model type (GPT3.5/4) later on.
 
 ## Installation
 
+### Node.JS
+
 To install Chat Playground, first, make sure you have Node.js installed. You can use `conda` to install Node.js as follows:
 
 ```
 conda install -c conda-forge nodejs
 ```
 
-Or, to install a specific version of Node.js (this one worked for me):
+Or, to install a specific version of Node.js (this one worked for me on my MacBook---so this will not work on Linux):
 
 ```
 conda install -c conda-forge nodejs=18.15.0=h26a3f6d_0
 ```
 
+### Chat Playground
+
 Once Node.js is installed, you can install Chat Playground using `pip` or `pipx` (if you have nodejs available in your base environment):
 
 ```
 pipx install chatplayground
 ```
 
+### OpenAI Key :key:
+
 Ensure that your OpenAI key is set in an OPENAI_API_KEY environment variable. You then can run the playground with
 
 ```
 chatplayground
 ```
 
-## Documentation
-
-* Official Documentation: <https://blackhc.github.io/chatplayground>
-* Source Code: <https://github.com/blackhc/chatplayground>
-* PyPI Package: <https://pypi.org/project/chatplayground/>
-* License: GPL-3.0-only
-
 ## Features
 
 * Preview of possible alternative message threads as an exposee view.
 * Preview of possible alternatives at the message level.
 * Editing messages within a message thread without deleting everything below.
 * Forking message threads (similar to the ChatGPT web app).
 * Messages stored as JSON files in a local directory.
@@ -131,14 +130,21 @@
 - No tests currently.
 - Calling event functions in State classes requires passing self, even though it shouldn't: `self.state_event_function(self)`.
 - Issues with streaming events from the OpenAI request to the UI, requiring a hacky workaround for updates to propagate to the UI correctly.
 - Known Pynecone issues, as mentioned in the code.
 
 Despite these issues, the project came together very quickly with PyneCone and works quite well.
 
+## Documentation
+
+* License: GPL-3.0-only
+* Source Code: <https://github.com/blackhc/chatplayground>
+* PyPI Package: <https://pypi.org/project/chatplayground/>
+* Official Documentation: <https://blackhc.github.io/chatplayground>
+
 ## Contributing
 
 Bug fixes, feature requests, and pull requests are welcome! If you have any questions or suggestions, please open an issue on GitHub.
 
 ## License
 
 Chat Playground is licensed under AGPL3.0. If you require a commercial license for any part of the project, please contact the author.
```

