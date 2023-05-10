# Comparing `tmp/connpy-3.2.1.tar.gz` & `tmp/connpy-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.1.tar", last modified: Fri May  5 17:20:30 2023, max compression
+gzip compressed data, was "connpy-3.2.2.tar", last modified: Wed May 10 15:54:51 2023, max compression
```

## Comparing `connpy-3.2.1.tar` & `connpy-3.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 17:20:16.000000 connpy-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 17:20:30.069119 connpy-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 17:20:16.000000 connpy-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14755 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4713 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-05 17:20:30.069119 connpy-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 17:20:16.000000 connpy-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.567473 connpy-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 15:54:40.000000 connpy-3.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:54:51.567473 connpy-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-10 15:54:40.000000 connpy-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.563472 connpy-3.2.2/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15368 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.567473 connpy-3.2.2/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 15:54:51.567473 connpy-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 15:54:40.000000 connpy-3.2.2/setup.py
```

### Comparing `connpy-3.2.1/LICENSE` & `connpy-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/PKG-INFO` & `connpy-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.1
+Version: 3.2.2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.1/README.md` & `connpy-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy/__init__.py` & `connpy-3.2.2/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy/ai.py` & `connpy-3.2.2/connpy/ai.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,16 +160,18 @@
         info_dict["variables"] = {}
         info_dict["variables"]["__global__"] = {}
         for line in raw_response.split("\n"):
             if ":" in line:
                 key, value = line.split(":", 1)
                 key = key.strip()
                 newvalue = {}
+                pattern = r'\[.*?\]'
+                match = re.search(pattern, value.strip())
                 try:
-                    value = ast.literal_eval(value.strip())
+                    value = ast.literal_eval(match.group(0))
                     for i,e in enumerate(value, start=1):
                         newvalue[f"command{i}"] = e
                         if f"{{command{i}}}" not in info_dict["commands"]:
                             info_dict["commands"].append(f"{{command{i}}}")
                             info_dict["variables"]["__global__"][f"command{i}"] = ""
                     info_dict["variables"][key] = newvalue
                 except:
@@ -201,37 +203,41 @@
             )
         output = {}
         output["dict_response"] = response
         output["raw_response"] = response["choices"][0]["message"]["content"] 
         output["response"] = self._clean_command_response(output["raw_response"])
         return output
 
-    def _get_filter(self, user_input):
+    def _get_filter(self, user_input, chat_history = None):
         #Send the request to identify the filter and other attributes from the user input to GPT.
         message = []
         message.append({"role": "system", "content": dedent(self.__prompt["original_system"])})
         message.append({"role": "user", "content": dedent(self.__prompt["original_user"])})
         message.append({"role": "assistant", "content": dedent(self.__prompt["original_assistant"])})
-        message.append({"role": "user", "content": user_input})
-
+        if not chat_history:
+            chat_history = []
+        chat_history.append({"role": "user", "content": user_input})
+        message.extend(chat_history)
         response = openai.ChatCompletion.create(
             model=self.model,
             messages=message,
             temperature=self.temp,
             top_p=1
             )
 
         output = {}
         output["dict_response"] = response
         output["raw_response"] = response["choices"][0]["message"]["content"] 
+        chat_history.append({"role": "assistant", "content": output["raw_response"]})
+        output["chat_history"] = chat_history
         clear_response = self._clean_original_response(output["raw_response"])
         output["response"] = self._clean_original_response(output["raw_response"])
         return output
         
-    def ask(self, user_input, dryrun = False):
+    def ask(self, user_input, dryrun = False, chat_history = None):
         '''
         Send the user input to openAI GPT and parse the response to run an action in the application.
 
         ### Parameters:  
 
             - user_input (str): Request to send to openAI that will be parsed
                                 and returned to execute on the application.
@@ -262,22 +268,26 @@
                     to get the list of nodes to work on.
                   - nodes: If it's not a dryrun, the list of nodes matched by
                     the filter.
                   - args: A dictionary of arguments required to run command(s)
                     on the nodes.
                   - result: A dictionary with the output of the commands or 
                     the test.
+                  - chat_history: The chat history between user and chatbot.
+                    It can be used as an attribute for next request.
+                
                     
 
         '''
         output = {}
-        original = self._get_filter(user_input)
+        original = self._get_filter(user_input, chat_history)
         output["input"] = user_input
         output["app_related"] = original["response"]["app_related"]
         output["dryrun"] = dryrun
+        output["chat_history"] = original["chat_history"]
         if not output["app_related"]:
             output["response"] = original["response"]["response"]
         else:
             type = original["response"]["type"].lower()
             if "filter" in original["response"]:
                 output["filter"] = original["response"]["filter"]
                 if not self.config.config["case"]:
@@ -285,15 +295,15 @@
                         output["filter"] = [item.lower() for item in output["filter"]]
                     else:
                         output["filter"] = output["filter"].lower()
                 if not dryrun or type == "command":
                     thisnodes = self.config._getallnodesfull(output["filter"])
                     output["nodes"] = list(thisnodes.keys())
             if not type == "command":
-                output["action"] = type
+                output["action"] = "list_nodes"
             else:
                 commands = self._get_commands(user_input, thisnodes)
                 output["args"] = {}
                 output["args"]["commands"] = commands["response"]["commands"]
                 output["args"]["vars"] = commands["response"]["variables"]
                 if original["response"]["expected"]:
                     output["args"]["expected"] = original["response"]["expected"]
```

### Comparing `connpy-3.2.1/connpy/api.py` & `connpy-3.2.2/connpy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,20 @@
     conf = app.custom_config
     data = request.get_json()
     input = data["input"]
     if "dryrun" in data:
         dryrun = data["dryrun"] 
     else:
         dryrun = False
+    if "chat_history" in data:
+        chat_history = data["chat_history"]
+    else:
+        chat_history = None
     ai = myai(conf)
-    return ai.ask(input, dryrun)
+    return ai.ask(input, dryrun, chat_history)
 
 
 @app.route("/run_commands", methods=["POST"])
 def run_commands():
     conf = app.custom_config
     data = request.get_json()
     case = conf.config["case"]
```

### Comparing `connpy-3.2.1/connpy/completion.py` & `connpy-3.2.2/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy/configfile.py` & `connpy-3.2.2/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy/connapp.py` & `connpy-3.2.2/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy/core.py` & `connpy-3.2.2/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.1/connpy.egg-info/PKG-INFO` & `connpy-3.2.2/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.1
+Version: 3.2.2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.1/setup.cfg` & `connpy-3.2.2/setup.cfg`

 * *Files identical despite different names*

