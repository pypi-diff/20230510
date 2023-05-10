# Comparing `tmp/st_text_annotator-0.3.0.tar.gz` & `tmp/st_text_annotator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.3.0.tar", max compression
+gzip compressed data, was "st_text_annotator-0.3.1.tar", max compression
```

## Comparing `st_text_annotator-0.3.0.tar` & `st_text_annotator-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.3.0/LICENSE
--rw-r--r--   0        0        0     1951 2023-04-17 19:03:03.350393 st_text_annotator-0.3.0/README.md
--rw-r--r--   0        0        0      708 2023-05-07 22:19:59.569860 st_text_annotator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2762 2023-05-07 22:17:50.205705 st_text_annotator-0.3.0/src/st_text_annotator/__init__.py
--rw-r--r--   0        0        0      180 2023-04-18 15:31:27.032026 st_text_annotator-0.3.0/src/st_text_annotator/frontend/.env
--rw-r--r--   0        0        0       67 2023-04-18 15:31:27.033065 st_text_annotator-0.3.0/src/st_text_annotator/frontend/.prettierrc
--rw-r--r--   0        0        0      691 2023-05-07 22:22:35.760404 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2099 2023-05-07 22:22:35.760279 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/index.html
--rw-r--r--   0        0        0   489818 2023-05-07 22:22:35.770008 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js
--rw-r--r--   0        0        0     2280 2023-05-07 22:22:35.770468 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  1785435 2023-05-07 22:22:35.769132 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map
--rw-r--r--   0        0        0     7729 2023-05-07 22:22:35.768603 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/main.5de43153.chunk.js
--rw-r--r--   0        0        0    18961 2023-05-07 22:22:35.768644 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/main.5de43153.chunk.js.map
--rw-r--r--   0        0        0     1594 2023-05-07 22:22:35.761358 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js
--rw-r--r--   0        0        0     8373 2023-05-07 22:22:35.769595 st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map
--rw-r--r--   0        0        0      848 2023-05-07 22:21:25.699902 st_text_annotator-0.3.0/src/st_text_annotator/frontend/package.json
--rw-r--r--   0        0        0      895 2023-04-18 15:45:04.080620 st_text_annotator-0.3.0/src/st_text_annotator/frontend/public/index.html
--rw-r--r--   0        0        0     8946 2023-05-07 22:16:15.891756 st_text_annotator-0.3.0/src/st_text_annotator/frontend/src/Annotation.tsx
--rw-r--r--   0        0        0      229 2023-04-18 18:13:03.689669 st_text_annotator-0.3.0/src/st_text_annotator/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-18 15:31:27.070284 st_text_annotator-0.3.0/src/st_text_annotator/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      531 2023-04-18 15:43:10.838552 st_text_annotator-0.3.0/src/st_text_annotator/frontend/tsconfig.json
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 st_text_annotator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1951 2023-04-17 19:03:03.350393 st_text_annotator-0.3.1/README.md
+-rw-r--r--   0        0        0      708 2023-05-10 07:41:40.158341 st_text_annotator-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2791 2023-05-10 07:41:47.299730 st_text_annotator-0.3.1/src/st_text_annotator/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-18 15:31:27.032026 st_text_annotator-0.3.1/src/st_text_annotator/frontend/.env
+-rw-r--r--   0        0        0       67 2023-04-18 15:31:27.033065 st_text_annotator-0.3.1/src/st_text_annotator/frontend/.prettierrc
+-rw-r--r--   0        0        0      691 2023-05-10 07:46:07.482983 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2099 2023-05-10 07:46:07.482861 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/index.html
+-rw-r--r--   0        0        0   489818 2023-05-10 07:46:07.488310 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js
+-rw-r--r--   0        0        0     2280 2023-05-10 07:46:07.489092 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1785435 2023-05-10 07:46:07.488861 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map
+-rw-r--r--   0        0        0     7780 2023-05-10 07:46:07.484666 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js
+-rw-r--r--   0        0        0    19645 2023-05-10 07:46:07.489824 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map
+-rw-r--r--   0        0        0     1594 2023-05-10 07:46:07.489935 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js
+-rw-r--r--   0        0        0     8373 2023-05-10 07:46:07.488921 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map
+-rw-r--r--   0        0        0  1579776 2023-05-10 07:45:44.860303 st_text_annotator-0.3.1/src/st_text_annotator/frontend/package-lock.json
+-rw-r--r--   0        0        0      848 2023-05-10 07:41:49.071479 st_text_annotator-0.3.1/src/st_text_annotator/frontend/package.json
+-rw-r--r--   0        0        0      895 2023-04-18 15:45:04.080620 st_text_annotator-0.3.1/src/st_text_annotator/frontend/public/index.html
+-rw-r--r--   0        0        0     9382 2023-05-10 07:35:55.735595 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/Annotation.tsx
+-rw-r--r--   0        0        0      229 2023-04-18 18:13:03.689669 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-18 15:31:27.070284 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      531 2023-04-18 15:43:10.838552 st_text_annotator-0.3.1/src/st_text_annotator/frontend/tsconfig.json
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 st_text_annotator-0.3.1/PKG-INFO
```

### Comparing `st_text_annotator-0.3.0/LICENSE` & `st_text_annotator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/README.md` & `st_text_annotator-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/pyproject.toml` & `st_text_annotator-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-text-annotator"
-version = "0.3.0"
+version = "0.3.1"
 description = "Component for annotating text for NLP resolution"
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 authors = ["Robin Marquet <robin.marquet@epitech.eu>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["streamlit", "text", "annotation", "nlp"]
 include = ["./src/st_text_annotator/frontend/build/**/*"]
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/__init__.py` & `st_text_annotator-0.3.1/src/st_text_annotator/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import streamlit.components.v1 as components
 
-RELEASE = True
+RELEASE = False
 
 if not RELEASE:
     _component_func = components.declare_component("st_text_annotator", url="http://localhost:3001")
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("StTextAnnotator", path=build_dir)
@@ -72,15 +72,15 @@
 if __name__ == "__main__":
     # This is an example of how to use the component in a Streamlit app.
     # It's not required for the component to work.
     import streamlit as st
 
     st.title("StTextAnnotator")
 
-    text = "Lorem ipsum dolor sit et amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua"
+    text = "Lorem ipsum dolor sit et amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua, Apple Inc. is good company"
 
     annotations = [
       [
         { "start": 0, "end": 5, "label": "Lorem" },
         { "start": 12, "end": 17, "label": "dolor" },
       ],
       [
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/asset-manifest.json` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/asset-manifest.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.4ce3c4a6.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.4ce3c4a6.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.4ce3c4a6.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.6ab9b2fc.js",
         "static/js/2.d11c6839.chunk.js",
-        "static/js/main.5de43153.chunk.js"
+        "static/js/main.4ce3c4a6.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.5de43153.chunk.js",
-        "main.js.map": "./static/js/main.5de43153.chunk.js.map",
+        "main.js": "./static/js/main.4ce3c4a6.chunk.js",
+        "main.js.map": "./static/js/main.4ce3c4a6.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.6ab9b2fc.js",
         "runtime-main.js.map": "./static/js/runtime-main.6ab9b2fc.js.map",
         "static/js/2.d11c6839.chunk.js": "./static/js/2.d11c6839.chunk.js",
         "static/js/2.d11c6839.chunk.js.LICENSE.txt": "./static/js/2.d11c6839.chunk.js.LICENSE.txt",
         "static/js/2.d11c6839.chunk.js.map": "./static/js/2.d11c6839.chunk.js.map"
     }
 }
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/index.html` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><script src="https://cdn.tailwindcss.com"></script></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(t){function e(e){for(var n,a,l=e[0],i=e[1],f=e[2],c=0,s=[];c<l.length;c++)a=l[c],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&s.push(o[a][0]),o[a]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(t[n]=i[n]);for(p&&p(e);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var t,e=0;e<u.length;e++){for(var r=u[e],n=!0,l=1;l<r.length;l++){var i=r[l];0!==o[i]&&(n=!1)}n&&(u.splice(e--,1),t=a(a.s=r[0]))}return t}var n={},o={1:0},u=[];function a(e){if(n[e])return n[e].exports;var r=n[e]={i:e,l:!1,exports:{}};return t[e].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.m=t,a.c=n,a.d=function(t,e,r){a.o(t,e)||Object.defineProperty(t,e,{enumerable:!0,get:r})},a.r=function(t){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(t,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(t,"__esModule",{value:!0})},a.t=function(t,e){if(1&e&&(t=a(t)),8&e)return t;if(4&e&&"object"==typeof t&&t&&t.__esModule)return t;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:t}),2&e&&"string"!=typeof t)for(var n in t)a.d(r,n,function(e){return t[e]}.bind(null,n));return r},a.n=function(t){var e=t&&t.__esModule?function(){return t.default}:function(){return t};return a.d(e,"a",e),e},a.o=function(t,e){return Object.prototype.hasOwnProperty.call(t,e)},a.p="./";var l=this["webpackJsonpsteamlit-text-annotator"]=this["webpackJsonpsteamlit-text-annotator"]||[],i=l.push.bind(l);l.push=e,l=l.slice();for(var f=0;f<l.length;f++)e(l[f]);var p=i;r()}([])</script><script src="./static/js/2.d11c6839.chunk.js"></script><script src="./static/js/main.5de43153.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><script src="https://cdn.tailwindcss.com"></script></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(t){function e(e){for(var n,a,l=e[0],i=e[1],f=e[2],c=0,s=[];c<l.length;c++)a=l[c],Object.prototype.hasOwnProperty.call(o,a)&&o[a]&&s.push(o[a][0]),o[a]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(t[n]=i[n]);for(p&&p(e);s.length;)s.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var t,e=0;e<u.length;e++){for(var r=u[e],n=!0,l=1;l<r.length;l++){var i=r[l];0!==o[i]&&(n=!1)}n&&(u.splice(e--,1),t=a(a.s=r[0]))}return t}var n={},o={1:0},u=[];function a(e){if(n[e])return n[e].exports;var r=n[e]={i:e,l:!1,exports:{}};return t[e].call(r.exports,r,r.exports,a),r.l=!0,r.exports}a.m=t,a.c=n,a.d=function(t,e,r){a.o(t,e)||Object.defineProperty(t,e,{enumerable:!0,get:r})},a.r=function(t){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(t,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(t,"__esModule",{value:!0})},a.t=function(t,e){if(1&e&&(t=a(t)),8&e)return t;if(4&e&&"object"==typeof t&&t&&t.__esModule)return t;var r=Object.create(null);if(a.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:t}),2&e&&"string"!=typeof t)for(var n in t)a.d(r,n,function(e){return t[e]}.bind(null,n));return r},a.n=function(t){var e=t&&t.__esModule?function(){return t.default}:function(){return t};return a.d(e,"a",e),e},a.o=function(t,e){return Object.prototype.hasOwnProperty.call(t,e)},a.p="./";var l=this["webpackJsonpsteamlit-text-annotator"]=this["webpackJsonpsteamlit-text-annotator"]||[],i=l.push.bind(l);l.push=e,l=l.slice();for(var f=0;f<l.length;f++)e(l[f]);var p=i;r()}([])</script><script src="./static/js/2.d11c6839.chunk.js"></script><script src="./static/js/main.4ce3c4a6.chunk.js"></script></body></html>
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/main.5de43153.chunk.js` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -29,76 +29,77 @@
                             for (var n = document.createTreeWalker(t || document.body, NodeFilter.SHOW_TEXT, null), a = 0; n.nextNode();) {
                                 var r;
                                 if (n.currentNode === e) break;
                                 a += (null === (r = n.currentNode.textContent) || void 0 === r ? void 0 : r.length) || 0
                             }
                             return a
                         }, e.handleMouseUp = Object(s.a)(Object(r.a)().mark((function t() {
-                            var n, a, s, c, o, i, u, d, f, x, h, v, b, p, m, j, g, O, y, k, w, C, S, R, A, N, T;
+                            var n, a, s, c, o, i, u, d, f, x, h, v, b, p, m, j, g, O, y, k, w, C, S, R, A, N, T, _, q, M, U;
                             return Object(r.a)().wrap((function(t) {
                                 for (;;) switch (t.prev = t.next) {
                                     case 0:
                                         if (!(a = null === (n = document.getSelection()) || void 0 === n ? void 0 : n.getRangeAt(0)) || "" === a.toString().trim()) {
-                                            t.next = 37;
+                                            t.next = 40;
                                             break
                                         }
-                                        o = a.toString(), i = a.startOffset, u = a.endOffset, d = document.getElementById("actual-text"), f = e.getCharactersCountUntilNode(a.startContainer, d), x = e.getCharactersCountUntilNode(a.endContainer, d), i += f, u += x;
-                                    case 10:
-                                        if (" " === (null === (h = document.querySelector("#actual-text")) || void 0 === h || null === (v = h.textContent) || void 0 === v ? void 0 : v.charAt(i - 1)) || void 0 === (null === (b = document.querySelector("#actual-text")) || void 0 === b || null === (p = b.textContent) || void 0 === p ? void 0 : p.charAt(i - 1))) {
-                                            t.next = 16;
+                                        o = a.toString(), i = a.startOffset, u = a.endOffset, d = 0, f = 0, x = document.getElementById("actual-text"), h = e.getCharactersCountUntilNode(a.startContainer, x), v = e.getCharactersCountUntilNode(a.endContainer, x), i += h, u += v;
+                                    case 12:
+                                        if (" " === (null === (b = document.querySelector("#actual-text")) || void 0 === b || null === (p = b.textContent) || void 0 === p ? void 0 : p.charAt(i + d - 1)) || void 0 === (null === (m = document.querySelector("#actual-text")) || void 0 === m || null === (j = m.textContent) || void 0 === j ? void 0 : j.charAt(i + d - 1))) {
+                                            t.next = 18;
                                             break
                                         }
-                                        if ("" !== (null === (m = document.querySelector("#actual-text")) || void 0 === m || null === (j = m.textContent) || void 0 === j ? void 0 : j.charAt(i - 1))) {
-                                            t.next = 13;
+                                        if ("" !== (null === (g = document.querySelector("#actual-text")) || void 0 === g || null === (O = g.textContent) || void 0 === O ? void 0 : O.charAt(i + d - 1))) {
+                                            t.next = 15;
                                             break
                                         }
-                                        return t.abrupt("break", 16);
-                                    case 13:
-                                        i -= 1, t.next = 10;
+                                        return t.abrupt("break", 18);
+                                    case 15:
+                                        d -= 1, t.next = 12;
                                         break;
-                                    case 16:
-                                        if (" " === (null === (g = document.querySelector("#actual-text")) || void 0 === g || null === (O = g.textContent) || void 0 === O ? void 0 : O.charAt(u)) || void 0 === (null === (y = document.querySelector("#actual-text")) || void 0 === y || null === (k = y.textContent) || void 0 === k ? void 0 : k.charAt(u))) {
-                                            t.next = 22;
+                                    case 18:
+                                        if (" " === (null === (y = document.querySelector("#actual-text")) || void 0 === y || null === (k = y.textContent) || void 0 === k ? void 0 : k.charAt(u + f)) || void 0 === (null === (w = document.querySelector("#actual-text")) || void 0 === w || null === (C = w.textContent) || void 0 === C ? void 0 : C.charAt(u + f))) {
+                                            t.next = 24;
                                             break
                                         }
-                                        if ("" !== (null === (w = document.querySelector("#actual-text")) || void 0 === w || null === (C = w.textContent) || void 0 === C ? void 0 : C.charAt(u))) {
-                                            t.next = 19;
+                                        if ("" !== (null === (S = document.querySelector("#actual-text")) || void 0 === S || null === (R = S.textContent) || void 0 === R ? void 0 : R.charAt(u + f))) {
+                                            t.next = 21;
                                             break
                                         }
-                                        return t.abrupt("break", 22);
-                                    case 19:
-                                        u += 1, t.next = 16;
+                                        return t.abrupt("break", 24);
+                                    case 21:
+                                        f += 1, t.next = 18;
                                         break;
-                                    case 22:
-                                        for (o = (null === (s = document.querySelector("#actual-text")) || void 0 === s || null === (c = s.textContent) || void 0 === c ? void 0 : c.slice(i, u)) || "", S = /[.,/#!$%^&*;:{}=\-_`~()]$/g; o.match(S);) o = o.slice(0, -1), u -= 1;
-                                        if (R = e.state, A = R.annotations, N = R.selectedReference, A[N] || (A[N] = []), !e.isAnnotated(i, u)) {
-                                            t.next = 33;
+                                    case 24:
+                                        if (o = (null === (s = document.querySelector("#actual-text")) || void 0 === s || null === (c = s.textContent) || void 0 === c ? void 0 : c.slice(i + d, u + f)) || "", f > 0)
+                                            for (A = /[.,/#!$%^&*;:{}=\-_`~()]$/g; o.match(A);) o = o.slice(0, -1), f -= 1;
+                                        if (N = e.state, T = N.annotations, _ = N.selectedReference, T[_] || (T[_] = []), q = i + d, M = u + f, !e.isAnnotated(q, M)) {
+                                            t.next = 36;
                                             break
                                         }
-                                        return T = e.removeAnnotation(i, u), t.next = 31, e.setState({
-                                            annotations: T
+                                        return U = e.removeAnnotation(q, M), t.next = 34, e.setState({
+                                            annotations: U
                                         });
-                                    case 31:
-                                        t.next = 36;
+                                    case 34:
+                                        t.next = 39;
                                         break;
-                                    case 33:
-                                        return A[N].push({
-                                            start: i,
-                                            end: u,
+                                    case 36:
+                                        return T[_].push({
+                                            start: q,
+                                            end: M,
                                             label: o
-                                        }), t.next = 36, e.setState({
-                                            annotations: A
+                                        }), t.next = 39, e.setState({
+                                            annotations: T
                                         });
-                                    case 36:
-                                        l.a.setComponentValue(A);
-                                    case 37:
+                                    case 39:
+                                        l.a.setComponentValue(T);
+                                    case 40:
                                         e.setState({
                                             actual_text: e.renderText()
                                         });
-                                    case 38:
+                                    case 41:
                                     case "end":
                                         return t.stop()
                                 }
                             }), t)
                         }))), e
                     }
                     return Object(o.a)(n, [{
@@ -314,8 +315,8 @@
             Object(a.createRoot)(h).render(Object(d.jsx)(x, {}))
         }
     },
     [
         [33, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.5de43153.chunk.js.map
+//# sourceMappingURL=main.4ce3c4a6.chunk.js.map
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/main.5de43153.chunk.js.map` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8076804915514594%*

 * *Differences: {"'file'": "'static/js/main.4ce3c4a6.chunk.js'",*

 * * "'mappings'": "'6NAoBMA,EAAU,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GAAA,SAAAA,IAAA,IAAAK,EAAAC,YAAA,KAAAN,GAAA,QAAAO,EAAAC,UAAAC,OAAAC,EAAA,IAAAC,MAAAJ,GAAAK,EAAA,EAAAA,EAAAL,EAAAK,IAAAF,EAAAE,GAAAJ,UAAAI,GA8Ib,OA9IaP,EAAAF,EAAAU,KAAAC,MAAAX,EAAA,OAAAY,OAAAL,KACdM,MAAe,CACbC,KAAM,GACNC,YAAa,GACbC,YAAa,GACbC,kBAAmB,GACpBf,EAoDDgB,4BAA8B,SAACC,EAAYC,GAQzC,IAPA,IAAMC,EAASC,SAASC,iBACtBH,GAAUE,SAASE,KACnBC,WAAWC,UACX,MAGEC,EAAY,EACTN,EAAOO,YAAY,CAAC,IAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.5de43153.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.4ce3c4a6.chunk.js",
+    "mappings": "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",
     "names": [
         "Annotation",
         "_StreamlitComponentBa",
         "_inherits",
         "_super",
         "_createSuper",
         "_this",
@@ -45,14 +45,16 @@
         "_document$getSelectio",
         "selection",
         "_document$querySelect13",
         "_document$querySelect14",
         "selectedText",
         "startIndex",
         "endIndex",
+        "startAdjustment",
+        "endAdjustment",
         "container",
         "charsBeforeStart",
         "charsBeforeEnd",
         "_document$querySelect",
         "_document$querySelect2",
         "_document$querySelect3",
         "_document$querySelect4",
@@ -62,14 +64,16 @@
         "_document$querySelect8",
         "_document$querySelect9",
         "_document$querySelect10",
         "_document$querySelect11",
         "_document$querySelect12",
         "re",
         "_this$state",
+        "finalStartIndex",
+        "finalEndIndex",
         "newAnnotations",
         "wrap",
         "_context",
         "prev",
         "next",
         "getSelection",
         "getRangeAt",
@@ -156,12 +160,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "Annotation.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React from \"react\"\n\ninterface Reference {\n  start: number,\n  end: number,\n  label: string\n}\n\ninterface State {\n  text: string\n  actual_text: JSX.Element[]\n  selectedReference: number\n  annotations: Reference[][]\n}\n\nclass Annotation extends StreamlitComponentBase<State> {\n  state: State = {\n    text: \"\",\n    actual_text: [],\n    annotations: [],\n    selectedReference: 0\n  }\n\n  async componentDidMount(): Promise<void> {\n    const { text, annotations } = this.props.args\n\n    await this.setState({ text, annotations })\n    await this.setState({ actual_text: this.renderText() })\n    Streamlit.setComponentValue(annotations)\n  }\n\n  isAnnotated(start: number, end: number): boolean {\n    const { annotations, selectedReference } = this.state\n    \n    if (!annotations[selectedReference]) {\n      return false\n    }\n\n    for (let i = 0; i < annotations[selectedReference].length; i++) {\n      if (\n        (start >= annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end >= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end > annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start >= annotations[selectedReference][i].start && start < annotations[selectedReference][i].end && end >= annotations[selectedReference][i].end)\n        ) {\n        return true\n      }\n    }\n    return false\n  }\n\n  removeAnnotation(start: number, end: number): Reference[][] {\n    const { annotations, selectedReference } = this.state\n\n    for (let i = 0; i < annotations[selectedReference].length; i++) {\n      if (\n        (start >= annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end >= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end > annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start >= annotations[selectedReference][i].start && start < annotations[selectedReference][i].end && end >= annotations[selectedReference][i].end)\n        ) {\n        annotations[selectedReference].splice(i, 1)\n        break\n      }\n    }\n\n    if (annotations[selectedReference].length === 0) {\n      annotations.splice(selectedReference, 1)\n    }\n\n    return annotations\n  }\n\n  getCharactersCountUntilNode = (node: Node, parent: HTMLElement | null) => {\n    const walker = document.createTreeWalker(\n      parent || document.body,\n      NodeFilter.SHOW_TEXT,\n      null,\n    );\n    \n    let charCount = 0;\n    while (walker.nextNode()) {\n      if (walker.currentNode === node) {\n        break;\n      }\n      charCount += walker.currentNode.textContent?.length || 0;\n    }\n\n    return charCount;\n  }\n\n  handleMouseUp = async () => {\n    const selection = document.getSelection()?.getRangeAt(0)\n\n    if (selection && selection.toString().trim() !== \"\") {\n      let selectedText = selection.toString()\n\n      let startIndex = selection.startOffset\n      let endIndex = selection.endOffset\n\n      const container = document.getElementById(\"actual-text\")\n      const charsBeforeStart = this.getCharactersCountUntilNode(selection.startContainer, container);\n      const charsBeforeEnd = this.getCharactersCountUntilNode(selection.endContainer, container);\n\n      startIndex += charsBeforeStart\n      endIndex += charsBeforeEnd\n\n      while (document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex - 1) !== \" \" && document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex - 1) !== undefined) {\n        if (document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex - 1) === '') {\n          break\n        }\n\n        startIndex -= 1\n      }\n\n      while (document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex) !== \" \" && document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex) !== undefined) {\n        if (document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex) === '') {\n          break\n        }\n\n        endIndex += 1\n      }\n\n      selectedText = document.querySelector(\"#actual-text\")?.textContent?.slice(startIndex, endIndex) || \"\"\n\n      // remove commas, periods, etc. from the end of the selection\n      const re = /[.,/#!$%^&*;:{}=\\-_`~()]$/g\n      while (selectedText.match(re)) {\n        selectedText = selectedText.slice(0, -1)\n        endIndex -= 1\n      }\n\n      const { annotations, selectedReference } = this.state\n\n      if (!annotations[selectedReference]) {\n        annotations[selectedReference] = []\n      }\n\n      if (this.isAnnotated(startIndex, endIndex)) {\n        const newAnnotations = this.removeAnnotation(startIndex, endIndex)\n        await this.setState({ annotations: newAnnotations })\n      } else {\n        annotations[selectedReference].push({ start: startIndex, end: endIndex, label: selectedText })\n        await this.setState({ annotations })\n      }\n\n      Streamlit.setComponentValue(annotations)\n    }\n\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async addReference(): Promise<void> {\n    const { annotations } = this.state\n\n    // if selected annotation is empty do not add a new one\n    if (annotations[this.state.selectedReference] && annotations[this.state.selectedReference].length === 0) {\n      return\n    }\n\n    const index = annotations.length + 1\n    \n    if (!annotations[index]) {\n      annotations[index] = []\n    }\n\n    await this.setState({ \n      selectedReference: index,\n      annotations\n    })\n\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async selectReference(index: number): Promise<void> {\n    if (this.state.selectedReference === index || !this.state.annotations[index]) {\n      return\n    }\n\n    await this.setState({ selectedReference: index })\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async removeReference(index: number): Promise<void> {\n    const { annotations } = this.state\n\n    annotations.splice(index, 1)\n\n    await this.setState({ annotations, selectedReference: 0 })\n    this.setState({ actual_text: this.renderText() })\n    Streamlit.setComponentValue(annotations)\n  }\n\n  renderText(): JSX.Element[] {\n    const { text, annotations, selectedReference } = this.state\n    const actual_text: JSX.Element[] = []\n\n    if (!annotations[selectedReference]) {\n      return [<span>{text}</span>]\n    }\n\n\n    let start = 0\n\n    if (annotations[selectedReference].length > 0) {\n      annotations[selectedReference].sort((a, b) => a.start - b.start)\n    }\n\n    annotations[selectedReference].forEach((annotation, index) => {\n      actual_text.push(<span>{text.substring(start, annotation.start)}</span>)\n      actual_text.push(<span className=\"annotated bg-blue-500 text-gray-100\">{text.substring(annotation.start, annotation.end)}</span>)\n      start = annotation.end\n    })\n    actual_text.push(<span>{text.substring(start, text.length)}</span>)\n\n\n    return actual_text\n  }\n\n  render(): React.ReactNode {\n    return (\n      <div>\n        <div className=\"flex flex-row flex-wrap\">\n          <div\n            className=\"flex flex-wrap px-4 py-2 m-1 justify-between items-center text-sm font-medium cursor-pointer hover:bg-blue-600 hover:text-gray-100 bg-blue-500 text-gray-100\"\n            onClick={ () => this.addReference() }\n            >\n            <span>Add</span>\n          </div>\n          {this.state.annotations.map((reference, index) => (\n            <span\n              key={index}\n              className={\"flex flex-wrap pl-4 pr-2 py-2 m-1 justify-between items-center text-sm font-medium cursor-pointer hover:bg-blue-600 hover:text-gray-100\" + (this.state.selectedReference === index ? \" bg-blue-500 text-gray-100\" : \" bg-blue-900 text-gray-200\")}\n              onClick={() => { this.selectReference(index) }}\n            >\n              {reference[0]?.label}\n              <svg\n                xmlns=\"http://www.w3.org/2000/svg\"\n                className=\"h-5 w-5 ml-3 hover:text-gray-300\" viewBox=\"0 0 20 20\"\n                fill=\"currentColor\"\n                onClick={() => { this.removeReference(index) }}\n              >\n                <path\n                  fillRule=\"evenodd\"\n                  d=\"M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z\"\n                />\n              </svg>\n            </span>\n          ))}\n        </div>\n        <div id=\"actual-text\" className=\"mt-5 h-full\" onMouseUp={this.handleMouseUp}>\n          {this.state.actual_text}\n        </div>\n      </div>\n    )\n  }\n}\n\n\nexport default withStreamlitConnection(Annotation)\n\n",
+        "import {\n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React from \"react\"\n\ninterface Reference {\n  start: number,\n  end: number,\n  label: string\n}\n\ninterface State {\n  text: string\n  actual_text: JSX.Element[]\n  selectedReference: number\n  annotations: Reference[][]\n}\n\nclass Annotation extends StreamlitComponentBase<State> {\n  state: State = {\n    text: \"\",\n    actual_text: [],\n    annotations: [],\n    selectedReference: 0\n  }\n\n  async componentDidMount(): Promise<void> {\n    const { text, annotations } = this.props.args\n\n    await this.setState({ text, annotations })\n    await this.setState({ actual_text: this.renderText() })\n    Streamlit.setComponentValue(annotations)\n  }\n\n  isAnnotated(start: number, end: number): boolean {\n    const { annotations, selectedReference } = this.state\n    \n    if (!annotations[selectedReference]) {\n      return false\n    }\n\n    for (let i = 0; i < annotations[selectedReference].length; i++) {\n      if (\n        (start >= annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end >= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end > annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start >= annotations[selectedReference][i].start && start < annotations[selectedReference][i].end && end >= annotations[selectedReference][i].end)\n        ) {\n        return true\n      }\n    }\n    return false\n  }\n\n  removeAnnotation(start: number, end: number): Reference[][] {\n    const { annotations, selectedReference } = this.state\n\n    for (let i = 0; i < annotations[selectedReference].length; i++) {\n      if (\n        (start >= annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end >= annotations[selectedReference][i].end) ||\n        (start <= annotations[selectedReference][i].start && end > annotations[selectedReference][i].start && end <= annotations[selectedReference][i].end) ||\n        (start >= annotations[selectedReference][i].start && start < annotations[selectedReference][i].end && end >= annotations[selectedReference][i].end)\n        ) {\n        annotations[selectedReference].splice(i, 1)\n        break\n      }\n    }\n\n    if (annotations[selectedReference].length === 0) {\n      annotations.splice(selectedReference, 1)\n    }\n\n    return annotations\n  }\n\n  getCharactersCountUntilNode = (node: Node, parent: HTMLElement | null) => {\n    const walker = document.createTreeWalker(\n      parent || document.body,\n      NodeFilter.SHOW_TEXT,\n      null,\n    );\n    \n    let charCount = 0;\n    while (walker.nextNode()) {\n      if (walker.currentNode === node) {\n        break;\n      }\n      charCount += walker.currentNode.textContent?.length || 0;\n    }\n\n    return charCount;\n  }\n\n  handleMouseUp = async () => {\n    const selection = document.getSelection()?.getRangeAt(0)\n\n    if (selection && selection.toString().trim() !== \"\") {\n      let selectedText = selection.toString()\n\n      let startIndex = selection.startOffset\n      let endIndex = selection.endOffset\n      let startAdjustment = 0\n      let endAdjustment = 0\n\n      const container = document.getElementById(\"actual-text\")\n      const charsBeforeStart = this.getCharactersCountUntilNode(selection.startContainer, container);\n      const charsBeforeEnd = this.getCharactersCountUntilNode(selection.endContainer, container);\n\n      startIndex += charsBeforeStart\n      endIndex += charsBeforeEnd\n\n      while (document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex + startAdjustment - 1) !== \" \" && document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex + startAdjustment - 1) !== undefined) {\n        if (document.querySelector(\"#actual-text\")?.textContent?.charAt(startIndex + startAdjustment - 1) === '') {\n          break\n        }\n\n        startAdjustment -= 1\n      }\n\n      while (document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex + endAdjustment) !== \" \" && document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex + endAdjustment) !== undefined) {\n        if (document.querySelector(\"#actual-text\")?.textContent?.charAt(endIndex + endAdjustment) === '') {\n          break\n        }\n\n        endAdjustment += 1\n      }\n\n      selectedText = document.querySelector(\"#actual-text\")?.textContent?.slice(startIndex + startAdjustment, endIndex + endAdjustment) || \"\"\n\n      // remove commas, periods, etc. from the end of the selection if end adjustment is superior to 0\n      if (endAdjustment > 0) {\n        const re = /[.,/#!$%^&*;:{}=\\-_`~()]$/g\n        while (selectedText.match(re)) {\n          selectedText = selectedText.slice(0, -1)\n          endAdjustment -= 1\n        }\n      }\n\n      const { annotations, selectedReference } = this.state\n\n      if (!annotations[selectedReference]) {\n        annotations[selectedReference] = []\n      }\n\n      const finalStartIndex = startIndex + startAdjustment\n      const finalEndIndex = endIndex + endAdjustment\n\n      if (this.isAnnotated(finalStartIndex, finalEndIndex)) {\n        const newAnnotations = this.removeAnnotation(finalStartIndex, finalEndIndex)\n        await this.setState({ annotations: newAnnotations })\n      } else {\n        annotations[selectedReference].push({ start: finalStartIndex, end: finalEndIndex, label: selectedText })\n        await this.setState({ annotations })\n      }\n\n      Streamlit.setComponentValue(annotations)\n    }\n\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async addReference(): Promise<void> {\n    const { annotations } = this.state\n\n    // if selected annotation is empty do not add a new one\n    if (annotations[this.state.selectedReference] && annotations[this.state.selectedReference].length === 0) {\n      return\n    }\n\n    const index = annotations.length + 1\n    \n    if (!annotations[index]) {\n      annotations[index] = []\n    }\n\n    await this.setState({ \n      selectedReference: index,\n      annotations\n    })\n\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async selectReference(index: number): Promise<void> {\n    if (this.state.selectedReference === index || !this.state.annotations[index]) {\n      return\n    }\n\n    await this.setState({ selectedReference: index })\n    this.setState({ actual_text: this.renderText() })\n  }\n\n  async removeReference(index: number): Promise<void> {\n    const { annotations } = this.state\n\n    annotations.splice(index, 1)\n\n    await this.setState({ annotations, selectedReference: 0 })\n    this.setState({ actual_text: this.renderText() })\n    Streamlit.setComponentValue(annotations)\n  }\n\n  renderText(): JSX.Element[] {\n    const { text, annotations, selectedReference } = this.state\n    const actual_text: JSX.Element[] = []\n\n    if (!annotations[selectedReference]) {\n      return [<span>{text}</span>]\n    }\n\n\n    let start = 0\n\n    if (annotations[selectedReference].length > 0) {\n      annotations[selectedReference].sort((a, b) => a.start - b.start)\n    }\n\n    annotations[selectedReference].forEach((annotation, index) => {\n      actual_text.push(<span>{text.substring(start, annotation.start)}</span>)\n      actual_text.push(<span className=\"annotated bg-blue-500 text-gray-100\">{text.substring(annotation.start, annotation.end)}</span>)\n      start = annotation.end\n    })\n    actual_text.push(<span>{text.substring(start, text.length)}</span>)\n\n\n    return actual_text\n  }\n\n  render(): React.ReactNode {\n    return (\n      <div>\n        <div className=\"flex flex-row flex-wrap\">\n          <div\n            className=\"flex flex-wrap px-4 py-2 m-1 justify-between items-center text-sm font-medium cursor-pointer hover:bg-blue-600 hover:text-gray-100 bg-blue-500 text-gray-100\"\n            onClick={ () => this.addReference() }\n            >\n            <span>Add</span>\n          </div>\n          {this.state.annotations.map((reference, index) => (\n            <span\n              key={index}\n              className={\"flex flex-wrap pl-4 pr-2 py-2 m-1 justify-between items-center text-sm font-medium cursor-pointer hover:bg-blue-600 hover:text-gray-100\" + (this.state.selectedReference === index ? \" bg-blue-500 text-gray-100\" : \" bg-blue-900 text-gray-200\")}\n              onClick={() => { this.selectReference(index) }}\n            >\n              {reference[0]?.label}\n              <svg\n                xmlns=\"http://www.w3.org/2000/svg\"\n                className=\"h-5 w-5 ml-3 hover:text-gray-300\" viewBox=\"0 0 20 20\"\n                fill=\"currentColor\"\n                onClick={() => { this.removeReference(index) }}\n              >\n                <path\n                  fillRule=\"evenodd\"\n                  d=\"M10 18a8 8 0 100-16 8 8 0 000 16zM8.707 7.293a1 1 0 00-1.414 1.414L8.586 10l-1.293 1.293a1 1 0 101.414 1.414L10 11.414l1.293 1.293a1 1 0 001.414-1.414L11.414 10l1.293-1.293a1 1 0 00-1.414-1.414L10 8.586 8.707 7.293z\"\n                />\n              </svg>\n            </span>\n          ))}\n        </div>\n        <div id=\"actual-text\" className=\"mt-5 h-full\" onMouseUp={this.handleMouseUp}>\n          {this.state.actual_text}\n        </div>\n      </div>\n    )\n  }\n}\n\n\nexport default withStreamlitConnection(Annotation)\n\n",
         "import { createRoot } from 'react-dom/client';\nimport MyComponent from \"./Annotation\"\nimport React from 'react';\n\nconst container = document.getElementById(\"root\")\nconst root = createRoot(container)\n\nroot.render(<MyComponent />)\n"
     ],
     "version": 3
 }
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/package.json` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -30,9 +30,9 @@
     "private": true,
     "scripts": {
         "build": "react-scripts build",
         "eject": "react-scripts eject",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/public/index.html` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/src/Annotation.tsx` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/Annotation.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -98,58 +98,65 @@
     const selection = document.getSelection()?.getRangeAt(0)
 
     if (selection && selection.toString().trim() !== "") {
       let selectedText = selection.toString()
 
       let startIndex = selection.startOffset
       let endIndex = selection.endOffset
+      let startAdjustment = 0
+      let endAdjustment = 0
 
       const container = document.getElementById("actual-text")
       const charsBeforeStart = this.getCharactersCountUntilNode(selection.startContainer, container);
       const charsBeforeEnd = this.getCharactersCountUntilNode(selection.endContainer, container);
 
       startIndex += charsBeforeStart
       endIndex += charsBeforeEnd
 
-      while (document.querySelector("#actual-text")?.textContent?.charAt(startIndex - 1) !== " " && document.querySelector("#actual-text")?.textContent?.charAt(startIndex - 1) !== undefined) {
-        if (document.querySelector("#actual-text")?.textContent?.charAt(startIndex - 1) === '') {
+      while (document.querySelector("#actual-text")?.textContent?.charAt(startIndex + startAdjustment - 1) !== " " && document.querySelector("#actual-text")?.textContent?.charAt(startIndex + startAdjustment - 1) !== undefined) {
+        if (document.querySelector("#actual-text")?.textContent?.charAt(startIndex + startAdjustment - 1) === '') {
           break
         }
 
-        startIndex -= 1
+        startAdjustment -= 1
       }
 
-      while (document.querySelector("#actual-text")?.textContent?.charAt(endIndex) !== " " && document.querySelector("#actual-text")?.textContent?.charAt(endIndex) !== undefined) {
-        if (document.querySelector("#actual-text")?.textContent?.charAt(endIndex) === '') {
+      while (document.querySelector("#actual-text")?.textContent?.charAt(endIndex + endAdjustment) !== " " && document.querySelector("#actual-text")?.textContent?.charAt(endIndex + endAdjustment) !== undefined) {
+        if (document.querySelector("#actual-text")?.textContent?.charAt(endIndex + endAdjustment) === '') {
           break
         }
 
-        endIndex += 1
+        endAdjustment += 1
       }
 
-      selectedText = document.querySelector("#actual-text")?.textContent?.slice(startIndex, endIndex) || ""
+      selectedText = document.querySelector("#actual-text")?.textContent?.slice(startIndex + startAdjustment, endIndex + endAdjustment) || ""
 
-      // remove commas, periods, etc. from the end of the selection
-      const re = /[.,/#!$%^&*;:{}=\-_`~()]$/g
-      while (selectedText.match(re)) {
-        selectedText = selectedText.slice(0, -1)
-        endIndex -= 1
+      // remove commas, periods, etc. from the end of the selection if end adjustment is superior to 0
+      if (endAdjustment > 0) {
+        const re = /[.,/#!$%^&*;:{}=\-_`~()]$/g
+        while (selectedText.match(re)) {
+          selectedText = selectedText.slice(0, -1)
+          endAdjustment -= 1
+        }
       }
 
       const { annotations, selectedReference } = this.state
 
       if (!annotations[selectedReference]) {
         annotations[selectedReference] = []
       }
 
-      if (this.isAnnotated(startIndex, endIndex)) {
-        const newAnnotations = this.removeAnnotation(startIndex, endIndex)
+      const finalStartIndex = startIndex + startAdjustment
+      const finalEndIndex = endIndex + endAdjustment
+
+      if (this.isAnnotated(finalStartIndex, finalEndIndex)) {
+        const newAnnotations = this.removeAnnotation(finalStartIndex, finalEndIndex)
         await this.setState({ annotations: newAnnotations })
       } else {
-        annotations[selectedReference].push({ start: startIndex, end: endIndex, label: selectedText })
+        annotations[selectedReference].push({ start: finalStartIndex, end: finalEndIndex, label: selectedText })
         await this.setState({ annotations })
       }
 
       Streamlit.setComponentValue(annotations)
     }
 
     this.setState({ actual_text: this.renderText() })
```

### Comparing `st_text_annotator-0.3.0/src/st_text_annotator/frontend/tsconfig.json` & `st_text_annotator-0.3.1/src/st_text_annotator/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.0/PKG-INFO` & `st_text_annotator-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-text-annotator
-Version: 0.3.0
+Version: 0.3.1
 Summary: Component for annotating text for NLP resolution
 License: MIT
 Keywords: streamlit,text,annotation,nlp
 Author: Robin Marquet
 Author-email: robin.marquet@epitech.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

