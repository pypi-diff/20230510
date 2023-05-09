# Comparing `tmp/hnxwidget-0.1.1b1.tar.gz` & `tmp/hnxwidget-0.1.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hnxwidget-0.1.1b1.tar", last modified: Fri Oct 22 17:45:58 2021, max compression
+gzip compressed data, was "hnxwidget-0.1.1b3.tar", last modified: Tue May  9 22:14:17 2023, max compression
```

## Comparing `hnxwidget-0.1.1b1.tar` & `hnxwidget-0.1.1b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 aren438  (503616761) PNL\Domain Users (2016721313)        0 2021-10-22 17:45:57.979965 hnxwidget-0.1.1b1/
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)       63 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/MANIFEST.in
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      998 2021-10-22 17:45:57.980181 hnxwidget-0.1.1b1/PKG-INFO
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      956 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/README.md
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)       64 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnx-widget.json
-drwxr-xr-x   0 aren438  (503616761) PNL\Domain Users (2016721313)        0 2021-10-22 17:45:57.763994 hnxwidget-0.1.1b1/hnxwidget/
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     1039 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnxwidget/__init__.py
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      388 2021-10-22 17:29:31.000000 hnxwidget-0.1.1b1/hnxwidget/_version.py
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     1233 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnxwidget/example.py
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     4718 2021-10-22 16:45:44.000000 hnxwidget-0.1.1b1/hnxwidget/hypernetx_widget.py
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      717 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnxwidget/react_jupyter_widget.py
-drwxr-xr-x   0 aren438  (503616761) PNL\Domain Users (2016721313)        0 2021-10-22 17:45:57.944398 hnxwidget-0.1.1b1/hnxwidget/static/
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     3336 2021-09-30 23:17:53.000000 hnxwidget-0.1.1b1/hnxwidget/static/extension.js
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313) 14903972 2021-09-30 23:18:14.000000 hnxwidget-0.1.1b1/hnxwidget/static/index.js
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313) 13736625 2021-09-30 23:18:14.000000 hnxwidget-0.1.1b1/hnxwidget/static/index.js.map
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      778 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnxwidget/stats.py
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     3357 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/hnxwidget/util.py
-drwxr-xr-x   0 aren438  (503616761) PNL\Domain Users (2016721313)        0 2021-10-22 17:45:57.795061 hnxwidget-0.1.1b1/hnxwidget.egg-info/
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      998 2021-10-22 17:45:56.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/PKG-INFO
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)      504 2021-10-22 17:45:56.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/SOURCES.txt
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)        1 2021-10-22 17:45:56.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/dependency_links.txt
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)        1 2021-06-02 03:42:42.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/not-zip-safe
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)       18 2021-10-22 17:45:56.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/requires.txt
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)       10 2021-10-22 17:45:56.000000 hnxwidget-0.1.1b1/hnxwidget.egg-info/top_level.txt
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)       67 2021-10-22 17:45:57.981985 hnxwidget-0.1.1b1/setup.cfg
--rw-r--r--   0 aren438  (503616761) PNL\Domain Users (2016721313)     5765 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b1/setup.py
+drwxr-xr-x   0 aren438    (501) staff       (20)        0 2023-05-09 22:14:17.344708 hnxwidget-0.1.1b3/
+-rw-r--r--   0 aren438    (501) staff       (20)       63 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/MANIFEST.in
+-rw-r--r--   0 aren438    (501) staff       (20)      987 2023-05-09 22:14:17.344869 hnxwidget-0.1.1b3/PKG-INFO
+-rw-r--r--   0 aren438    (501) staff       (20)      956 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/README.md
+-rw-r--r--   0 aren438    (501) staff       (20)       64 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnx-widget.json
+drwxr-xr-x   0 aren438    (501) staff       (20)        0 2023-05-09 22:14:17.312210 hnxwidget-0.1.1b3/hnxwidget/
+-rw-r--r--   0 aren438    (501) staff       (20)     1039 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnxwidget/__init__.py
+-rw-r--r--   0 aren438    (501) staff       (20)      388 2023-05-04 19:31:26.000000 hnxwidget-0.1.1b3/hnxwidget/_version.py
+-rw-r--r--   0 aren438    (501) staff       (20)     1233 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnxwidget/example.py
+-rw-r--r--   0 aren438    (501) staff       (20)     5885 2023-05-04 18:50:28.000000 hnxwidget-0.1.1b3/hnxwidget/hypernetx_widget.py
+-rw-r--r--   0 aren438    (501) staff       (20)      717 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnxwidget/react_jupyter_widget.py
+drwxr-xr-x   0 aren438    (501) staff       (20)        0 2023-05-09 22:14:17.331708 hnxwidget-0.1.1b3/hnxwidget/static/
+-rw-r--r--   0 aren438    (501) staff       (20)     3336 2023-03-23 18:54:05.000000 hnxwidget-0.1.1b3/hnxwidget/static/extension.js
+-rw-r--r--   0 aren438    (501) staff       (20) 14903962 2023-03-23 18:54:14.000000 hnxwidget-0.1.1b3/hnxwidget/static/index.js
+-rw-r--r--   0 aren438    (501) staff       (20) 13736615 2023-03-23 18:54:14.000000 hnxwidget-0.1.1b3/hnxwidget/static/index.js.map
+-rw-r--r--   0 aren438    (501) staff       (20)      778 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnxwidget/stats.py
+-rw-r--r--   0 aren438    (501) staff       (20)     3357 2021-09-30 22:27:20.000000 hnxwidget-0.1.1b3/hnxwidget/util.py
+drwxr-xr-x   0 aren438    (501) staff       (20)        0 2023-05-09 22:14:17.317745 hnxwidget-0.1.1b3/hnxwidget.egg-info/
+-rw-r--r--   0 aren438    (501) staff       (20)      987 2023-05-09 22:14:16.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/PKG-INFO
+-rw-r--r--   0 aren438    (501) staff       (20)      504 2023-05-09 22:14:17.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 aren438    (501) staff       (20)        1 2023-05-09 22:14:16.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 aren438    (501) staff       (20)        1 2021-06-02 03:42:42.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/not-zip-safe
+-rw-r--r--   0 aren438    (501) staff       (20)       18 2023-05-09 22:14:17.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/requires.txt
+-rw-r--r--   0 aren438    (501) staff       (20)       10 2023-05-09 22:14:17.000000 hnxwidget-0.1.1b3/hnxwidget.egg-info/top_level.txt
+-rw-r--r--   0 aren438    (501) staff       (20)       67 2023-05-09 22:14:17.347187 hnxwidget-0.1.1b3/setup.cfg
+-rw-r--r--   0 aren438    (501) staff       (20)     5765 2023-03-23 20:01:58.000000 hnxwidget-0.1.1b3/setup.py
```

### Comparing `hnxwidget-0.1.1b1/PKG-INFO` & `hnxwidget-0.1.1b3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: hnxwidget
-Version: 0.1.1b1
+Version: 0.1.1b3
 Summary: A widget for interractive visualization of the hypernetx package.
 Home-page: https://github.com/pnnl/hypernetx-widget
 Author: Dustin Arendt
 Author-email: dustin.arendt@pnnl.gov
 License: UNKNOWN
-Description: A widget for interactive visualization of the hypernetx package.
 Keywords: ipython,jupyter,widgets
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
@@ -18,7 +17,10 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+
+A widget for interactive visualization of the hypernetx package.
+
```

### Comparing `hnxwidget-0.1.1b1/README.md` & `hnxwidget-0.1.1b3/README.md`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/__init__.py` & `hnxwidget-0.1.1b3/hnxwidget/__init__.py`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/example.py` & `hnxwidget-0.1.1b3/hnxwidget/example.py`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/hypernetx_widget.py` & `hnxwidget-0.1.1b3/hnxwidget/hypernetx_widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from .react_jupyter_widget import ReactJupyterWidget
 
 import ipywidgets as widgets
 from traitlets import Dict
 
+import pandas as pd
+
 import matplotlib.pyplot as plt
 from matplotlib.colors import to_rgba_array, to_hex
 import numpy as np
 
 from .util import get_set_layering, inflate_kwargs
 
 from itertools import chain
@@ -68,14 +70,30 @@
     
     # if not otherwise specified, set the edge label color
     # to be the same as the edge color
     props.setdefault('edgeLabelColor', props['edgeStroke'])
 
     return {**props, **rename_kwargs(**kwargs)}
 
+
+def to_dict_without_nans(df):
+    df = df.copy()
+    df.index = df.index.astype(str)
+
+    return {
+        c: df[c].dropna().to_dict()
+        for c in df
+    }
+
+def incidence_dict_astype_str(H):
+    return {
+        str(k): list(map(str, v))
+        for k, v in H.items()
+    }
+
 @widgets.register
 class HypernetxWidgetView(ReactJupyterWidget):
     pos = Dict().tag(sync=True)
     node_fill = Dict().tag(sync=True)
     edge_stroke = Dict().tag(sync=True)
     selected_nodes = Dict().tag(sync=True)
     selected_edges = Dict().tag(sync=True)
@@ -113,20 +131,23 @@
     def selected_edge_data(self):
         return self.edge_data.loc[self.get_index(self.selected_edges)]
 
     def __init__(self, H,
         collapse=True,
         node_styles={},
         with_color=True,
+        ignore_hnx_properties=False,
         **kwargs
     ):
-        incidence_dict = {k: list(v) for k, v in H.incidence_dict.items()}\
+        incidence_dict = H.edges.incidence_dict\
             if H.__class__.__name__ == 'Hypergraph'\
             else H
 
+        incidence_dict = incidence_dict_astype_str(incidence_dict)
+
         def get_property(id, value, default):
             if value is None:
                 return default
             elif hasattr(value, 'get'):
                 return value.get(id, default)
             else:
                 return value
@@ -135,30 +156,46 @@
         E = list(incidence_dict)
 
         nodes = [{'uid': uid} for uid in V]
         
         # js friendly representation of the hypergraph
         edges = [
             {
-                'uid': str(uid),
+                'uid': uid,
                 'elements': elements
             }
             for uid, elements in incidence_dict.items()
         ]
 
+        # used to convert Hnx 1.2 style properties into dataframes compatible with widget
+        def prepare_properties(props):
+            df = pd.concat([
+                props.drop(columns=['properties', 'uid']),
+                pd.DataFrame(props.properties.tolist(), index=props.properties.index)
+            ], axis=1)
+            
+            col_mask = (~df.isnull()).any(axis=0)
+            
+            return df[df.columns[col_mask]]
+
+        if not ignore_hnx_properties and hasattr(H, 'edges') and hasattr(H, 'nodes'):
+            # check if Hypergraph object contains properties
+            kwargs['edge_data'] = prepare_properties(H.edges.properties.loc[0])
+            kwargs['node_data'] = prepare_properties(H.nodes.properties.loc[0])
+
         if 'node_data' in kwargs:
             self.node_data = kwargs['node_data']
-            kwargs['node_data'] = self.node_data.T.to_dict()
+            kwargs['node_data'] = to_dict_without_nans(self.node_data.T)
 
         if 'edge_data' in kwargs:
             self.edge_data = kwargs['edge_data']
-            kwargs['edge_data'] = self.edge_data.T.to_dict()
-
+            kwargs['edge_data'] = to_dict_without_nans(self.edge_data.T)
+            
         super().__init__(
             nodes=nodes,
             edges=edges,
             **hnx_kwargs_to_props(V, E, **kwargs)
         )
 
 @widgets.register
 class HypernetxWidget(HypernetxWidgetView):
-    pass
+    pass
```

### Comparing `hnxwidget-0.1.1b1/hnxwidget/react_jupyter_widget.py` & `hnxwidget-0.1.1b3/hnxwidget/react_jupyter_widget.py`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/static/extension.js` & `hnxwidget-0.1.1b3/hnxwidget/static/extension.js`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/static/index.js` & `hnxwidget-0.1.1b3/hnxwidget/static/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -399910,15 +399910,15 @@
                     "test": "echo \"Error: no test specified\" && exit 1"
                 },
                 "devDependencies": {
                     "rimraf": "^2.6.1",
                     "webpack": "^3.5.5"
                 },
                 "dependencies": {
-                    "@jupyter-widgets/base": "^1.1 || ^2 || ^3",
+                    "@jupyter-widgets/base": "^4.0.0",
                     "lodash": "^4.17.4"
                 },
                 "jupyterlab": {
                     "extension": "lib/labplugin"
                 }
             }
```

### Comparing `hnxwidget-0.1.1b1/hnxwidget/static/index.js.map` & `hnxwidget-0.1.1b3/hnxwidget/static/index.js.map`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 7b22 7665 7273 696f 6e22 3a33 2c22 736f  {"version":3,"so
 00000010: 7572 6365 7322 3a5b 2277 6562 7061 636b  urces":["webpack
 00000020: 3a2f 2f2f 7765 6270 6163 6b2f 626f 6f74  :///webpack/boot
-00000030: 7374 7261 7020 3934 3131 3865 3638 6261  strap 94118e68ba
-00000040: 3136 3031 3938 6665 3836 222c 2277 6562  160198fe86","web
+00000030: 7374 7261 7020 3865 3139 3537 3761 6431  strap 8e19577ad1
+00000040: 6632 6139 3364 6430 6363 222c 2277 6562  f2a93dd0cc","web
 00000050: 7061 636b 3a2f 2f2f 2f55 7365 7273 2f61  pack:////Users/a
 00000060: 7265 6e34 3338 2f70 726f 6a65 6374 732f  ren438/projects/
 00000070: 686e 782d 7769 6467 6574 2f6e 6f64 655f  hnx-widget/node_
 00000080: 6d6f 6475 6c65 732f 7265 6163 742f 696e  modules/react/in
 00000090: 6465 782e 6a73 222c 2277 6562 7061 636b  dex.js","webpack
 000000a0: 3a2f 2f2f 2f55 7365 7273 2f61 7265 6e34  :////Users/aren4
 000000b0: 3338 2f70 726f 6a65 6374 732f 686e 782d  38/projects/hnx-
@@ -169861,16 +169861,16 @@
 00297840: 4d41 414d 2c6f 4241 416f 422c 4d41 414d  MAAM,oBAAoB,MAAM
 00297850: 2c6f 4241 416f 422c 4d41 414d 2c6f 4241  ,oBAAoB,MAAM,oBA
 00297860: 416f 422c 6541 4165 2c6f 4241 416f 422c  AoB,eAAe,oBAAoB,
 00297870: 6541 4165 2c69 423b 3b3b 3b3b 3b41 4341  eAAe,iB;;;;;;ACA
 00297880: 3172 442c 6b42 4141 6b42 2c6f 4c41 416f  1rD,kBAAkB,oLAAo
 00297890: 4c2c 3444 4141 3444 2c2b 4841 412b 482c  L,4DAA4D,+HAA+H,
 002978a0: 6b4a 4141 6b4a 2c6f 4241 416f 422c 7143  kJAAkJ,oBAAoB,qC
-002978b0: 4141 7143 2c69 4241 4169 422c 3844 4141  AAqC,iBAAiB,8DAA
-002978c0: 3844 2c65 4141 652c 3642 222c 2266 696c  8D,eAAe,6B","fil
+002978b0: 4141 7143 2c69 4241 4169 422c 6f44 4141  AAqC,iBAAiB,oDAA
+002978c0: 6f44 2c65 4141 652c 3642 222c 2266 696c  oD,eAAe,6B","fil
 002978d0: 6522 3a22 696e 6465 782e 6a73 222c 2273  e":"index.js","s
 002978e0: 6f75 7263 6573 436f 6e74 656e 7422 3a5b  ourcesContent":[
 002978f0: 2220 5c74 2f2f 2054 6865 206d 6f64 756c  " \t// The modul
 00297900: 6520 6361 6368 655c 6e20 5c74 7661 7220  e cache\n \tvar 
 00297910: 696e 7374 616c 6c65 644d 6f64 756c 6573  installedModules
 00297920: 203d 207b 7d3b 5c6e 5c6e 205c 742f 2f20   = {};\n\n \t// 
 00297930: 5468 6520 7265 7175 6972 6520 6675 6e63  The require func
@@ -169988,16 +169988,16 @@
 00298030: 5c6e 205c 7472 6574 7572 6e20 5f5f 7765  \n \treturn __we
 00298040: 6270 6163 6b5f 7265 7175 6972 655f 5f28  bpack_require__(
 00298050: 5f5f 7765 6270 6163 6b5f 7265 7175 6972  __webpack_requir
 00298060: 655f 5f2e 7320 3d20 3835 3529 3b5c 6e5c  e__.s = 855);\n\
 00298070: 6e5c 6e5c 6e2f 2f20 5745 4250 4143 4b20  n\n\n// WEBPACK 
 00298080: 464f 4f54 4552 202f 2f5c 6e2f 2f20 7765  FOOTER //\n// we
 00298090: 6270 6163 6b2f 626f 6f74 7374 7261 7020  bpack/bootstrap 
-002980a0: 3934 3131 3865 3638 6261 3136 3031 3938  94118e68ba160198
-002980b0: 6665 3836 222c 2227 7573 6520 7374 7269  fe86","'use stri
+002980a0: 3865 3139 3537 3761 6431 6632 6139 3364  8e19577ad1f2a93d
+002980b0: 6430 6363 222c 2227 7573 6520 7374 7269  d0cc","'use stri
 002980c0: 6374 273b 5c6e 5c6e 6966 2028 7072 6f63  ct';\n\nif (proc
 002980d0: 6573 732e 656e 762e 4e4f 4445 5f45 4e56  ess.env.NODE_ENV
 002980e0: 203d 3d3d 2027 7072 6f64 7563 7469 6f6e   === 'production
 002980f0: 2729 207b 5c6e 2020 6d6f 6475 6c65 2e65  ') {\n  module.e
 00298100: 7870 6f72 7473 203d 2072 6571 7569 7265  xports = require
 00298110: 2827 2e2f 636a 732f 7265 6163 742e 7072  ('./cjs/react.pr
 00298120: 6f64 7563 7469 6f6e 2e6d 696e 2e6a 7327  oduction.min.js'
@@ -858519,22 +858519,21 @@
 00d19960: 6974 2031 5c22 7d2c 5c22 6465 7644 6570  it 1\"},\"devDep
 00d19970: 656e 6465 6e63 6965 735c 223a 7b5c 2272  endencies\":{\"r
 00d19980: 696d 7261 665c 223a 5c22 5e32 2e36 2e31  imraf\":\"^2.6.1
 00d19990: 5c22 2c5c 2277 6562 7061 636b 5c22 3a5c  \",\"webpack\":\
 00d199a0: 225e 332e 352e 355c 227d 2c5c 2264 6570  "^3.5.5\"},\"dep
 00d199b0: 656e 6465 6e63 6965 735c 223a 7b5c 2240  endencies\":{\"@
 00d199c0: 6a75 7079 7465 722d 7769 6467 6574 732f  jupyter-widgets/
-00d199d0: 6261 7365 5c22 3a5c 225e 312e 3120 7c7c  base\":\"^1.1 ||
-00d199e0: 205e 3220 7c7c 205e 335c 222c 5c22 6c6f   ^2 || ^3\",\"lo
-00d199f0: 6461 7368 5c22 3a5c 225e 342e 3137 2e34  dash\":\"^4.17.4
-00d19a00: 5c22 7d2c 5c22 6a75 7079 7465 726c 6162  \"},\"jupyterlab
-00d19a10: 5c22 3a7b 5c22 6578 7465 6e73 696f 6e5c  \":{\"extension\
-00d19a20: 223a 5c22 6c69 622f 6c61 6270 6c75 6769  ":\"lib/labplugi
-00d19a30: 6e5c 227d 7d5c 6e5c 6e5c 6e2f 2f2f 2f2f  n\"}}\n\n\n/////
-00d19a40: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f5c 6e2f  /////////////\n/
-00d19a50: 2f20 5745 4250 4143 4b20 464f 4f54 4552  / WEBPACK FOOTER
-00d19a60: 5c6e 2f2f 202e 2f70 6163 6b61 6765 2e6a  \n// ./package.j
-00d19a70: 736f 6e5c 6e2f 2f20 6d6f 6475 6c65 2069  son\n// module i
-00d19a80: 6420 3d20 3736 3039 5c6e 2f2f 206d 6f64  d = 7609\n// mod
-00d19a90: 756c 6520 6368 756e 6b73 203d 2030 225d  ule chunks = 0"]
-00d19aa0: 2c22 736f 7572 6365 526f 6f74 223a 2222  ,"sourceRoot":""
-00d19ab0: 7d                                       }
+00d199d0: 6261 7365 5c22 3a5c 225e 342e 302e 305c  base\":\"^4.0.0\
+00d199e0: 222c 5c22 6c6f 6461 7368 5c22 3a5c 225e  ",\"lodash\":\"^
+00d199f0: 342e 3137 2e34 5c22 7d2c 5c22 6a75 7079  4.17.4\"},\"jupy
+00d19a00: 7465 726c 6162 5c22 3a7b 5c22 6578 7465  terlab\":{\"exte
+00d19a10: 6e73 696f 6e5c 223a 5c22 6c69 622f 6c61  nsion\":\"lib/la
+00d19a20: 6270 6c75 6769 6e5c 227d 7d5c 6e5c 6e5c  bplugin\"}}\n\n\
+00d19a30: 6e2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  n///////////////
+00d19a40: 2f2f 2f5c 6e2f 2f20 5745 4250 4143 4b20  ///\n// WEBPACK 
+00d19a50: 464f 4f54 4552 5c6e 2f2f 202e 2f70 6163  FOOTER\n// ./pac
+00d19a60: 6b61 6765 2e6a 736f 6e5c 6e2f 2f20 6d6f  kage.json\n// mo
+00d19a70: 6475 6c65 2069 6420 3d20 3736 3039 5c6e  dule id = 7609\n
+00d19a80: 2f2f 206d 6f64 756c 6520 6368 756e 6b73  // module chunks
+00d19a90: 203d 2030 225d 2c22 736f 7572 6365 526f   = 0"],"sourceRo
+00d19aa0: 6f74 223a 2222 7d                        ot":""}
```

### Comparing `hnxwidget-0.1.1b1/hnxwidget/stats.py` & `hnxwidget-0.1.1b3/hnxwidget/stats.py`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget/util.py` & `hnxwidget-0.1.1b3/hnxwidget/util.py`

 * *Files identical despite different names*

### Comparing `hnxwidget-0.1.1b1/hnxwidget.egg-info/PKG-INFO` & `hnxwidget-0.1.1b3/hnxwidget.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: hnxwidget
-Version: 0.1.1b1
+Version: 0.1.1b3
 Summary: A widget for interractive visualization of the hypernetx package.
 Home-page: https://github.com/pnnl/hypernetx-widget
 Author: Dustin Arendt
 Author-email: dustin.arendt@pnnl.gov
 License: UNKNOWN
-Description: A widget for interactive visualization of the hypernetx package.
 Keywords: ipython,jupyter,widgets
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
@@ -18,7 +17,10 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+
+A widget for interactive visualization of the hypernetx package.
+
```

### Comparing `hnxwidget-0.1.1b1/setup.py` & `hnxwidget-0.1.1b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             'hnxwidget/static/extension.js',
             'hnxwidget/static/index.js',
             'hnxwidget/static/index.js.map',
         ],),
         ('etc/jupyter/nbconfig/notebook.d' ,['hnx-widget.json'])
     ],
     install_requires=[
-        'ipywidgets>=7.0.0',
+        'ipywidgets==7.6.5',
     ],
     packages=find_packages(),
     zip_safe=False,
     cmdclass={
         'build_py': js_prerelease(build_py),
         'egg_info': js_prerelease(egg_info),
         'sdist': js_prerelease(sdist, strict=True),
```

