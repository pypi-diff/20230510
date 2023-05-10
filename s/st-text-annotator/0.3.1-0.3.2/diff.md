# Comparing `tmp/st_text_annotator-0.3.1.tar.gz` & `tmp/st_text_annotator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.3.1.tar", max compression
+gzip compressed data, was "st_text_annotator-0.3.2.tar", max compression
```

## Comparing `st_text_annotator-0.3.1.tar` & `st_text_annotator-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.3.1/LICENSE
--rw-r--r--   0        0        0     1951 2023-04-17 19:03:03.350393 st_text_annotator-0.3.1/README.md
--rw-r--r--   0        0        0      708 2023-05-10 07:41:40.158341 st_text_annotator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2791 2023-05-10 07:41:47.299730 st_text_annotator-0.3.1/src/st_text_annotator/__init__.py
--rw-r--r--   0        0        0      180 2023-04-18 15:31:27.032026 st_text_annotator-0.3.1/src/st_text_annotator/frontend/.env
--rw-r--r--   0        0        0       67 2023-04-18 15:31:27.033065 st_text_annotator-0.3.1/src/st_text_annotator/frontend/.prettierrc
--rw-r--r--   0        0        0      691 2023-05-10 07:46:07.482983 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2099 2023-05-10 07:46:07.482861 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/index.html
--rw-r--r--   0        0        0   489818 2023-05-10 07:46:07.488310 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js
--rw-r--r--   0        0        0     2280 2023-05-10 07:46:07.489092 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0  1785435 2023-05-10 07:46:07.488861 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map
--rw-r--r--   0        0        0     7780 2023-05-10 07:46:07.484666 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js
--rw-r--r--   0        0        0    19645 2023-05-10 07:46:07.489824 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map
--rw-r--r--   0        0        0     1594 2023-05-10 07:46:07.489935 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js
--rw-r--r--   0        0        0     8373 2023-05-10 07:46:07.488921 st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map
--rw-r--r--   0        0        0  1579776 2023-05-10 07:45:44.860303 st_text_annotator-0.3.1/src/st_text_annotator/frontend/package-lock.json
--rw-r--r--   0        0        0      848 2023-05-10 07:41:49.071479 st_text_annotator-0.3.1/src/st_text_annotator/frontend/package.json
--rw-r--r--   0        0        0      895 2023-04-18 15:45:04.080620 st_text_annotator-0.3.1/src/st_text_annotator/frontend/public/index.html
--rw-r--r--   0        0        0     9382 2023-05-10 07:35:55.735595 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/Annotation.tsx
--rw-r--r--   0        0        0      229 2023-04-18 18:13:03.689669 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-18 15:31:27.070284 st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      531 2023-04-18 15:43:10.838552 st_text_annotator-0.3.1/src/st_text_annotator/frontend/tsconfig.json
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 st_text_annotator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1951 2023-04-17 19:03:03.350393 st_text_annotator-0.3.2/README.md
+-rw-r--r--   0        0        0      708 2023-05-10 08:22:07.575782 st_text_annotator-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2790 2023-05-10 08:22:20.179907 st_text_annotator-0.3.2/src/st_text_annotator/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-18 15:31:27.032026 st_text_annotator-0.3.2/src/st_text_annotator/frontend/.env
+-rw-r--r--   0        0        0       67 2023-04-18 15:31:27.033065 st_text_annotator-0.3.2/src/st_text_annotator/frontend/.prettierrc
+-rw-r--r--   0        0        0      691 2023-05-10 07:46:07.482983 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2099 2023-05-10 07:46:07.482861 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/index.html
+-rw-r--r--   0        0        0   489818 2023-05-10 07:46:07.488310 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js
+-rw-r--r--   0        0        0     2280 2023-05-10 07:46:07.489092 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1785435 2023-05-10 07:46:07.488861 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map
+-rw-r--r--   0        0        0     7780 2023-05-10 07:46:07.484666 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js
+-rw-r--r--   0        0        0    19645 2023-05-10 07:46:07.489824 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map
+-rw-r--r--   0        0        0     1594 2023-05-10 07:46:07.489935 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js
+-rw-r--r--   0        0        0     8373 2023-05-10 07:46:07.488921 st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map
+-rw-r--r--   0        0        0      848 2023-05-10 08:22:16.333577 st_text_annotator-0.3.2/src/st_text_annotator/frontend/package.json
+-rw-r--r--   0        0        0      895 2023-04-18 15:45:04.080620 st_text_annotator-0.3.2/src/st_text_annotator/frontend/public/index.html
+-rw-r--r--   0        0        0     9382 2023-05-10 07:35:55.735595 st_text_annotator-0.3.2/src/st_text_annotator/frontend/src/Annotation.tsx
+-rw-r--r--   0        0        0      229 2023-04-18 18:13:03.689669 st_text_annotator-0.3.2/src/st_text_annotator/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-18 15:31:27.070284 st_text_annotator-0.3.2/src/st_text_annotator/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      531 2023-04-18 15:43:10.838552 st_text_annotator-0.3.2/src/st_text_annotator/frontend/tsconfig.json
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 st_text_annotator-0.3.2/PKG-INFO
```

### Comparing `st_text_annotator-0.3.1/LICENSE` & `st_text_annotator-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/README.md` & `st_text_annotator-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/pyproject.toml` & `st_text_annotator-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "st-text-annotator"
-version = "0.3.1"
+version = "0.3.2"
 description = "Component for annotating text for NLP resolution"
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 authors = ["Robin Marquet <robin.marquet@epitech.eu>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["streamlit", "text", "annotation", "nlp"]
 include = ["./src/st_text_annotator/frontend/build/**/*"]
```

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/__init__.py` & `st_text_annotator-0.3.2/src/st_text_annotator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import streamlit.components.v1 as components
 
-RELEASE = False
+RELEASE = True
 
 if not RELEASE:
     _component_func = components.declare_component("st_text_annotator", url="http://localhost:3001")
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("StTextAnnotator", path=build_dir)
```

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/asset-manifest.json` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/index.html` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/2.d11c6839.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/main.4ce3c4a6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/build/static/js/runtime-main.6ab9b2fc.js.map`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/package.json` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/package.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/public/index.html` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/src/Annotation.tsx` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/src/Annotation.tsx`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/src/st_text_annotator/frontend/tsconfig.json` & `st_text_annotator-0.3.2/src/st_text_annotator/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.3.1/PKG-INFO` & `st_text_annotator-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-text-annotator
-Version: 0.3.1
+Version: 0.3.2
 Summary: Component for annotating text for NLP resolution
 License: MIT
 Keywords: streamlit,text,annotation,nlp
 Author: Robin Marquet
 Author-email: robin.marquet@epitech.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

