# Comparing `tmp/pygame-json-ui-0.0.0.4.tar.gz` & `tmp/pygame-json-ui-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-json-ui-0.0.0.4.tar", last modified: Wed Apr 26 23:33:15 2023, max compression
+gzip compressed data, was "pygame-json-ui-1.0.0.0.tar", last modified: Wed May 10 15:49:18 2023, max compression
```

## Comparing `pygame-json-ui-0.0.0.4.tar` & `pygame-json-ui-1.0.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.094774 pygame-json-ui-0.0.0.4/
--rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0     9225 2023-04-26 23:33:15.092769 pygame-json-ui-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8632 2023-04-26 23:30:32.000000 pygame-json-ui-0.0.0.4/README.md
--rw-rw-rw-   0        0        0      713 2023-04-26 23:23:42.000000 pygame-json-ui-0.0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 23:33:15.094774 pygame-json-ui-0.0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.004381 pygame-json-ui-0.0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.064578 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/
--rw-rw-rw-   0        0        0     9225 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 23:33:14.000000 pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 23:33:15.091072 pygame-json-ui-0.0.0.4/src/pygame_ui/
--rw-rw-rw-   0        0        0      711 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/__init__.py
--rw-rw-rw-   0        0        0     4592 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/base.py
--rw-rw-rw-   0        0        0      404 2023-04-24 17:34:20.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/constants.py
--rw-rw-rw-   0        0        0     5791 2023-04-26 23:24:05.000000 pygame-json-ui-0.0.0.4/src/pygame_ui/elements.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:49:18.487063 pygame-json-ui-1.0.0.0/
+-rw-rw-rw-   0        0        0     1084 2023-04-21 11:56:45.000000 pygame-json-ui-1.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9922 2023-05-10 15:49:18.487063 pygame-json-ui-1.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9329 2023-05-10 12:47:33.000000 pygame-json-ui-1.0.0.0/README.md
+-rw-rw-rw-   0        0        0      713 2023-05-10 15:47:19.000000 pygame-json-ui-1.0.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 15:49:18.487063 pygame-json-ui-1.0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 15:49:18.409977 pygame-json-ui-1.0.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:49:18.471430 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/
+-rw-rw-rw-   0        0        0     9922 2023-05-10 15:49:18.000000 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-10 15:49:18.000000 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:49:18.000000 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 15:49:18.000000 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 15:49:18.000000 pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:49:18.487063 pygame-json-ui-1.0.0.0/src/pygame_ui/
+-rw-rw-rw-   0        0        0      812 2023-05-10 12:40:43.000000 pygame-json-ui-1.0.0.0/src/pygame_ui/__init__.py
+-rw-rw-rw-   0        0        0     7273 2023-05-10 11:35:48.000000 pygame-json-ui-1.0.0.0/src/pygame_ui/base.py
+-rw-rw-rw-   0        0        0      719 2023-05-10 11:21:08.000000 pygame-json-ui-1.0.0.0/src/pygame_ui/constants.py
+-rw-rw-rw-   0        0        0     7108 2023-05-10 11:56:33.000000 pygame-json-ui-1.0.0.0/src/pygame_ui/elements.py
```

### Comparing `pygame-json-ui-0.0.0.4/LICENSE` & `pygame-json-ui-1.0.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame-json-ui-0.0.0.4/PKG-INFO` & `pygame-json-ui-1.0.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-json-ui
-Version: 0.0.0.4
+Version: 1.0.0.0
 Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
 Author-email: Xander de Haan <sissydeslang@gmail.com>
 Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
 Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,15 @@
       - [Python](#python-file)
       - [JSON](#json-file)
 - [Element List](#element-list)
 - [Attribute List](#attribute-list)
    - [General](#general)
    - [Frame](#frame)
    - [Label](#label)
+   - [Text Input](#text-input)
    - [Button](#button)
    - [Switch](#switch)
    - [Slider](#slider)
 - [Frames](#frames)
    - [Frame Path](#frame-path)
 - [Examples](#examples)
 - [FAQ](#faq)
@@ -123,25 +124,28 @@
 ```
 
 ## Element List
 
 All of the following items will be refered to as `elements`:
 - Frame
 - Label
+- Text Input
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
 - `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
 - `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
+- `position_anchor: str` "top/center/bottom left/center/right" or "center" ("top left").
+- `position_relative: bool` Whether given position will be interpreted as relative to parent or absolute (false).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
 ### Frame
@@ -154,14 +158,23 @@
 - `text_aa: bool` anti-aliasing (true)
 - `font_name: str` ('Arial')
 - `font_size: int` (10)
 - `font_bold: bool` (false)
 - `font_italic: bool` (false)
 - `auto_size: bool` This will overwrite size of the boundry box to fit the text within (false).
 
+### Text Input
+
+- `typing_start_on_click: bool` Will set typing to True when the hitbox is clicked (true).
+- `typing_end_on_enter: bool` Will set typing to False when `enter` is pressed (true).
+- `typing: bool` Whether or not the users button presses will be processed (false).
+- `text: str` The currently typed string ("Your text here").
+- `caret: bool` Only used for backend (false).
+- `caret_timer: float` Only used for backend (0).
+
 ### Button
 
 - `contents: {}` The button is basically just a frame with the following default attributes added to it. Making a button manually from a frame is possible, but deprecated.
 - `is_clickable: bool` (true)
 - `is_hoverable: bool` (true)
 - `click_start: bool` (false)
 - `click_end: bool` (false)
```

### Comparing `pygame-json-ui-0.0.0.4/README.md` & `pygame-json-ui-1.0.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
       - [Python](#python-file)
       - [JSON](#json-file)
 - [Element List](#element-list)
 - [Attribute List](#attribute-list)
    - [General](#general)
    - [Frame](#frame)
    - [Label](#label)
+   - [Text Input](#text-input)
    - [Button](#button)
    - [Switch](#switch)
    - [Slider](#slider)
 - [Frames](#frames)
    - [Frame Path](#frame-path)
 - [Examples](#examples)
 - [FAQ](#faq)
@@ -109,25 +110,28 @@
 ```
 
 ## Element List
 
 All of the following items will be refered to as `elements`:
 - Frame
 - Label
+- Text Input
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
 - `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
 - `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
+- `position_anchor: str` "top/center/bottom left/center/right" or "center" ("top left").
+- `position_relative: bool` Whether given position will be interpreted as relative to parent or absolute (false).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
 ### Frame
@@ -140,14 +144,23 @@
 - `text_aa: bool` anti-aliasing (true)
 - `font_name: str` ('Arial')
 - `font_size: int` (10)
 - `font_bold: bool` (false)
 - `font_italic: bool` (false)
 - `auto_size: bool` This will overwrite size of the boundry box to fit the text within (false).
 
+### Text Input
+
+- `typing_start_on_click: bool` Will set typing to True when the hitbox is clicked (true).
+- `typing_end_on_enter: bool` Will set typing to False when `enter` is pressed (true).
+- `typing: bool` Whether or not the users button presses will be processed (false).
+- `text: str` The currently typed string ("Your text here").
+- `caret: bool` Only used for backend (false).
+- `caret_timer: float` Only used for backend (0).
+
 ### Button
 
 - `contents: {}` The button is basically just a frame with the following default attributes added to it. Making a button manually from a frame is possible, but deprecated.
 - `is_clickable: bool` (true)
 - `is_hoverable: bool` (true)
 - `click_start: bool` (false)
 - `click_end: bool` (false)
```

### Comparing `pygame-json-ui-0.0.0.4/pyproject.toml` & `pygame-json-ui-1.0.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygame-json-ui"
-version = "0.0.0.4"
+version = "1.0.0.0"
 authors = [
   { name="Xander de Haan", email="sissydeslang@gmail.com" },
 ]
 description = "Pygame UI is a package for building user interfaces for pygame in a JSON Format."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `pygame-json-ui-0.0.0.4/src/pygame_json_ui.egg-info/PKG-INFO` & `pygame-json-ui-1.0.0.0/src/pygame_json_ui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-json-ui
-Version: 0.0.0.4
+Version: 1.0.0.0
 Summary: Pygame UI is a package for building user interfaces for pygame in a JSON Format.
 Author-email: Xander de Haan <sissydeslang@gmail.com>
 Project-URL: Homepage, https://github.com/RednaxGaming/pygame_ui
 Project-URL: Bug Tracker, https://github.com/RednaxGaming/pygame_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,15 @@
       - [Python](#python-file)
       - [JSON](#json-file)
 - [Element List](#element-list)
 - [Attribute List](#attribute-list)
    - [General](#general)
    - [Frame](#frame)
    - [Label](#label)
+   - [Text Input](#text-input)
    - [Button](#button)
    - [Switch](#switch)
    - [Slider](#slider)
 - [Frames](#frames)
    - [Frame Path](#frame-path)
 - [Examples](#examples)
 - [FAQ](#faq)
@@ -123,25 +124,28 @@
 ```
 
 ## Element List
 
 All of the following items will be refered to as `elements`:
 - Frame
 - Label
+- Text Input
 - Button
 - Switch
 - Slider
 - Dropdown (Coming soon)
 
 ## Attribute List
 - `attribute: data type` description (default value).
 ### General
 These attributes can be given to any element type
 - `type: str` REQUIRED, specifies which element this is choose from [this](#element-list) list.
 - `position: [x,y]` Sets position from top-left of screen to top-left of element boundry box ([0, 0]).
+- `position_anchor: str` "top/center/bottom left/center/right" or "center" ("top left").
+- `position_relative: bool` Whether given position will be interpreted as relative to parent or absolute (false).
 - `size: [x,y]` Sets the size of the element boundry box ([0, 0]).
 - `background_color: (r,g,b)` The boundry box will be filled with this color (none).
 - `is_visible: bool` (true).
 - `is_hoverable: bool` (false).
 - `is_clickable: bool` (false).
 
 ### Frame
@@ -154,14 +158,23 @@
 - `text_aa: bool` anti-aliasing (true)
 - `font_name: str` ('Arial')
 - `font_size: int` (10)
 - `font_bold: bool` (false)
 - `font_italic: bool` (false)
 - `auto_size: bool` This will overwrite size of the boundry box to fit the text within (false).
 
+### Text Input
+
+- `typing_start_on_click: bool` Will set typing to True when the hitbox is clicked (true).
+- `typing_end_on_enter: bool` Will set typing to False when `enter` is pressed (true).
+- `typing: bool` Whether or not the users button presses will be processed (false).
+- `text: str` The currently typed string ("Your text here").
+- `caret: bool` Only used for backend (false).
+- `caret_timer: float` Only used for backend (0).
+
 ### Button
 
 - `contents: {}` The button is basically just a frame with the following default attributes added to it. Making a button manually from a frame is possible, but deprecated.
 - `is_clickable: bool` (true)
 - `is_hoverable: bool` (true)
 - `click_start: bool` (false)
 - `click_end: bool` (false)
```

### Comparing `pygame-json-ui-0.0.0.4/src/pygame_ui/elements.py` & `pygame-json-ui-1.0.0.0/src/pygame_ui/elements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 blabla
 """
 
-from importlib import import_module
 import os
 import sys
 
 import pygame.font as pygfont
 import pygame.rect as pygrect
 import pygame.draw as pygdraw
 
@@ -19,41 +18,50 @@
 
 
 class UI_Element:
 	is_visible = True
 	is_hoverable = False
 	is_clickable = False
 	position = [0,0]
+	position_anchor = "top left"
+	position_relative = False
 	size = [0,0]
-	anchor = "absolute"
 	auto_size = False
 	background_color = None
 
 	def __init__(self, initial_data, kwargs):
 		for dictionary in initial_data:
 			for key in dictionary:
 				setattr(self, key, dictionary[key])
+		self.parent = kwargs.pop('parent')
 		for key in kwargs:
 			setattr(self, key, kwargs[key])
-		
-		self.rectangle = pygrect.Rect(self.position, self.size)
-	
+
+		self.change_position(self.position)
+
 	def change_position(self, new_position):
 		"""
 		You can figure this one out yourself. If you can't then... *sigh*
 		"""
-		self.position = new_position
+		position_zero = [0,0]
+		if self.position_relative:
+			position_zero = [position_zero[i] + self.parent.position[i] for i in [0,1]]
+		if self.position_anchor == 'center':
+			anchor = [0,0]
+		else:
+			anchor = [ANCHORS[self.position_anchor.split(' ')[i]] for i in [1,0]]
+		self.position = [new_position[i] - (anchor[i]/2+.5)*self.size[i] + position_zero[i] for i in [0,1]]
 		self.rectangle = pygrect.Rect(self.position, self.size)
 
 	def change_size(self, new_size):
 		"""
 		You can figure this one out yourself. If you can't then... *sigh*
 		"""
 		self.size = new_size
-		self.rectangle = pygrect.Rect(self.position, self.size)
+		self.change_position(self.position)
 	
 	def draw_bg(self, pygame_window):
 		if self.auto_size:
 			if isinstance(self, label):
 				auto_rect = pygrect.Rect(self.position, self.font.size(self.text))
 			pygdraw.rect(pygame_window, self.background_color, auto_rect)
 		else:
@@ -70,16 +78,26 @@
 	contents = {}
 
 	def __init__(self, *initial_data, **kwargs):
 		self.elements = {}
 		super().__init__(initial_data, kwargs)
 		for name, data in self.contents.items():
 			element_type = data.pop('type')
-			self.elements[name] = globals()[element_type](data)
+			self.elements[name] = globals()[element_type](data, parent=self)
 	
+	def get_text_input_elements(self):
+		text_input_elements = []
+		for name, element in self.elements.items():
+			if element.is_visible:
+				if isinstance(element, frame):
+					text_input_elements.extend(element.get_text_input_elements())
+				elif isinstance(element, text_input):
+					text_input_elements.append(element)
+		return text_input_elements
+
 	def get_interactive_elements(self):
 		interactives = []
 		for name, element in self.elements.items():
 			if element.is_visible:
 				if isinstance(element, frame) and not isinstance(element, button):
 					interactives.extend(element.get_interactive_elements())
 				elif element.is_hoverable or element.is_clickable:
@@ -125,16 +143,41 @@
 			if key in FONT_ATTRIBUTES:
 				setattr(self, key, kwargs[key])
 			else:
 				raise KeyError(key+' is not a font attribute. '+MUST_BE+FONT_ATTRIBUTES+'\n'+ISSUE_REPORT)
 		self.font = pygfont.SysFont(self.font_name, self.font_size, self.font_bold, self.font_italic)
 
 	def draw(self, pygame_window):
-		text_render = self.font.render(self.text, self.text_aa, self.text_color, self.background_color)
-		pygame_window.blit(text_render, self.position)
+		text_surface = self.font.render(self.text, self.text_aa, self.text_color, self.background_color)
+		pygame_window.blit(text_surface, self.position)
+
+
+class text_input(label):
+	"""
+	The UI element for an input field.
+
+	My quote-bucket is empty :(
+	"""
+	is_clickable = True
+	click_start = False
+	click_end = False
+	click_held = False
+	typing_start_on_click = True
+	typing_end_on_enter = True
+	typing = False
+	text = "Your input here"
+	caret = False
+	caret_timer = 0
+
+	def draw(self, pygame_window):
+		text_to_render = self.text
+		if self.caret:
+			text_to_render += '|'
+		text_surface = self.font.render(text_to_render, self.text_aa, self.text_color, self.background_color)
+		pygame_window.blit(text_surface, self.position)
 
 
 class button(frame):
 	"""
 	The UI element for a button.
 
 	What does this button do?
```

