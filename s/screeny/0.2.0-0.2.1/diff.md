# Comparing `tmp/screeny-0.2.0.tar.gz` & `tmp/screeny-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.2.0.tar", last modified: Wed May 10 13:57:31 2023, max compression
+gzip compressed data, was "screeny-0.2.1.tar", last modified: Wed May 10 19:38:17 2023, max compression
```

## Comparing `screeny-0.2.0.tar` & `screeny-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.605181 screeny-0.2.0/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.2.0/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    25653 2023-05-10 13:55:29.000000 screeny-0.2.0/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)     1617 2023-05-10 13:57:31.605320 screeny-0.2.0/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)     1236 2023-05-10 13:47:16.000000 screeny-0.2.0/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.2.0/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.602661 screeny-0.2.0/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.2.0/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)      446 2023-05-10 13:56:04.000000 screeny-0.2.0/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     4326 2023-05-10 13:36:01.000000 screeny-0.2.0/screeny/screeny.py
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 13:57:31.604889 screeny-0.2.0/screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)     1617 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      274 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       43 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-10 13:57:31.000000 screeny-0.2.0/screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      515 2023-05-10 13:57:31.606038 screeny-0.2.0/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.342211 screeny-0.2.1/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.2.1/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25653 2023-05-10 14:08:09.000000 screeny-0.2.1/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     1753 2023-05-10 19:38:17.342375 screeny-0.2.1/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     1373 2023-05-10 14:13:59.000000 screeny-0.2.1/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.2.1/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.337043 screeny-0.2.1/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)       28 2023-04-28 18:03:41.000000 screeny-0.2.1/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      446 2023-05-10 14:08:09.000000 screeny-0.2.1/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     4680 2023-05-10 19:32:34.000000 screeny-0.2.1/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-10 19:38:17.341832 screeny-0.2.1/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1753 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      274 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       43 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-10 19:38:17.000000 screeny-0.2.1/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      515 2023-05-10 19:38:17.343171 screeny-0.2.1/setup.cfg
```

### Comparing `screeny-0.2.0/LICENSE` & `screeny-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.2.0/LICENSE-3RD-Party.txt` & `screeny-0.2.1/LICENSE-3RD-Party.txt`

 * *Files identical despite different names*

### Comparing `screeny-0.2.0/PKG-INFO` & `screeny-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -29,16 +29,16 @@
 img = sc.take_screenshot()
 ```
 
 ## API-Reference
 
 * [screeny.take_screenshot](#screenytake_screenshotrect-qrect--none)
 * [screeny.get_mouse_pos](#screenyget_mouse_pos)
-* [screeny.locate_image_on_screen](#screenylocate_image_on_screen)
-* [screeny.locate_image_in_image](#screenylocate_image_in_image)
+* [screeny.locate_image_on_screen](#screenylocate_image_on_screenimage-str--typenparray-rect-qrect--none-confidence-float--08)
+* [screeny.locate_image_in_image](#locate_image_in_imageimg_to_find-str--typenparray-in_img_to_search-str--typenparray-confidence-float--08)
 
 
 ### screeny.take_screenshot(rect: QRect = None)
 
 Takes a screenshot of the complete monitor or a given area as "rect".
 Returns the image as a numpy-array.
```

### Comparing `screeny-0.2.0/README.md` & `screeny-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 img = sc.take_screenshot()
 ```
 
 ## API-Reference
 
 * [screeny.take_screenshot](#screenytake_screenshotrect-qrect--none)
 * [screeny.get_mouse_pos](#screenyget_mouse_pos)
-* [screeny.locate_image_on_screen](#screenylocate_image_on_screen)
-* [screeny.locate_image_in_image](#screenylocate_image_in_image)
+* [screeny.locate_image_on_screen](#screenylocate_image_on_screenimage-str--typenparray-rect-qrect--none-confidence-float--08)
+* [screeny.locate_image_in_image](#locate_image_in_imageimg_to_find-str--typenparray-in_img_to_search-str--typenparray-confidence-float--08)
 
 
 ### screeny.take_screenshot(rect: QRect = None)
 
 Takes a screenshot of the complete monitor or a given area as "rect".
 Returns the image as a numpy-array.
 
@@ -37,8 +37,8 @@
 
 Search for an image on the screen.
 Returns the location of the found image in pixel or False, if no image was found.
 
 ### locate_image_in_image(img_to_find: str | type[np.array], in_img_to_search: str | type[np.array], confidence: float = 0.8)
 
 Search for an image in another image and returns the location of the found image in pixels.
-Returns False, if no image was found.
+Returns False, if no image was found.
```

### Comparing `screeny-0.2.0/screeny/screeny.py` & `screeny-0.2.1/screeny/screeny.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,22 @@
 
     def __init__(self):
         """
         Initializing variables of the class.
         """
         self.mss = m.mss()
         self.mss_monitor = self.mss.monitors[1]
-        self.q_screen = QGuiApplication().primaryScreen()
+
+        # Because QGuiApplication is a singleton, it needs to be checked if already an instance exists of it.
+        # Otherwise, it'll lead to a runtime error, if multiple instances of the screeny class will be created.
+        if isinstance(QGuiApplication, type(None)):
+            self.q_screen = QGuiApplication().primaryScreen()
+        else:
+            self.q_screen = QGuiApplication.primaryScreen()
+
         self.mouse = Mouse(self.q_screen)
 
     def locate_image_on_screen(
             self, image: str | type[np.array], rect: QRect = None, confidence: float = 0.8
     ) -> QPoint | bool:
         """
         Search for an image on the screen and returns the location of the found image in pixel or False, if no image was found.
```

### Comparing `screeny-0.2.0/screeny.egg-info/PKG-INFO` & `screeny-0.2.1/screeny.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -29,16 +29,16 @@
 img = sc.take_screenshot()
 ```
 
 ## API-Reference
 
 * [screeny.take_screenshot](#screenytake_screenshotrect-qrect--none)
 * [screeny.get_mouse_pos](#screenyget_mouse_pos)
-* [screeny.locate_image_on_screen](#screenylocate_image_on_screen)
-* [screeny.locate_image_in_image](#screenylocate_image_in_image)
+* [screeny.locate_image_on_screen](#screenylocate_image_on_screenimage-str--typenparray-rect-qrect--none-confidence-float--08)
+* [screeny.locate_image_in_image](#locate_image_in_imageimg_to_find-str--typenparray-in_img_to_search-str--typenparray-confidence-float--08)
 
 
 ### screeny.take_screenshot(rect: QRect = None)
 
 Takes a screenshot of the complete monitor or a given area as "rect".
 Returns the image as a numpy-array.
```

### Comparing `screeny-0.2.0/setup.cfg` & `screeny-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = screeny
-version = 0.2.0
+version = 0.2.1
 author = Paul Pol
 author_email = mail@paul-pol.de
 description = A simple python library for working with screens and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

