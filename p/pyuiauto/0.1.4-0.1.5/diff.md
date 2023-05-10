# Comparing `tmp/pyUIauto-0.1.4.tar.gz` & `tmp/pyUIauto-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUIauto-0.1.4.tar", max compression
+gzip compressed data, was "pyUIauto-0.1.5.tar", max compression
```

## Comparing `pyUIauto-0.1.4.tar` & `pyUIauto-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.4/LICENSE
--rw-r--r--   0        0        0      905 2023-05-05 09:46:59.398664 pyUIauto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.4/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.4/pyuiauto/application.py
--rw-r--r--   0        0        0     7054 2023-05-05 08:36:46.552241 pyUIauto-0.1.4/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16286 2023-05-05 08:45:27.938656 pyUIauto-0.1.4/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.4/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.4/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.4/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.4/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    10349 2023-05-05 09:46:30.530861 pyUIauto-0.1.4/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.4/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.4/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.4/pyuiauto/win/application.py
--rw-r--r--   0        0        0     9670 2023-05-05 09:45:20.768597 pyUIauto-0.1.4/pyuiauto/win/components.py
--rw-r--r--   0        0        0     3923 2023-05-05 09:43:34.856284 pyUIauto-0.1.4/README.md
--rw-r--r--   0        0        0     4927 2023-05-05 09:47:15.645693 pyUIauto-0.1.4/setup.py
--rw-r--r--   0        0        0     4802 2023-05-05 09:47:15.645693 pyUIauto-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.5/LICENSE
+-rw-r--r--   0        0        0      905 2023-05-10 15:39:14.372245 pyUIauto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.5/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.5/pyuiauto/application.py
+-rw-r--r--   0        0        0     8169 2023-05-10 15:15:17.698897 pyUIauto-0.1.5/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16286 2023-05-09 13:30:03.726429 pyUIauto-0.1.5/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.5/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.5/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.5/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     5023 2023-05-10 14:55:26.618887 pyUIauto-0.1.5/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    11300 2023-05-09 16:48:31.229370 pyUIauto-0.1.5/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.5/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.5/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-10 15:17:43.023116 pyUIauto-0.1.5/pyuiauto/win/application.py
+-rw-r--r--   0        0        0    10500 2023-05-10 14:55:05.472451 pyUIauto-0.1.5/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     3995 2023-05-10 15:39:01.251510 pyUIauto-0.1.5/README.md
+-rw-r--r--   0        0        0     4999 2023-05-10 15:39:24.046791 pyUIauto-0.1.5/setup.py
+-rw-r--r--   0        0        0     4872 2023-05-10 15:39:24.047787 pyUIauto-0.1.5/PKG-INFO
```

### Comparing `pyUIauto-0.1.4/LICENSE` & `pyUIauto-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.4/pyproject.toml` & `pyUIauto-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyUIauto-0.1.4/pyuiauto/base/application.py` & `pyUIauto-0.1.5/pyuiauto/base/application.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # ___MODULES___
 from __future__ import annotations
 import time
 from abc import ABC, abstractmethod
 import logging
+import contextlib
 
 # __MY_MODULES__
-from pyuiauto.base.components import UIWindowWrapper, UIButtonWrapper, UIMenuItemWrapper
+from pyuiauto.components import UIWindow, UIButton, UIMenuItem, UIMenuBarItem
 from pyuiauto.exceptions import ProcessNotFoundError
 
 
 # ___CLASSES___
 
 class UISystemTrayIconWrapper(ABC):
     '''UISystemTrayIconWrapper\n
     Provides a system tray icon manager to help find the system tray icon for an application\n
     whether it be hidden within the notification expand window or on the taskbar.'''
     def __init__(self, app: UIApplicationWrapper):
         self.app = app
 
     @abstractmethod
-    def __enter__(self) -> UIButtonWrapper:
+    def __enter__(self) -> UIButton:
         'Using a context manager helps to creates the UIButton dynamically.'
 
     @abstractmethod
     def __exit__(self, *args) -> None:
         'Using a context manager helps to dynamically tidy any open windows.'
     
 class UIPopupMenuWrapper(ABC):
@@ -39,15 +40,15 @@
     def __init__(self, app: UIApplicationWrapper, popup_naming_scheme: str = None) -> None:
         self.app = app
         self.win_name = popup_naming_scheme if popup_naming_scheme else app.appName
         self.current_popup = None
         self.steps = 0
 
     @abstractmethod
-    def getMenuItemFromPath(self, *path: str) -> UIMenuItemWrapper:
+    def getMenuItemFromPath(self, *path: str) -> UIMenuItem:
         '''PopupMenu class get menu item from path method\n
         Uses the specified path to return a menu item component at [-1] index of the path.'''
     
     @abstractmethod
     def back(self):
         'Go back a popup menu window to the previous item'
 
@@ -87,28 +88,28 @@
         Force quits the application.'''
         self.end_time = time.time()
     
     def getRuntime(self):
         return self.end_time - self.start_time
     
     @abstractmethod
-    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindowWrapper:
+    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindow:
         '''Application class window method\n
         Finds a window child component with the specified criteria.
         Raises an exception if the criteria matches no components (recursive).\n
         Args:                    
                     (criteria)
                     title: the name of the component (of type string)
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     component: window component wrapped to it's cross compatible custom wrapper of type UIWindowWrapper'''
     
     @abstractmethod
-    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindowWrapper]:
+    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindow]:
         '''Application class windows method\n
         Finds all window child components with the specified criteria.
         Raises an exception if the criteria matches > 1 or no components (recursive).\n
         Args:                    
                     (criteria)
                     title: the name of the component (of type string)
 
@@ -148,14 +149,38 @@
         
         The popup_naming_scheme can vary from app to app however, these are some examples:\n
         - *the application name* (default)
         - "Context"
         - "Pop-up"
         '''
 
+    @contextlib.contextmanager
+    def systemTrayPopupPath(self, *path: str) -> UIMenuBarItem:
+        '''Application class system tray popup select method\n
+        This method selects menu items after clicking the system tray, from the *args passed in as a path.'''
+        with self.getSystemTrayIcon() as icon:
+            icon.right_click()
+            with self.getPopupMenu() as popup:
+                try:
+                    yield popup.getMenuItemFromPath(*path)
+                except:
+                    logging.warning(f"{path} is disabled or not available")
+    
+    @contextlib.contextmanager
+    def menuBarPopupPath(self, window: UIWindow, *path: str) -> UIMenuBarItem:
+        '''Application class menu bar select method\n
+        This method selects menu items on the menubar from the *args passed in as a path.'''
+        menuBarItem = window.findFirstR(title=path[0], control_type=UIMenuBarItem)
+        if len(path) == 1:
+            yield menuBarItem
+        
+        menuBarItem.click()
+        with self.getPopupMenu() as popup:
+            yield popup.getMenuItemFromPath(*path[1:])
+
     @abstractmethod
     def getCrashReport(self) -> str:
         '''Application class get crash report method\n
         Gets all crash reports between the start and end time of the application running.'''
 
     def relaunchApp(self):
         '''Application class relaunch app method\n
```

### Comparing `pyUIauto-0.1.4/pyuiauto/base/components.py` & `pyUIauto-0.1.5/pyuiauto/base/components.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.4/pyuiauto/exceptions.py` & `pyUIauto-0.1.5/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.4/pyuiauto/mac/application.py` & `pyUIauto-0.1.5/pyuiauto/mac/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #___MODULES___
 from typing import Type
 import os
 import datetime
+import logging
 
 # pip installed modules
 try:
         import atomacos
 except ImportError: # requires pip install
         raise ModuleNotFoundError('To install the required modules use pip install atomacos (MacOS ONLY)')
 
@@ -105,12 +106,12 @@
 
                 if app == self.appName:
 
                     file_time = datetime.datetime(int(year), int(month), int(date), int(time_[:2]), int(time_[2:4]), int(time_[4:]))
                     start_time = datetime.datetime.fromtimestamp(self.start_time)
                     end_time = datetime.datetime.fromtimestamp(self.end_time)
                     
-                    print(f"Start Time: {start_time}, End Time: {end_time}, File Time: {file_time}")
+                    logging.debug(f"Start Time: {start_time}, End Time: {end_time}, File Time: {file_time}")
                     
                     
                     if ( (start_time <= file_time) and (end_time >= file_time) ):
                         return os.path.join(diagnostic_reports_path, file)
```

### Comparing `pyUIauto-0.1.4/pyuiauto/mac/components.py` & `pyUIauto-0.1.5/pyuiauto/win/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing import Type
 import time
 from abc import ABCMeta
 import logging
 
 # pip installed modules
 try:
-    from atomacos import NativeUIElement
+        from pywinauto.controls.uiawrapper import UIAWrapper
+        from pywinauto.keyboard import send_keys
+        from pywinauto.timings import wait_until
+        from pywinauto.uia_defines import NoPatternInterfaceError
 except ImportError: # requires pip install
-    raise ModuleNotFoundError('To install the required modules use pip install atomacos (MacOS ONLY)')
+        raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
 
 
-from ApplicationServices import AXValueCreate, kAXValueCGPointType, kAXValueCGSizeType
-import Quartz.CoreGraphics as CG
-
 #___MY_MODULES___
 from pyuiauto.exceptions import ElementNotFound
 from pyuiauto.base.components import *
 
 
 #___DEFINING_NATIVE_WRAPPER_META___
 
@@ -38,139 +38,123 @@
     @staticmethod
     def find_wrapper(component):
         """Find the correct wrapper for this UIA component"""
         # Set a general wrapper by default
         wrapper_match = UIBaseComponent
 
         # Check for a more specific wrapper in the registry
-        try:
-            control_type = component.AXRole
-        except:
-            control_type = "No Role"
-            logging.warning(f"Component: {component} | has no control type / AXRole attribute")
+        control_type = component.element_info.control_type
 
         if control_type in UIBaseComponentWrapperMeta.control_type_to_cls:
             wrapper_match = UIBaseComponentWrapperMeta.control_type_to_cls[control_type]
         else:
             raise NotImplementedError(f"{component} doesn't have an implemented wrapper")
 
         return wrapper_match
 
+
+
+
+
+
 #___DEFINING_NATIVE_METHODS___
 
 class UIBaseComponent(UIBaseComponentWrapper, metaclass=UIBaseComponentMeta):
 
-    def __new__(cls, component: NativeUIElement):
+    def __new__(cls, component: UIAWrapper):
         """Construct the control wrapper"""
         return super(UIBaseComponent, cls)._create_wrapper(cls, component, UIBaseComponent)
 
     # -----------------------------------------------------------
-    def __init__(self, component: NativeUIElement):
+    def __init__(self, component: UIAWrapper):
         UIBaseComponentWrapper.__init__(self, component)
 
     def getValue(self):
-        return self.component.AXValue
+        return self.component.iface_value
     
     def setValue(self, value):
-        self.component.AXValue = value
+        self.component.set_value(value)
     
     def setFocus(self):
-        self.component.activate()
+        self.component.set_focus()
     
     def invoke(self):
-        self.component.Press()
+        self.component.invoke()
 
     def click(self):
-        self.component.clickMouseButtonLeft(self.getMidpoint())
+        self.component.click_input()
     
     def right_click(self):
-        self.component.clickMouseButtonRight(self.getMidpoint())
+        self.component.right_click_input()
     
     def isVisible(self):
         x, y, _, _= self.getCoordinates()
-        is_visible = self.component.getApplication().getElementAtPosition((x, y)) == self.component
-        return is_visible
+        visible_at_point = self.component.from_point(x, y).element_info.name == self.component.element_info.name
+        return self.component.is_visible() and visible_at_point
     
     def getMidpoint(self):
-        return ((self.component.AXPosition[0] + self.component.AXSize[0] / 2), (self.component.AXPosition[1] + self.component.AXSize[1] / 2))
-
+        return self.component.rectangle().mid_point()
+    
     def getCoordinates(self):
-        x, y = self.component.AXPosition
-        w, h = self.component.AXSize
-        return x, y, x+w, y+h
+        rectangle = self.component.rectangle()
+        return rectangle.left, rectangle.top, rectangle.right, rectangle.bottom
     
     def getSizes(self):
-        return self.component.AXSize
+        rectangle = self.component.rectangle()
+        return rectangle.width(), rectangle.height()
     
     def getChildren(self):
-        return list(UIBaseComponent(component, component.AXRole) for component in self.component.AXChildren)
-    
-    getDescendants = getChildren
+        return list(UIBaseComponent(component) for component in self.component.children())
+
+    def getDescendants(self):
+        return list(UIBaseComponent(component) for component in self.component.descendants())
     
     def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        for i in (  {"conversion": "title", "apple": "AXTitle"},
-                    {"conversion": "description", "apple": "AXDescription"},
-                ):
-            try:
-                criteria[i["apple"]] = criteria.pop(i["conversion"])
-            except KeyError:
-                pass
-
         timeafter = time.time() + timeout
         while time.time() < timeafter:
-            item = function(AXRole=control_type.native_control_type, **criteria)
+            item = function(control_type=control_type.native_control_type, **criteria)
             item_check = check_function(item)
             if item_check:
                 if type(item) == list:
                     return list(UIBaseComponent(i) for i in item)
                 else:
                     return UIBaseComponent(item)
             time.sleep(retry_interval)
-        raise ElementNotFound(f"Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
-
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.findFirst,
-                                check_function=self._check_element_exists,
-                                control_type=control_type,
-                                timeout=timeout,
-                                retry_interval = retry_interval,
-                                **criteria)
-
+        raise ElementNotFound(f"CheckFunction returned: Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
+        
     def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.findAll,
-                                check_function=self._check_elements_exist,
-                                control_type=control_type,
-                                timeout=timeout,
-                                retry_interval = retry_interval,
-                                **criteria)
-
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.findFirstR,
-                                check_function=self._check_element_exists,
-                                control_type=control_type,
-                                timeout=timeout,
-                                retry_interval = retry_interval,
-                                **criteria)
-
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.findAllR,
-                                check_function=self._check_elements_exist,
-                                control_type=control_type,
-                                timeout=timeout,
-                                retry_interval = retry_interval,
-                                **criteria)
+        return self._wait_find(function=self.component.children,
+                        check_function=self._check_elements_exist,
+                        control_type=control_type,
+                        timeout=timeout,
+                        retry_interval=retry_interval,
+                        **criteria)
     
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self.findAll(control_type, timeout, retry_interval, **criteria)[0]
+
     def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAll(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
     
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self._wait_find(function=self.component.descendants,
+                        check_function=self._check_elements_exist,
+                        control_type=control_type,
+                        timeout=timeout,
+                        retry_interval=retry_interval,
+                        **criteria)
+    
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self.findAllR(control_type, timeout, retry_interval, **criteria)[0]
+
     def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAllR(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
@@ -182,107 +166,154 @@
     
     @classmethod
     @property
     def control_type(cls) -> Type:
         return type(cls)
     
     @property
-    def title(self) -> str:
-        return self.component.AXTitle
-
-
-# ============================================
-
-
-class UIAppRoot(UIBaseComponent):
-    native_control_type: str = "AXApplication"
-
-
-# ============================================
-
+    def title(self):
+        return self.component.element_info.name
+    
+    
 
 class UIButton(UIButtonWrapper, UIBaseComponent):
-    native_control_type: str = "AXButton"
+    native_control_type: str = "Button"
+
+    def getValue(self):
+        return self.component.get_toggle_state()
     
     def press(self):
-        self.invoke()
+        self.component.click()
     
     def setValue(self, value):
         return super().setValue(value)
 
 class UIRadioButton(UIRadioButtonWrapper, UIBaseComponent):
-    native_control_type: str = "AXRadioButton"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "RadioButton"
 
 class UIText(UITextWrapper, UIBaseComponent):
-    native_control_type: str = "AXText"
-
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Text"
+    
 class UISlider(UISliderWrapper, UIBaseComponent):
-    native_control_type: str = "AXSlider"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Slider"
+
+    def getValue(self):
+        return self.component.value()
 
 class UIEdit(UIEditWrapper, UIBaseComponent):
-    native_control_type: str = "AXTextArea"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Edit"
 
-class UIMenu(UIMenuWrapper, UIBaseComponent):
-    native_control_type: str = "AXMenu"
+    def getValue(self):
+        return self.component.get_value()
+    
+    def setValue(self, value):
+        self.component.set_focus()
+        self.component.invoke()
+        send_keys(str(value) + "{ENTER}")
 
+class UIMenu(UIMenuWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Menu"
+    
 class UIMenuItem(UIMenuItemWrapper, UIBaseComponent):
-    native_control_type: str = "AXMenuItem"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "MenuItem"
+
+    def getValue(self):
+        try:
+            return bool(self.component.iface_toggle)
+        except NoPatternInterfaceError:
+            return False
 
     def select(self):
-        self.invoke()
+        self.component.select()
     
     def setValue(self, value):
         return super().setValue(value)
 
 class UIWindow(UIWindowWrapper, UIBaseComponent):
-    native_control_type: str = "AXWindow"
-
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Window"
+    
     def moveResize(self, x=None, y=None, width=None, height=None):
-        left, top, _, _ = self.getCoordinates()
-        w, h = self.getSizes()
+        cur_rect = self.component.rectangle()
 
         # if no X is specified - so use current coordinate
         if x is None:
-            x = left
+            x = cur_rect.left
 
         # if no Y is specified - so use current coordinate
         if y is None:
-            y = top
+            y = cur_rect.top
 
         # if no width is specified - so use current width
         if width is None:
-            width = w
+            width = cur_rect.width()
 
         # if no height is specified - so use current height
         if height is None:
-            height = h
+            height = cur_rect.height()
 
         # ask for the window to be moved
-        point = CG.CGPoint(x=x, y=y)
-        self.component.AXPosition = AXValueCreate(kAXValueCGPointType, point)
-
-        # ask for the window to be resized
-        size = CG.CGSize(width=width, height=height)
-        self.component.AXSize = AXValueCreate(kAXValueCGSizeType, size)
+        self.component.iface_transform.Move(x, y)
+        self.component.iface_transform.Resize(width, height)
 
     def close(self):
-        self.component.AXCloseButton.Press()
+        self.component.close()
 
 class UIGroup(UIGroupWrapper, UIBaseComponent):
-    name="AXGroup"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Custom"
 
 class UIStaticText(UIStaticTextWrapper, UIBaseComponent):
-    name="AXStaticText"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Text"
 
-class UITitleBar(UITitleBarWrapper, UIBaseComponent):
-    name="AXTitleBar"
+    def getValue(self):
+        return self.component.window_text()
 
+class UITitleBar(UITitleBarWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "TitleBar"
+        
 class UIMenuBar(UIMenuBarWrapper, UIBaseComponent):
-    native_control_type: str = "AXMenuBar"
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "MenuBar"
 
-class UIProgressBar(UIBaseComponent, UIBaseComponent):
-    native_control_type: str = "AXProgressIndicator"
+class UIProgressBar(UIProgressBarWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "ProgressBar"
+
+    def getValue(self):
+        return int(self.component.legacy_properties()['Value'])
 
 # !!! Mac Specific !!!
 
-class UIMenuBarItem(UIMenuItemWrapper, UIBaseComponent):
-    native_control_type: str = "AXMenuBarItem"
+class UIMenuBarItem(UIMenuItem, UIBaseComponent): ...
```

### Comparing `pyUIauto-0.1.4/pyuiauto/wait.py` & `pyUIauto-0.1.5/pyuiauto/wait.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.4/pyuiauto/win/application.py` & `pyUIauto-0.1.5/pyuiauto/win/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #___MODULES___
 from __future__ import annotations
 from typing import Type
 import datetime
 import subprocess
+import logging
 
 # pip installed modules
 try:
         import pywinauto
         from pywinauto.application import process_get_modules
 except ImportError: # requires pip install
         raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
@@ -47,15 +48,18 @@
         try:
             self._getIcon(backendExplorer.taskbar)
         except:
                 self.__systrayExpandWindow = None
                 self._iconHidden = True
     
     def _getIcon(self, parent: pywinauto.WindowSpecification) -> UIButton:
-        return UIButton(parent.child_window(title_re=f".*of.*{self.app.appName}", control_type="Button", found_index=0).wrapper_object())
+        icon = parent.child_window(title_re=f".* {self.app.appName}", control_type="Button", found_index=0)
+        icon.wait('exists', timeout=2)
+        icon.wrapper_object()
+        return UIButton(icon)
 
     def __openSystemTrayExpand(self) -> pywinauto.WindowSpecification:
         # Open the system tray
         backendExplorer.taskbarExpand.invoke()
 
         # Select the audient icon
         try:
@@ -159,18 +163,18 @@
             if self.appPath == module[1]:
                  return True
         return False
 
     def isAppRunning(self):
         return self._app.is_process_running()
 
-    def getSystemTrayIcon(self):
+    def getSystemTrayIcon(self) -> UISystemTrayIcon:
         return UISystemTrayIcon(self)
     
-    def getPopupMenu(self, popup_naming_scheme: str = None):
+    def getPopupMenu(self, popup_naming_scheme: str = None) -> UIPopupMenu:
         return UIPopupMenu(self, popup_naming_scheme)
     
     def getCrashReport(self):
         # Convert epoch timestamp to a datetime object
         start_datetime = datetime.datetime.fromtimestamp(self.start_time)
         end_datetime = datetime.datetime.fromtimestamp(self.end_time)
```

### Comparing `pyUIauto-0.1.4/README.md` & `pyUIauto-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -83,13 +83,15 @@
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
   - 0.1.4
     - Fixed some issues with setValue() method on buttons and menus
+  - 0.1.5
+    - Added context managers for better popup menu handling
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyUIauto-0.1.4/setup.py` & `pyUIauto-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyUIauto-0.1.4/PKG-INFO` & `pyUIauto-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -105,14 +105,16 @@
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
   - 0.1.4
     - Fixed some issues with setValue() method on buttons and menus
+  - 0.1.5
+    - Added context managers for better popup menu handling
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

