# Comparing `tmp/indiek-gui-0.0.2.tar.gz` & `tmp/indiek-gui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-udfpk_0l/indiek-gui-0.0.2.tar", last modified: Sun May  7 13:36:30 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-4b78jphm/indiek-gui-0.0.3.tar", last modified: Tue May  9 22:20:56 2023, max compression
```

## Comparing `indiek-gui-0.0.2.tar` & `indiek-gui-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.2/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek/gui/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/indiek/gui/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    17488 2023-05-06 19:51:14.000000 indiek-gui-0.0.2/indiek/gui/app.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/indiek/gui/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek_gui.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      304 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/entry_points.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-07 13:35:40.000000 indiek-gui-0.0.2/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.3/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.3/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.981971 indiek-gui-0.0.3/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/indiek/gui/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-07 21:17:10.000000 indiek-gui-0.0.3/indiek/gui/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    18645 2023-05-09 22:04:25.000000 indiek-gui-0.0.3/indiek/gui/app.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1452 2023-05-07 22:15:22.000000 indiek-gui-0.0.3/indiek/gui/items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/indiek_gui.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      304 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:20:56.000000 indiek-gui-0.0.3/indiek_gui.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-09 22:20:56.993971 indiek-gui-0.0.3/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-09 22:20:47.000000 indiek-gui-0.0.3/setup.py
```

### Comparing `indiek-gui-0.0.2/LICENSE` & `indiek-gui-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.2/PKG-INFO` & `indiek-gui-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.2/README.rst` & `indiek-gui-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.2/indiek/gui/app.py` & `indiek-gui-0.0.3/indiek/gui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 # -*- coding: utf-8 -*-
 from typing import Optional, Mapping
 from tkinter import *
 from tkinter import ttk
 from functools import partial
-from indiek.core.items import Item as CoreItem
-from indiek.core.search import list_all_items
-from indiek.gui.items import core_to_gui_item, GUIItem
+from indiek.core.search import list_all_items, filter_str
+from indiek.gui.items import core_to_gui_item, Item as GUIItem, Definition, Theorem, Proof
+from indiek.core.items import (Definition as CoreDefinition, 
+                               Theorem as CoreTheorem, 
+                               Proof as CoreProof)
 from . import __version__
 
-# # initial_item below is just to simulate that DB is not empty
-# initial_item = CoreItem(
-#     name="dummy item", 
-#     content="dummy content"
-#     )
-# initial_item.save()
+
+ITEM_TYPES = [Definition, Theorem, Proof]
+"""List of item types."""
+
+
+FILTER_NAMES = ['Definitions', 'Theorems', 'Proofs']
+"""Strings used in filter radio buttons for each Item type."""
+
+
+NAME_TO_ITEM_TYPE = {
+    'Definitions': CoreDefinition, 
+    'Theorems': CoreTheorem, 
+    'Proofs': CoreProof
+}
+assert set(NAME_TO_ITEM_TYPE.keys()) == set(FILTER_NAMES)
+
 
 WRAP_1 = 380
 ENTRY_DEFAULT_LENGTH = 54
 
 
 class Orchestrator:
     item_result_height = 40
@@ -67,15 +79,14 @@
         self.mainframe.grid(column=0, row=0, sticky='news')
         self.mainframe.columnconfigure(0, weight=1)
         self.mainframe.columnconfigure(1, weight=2)
         self.mainframe.rowconfigure(0, weight=1)
 
         self._initialize_right_panel()
         self._initialize_left_panel()
-        # self.refresh_results()
 
         self.mainframe.add(self.left_panel, weight=1)
         self.mainframe.add(self.right_panel, weight=2)
 
     def initialize_item_view(self, frame, gui_item: GUIItem):
         local_frame = ttk.Frame(frame)
         local_frame.grid(row=0, column=0, sticky='news')
@@ -152,33 +163,33 @@
             gui_item=self.view_var, 
             )
         # TODO: add scrollbar?
 
         btn_frame = ttk.Frame(view)
         btn_frame.grid(row=0, column=1, sticky='news')
         btn_frame.grid_columnconfigure(0, weight=1)
-        btn_frame.grid_rowconfigure(0, weight=0)
-        btn_frame.grid_rowconfigure(1, weight=0)
-        btn_frame.grid_rowconfigure(2, weight=0)
 
-        self.new_item_button = ttk.Button(
-            btn_frame,
-            text='New Item',
-            command=self.switch_to_edit_new,
-            state='normal'
-        )
-        self.new_item_button.grid(row=0, column=0, sticky=(N,))
+        self.new_item_buttons = {}
+        for row_ix, item_type in enumerate(ITEM_TYPES):
+            btn_frame.grid_rowconfigure(row_ix, weight=0)
+            self.new_item_buttons[item_type] = ttk.Button(
+                btn_frame,
+                text=f'New {item_type.__name__}',
+                command=partial(self.switch_to_edit_new, item_type),
+                state='normal'
+            )
+            self.new_item_buttons[item_type].grid(row=row_ix, column=0, sticky=(N,))
 
         self.edit_button = ttk.Button(
             btn_frame,
             text='Edit',
             command=self.switch_to_edit,
             state='disabled'
         )
-        self.edit_button.grid(row=1, column=0, sticky=(N,))
+        self.edit_button.grid(row=row_ix + 1, column=0, sticky=(N,))
 
         # Edit tab
         edit = ttk.Frame(self.view_nb)
         edit.grid(row=0, column=0, sticky='news')
         edit.grid_rowconfigure(0, weight=1)
         edit.grid_columnconfigure(0, weight=1)
         edit.grid_columnconfigure(1, weight=0)
@@ -215,17 +226,17 @@
         self.text['content'].grid(row=1, column=1, sticky='w')
 
     def switch_to_edit(self):
         """Switch focus from item view to item edition."""
         self.view_nb.tab(self.edit_id, state='normal')
         self.view_nb.select(self.edit_id)
     
-    def switch_to_edit_new(self):
+    def switch_to_edit_new(self, item_cls: GUIItem):
         """Switch to edit tab for new item creation."""
-        new_item = GUIItem(name_var=StringVar(), content_var=StringVar())
+        new_item = item_cls(name_var=StringVar(), content_var=StringVar())
         self.populate_view_pane(new_item)
         self.view_nb.tab(self.edit_id, state='normal')
         self.view_nb.select(self.edit_id)
 
     def switch_to_view(self):
         """When focus is on Edit tab; save and switch to View tab."""
 
@@ -237,15 +248,15 @@
         name_str = self.text['name'].get('1.0', 'end')
         self.view_var.update_name(name_str)
 
         # save to DB
         self.view_var.save()
 
         # refresh search results
-        self.refresh_results()
+        self.collect_search()
 
         # hide editor
         self.view_nb.tab(self.edit_id, state='hidden')
 
         # focus back on view
         self.view_nb.select(self.view_id)
 
@@ -255,15 +266,15 @@
          .grid(column=0, row=0, sticky=(N, W, E, S)))
 
         self.check_buttons_frame = ttk.Frame(
             self.left_search_pane, borderwidth=5)
         self.check_buttons_frame.grid(column=1, row=0, sticky='w')
 
         # setup callbacks for filter's CheckButtons
-        cats = ['Definitions', 'Theorems', 'Proofs']
+        cats = FILTER_NAMES
         for cat in cats:
             custom_var = StringVar(value='')
             self.filter_vars[cat] = custom_var
             custom_filter = partial(self.update_filter, cat, custom_var)
             self.filter_callbacks[cat] = custom_filter
         # create the check buttons
         for colix, cat in enumerate(cats):
@@ -344,14 +355,17 @@
 
         # -------------------
         # DUMMY RESULT PANES
         # -------------------
         self.populate_search_results_canvas(self.search_results_list)
 
     def populate_search_results_canvas(self, results_list):
+        # clear canvas
+        result_tag = 'result_item'
+        self.results_canvas.delete(result_tag)
         for result_ix, gui_item in enumerate(results_list):
             search_result = ttk.Label(
                 self.results_canvas,
                 textvariable=gui_item.name_var,
                 wraplength=WRAP_1,  # pixels
             )
             self.view_callbacks[result_ix] = partial(
@@ -361,15 +375,15 @@
 
             _ = self.results_canvas.create_window(
                 0,
                 self.item_result_height * result_ix,
                 anchor='nw',
                 window=search_result,
                 height=self.item_result_height,
-                tags=('palette')
+                tags=(result_tag)
             )
 
     def populate_view_pane(self, gui_item: GUIItem, *args):
         """Populate View & Edit tabs with GUIItem data.
 
         This callback gets triggered when:
          - item from search results gets clicked upon, or,
@@ -466,40 +480,56 @@
 
         Args:
             search_params (Optional[Mapping], optional): Search parameters. Defaults to None.
 
         Raises:
             NotImplementedError: If search_params is not None.
         """
-        if search_params is None:
-            self.search_results_list = []
-            for result_ix, core_item in enumerate(list_all_items()):
-                gui_item = core_to_gui_item(
-                    core_item,
-                    name_var=StringVar(value=core_item.name),
-                    content_var=StringVar(value=core_item.content),
-                    )
-                self.search_results_list.append(gui_item)
-                self.ikid_to_result_slot[gui_item._ikid] = result_ix
+        self.search_results_list = []
+        # TODO: current logic ignores searchbar
+        # TODO: setup logging instead of print() below
+
+        # print(f"{search_params=}")
+        if search_params is not None:
+            item_type_filter = [NAME_TO_ITEM_TYPE[f] for f in search_params['filters']]
+            search_str = search_params['search']
+            if search_str:
+                item_buckets = filter_str(search_str, item_type_filter)
+            else:
+                item_buckets = list_all_items(item_type_filter)
+            # print(f"   {item_buckets=}")
         else:
-            pass
-            # raise NotImplementedError()
+            item_buckets = list_all_items()
+
+        # TODO: keep item types separate below
+        item_list = []
+        for ll in item_buckets.values():
+            item_list += ll
+        # print(f"   {item_list=}")
+        for result_ix, core_item in enumerate(item_list):
+            gui_item = core_to_gui_item(
+                core_item,
+                name_var=StringVar(value=core_item.name),
+                content_var=StringVar(value=core_item.content),
+                )
+            self.search_results_list.append(gui_item)
+            self.ikid_to_result_slot[gui_item._ikid] = result_ix
+        # print(f"   {self.search_results_list=}")
         self.populate_search_results_canvas(self.search_results_list)
 
 def main():
     """Launch main Tkinter event loop."""
     root = Tk()
     root.title(f"indiek-gui v{__version__}")
     root.columnconfigure(0, weight=1)
     root.rowconfigure(0, weight=1)
 
     # for some reason width and height below have no effect
     root.configure(width=2000, height=1000)
 
     Orchestrator(root)
 
-    root.bind('q', lambda e: root.destroy())
     root.mainloop()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `indiek-gui-0.0.2/indiek/gui/items.py` & `indiek-gui-0.0.3/indiek/gui/items.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 from tkinter import StringVar
-from indiek.core.items import Item as CoreItem
+from indiek.core.items import (Item as CoreItem,
+                               Definition as CoreDefinition,
+                               Proof as CoreProof,
+                               Theorem as CoreTheorem)
 
 
-class GUIItem(CoreItem):
+class Item(CoreItem):
     """
     Indiek GUI Item.
 
     This subclasses the core Item class and adds some GUI-specific functionality.
     """
+
     def __str__(self):
-        return f"GUI Item with ID {self._ikid} and name {self.name}"
-    
+        return f"GUI {self.__class__.__name__} with ID {self._ikid} and name {self.name}"
+
     def __init__(self, name_var: StringVar, content_var: StringVar, **kwargs):
         super().__init__(**kwargs)
         self.name_var = name_var
         self.content_var = content_var
 
     def update_name(self, name: str):
         self.name_var.set(name)
         self.name = name
 
     def update_content(self, content: str):
         self.content_var.set(content)
         self.content = content
 
 
-def core_to_gui_item(core_item: CoreItem, name_var: StringVar, content_var: StringVar) -> GUIItem:
-    return GUIItem(
+class Definition(Item, CoreDefinition):
+    pass
+
+
+class Proof(Item, CoreProof):
+    pass
+
+
+class Theorem(Item, CoreTheorem):
+    pass
+
+
+CORE_TO_GUI_TYPES = {
+    CoreDefinition: Definition,
+    CoreProof: Proof,
+    CoreTheorem: Theorem
+}
+
+
+def core_to_gui_item(core_item: CoreItem, name_var: StringVar, content_var: StringVar) -> Item:
+    return CORE_TO_GUI_TYPES[core_item.__class__](
         name_var=name_var,
         content_var=content_var,
-        name=core_item.name, 
-        content=core_item.content, 
+        name=core_item.name,
+        content=core_item.content,
         _ikid=core_item._ikid
-        )
+    )
```

### Comparing `indiek-gui-0.0.2/indiek_gui.egg-info/PKG-INFO` & `indiek-gui-0.0.3/indiek_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.2/setup.py` & `indiek-gui-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-gui',
     python_requires='>=3.8',
-    version='0.0.2',
+    version='0.0.3',
     url='https://pypi.org/project/indiek-gui/',
     description='Tkinter GUI for IndieK',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.gui'],
-    install_requires=['indiek-core == 0.1.2'],
+    install_requires=['indiek-core == 0.1.3'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

