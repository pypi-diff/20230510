# Comparing `tmp/graphdisplay-0.3.3.tar.gz` & `tmp/graphdisplay-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.3.3.tar", last modified: Sun May  7 19:46:29 2023, max compression
+gzip compressed data, was "graphdisplay-0.3.6.tar", last modified: Wed May 10 08:25:33 2023, max compression
```

## Comparing `graphdisplay-0.3.3.tar` & `graphdisplay-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.419618 graphdisplay-0.3.3/
--rw-rw-rw-   0        0        0     5408 2023-05-07 19:46:29.418620 graphdisplay-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.406652 graphdisplay-0.3.3/graphdisplay/
--rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.3/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     2440 2023-05-07 19:37:48.000000 graphdisplay-0.3.3/graphdisplay/general_config.py
--rw-rw-rw-   0        0        0    17455 2023-05-07 10:31:30.000000 graphdisplay-0.3.3/graphdisplay/graph.py
--rw-rw-rw-   0        0        0    17579 2023-05-07 19:42:11.000000 graphdisplay-0.3.3/graphdisplay/graphdisplay.py
--rw-rw-rw-   0        0        0     7108 2023-05-07 19:37:48.000000 graphdisplay-0.3.3/graphdisplay/json_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.417623 graphdisplay-0.3.3/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.3/graphdisplay/store/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.416626 graphdisplay-0.3.3/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     5408 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 19:46:29.419618 graphdisplay-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1322 2023-05-07 19:46:27.000000 graphdisplay-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.328259 graphdisplay-0.3.6/
+-rw-rw-rw-   0        0        0     5408 2023-05-10 08:25:33.328259 graphdisplay-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.312301 graphdisplay-0.3.6/graphdisplay/
+-rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.6/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     4209 2023-05-09 05:43:15.000000 graphdisplay-0.3.6/graphdisplay/general_config.py
+-rw-rw-rw-   0        0        0    17455 2023-05-07 10:31:30.000000 graphdisplay-0.3.6/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0    18618 2023-05-10 08:25:15.000000 graphdisplay-0.3.6/graphdisplay/graphdisplay.py
+-rw-rw-rw-   0        0        0     7145 2023-05-09 06:25:44.000000 graphdisplay-0.3.6/graphdisplay/json_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.326264 graphdisplay-0.3.6/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.6/graphdisplay/store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:25:33.324270 graphdisplay-0.3.6/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     5408 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 08:25:33.000000 graphdisplay-0.3.6/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:25:33.329256 graphdisplay-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1322 2023-05-10 08:25:31.000000 graphdisplay-0.3.6/setup.py
```

### Comparing `graphdisplay-0.3.3/PKG-INFO` & `graphdisplay-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.3.3
+Version: 0.3.6
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.3.3/README.md` & `graphdisplay-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.3.3/graphdisplay/general_config.py` & `graphdisplay-0.3.6/graphdisplay/general_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "VERTEX_COLOR": "#215C41",
         "BACKGROUND_CANVAS_COLOR": "#163623",
         "FRAME_COLOR": "#0C2B1A",
         "AUTHOR_NAME_COLOR": "#FFFFFF"
     },
     "UBUNTU":{
         "BUTTON_COLOR": "#b35625",
-        "VERTEX_COLOR": "#94471e",
+        "VERTEX_COLOR": "#d45102",
         "BACKGROUND_CANVAS_COLOR": "#404040",
         "FRAME_COLOR": "#303030",
         "AUTHOR_NAME_COLOR": "#FFFFFF"
     },
     "LA NOCHE ESTRELLADA":{
         "BUTTON_COLOR": "#9bafaa",
         "VERTEX_COLOR": "#7b94a4",
@@ -71,9 +71,65 @@
     },
     "ANTARTICA":{
         "BUTTON_COLOR": "#9BA4B5",
         "VERTEX_COLOR": "#9BA4B5",
         "BACKGROUND_CANVAS_COLOR": "#394867",
         "FRAME_COLOR": "#212A3E",
         "AUTHOR_NAME_COLOR": "#83764F"
+    },
+    "BREAKING BAD":{
+        "BUTTON_COLOR": "#F7E1AE",
+        "VERTEX_COLOR": "#F7E1AE",
+        "BACKGROUND_CANVAS_COLOR": "#617A55",
+        "FRAME_COLOR": "#3d4d36",
+        "AUTHOR_NAME_COLOR": "#F7E1AE"
+    },
+    "SOFT":{
+        "BUTTON_COLOR": "#E4D0D0",
+        "VERTEX_COLOR": "#E4D0D0",
+        "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
+        "FRAME_COLOR": "#867070",
+        "AUTHOR_NAME_COLOR": "#000000"
+    },
+    "TURQUOISE": {
+        "BUTTON_COLOR": "#0E8388",
+        "VERTEX_COLOR": "#83918e",
+        "BACKGROUND_CANVAS_COLOR": "#2E4F4F",
+        "FRAME_COLOR": "#2C3333",
+        "AUTHOR_NAME_COLOR": "#CBE4DE"
+    },
+    "DEEP PURPLE":{
+        "BUTTON_COLOR": "#bdb8ac",
+        "VERTEX_COLOR": "#bdb8ac",
+        "BACKGROUND_CANVAS_COLOR": "#6D5D6E",
+        "FRAME_COLOR": "#4F4557",
+        "AUTHOR_NAME_COLOR": "#F4EEE0"
+    },
+    "THIS ONE IS UGLY":{
+        "BUTTON_COLOR": "#F67280",
+        "VERTEX_COLOR": "#C06C84",
+        "BACKGROUND_CANVAS_COLOR": "#6C5B7B",
+        "FRAME_COLOR": "#355C7D",
+        "AUTHOR_NAME_COLOR": "#F67280"
+    },
+    "FROST": {
+        "BUTTON_COLOR": "#00ADB5",
+        "VERTEX_COLOR": "#00ADB5",
+        "BACKGROUND_CANVAS_COLOR": "#393E46",
+        "FRAME_COLOR": "#222831",
+        "AUTHOR_NAME_COLOR": "#EEEEEE"
+    },
+    "NEKOS": {
+        "BUTTON_COLOR": "#DEFCF9",
+        "VERTEX_COLOR": "#CADEFC",
+        "BACKGROUND_CANVAS_COLOR": "#C3BEF0",
+        "FRAME_COLOR": "#CCA8E9",
+        "AUTHOR_NAME_COLOR": "#DEFCF9"
+    },
+    "VAMPIRE": {
+        "BUTTON_COLOR": "#FF0000",
+        "VERTEX_COLOR": "#FF0000",
+        "BACKGROUND_CANVAS_COLOR": "#950101",
+        "FRAME_COLOR": "#3D0000",
+        "AUTHOR_NAME_COLOR": "#FF0000"
     }
 }
```

### Comparing `graphdisplay-0.3.3/graphdisplay/graph.py` & `graphdisplay-0.3.6/graphdisplay/graph.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.3.3/graphdisplay/graphdisplay.py` & `graphdisplay-0.3.6/graphdisplay/graphdisplay.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,47 @@
 import tkinter as tk
 import math
+import platform
+import multiprocessing as mp
 from .json_manager import JsonManager
 from .general_config import *
 
 class GraphGUI:
 
     instance = 0
 
-    def __new__(cls, graph, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
+    def __new__(cls, graph, node_radius: int = 30, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
         GraphGUI.instance += 1
         if GraphGUI.instance > 5:
             raise Exception("For safety reasons, only five instances of GraphGUI can be created")
-        return GraphGUI.__GraphGUI(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme)
+        if platform.system() == "Linux":
+            mp.Process(target=cls._generate, args=(graph,
+                                                    GraphGUI.instance,
+                                                    node_radius,
+                                                    scr_width,
+                                                    scr_height,
+                                                    theme)).start()
+        else:
+            try:
+                pid = mp.Process(target=cls._generate, args=(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme))
+                pid.start()
+            except RuntimeError:
+                pass
+                #return GraphGUI.__GraphGUI(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme)
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __setattr__(self, name, value):
         return setattr(self.instance, name, value)
 
+    @staticmethod
+    def _generate(graph, instance, node_radius, scr_width, scr_height, theme):
+        GraphGUI.__GraphGUI(graph, instance, node_radius, scr_width, scr_height, theme)
+
     class __GraphGUI:
         def __init__(self, graph, instance, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
             """
             Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
             The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
             to create the GraphGUI object at the end of the program.
             :param graph: The graph to be displayed
@@ -128,16 +147,16 @@
 
         def display_reset(self, new_data: dict = None):
             self.canvas.delete("all")
             self.__display(new_data)
 
         def __display(self, data: dict = None):
             # Preparation for the nodes display
-            scr_center = (self.__scr_width // 2, self.__scr_height // 2)
-            display_radius = min(self.__scr_width, self.__scr_height) // 2 - self.__node_radius - 10
+            scr_center = ((self.__scr_width - 14) // 2, (self.__scr_height - 30) // 2)
+            display_radius = min(self.__scr_width - 30 - self.__node_radius, self.__scr_height - 14 - self.__node_radius) // 2 - self.__node_radius - 10
             arch_angle = 360 / len(self.__graph._vertices)
             first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
 
             # Display the nodes
             self.nodes = []
             i = 0
             angle = 0
@@ -342,8 +361,11 @@
         y2 = center_end[1]
 
         x = x2 - x1
         y = y2 - y1
         edge_angle = math.atan2(y, x) * (180.0 / math.pi)
         x = math.cos(math.radians(edge_angle)) * end.radius
         y = math.sin(math.radians(edge_angle)) * end.radius
-        return  (center_end[0] - int(x), center_end[1] - int(y))
+        return  (center_end[0] - int(x), center_end[1] - int(y))
+
+if __name__ == "__main__":
+    pass
```

### Comparing `graphdisplay-0.3.3/graphdisplay/json_manager.py` & `graphdisplay-0.3.6/graphdisplay/json_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     def __on_delete(self):
         selection = self.__selecion.get()
         if selection not in self.__manager._JsonManager__permanent:
             messagebox.showerror("Error", "The selected save does not exist")
             self.destroy()
         self.__manager.delete_permanent(selection)
         messagebox.showinfo("Confirm", f"Removed : {selection}")
-        self.destroy()
 
     def __on_cancel(self):
         self.destroy()
 
 class LoadWindow(tk.Toplevel):
     def __init__(self, root, json_manager: JsonManager):
         super().__init__(root)
@@ -136,28 +135,29 @@
         self.title("Save")
         self.geometry("200x100")
         self.resizable(False, False)
         self.__current_position = graph_position
         self.__manager = json_manager
         self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
         self.__root = root
+        self.bind("<Return>", self.__on_save)
 
         self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
         self.__label.pack(side=tk.TOP)
 
         self.__entry = tk.Entry(self)
         self.__entry.pack(side=tk.TOP)
 
         self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
         self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
 
         self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
         self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
 
-    def __on_save(self):
+    def __on_save(self, event = None):
         word = self.__entry.get()
         word = word.strip()
         word = word.replace(" ", "_")
         if word:
             self.__manager.save_data(word, self.__current_position)
             self.__manager.add_permanent(word)
             messagebox.showinfo("Confirmación", f"Guardado : {word}")
```

### Comparing `graphdisplay-0.3.3/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.3.6/graphdisplay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.3.3
+Version: 0.3.6
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.3.3/setup.py` & `graphdisplay-0.3.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.3.3'
+VERSION = '0.3.6'
 PACKAGE_NAME = 'graphdisplay'
 AUTHOR = 'Alberto Penas Díaz'
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
 URL = 'https://github.com/seniorbeto'
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
```

