# Comparing `tmp/nodered.py-0.2.0.tar.gz` & `tmp/nodered.py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.0.tar", last modified: Sun May  7 12:38:52 2023, max compression
+gzip compressed data, was "nodered.py-0.2.1.tar", last modified: Wed May 10 10:49:17 2023, max compression
```

## Comparing `nodered.py-0.2.0.tar` & `nodered.py-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.0/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2229 2023-05-07 12:38:52.540000 nodered.py-0.2.0/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1913 2023-05-07 12:35:08.000000 nodered.py-0.2.0/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2229 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-05-07 12:38:52.000000 nodered.py-0.2.0/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.0/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.420000 nodered.py-0.2.0/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-05-07 12:04:58.000000 nodered.py-0.2.0/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    10262 2023-05-07 12:14:13.000000 nodered.py-0.2.0/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.0/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.0/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      807 2023-05-07 08:57:45.000000 nodered.py-0.2.0/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.0/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2512 2023-05-07 01:35:50.000000 nodered.py-0.2.0/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.2.0/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-07 12:38:52.430000 nodered.py-0.2.0/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7480 2023-05-07 08:38:57.000000 nodered.py-0.2.0/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.2.0/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.0/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.2.0/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-07 12:38:52.540000 nodered.py-0.2.0/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-05-07 01:29:24.000000 nodered.py-0.2.0/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.450000 nodered.py-0.2.1/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.1/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-05-10 10:49:17.570000 nodered.py-0.2.1/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2026 2023-05-10 10:48:39.000000 nodered.py-0.2.1/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2342 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       14 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-05-10 10:49:17.000000 nodered.py-0.2.1/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.1/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      403 2023-05-10 09:35:45.000000 nodered.py-0.2.1/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    11475 2023-05-10 10:42:26.000000 nodered.py-0.2.1/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.2.1/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.1/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.1/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.1/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2512 2023-05-07 01:35:50.000000 nodered.py-0.2.1/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.2.1/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-10 10:49:17.460000 nodered.py-0.2.1/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7985 2023-05-10 10:44:33.000000 nodered.py-0.2.1/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.1/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3766 2023-05-07 11:55:40.000000 nodered.py-0.2.1/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.1/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-10 10:49:17.570000 nodered.py-0.2.1/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-05-07 01:29:24.000000 nodered.py-0.2.1/setup.py
```

### Comparing `nodered.py-0.2.0/LICENSE` & `nodered.py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/PKG-INFO` & `nodered.py-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.0
+Version: 0.2.1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -71,14 +71,15 @@
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
 
 red.register("test", api.test)
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/master/tests/server_test.py">example</a> for details.
 
 <br/>
 
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.0 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.1 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -17,14 +17,14 @@
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy.decorator import register
 @register("test") def test(props:dict, msg:dict) -> dict: # user codes here
 return msg ``` - register from Node-RED object - See noredpy.decorator.register
 function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property"
+See noderedpy._property for details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.0/README.md` & `nodered.py-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
 
 red.register("test", api.test)
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/master/tests/server_test.py">example</a> for details.
 
 <br/>
 
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
```

#### html2text {}

```diff
@@ -12,14 +12,14 @@
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy.decorator import register
 @register("test") def test(props:dict, msg:dict) -> dict: # user codes here
 return msg ``` - register from Node-RED object - See noredpy.decorator.register
 function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property"
+See noderedpy._property for details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.0/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.1/nodered.py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.0
+Version: 0.2.1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -71,14 +71,15 @@
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/c205b617296d3ef14e93f08e72657fd41ab8d081/noderedpy/_nodered.py#L85">noredpy.decorator.register function</a> for details
 ```python
 api = API()
 
 red.register("test", api.test)
 ```
 - See <a href="https://github.com/oyajiDev/NodeRED.py/blob/08b2295ab537be97ad9e9a2f94154cdcb36685d0/noderedpy/_property.py">noderedpy._property</a> for details of "Property"
+- See <a href="https://github.com/oyajiDev/NodeRED.py/blob/master/tests/server_test.py">example</a> for details.
 
 <br/>
 
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.0 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.1 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -17,14 +17,14 @@
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
 "node_red_dir"), "/node-red", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy.decorator import register
 @register("test") def test(props:dict, msg:dict) -> dict: # user codes here
 return msg ``` - register from Node-RED object - See noredpy.decorator.register
 function for details ```python api = API() red.register("test", api.test) ``` -
-See noderedpy._property for details of "Property"
+See noderedpy._property for details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
 ## Todos [x] type support for "list" and "dict"
 
 ## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
```

### Comparing `nodered.py-0.2.0/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.1/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/noderedpy/_nodered.py` & `nodered.py-0.2.1/noderedpy/_nodered.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import os, sys, subprocess, shutil, json, traceback
 from types import MethodType
-from typing import Type, List
+from typing import List
 from glob import glob
 from .templates import package_json, node_html, node_js
 from ._property import Property
 from . import __path__
 
 
 class RED:
@@ -64,45 +64,65 @@
             "favicon": page_theme.pop("favicon", os.path.join(__path__[0], "assets", "python-logo.png"))
         })
         header_theme = editor_theme.pop("header", {})
         header_theme.update({
             "title": "Node-RED.py",
             "image": None
         })
+        menu_theme = editor_theme.pop("menu", {})
+        menu_theme.update({
+            "menu-item-palette": False
+        })
         project_feature = editor_theme.pop("projects", {})
         project_feature.update({
             "enabled": project_feature.pop("enabled", False)
         })
 
         editor_theme.update({
             "page": page_theme,
             "header": header_theme,
+            "menu": menu_theme,
             "userMenu": editor_theme.pop("userMenu", False),
             "projects": project_feature
         })
 
         return editor_theme
     
-    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[Property] = []):
+    def register(self, node_func:MethodType, name:str, category:str = "nodered_py", version:str = "1.0.0", description:str = "", author:str = "nodered.py", keywords:List[str] = [], icon:str = "function.png", properties:List[Property] = []):
         """
         Function to register Node function
 
         Parameters
         ----------
         node_func: MethodType, required
             Node function to register
         name: str, required
             name of Node to register
         category: str, default nodered_py
             category of Node
+        version: str, default 1.0.0
+            version of Node
+        description: str, default ""
+            description of Node
+        author: str, default nodered.py
+            author of Node
+        keywords: List[str], default []
+            extra keywords of Node
+        icon: str, default function.png
+            icon of Node(html)
         properties: List[noderedpy._property.Property]
             propertis of Node
         """
-        node = Node(name if name.startswith("nodered-py") else f"nodered-py-{name}", category, properties, node_func)
-        RED.registered_nodes.append(node)
+        RED.registered_nodes.append(
+            Node(
+                name, category,
+                version, description, author, keywords,
+                icon, properties, node_func
+            )
+        )
 
     # check input and run node
     def __check_input_from_node(self):
         input_file, output_file = os.path.join(self.__cache_dir, "input.json"), os.path.join(self.__cache_dir, "output.json")
 
         while True:
             if os.path.exists(input_file):
@@ -148,15 +168,15 @@
         if os.path.exists(self.__cache_dir):
             shutil.rmtree(self.__cache_dir)
 
         os.mkdir(self.__cache_dir)
 
         # save editor_theme
         with open(os.path.join(self.node_red_dir, "editorTheme.json"), "w", encoding = "utf-8") as tjw:
-            json.dump(self.editor_theme, tjw)
+            json.dump(self.editor_theme, tjw, indent = 4)
 
         # remove existing nodes
         for node_dir in glob(os.path.join(self.user_dir, "node_modules", "nodered-py-*")):
             shutil.rmtree(node_dir)
 
         # create custom nodes
         for node in RED.registered_nodes:
@@ -232,28 +252,37 @@
             except ( psutil.AccessDenied, psutil.ZombieProcess ):
                 pass
 
             if killed:
                 break
 
 class Node:
-    def __init__(self, name:str, category:str, properties:List[Property], node_func:MethodType):
+    def __init__(self, name:str, category:str, version:str, description:str, author:str, keywords:List[str], icon:str, properties:List[Property], node_func:MethodType):
+        # name of node cannot contain spaces
         if " " in name.strip():
             raise NameError("Node name cannot contain spaces!")
         
+        # category of node cannot contain - or ,
         if "-" in category.strip() or "," in category.strip():
             raise NameError("Category cannot contain '-' or ','!")
+        
+        # remove default keyword in extra keywords
+        self.keywords = [
+            keyword
+            for keyword in keywords
+            if not keyword in ( "node-red", )
+        ]
 
-        self.name, self.category, self.properties =\
-            name, category, properties
+        self.name, self.category, self.version, self.description, self.author, self.icon, self.properties =\
+            name, category, version, description, author, icon, properties
         
         self.__node_func = node_func
 
     def create(self, node_red_user_dir:str, node_red_user_cache_dir:str):
-        node_dir = os.path.join(node_red_user_dir, "node_modules", self.name)
+        node_dir = os.path.join(node_red_user_dir, "node_modules", self.name if self.name.startswith("nodered-py-") else f"nodered-py-{self.name}")
         os.makedirs(os.path.join(node_dir, "lib"))
 
         with open(os.path.join(node_dir, "package.json"), "w", encoding = "utf-8") as pjw:
             pjw.write(package_json(self))
 
         with open(os.path.join(node_dir, "lib", f"{self.name}.html"), "w", encoding = "utf-8") as nhw:
             nhw.write(node_html(self))
```

### Comparing `nodered.py-0.2.0/noderedpy/_property.py` & `nodered.py-0.2.1/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/noderedpy/assets/python-logo.png` & `nodered.py-0.2.1/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.1/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/noderedpy/templates/__init__.py` & `nodered.py-0.2.1/noderedpy/templates/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 # -*- coding: utf-8 -*-
-import os, json, noderedpy
+import os, noderedpy
 from .._property import (
     InputProperty, ListProperty,
     SpinnerProperty, ComboBoxProperty, CodeProperty
 )
 from . import __path__
 
 
 def package_json(node:"noderedpy._nodered.Node") -> str:
     with open(os.path.join(__path__[0], "template.json"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
 
-    return tt.replace(
+    tt = tt.replace(
         "{$node_name}", node.name
+    ).replace(
+        "{$node_version}", node.version
+    ).replace(
+        "{$node_description}", node.description
+    ).replace(
+        "{$node_author}", node.author
     )
+    
+    if node.keywords == []:
+        tt = tt.replace(
+            "{$node_keywords}", ""
+        )
+    else:
+        tt = tt.replace(
+            "{$node_keywords}", ", " + ", ".join([ f'"{keyword}"' for keyword in node.keywords ])
+        )
+
+    return tt
 
 def node_html(node:"noderedpy._nodered.Node") -> str:
     properties_html, properties_js, properties_js_prepare, properties_js_cancel, properties_js_save = [], [], [], [], []
     default_value = None
     for property in node.properties:
         if isinstance(property, InputProperty):
             properties_html.append(f"""
@@ -153,14 +170,16 @@
         tt = tr.read()
 
     return tt.replace(
         "{$node_name}", node.name
     ).replace(
         "{$node_category}", node.category
     ).replace(
+        "{$node_icon}", f'"{node.icon}"' if node.icon else "null"
+    ).replace(
         "{$properties_html}", "".join(properties_html)
     ).replace(
         "{$properties_js}", ",\n".join(properties_js)
     ).replace(
         "{$properties_js_prepare}", "\n".join(properties_js_prepare)
     ).replace(
         "{$properties_js_cancel}", "\n".join(properties_js_cancel)
```

### Comparing `nodered.py-0.2.0/noderedpy/templates/template.html` & `nodered.py-0.2.1/noderedpy/templates/template.html`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         category: "{$node_category}",
         color: "#FDD0A2",
         defaults: {
             name: { value: "" },
 {$properties_js}
         },
         inputs: 1, outputs: 1,
-        icon: "function.png",
+        icon: {$node_icon},
         label: function() {
             return this.name;
         },
         oneditprepare: function() {
 {$properties_js_prepare}
         },
         oneditcancel: function() {
```

### Comparing `nodered.py-0.2.0/noderedpy/templates/template.js` & `nodered.py-0.2.1/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.0/setup.py` & `nodered.py-0.2.1/setup.py`

 * *Files identical despite different names*

