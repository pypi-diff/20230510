# Comparing `tmp/smartjs-0.1.0.tar.gz` & `tmp/smartjs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.1.0.tar", max compression
+gzip compressed data, was "smartjs-0.1.1.tar", max compression
```

## Comparing `smartjs-0.1.0.tar` & `smartjs-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      383 2023-05-07 23:02:01.983688 smartjs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.1.0/smartjs/__init__.py
--rw-r--r--   0        0        0    13214 2023-05-07 13:14:18.303555 smartjs-0.1.0/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.0/smartjs/constants.py
--rw-r--r--   0        0        0     4880 2023-05-07 23:02:01.978824 smartjs-0.1.0/smartjs/elements.py
--rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.1.0/smartjs/functions.py
--rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.1.0/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.0/smartjs/page.py
--rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.1.0/smartjs/path.py
--rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.0/smartjs/style.py
--rw-r--r--   0        0        0      665 2023-05-07 23:02:06.918074 smartjs-0.1.0/setup.py
--rw-r--r--   0        0        0      414 2023-05-07 23:02:06.918310 smartjs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      376 2023-05-10 13:12:48.909432 smartjs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.1.1/smartjs/__init__.py
+-rw-r--r--   0        0        0    13770 2023-05-10 13:11:56.805246 smartjs-0.1.1/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.1.1/smartjs/constants.py
+-rw-r--r--   0        0        0     4970 2023-05-10 13:03:07.134383 smartjs-0.1.1/smartjs/elements.py
+-rw-r--r--   0        0        0     5808 2023-05-10 13:03:37.759379 smartjs-0.1.1/smartjs/functions.py
+-rw-r--r--   0        0        0    11908 2023-05-10 11:42:41.551886 smartjs-0.1.1/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.1.1/smartjs/page.py
+-rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.1.1/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.1.1/smartjs/style.py
+-rw-r--r--   0        0        0      658 2023-05-10 13:13:00.510127 smartjs-0.1.1/setup.py
+-rw-r--r--   0        0        0      407 2023-05-10 13:13:00.510525 smartjs-0.1.1/PKG-INFO
```

### Comparing `smartjs-0.1.0/smartjs/base.py` & `smartjs-0.1.1/smartjs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = [
         'Tag',
         'InputType',
         'SmartList',
         'BaseScript',
         'BaseElement',
         'BaseArg',
@@ -11,15 +13,16 @@
         'Text',
         'StyleItem',
         'BaseStyle',
         'SmartSet'
 ]
 
 from enum import Enum
-from collections import UserList, UserString
+from typing import Union, Iterable
+from collections import UserList, UserString, deque
 from smartjs.constants import *
 from smartjs.functions import *
 
 
 class Tag(Enum):
     _ignore_ = 'Tag i'
     Tag = vars()
@@ -302,28 +305,30 @@
     def __init__(self, *args, **kwargs):
         tag = list_of_type(args, Tag) or kwargs.pop('tag', None)
         if tag:
             if isinstance(tag, str):
                 tag = Tag(tag)
             elif isinstance(tag, list):
                 tag = tag[0]
-        self.tag = tag
-        self.klass = SmartList(list_of_type(args, Klass), kwargs.pop('klass', None))
+        self.tag: Tag = tag
+        self.klass: SmartList[Klass] = SmartList(list_of_type(args, Klass), kwargs.pop('klass', None))
         if self.KLASS:
             self.klass =[*self.KLASS.split(), *self.klass]
-        self.style = SmartList(list_of_type(args, StyleItem), kwargs.pop('style', None))
-        self.elements = SmartList(list_of_type(args, (BaseElement, Text)), kwargs.pop('elements', []))
-        self.after = SmartList(kwargs.pop('after', []))
-        self.before = SmartList(kwargs.pop('before', []))
-        self.list_kwargs = SmartList(list_of_type(args, Kwarg), kwargs.pop('kwargs', None))
-        self.args = SmartList(list_of_type(args, Arg), kwargs.pop('args', None))
-        self.script: SmartList[BaseScript, str] = SmartList(*kwargs.pop('script', list()))
-        self.dict_kwargs = kwargs
+        self.style_args: SmartList[StyleItem] = SmartList(list_of_type(args, StyleItem), None)
+        self.style_kwarg: Union[str, StyleItem] = kwargs.pop('style', '')
+        self.style = SmartList(self.style_kwarg, *self.style_args)
+        self.elements: SmartList[Union[BaseElement, Text]] = SmartList(list_of_type(args, (BaseElement, Text)), kwargs.pop('elements', []))
+        self.after: SmartList[Union[BaseElement, Text]] = SmartList(kwargs.pop('after', None))
+        self.before: SmartList[Union[BaseElement, Text]] = SmartList(kwargs.pop('before', None))
+        self.list_kwargs: SmartList[Kwarg] = SmartList(list_of_type(args, Kwarg), None)
+        self.args: SmartList[Arg] = SmartList(list_of_type(args, Arg), kwargs.pop('args', None))
+        self.dict_kwargs: dict[str, str] = kwargs
         self.dict_kwargs.update({k:v for k, v in self.post_init_kwargs.items() if not k in self.dict_kwargs.keys()})
         self.elements.extend(self.post_init_elements)
+        self.script: SmartList[BaseScript, str] = SmartList(kwargs.pop('script', list()))
         super().__init__(str(self))
 
         
     def __str__(self):
         self.update()
         return self.data
         
@@ -331,25 +336,25 @@
         self.data = remove_html_extra_whitespaces(self.render())
         
     @property
     def post_init_kwargs(self) -> dict:
         return {}
     
     @property
-    def post_init_elements(self) -> list['BaseElement', str]:
+    def post_init_elements(self) -> list[BaseElement, str]:
         return []
         
     def render_kwargs(self):
         return f'{join(set_filtered(self.list_kwargs))} {repr_dict(self.dict_kwargs)}'
     
     def render_klass(self):
-        return f'class="{join(set_filtered(self.klass))}"' if list_filtered(self.klass) else ''
+        return f'class="{join(set_filtered(self.klass))}"'  if list_filtered(self.klass) else ''
     
     def render_style(self):
-        return f'style="{join(set_filtered(self.style), sep="; ")}"' if list_filtered(self.style) else ''
+        return f'style="{join(list_filtered(self.style), sep="; ")}"' if list_filtered(self.style) else ''
     
     def render_after(self):
         return join(self.after) if list_filtered(self.after) else ''
     
     def render_before(self):
         return join(self.before) if list_filtered(self.before) else ''
     
@@ -385,36 +390,38 @@
         super().__init__(self.data)
     
     def __call__(self, *args):
         self.include(*args)
     
     def include(self, *args):
         for item in args:
-            if isinstance(item, (tuple, list, set)):
+            if isinstance(item, (tuple, list, set, deque)):
                 self.include(*item)
             else:
                 self.data.append(item)
+                
+    def extend(self, other: Iterable) -> None:
+        self.include(*other)
+        
+    def append(self, item) -> None:
+        self.include(item)
 
 
 class SmartSet(set):
     def __init__(self, *args):
         self.data = SmartList(*args)
         super().__init__(set(self.data))
 
     def __call__(self, *args):
         self.include(*args)
 
     def include(self, *args):
         for item in args:
-            if isinstance(item, (tuple, list, set)):
+            if isinstance(item, (tuple, list, set, deque)):
                 self.include(*item)
             else:
                 self.data.append(item)
         super().__init__(set(self.data))
         
 
     
-    
-
-    
-
-    
+
```

### Comparing `smartjs-0.1.0/smartjs/constants.py` & `smartjs-0.1.1/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.0/smartjs/elements.py` & `smartjs-0.1.1/smartjs/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,43 +48,50 @@
 from smartjs.functions import *
 from smartjs.javascript import *
 
 
 class HR(BaseElement):
 	pass
 
+
 class BR(BaseElement):
 	pass
 
+
 class Heading(BaseElement):
 	def __init__(self, size: int, *args, **kwargs):
 		self.size = size
 		super().__init__(*args, **kwargs)
 		
 	@property
 	def computed_tag(self):
 		return Tag(f'h{self.size}')
 	
 
 	
 class H1(BaseElement):
 	KLASS = 'text-primary'
 	
+	
 class H2(BaseElement):
 	KLASS = 'text-secondary'
 	
+	
 class H3(BaseElement):
 	KLASS = 'text-success'
 	
+	
 class H4(BaseElement):
 	KLASS = 'text-warning'
 	
+	
 class H5(BaseElement):
 	KLASS = 'text-danger'
 	
+	
 class H6(BaseElement):
 	KLASS = 'text-dark'
 
 
 class Div(BaseElement):
 	TAG = Tag('div')
 
@@ -110,15 +117,14 @@
 
 
 class Span(BaseElement):
 	pass
 
 
 
-
 class Aside(BaseElement):
 	pass
 
 
 class Ul(BaseElement):
 	pass
 
@@ -140,34 +146,34 @@
 	TAG = Tag('ul')
 	KLASS = 'list-group'
 	
 
 class ListGroupItemAction(BaseElement):
 	TAG = Tag('a')
 	KLASS = 'list-group-item-action'
-	
+
 
 class Anchor(BaseElement):
 	TAG = Tag('a')
-	
-	
+
+
 class NavList(BaseElement):
 	TAG = Tag('ul')
 	KLASS = 'nav'
-	
-	
+
+
 class NavItem(BaseElement):
 	TAG = Tag('li')
 	KLASS = 'nav-item'
-	
-	
+
+
 class NavLink(BaseElement):
 	TAG = Tag('a')
 	KLASS = 'nav-link'
-
+	
 
 class Input(BaseElement):
 	def __init__(self, *args, _type: str = 'text', **kwargs):
 		self.type = InputType(_type)
 		super().__init__(*args, **kwargs)
 		self.dict_kwargs['type'] = self.type.value
 		
@@ -212,14 +218,15 @@
 
 class BaseUniqueElement(BaseElement):
 	@property
 	def post_init_kwargs(self):
 		return dict(id=type(self).__name__.lower())
 
 
+
 class Main(BaseUniqueElement):
 	pass
 
 
 class Footer(BaseUniqueElement):
 	pass
 
@@ -291,7 +298,12 @@
 
 class HTML(BaseElement):
 	def __init__(self, head: Head, body: Body):
 		super().__init__(head, body)
 		
 	def render(self):
 		return f'<!DOCTYPE html>{super().render()}'
+
+
+if __name__ == '__main__':
+    x = ListGroupItemAction(href='/teste')
+    print(x)
```

### Comparing `smartjs-0.1.0/smartjs/functions.py` & `smartjs-0.1.1/smartjs/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 def list_filtered(items: Collection, func: Callable = lambda x: x not in [None, '']) -> list:
     return list(filter(func, items))
 
 
 def set_filtered(items: Collection, func: Callable = lambda x: x not in [None, '']) -> set:
-    return set(list_filtered(items, func))
+    return set(list_filtered([*items], func))
 
 
 def list_of_type(items: Collection, types: Union[type[GenericType], tuple[type[GenericType]]]) -> list[GenericType]:
     return [item for item in items if isinstance(item, types)]
 
 
 def list_of_strings(items: Collection) -> list[str]:
```

### Comparing `smartjs-0.1.0/smartjs/javascript.py` & `smartjs-0.1.1/smartjs/javascript.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         super().__init__(self.render())
         
     def render(self):
         return ScriptJoin(
                 self.const_create_element(self.form_name, 'form'),
                 self.set_attribute(self.form_name, 'action', self.action),
                 self.set_attribute(self.form_name, 'method', self.method),
-                self.class_name(self.form_name, self.form_class),
+                self.set_class_name(self.form_name, self.form_class),
                 *[self.set_attribute(self.form_name, k, v) for k, v in self.kwargs.items()],
                 self.set_id(self.form_name, self.id),
                 ScriptJoin(*self.form_fields),
                 *[self.set_append_to(self.form_name, *[item.container_name for item in self.form_fields])],
                 self.const_create_element(self.button_name, 'button'),
                 self.set_id(self.button_name, self.button_id),
                 self.set_append_to(self.form_name, self.button_name)
@@ -302,20 +302,21 @@
     def false(self, argument: str):
         self.args.append(self.set_false(self.name, argument))
         return self
     
 
 class Script(BaseScript):
     def __init__(self, *args, **kwargs):
-        self.args = args
+        self.args: SmartList = SmartList(*args)
         self.kwargs = kwargs
         super().__init__(f'<script {self.render_kwargs()}> {self.render_args()} </script>')
     
     def render_kwargs(self):
         return repr_dict(dict_filtered(self.kwargs), sep=" ")
     
     def render_args(self):
-        return join(SmartList(*self.args), '; ')
+        return join(self.args, '; ')
+
```

### Comparing `smartjs-0.1.0/smartjs/page.py` & `smartjs-0.1.1/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.0/smartjs/path.py` & `smartjs-0.1.1/smartjs/path.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.0/smartjs/style.py` & `smartjs-0.1.1/smartjs/style.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.1.0/setup.py` & `smartjs-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.1.0',
-    'description': 'Project for creation of javascript, html and style elements for use in web pages.',
+    'version': '0.1.1',
+    'description': 'Project for creation of javascript, html and style elements for web pages.',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
```

