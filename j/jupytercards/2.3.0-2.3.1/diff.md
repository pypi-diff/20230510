# Comparing `tmp/jupytercards-2.3.0.tar.gz` & `tmp/jupytercards-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.3.0.tar", last modified: Wed May 10 09:01:01 2023, max compression
+gzip compressed data, was "jupytercards-2.3.1.tar", last modified: Wed May 10 09:34:03 2023, max compression
```

## Comparing `jupytercards-2.3.0.tar` & `jupytercards-2.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.0/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.0/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.0/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.0/README.md
--rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.0/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.0/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.0/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.0/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-05-10 09:00:17.769712 jupytercards-2.3.0/jupytercards/__init__.py
--rw-r--r--   0        0        0     7234 2023-05-10 08:51:00.227700 jupytercards-2.3.0/jupytercards/dynamic.py
--rw-r--r--   0        0        0    10099 2023-05-10 08:57:49.469577 jupytercards-2.3.0/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-04-05 19:40:51.851785 jupytercards-2.3.0/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.0/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.1/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.1/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.1/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.1/README.md
+-rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.1/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.1/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.1/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.1/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-10 09:33:49.484437 jupytercards-2.3.1/jupytercards/__init__.py
+-rw-r--r--   0        0        0     7600 2023-05-10 09:28:41.207510 jupytercards-2.3.1/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10280 2023-05-10 09:30:15.686000 jupytercards-2.3.1/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-05-10 09:30:22.472298 jupytercards-2.3.1/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.1/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.1/PKG-INFO
```

### Comparing `jupytercards-2.3.0/.gitignore` & `jupytercards-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/LICENSE` & `jupytercards-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/Markdown-flashcards.ipynb` & `jupytercards-2.3.1/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/README.md` & `jupytercards-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/example.ipynb` & `jupytercards-2.3.1/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/extractdefinitions.py` & `jupytercards-2.3.1/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/flashcards.gif` & `jupytercards-2.3.1/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/jupytercards/__init__.py` & `jupytercards-2.3.1/jupytercards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.3.0/jupytercards/dynamic.py` & `jupytercards-2.3.1/jupytercards/dynamic.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import random
 import json
 import urllib.request
 import pkg_resources
 def display_flashcards(ref, keyControl = True, grabFocus=False,
                        front_colors=False,
                        back_colors=False,
+                       text_colors=False,
                        ):
 
     front_color_dict=[
         'var(--asparagus)',
         'var(--terra-cotta)',
         'var(--cyan-process)'
     ]
@@ -27,27 +28,36 @@
         'hsla(200,76.74%,83.14%, 1)'
     ]
 
     jupytercon_back = [
         'hsla(208.78,66.49%,36.27%,1)'
     ]
 
+    text_color_dict = [
+        'var(--snow)'
+    ]
+
 
     if front_colors:
         if type(front_colors) == list:
             front_color_dict = front_colors
         elif front_colors == 'jupytercon':
             front_color_dict = jupytercon_front
 
     if back_colors:
         if type(back_colors) == list:
             back_color_dict = back_colors
         elif back_colors == 'jupytercon':
             back_color_dict = jupytercon_back
 
+    if text_colors:
+        if type(text_colors) == list:
+            text_color_dict = text_colors
+
+
 
     resource_package = __name__
     styles = "<style>\n"
     css = pkg_resources.resource_string(resource_package, "styles.css")
     styles += css.decode("utf-8")
     styles += "\n</style>"
 
@@ -120,14 +130,20 @@
     loadData += f'"{front_color_dict[-1]}" ];\n'
 
     loadData += f"var backColors{div_id}= ["
     for color in back_color_dict[:-1]:
         loadData += f'"{color}", '
     loadData += f'"{back_color_dict[-1]}" ];\n'
 
+    loadData += f"var textColors{div_id}= ["
+    for color in text_color_dict[:-1]:
+        loadData += f'"{color}", '
+    loadData += f'"{text_color_dict[-1]}" ];\n'
+
+
 
     if static:
         loadData += f'''createCards("{div_id}", "{keyControl}", "{grabFocus}"); '''
 
         print()
     else:
         loadData += f'''
```

### Comparing `jupytercards-2.3.0/jupytercards/flashcards.js` & `jupytercards-2.3.1/jupytercards/flashcards.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -195,14 +195,15 @@
 
 }
 
 
 function createOneCard(mydiv, frontCard, cards, cardnum) {
     var colors = eval('frontColors' + mydiv.id);
     var backColors = eval('backColors' + mydiv.id);
+    var textColors = eval('textColors' + mydiv.id);
     //console.log(backColors)
 
     var flipper = document.createElement('div');
     if (frontCard) {
         flipper.className = "flipper frontcard";
     } else {
         flipper.className = "flipper backcard";
@@ -210,28 +211,30 @@
 
     var front = document.createElement('div');
     front.className = 'front flashcard';
 
     var frontSpan = document.createElement('span');
     frontSpan.className = 'flashcardtext';
     frontSpan.innerHTML = jaxify(cards[cardnum]['front']);
+    frontSpan.style.color = textColors[cardnum % textColors.length];
     //frontSpan.textContent=jaxify(cards[cardnum]['front']);
     //front.style.background='var(' + colors[cardnum % colors.length] + ')';
     front.style.background = colors[cardnum % colors.length];
 
     front.append(frontSpan);
     flipper.append(front);
 
     var back = document.createElement('div');
     back.className = 'back flashcard';
     back.style.background = backColors[cardnum % backColors.length];
 
     var backSpan = document.createElement('span');
     backSpan.className = 'flashcardtext';
     backSpan.innerHTML = jaxify(cards[cardnum]['back']);
+    backSpan.style.color = textColors[cardnum % textColors.length];
     back.append(backSpan);
 
     flipper.append(back);
 
     return flipper;
 
 }
```

### Comparing `jupytercards-2.3.0/jupytercards/styles.css` & `jupytercards-2.3.1/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/jupytercards/swiped-events.min.js` & `jupytercards-2.3.1/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.3.0/PKG-INFO` & `jupytercards-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.3.0
+Version: 2.3.1
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

