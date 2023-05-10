# Comparing `tmp/jupytercards-2.2.0.tar.gz` & `tmp/jupytercards-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupytercards-2.2.0.tar", last modified: Thu Apr 20 17:27:01 2023, max compression
+gzip compressed data, was "jupytercards-2.3.0.tar", last modified: Wed May 10 09:01:01 2023, max compression
```

## Comparing `jupytercards-2.2.0.tar` & `jupytercards-2.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.2.0/LICENSE
--rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.2.0/Markdown-flashcards.ipynb
--rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.2.0/README.md
--rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.2.0/example.ipynb
--rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.2.0/extractdefinitions.py
--rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.2.0/flashcards.gif
--rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.2.0/google73e9274d2fa18926.html
--rw-r--r--   0        0        0      657 2023-04-20 17:26:35.018537 jupytercards-2.2.0/jupytercards/__init__.py
--rw-r--r--   0        0        0     6042 2023-04-20 15:22:14.070372 jupytercards-2.2.0/jupytercards/dynamic.py
--rw-r--r--   0        0        0     9930 2023-04-20 17:13:57.229194 jupytercards-2.2.0/jupytercards/flashcards.js
--rw-r--r--   0        0        0     4217 2023-04-05 19:40:51.851785 jupytercards-2.2.0/jupytercards/styles.css
--rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.2.0/jupytercards/swiped-events.min.js
--rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1864 2022-08-26 19:15:29.921371 jupytercards-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2021-09-14 18:56:01.964070 jupytercards-2.3.0/LICENSE
+-rw-r--r--   0        0        0    26557 2022-03-17 14:56:01.735887 jupytercards-2.3.0/Markdown-flashcards.ipynb
+-rw-r--r--   0        0        0     3763 2022-11-18 02:28:35.734112 jupytercards-2.3.0/README.md
+-rw-r--r--   0        0        0    23266 2022-09-09 14:44:12.606945 jupytercards-2.3.0/example.ipynb
+-rwxr-xr-x   0        0        0     2692 2022-08-26 19:15:29.926367 jupytercards-2.3.0/extractdefinitions.py
+-rw-r--r--   0        0        0   898798 2021-09-14 19:02:50.323268 jupytercards-2.3.0/flashcards.gif
+-rw-r--r--   0        0        0       53 2021-09-20 15:24:49.422385 jupytercards-2.3.0/google73e9274d2fa18926.html
+-rw-r--r--   0        0        0      657 2023-05-10 09:00:17.769712 jupytercards-2.3.0/jupytercards/__init__.py
+-rw-r--r--   0        0        0     7234 2023-05-10 08:51:00.227700 jupytercards-2.3.0/jupytercards/dynamic.py
+-rw-r--r--   0        0        0    10099 2023-05-10 08:57:49.469577 jupytercards-2.3.0/jupytercards/flashcards.js
+-rw-r--r--   0        0        0     4217 2023-04-05 19:40:51.851785 jupytercards-2.3.0/jupytercards/styles.css
+-rw-r--r--   0        0        0     1769 2021-09-21 15:24:17.224804 jupytercards-2.3.0/jupytercards/swiped-events.min.js
+-rw-r--r--   0        0        0      330 2021-09-14 16:52:01.000000 jupytercards-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 jupytercards-2.3.0/PKG-INFO
```

### Comparing `jupytercards-2.2.0/.gitignore` & `jupytercards-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/LICENSE` & `jupytercards-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/Markdown-flashcards.ipynb` & `jupytercards-2.3.0/Markdown-flashcards.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/README.md` & `jupytercards-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/example.ipynb` & `jupytercards-2.3.0/example.ipynb`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/extractdefinitions.py` & `jupytercards-2.3.0/extractdefinitions.py`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/flashcards.gif` & `jupytercards-2.3.0/flashcards.gif`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/jupytercards/__init__.py` & `jupytercards-2.3.0/jupytercards/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.2.0'
+__version__ = '2.3.0'
 from .dynamic import display_flashcards, md2json
```

### Comparing `jupytercards-2.2.0/jupytercards/dynamic.py` & `jupytercards-2.3.0/jupytercards/dynamic.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,52 @@
 
 from IPython.core.display import display,  HTML, Javascript
 import string
 import random
 import json
 import urllib.request
 import pkg_resources
+def display_flashcards(ref, keyControl = True, grabFocus=False,
+                       front_colors=False,
+                       back_colors=False,
+                       ):
+
+    front_color_dict=[
+        'var(--asparagus)',
+        'var(--terra-cotta)',
+        'var(--cyan-process)'
+    ]
+
+    back_color_dict = [
+        'var(--dark-blue-gray)'
+        ]
+
+    jupytercon_front = [
+        'hsla(17.65,100%,50%,1)',
+        'rgb(234,196,53)',
+        'hsla(200,76.74%,83.14%, 1)'
+    ]
+
+    jupytercon_back = [
+        'hsla(208.78,66.49%,36.27%,1)'
+    ]
+
+
+    if front_colors:
+        if type(front_colors) == list:
+            front_color_dict = front_colors
+        elif front_colors == 'jupytercon':
+            front_color_dict = jupytercon_front
+
+    if back_colors:
+        if type(back_colors) == list:
+            back_color_dict = back_colors
+        elif back_colors == 'jupytercon':
+            back_color_dict = jupytercon_back
 
-def display_flashcards(ref, keyControl = True, grabFocus=False):
 
     resource_package = __name__
     styles = "<style>\n"
     css = pkg_resources.resource_string(resource_package, "styles.css")
     styles += css.decode("utf-8")
     styles += "\n</style>"
 
@@ -44,15 +80,15 @@
 
     # Next button will go here
     nextbutton=f"""<div class="next" id="{div_id}-next" onclick="window.checkFlip('{div_id}')"> </div> """
     
     #print(nextbutton)
     loadData = '\n'
 
-    loadData += "var cards"+div_id+"="
+    loadData += f"var cards{div_id}="
 
     if type(ref) == list:
         #print("List detected. Assuming JSON")
         loadData += json.dumps(ref)
         static = True
         url = ""
     elif type(ref) == str:
@@ -72,21 +108,29 @@
                 for line in file:
                     loadData += line
             static = True
             url = ""
     else:
         raise Exception("First argument must be list (JSON), URL, or file ref")
 
-    loadData += ''';
-    '''
-    
+    loadData += ';\n'
+
+    loadData += f"var frontColors{div_id}= ["
+    for color in front_color_dict[:-1]:
+        loadData += f'"{color}", '
+    loadData += f'"{front_color_dict[-1]}" ];\n'
+
+    loadData += f"var backColors{div_id}= ["
+    for color in back_color_dict[:-1]:
+        loadData += f'"{color}", '
+    loadData += f'"{back_color_dict[-1]}" ];\n'
+
+
     if static:
-        loadData += f'''
-        createCards("{div_id}", "{keyControl}", "{grabFocus}");
-        '''
+        loadData += f'''createCards("{div_id}", "{keyControl}", "{grabFocus}"); '''
 
         print()
     else:
         loadData += f'''
 
         {{
         const jmscontroller = new AbortController();
```

### Comparing `jupytercards-2.2.0/jupytercards/flashcards.js` & `jupytercards-2.3.0/jupytercards/flashcards.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 function jaxify(string) {
     var mystring = string;
-    console.log(mystring);
+    //console.log(mystring);
 
     var count = 0;
     var loc = mystring.search(/([^\\]|^)(\$)/);
 
     var count2 = 0;
     var loc2 = mystring.search(/([^\\]|^)(\$\$)/);
 
@@ -34,32 +34,32 @@
     }
 
     //console.log(mystring);
     return mystring;
 }
 
 window.flipCard = function flipCard(ths) {
-    console.log(ths);
-    console.log(ths.id);
+    //console.log(ths);
+    //console.log(ths.id);
     ths.classList.toggle("flip");
     ths.focus();
     var next = document.getElementById(ths.id + '-next');
     next.style.pointerEvents = 'none';
     /* ths.blur(); */
     next.classList.add('flipped');
     if (typeof MathJax != 'undefined') {
         var version = MathJax.version;
-        console.log('MathJax version', version);
+        //console.log('MathJax version', version);
         if (version[0] == "2") {
             MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
         } else if (version[0] == "3") {
             MathJax.typeset([ths]);
         }
     } else {
-        console.log('MathJax not detected');
+        //console.log('MathJax not detected');
     }
 
 
     setTimeout(reenableNext, 600, ths, next);
 }
 
 window.checkKey = function checkKey(container, event) {
@@ -147,37 +147,37 @@
     if (cardnum != 1) {
         next.innerHTML = "Next >";
     } else {
         //next.innerHTML="Reload \\(\\circlearrowleft\\) ";
         next.innerHTML = 'Reload <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewbox="0 0 25 26"> <path d="M7,6a10,10,0,1,0,9,0" style="fill:none;stroke:black;stroke-width:2px" id="e2_circleArc"/> <line id="e3_line" x1="17" y1="6.5" x2="17.5" y2="15" style="stroke:black;fill:none;stroke-width:2px"/> <line id="e4_line" x1="16.5" y1="6.5" x2="26" y2="8" style="stroke:black;fill:none;stroke-width:2px"/> </svg> '
         if (typeof MathJax != 'undefined') {
             var version = MathJax.version;
-            console.log('MathJax version', version);
+            //console.log('MathJax version', version);
             if (version[0] == "2") {
                 MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
             } else if (version[0] == "3") {
                 MathJax.typeset([next]);
             }
         } else {
-            console.log('MathJax not detected');
+            //console.log('MathJax not detected');
         }
 
 
     }
 
     if (typeof MathJax != 'undefined') {
         var version = MathJax.version;
-        console.log('MathJax version', version);
+        //console.log('MathJax version', version);
         if (version[0] == "2") {
             MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
         } else if (version[0] == "3") {
             MathJax.typeset();
         }
     } else {
-        console.log('MathJax not detected');
+        //console.log('MathJax not detected');
     }
 
 
     next.style.pointerEvents = 'auto';
     container.style.pointerEvents = 'auto';
     /* container.tabIndex= 0; */
     /* container.focus(); */
@@ -193,19 +193,17 @@
     });
 
 
 }
 
 
 function createOneCard(mydiv, frontCard, cards, cardnum) {
-    var colors = [
-        '--asparagus',
-        '--terra-cotta',
-        '--cyan-process'
-    ]
+    var colors = eval('frontColors' + mydiv.id);
+    var backColors = eval('backColors' + mydiv.id);
+    //console.log(backColors)
 
     var flipper = document.createElement('div');
     if (frontCard) {
         flipper.className = "flipper frontcard";
     } else {
         flipper.className = "flipper backcard";
     }
@@ -213,22 +211,23 @@
     var front = document.createElement('div');
     front.className = 'front flashcard';
 
     var frontSpan = document.createElement('span');
     frontSpan.className = 'flashcardtext';
     frontSpan.innerHTML = jaxify(cards[cardnum]['front']);
     //frontSpan.textContent=jaxify(cards[cardnum]['front']);
-    front.style.background = 'var(' + colors[cardnum % colors.length] + ')';
-
+    //front.style.background='var(' + colors[cardnum % colors.length] + ')';
+    front.style.background = colors[cardnum % colors.length];
 
     front.append(frontSpan);
     flipper.append(front);
 
     var back = document.createElement('div');
     back.className = 'back flashcard';
+    back.style.background = backColors[cardnum % backColors.length];
 
     var backSpan = document.createElement('span');
     backSpan.className = 'flashcardtext';
     backSpan.innerHTML = jaxify(cards[cardnum]['back']);
     back.append(backSpan);
 
     flipper.append(back);
@@ -249,24 +248,24 @@
     /*
     mydiv.addEventListener('click', function(){window.flipCard(mydiv);}, false);
     mydiv.addEventListener('keydown', function(event){window.checkKey(mydiv,event);}, true);
     */
     mydiv.onclick = function() {
         window.flipCard(mydiv);
     };
-    console.log(keyControl);
+    //console.log(keyControl);
     if (keyControl == "True") {
         mydiv.onkeydown = function(event) {
             window.checkKey(mydiv, event);
         };
     }
     /* mydiv.addEventListener('keydown', function(event){event.stopPropagation(); console.log(event); event.preventDefault();}, true); */
     /*mydiv.onkeypress = function(event){console.log(event); event.preventDefault();};*/
 
-    console.log(mydiv);
+    //console.log(mydiv);
 
     var cards = eval('cards' + id);
     mydiv.dataset.cardnum = 0;
     mydiv.dataset.numCards = cards.length;
     mydiv.addEventListener('swiped-left', function(e) {
         /*
           console.log(e.detail);
```

### Comparing `jupytercards-2.2.0/jupytercards/styles.css` & `jupytercards-2.3.0/jupytercards/styles.css`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/jupytercards/swiped-events.min.js` & `jupytercards-2.3.0/jupytercards/swiped-events.min.js`

 * *Files identical despite different names*

### Comparing `jupytercards-2.2.0/PKG-INFO` & `jupytercards-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercards
-Version: 2.2.0
+Version: 2.3.0
 Summary: Module to display dynamic quizzes in Jupyter notebooks and Jupyter Books. Uses JavaScript to provide
 Home-page: https://github.com/jmshea/jupytercards
 Author: John M. Shea
 Author-email: jshea@ieee.org
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

