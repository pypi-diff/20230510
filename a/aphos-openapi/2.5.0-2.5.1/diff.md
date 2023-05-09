# Comparing `tmp/aphos_openapi-2.5.0.tar.gz` & `tmp/aphos_openapi-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aphos_openapi-2.5.0.tar", last modified: Tue May  9 13:48:33 2023, max compression
+gzip compressed data, was "aphos_openapi-2.5.1.tar", last modified: Tue May  9 21:33:44 2023, max compression
```

## Comparing `aphos_openapi-2.5.0.tar` & `aphos_openapi-2.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/aphos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/flux_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/space_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/aphos_openapi/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/comparison_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/flux_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/night.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/photo_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/space_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/space_object_with_fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/aphos_openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/models/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/aphos_openapi/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:48:33.153122 aphos_openapi-2.5.0/aphos_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 13:48:33.000000 aphos_openapi-2.5.0/aphos_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:48:33.157122 aphos_openapi-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 13:48:22.000000 aphos_openapi-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.112702 aphos_openapi-2.5.1/aphos_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/aphos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/flux_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/space_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/comparison_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/flux_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/night.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/photo_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/space_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/space_object_with_fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.112702 aphos_openapi-2.5.1/aphos_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/setup.py
```

### Comparing `aphos_openapi-2.5.0/LICENSE` & `aphos_openapi-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/PKG-INFO` & `aphos_openapi-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aphos_openapi
-Version: 2.5.0
+Version: 2.5.1
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aphos_openapi-2.5.0/README.md` & `aphos_openapi-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/__init__.py` & `aphos_openapi-2.5.1/aphos_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/aphos.py` & `aphos_openapi-2.5.1/aphos_openapi/aphos.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/api/catalog_api.py` & `aphos_openapi-2.5.1/aphos_openapi/api/catalog_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/api/flux_api.py` & `aphos_openapi-2.5.1/aphos_openapi/api/flux_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/api/space_object_api.py` & `aphos_openapi-2.5.1/aphos_openapi/api/space_object_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/api/user_api.py` & `aphos_openapi-2.5.1/aphos_openapi/api/user_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/api_client.py` & `aphos_openapi-2.5.1/aphos_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/apis/__init__.py` & `aphos_openapi-2.5.1/aphos_openapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/configuration.py` & `aphos_openapi-2.5.1/aphos_openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/exceptions.py` & `aphos_openapi-2.5.1/aphos_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/comparison_object.py` & `aphos_openapi-2.5.1/aphos_openapi/model/comparison_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/error_message.py` & `aphos_openapi-2.5.1/aphos_openapi/model/error_message.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/flux.py` & `aphos_openapi-2.5.1/aphos_openapi/model/flux.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/flux_data.py` & `aphos_openapi-2.5.1/aphos_openapi/model/flux_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/night.py` & `aphos_openapi-2.5.1/aphos_openapi/model/night.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/photo_properties.py` & `aphos_openapi-2.5.1/aphos_openapi/model/photo_properties.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/space_object.py` & `aphos_openapi-2.5.1/aphos_openapi/model/space_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/space_object_with_fluxes.py` & `aphos_openapi-2.5.1/aphos_openapi/model/space_object_with_fluxes.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model/user.py` & `aphos_openapi-2.5.1/aphos_openapi/model/user.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/model_utils.py` & `aphos_openapi-2.5.1/aphos_openapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/models/__init__.py` & `aphos_openapi-2.5.1/aphos_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/models/coordinates.py` & `aphos_openapi-2.5.1/aphos_openapi/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi/models/graph_data.py` & `aphos_openapi-2.5.1/aphos_openapi/models/graph_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,47 +92,48 @@
         y-axis: Brightness [mag]
 
         Graph has also togglable error bars (deviations) and user filtering based on legend.
         """
         _, box = self._create_graph()
         _plt.show()
 
-    def _create_graph(self, ylabel: str = "Brightness [mag]") -> Tuple[List[Any], Optional[CheckButtons]]:
+    def _create_graph(self, ylabel: str = "Brightness [mag]", bottom: float = 0.2,
+                      rotation: int = 14) -> Tuple[List[Any], Optional[CheckButtons]]:
         """
         Create pyplot graph from data.
         Returns: Figure of given graph
 
         """
         d: Dict[str, List[Tuple[float, float, float]]] = dict()
         fig, ax = _plt.subplots(figsize=(11, 7))
-        fig.subplots_adjust(right=0.8, bottom=0.15)
+        fig.subplots_adjust(right=0.8, bottom=bottom)
         _plt.title(f"Light curve of {self._info_str()}")
         _plt.xlabel("Julian Date (JD)")
         _plt.ylabel(ylabel)
         for a, b, c, u in self.data_list:
             key = u[0:15]
             d.setdefault(key, []).append((a, b, c))
         errs = []
         plts = []
         for key, val in d.items():
             a, b, c = zip(*val)
-            plt, = ax.plot(a, b, "o", label=key)
-            plts.append(plt)
-            errs.append(ax.errorbar(a, b, yerr=c, fmt=" ", label=key, color="#1f77b4", visible=False))
+            errs.append(ax.errorbar(a, b, yerr=c, fmt="o", label=key, visible=True))
+            plts.append(errs[-1].lines[0])
+            plts[-1].set_label(key)
         _, labels = ax.get_legend_handles_labels()
         legend = ax.legend(plts, labels, loc='upper left', title="Username", bbox_to_anchor=(1, 0, 0.07, 1))
-        box = deviations(_plt, errs, plts, legend)
+        box = deviations(_plt, errs)
 
         if len(errs) > 10:
             scroll(fig, legend)
-        toggle_legend(legend, plts, errs)
+        toggle_legend(legend, errs, box)
 
         ax.invert_yaxis()
         ax.ticklabel_format(useOffset=False, style='plain')
-        _plt.setp(ax.get_xticklabels(), rotation=10, horizontalalignment='right')
+        _plt.setp(ax.get_xticklabels(), rotation=rotation, horizontalalignment='right')
         return plts, box
 
     def composite_graph(self) -> None:
         """
         Composite (compressed) graph representation of light curve in time.
 
         Similar to graph() but biggest "jump" between two measurements is defined by
@@ -180,17 +181,16 @@
                 # keep relative time in days
                 curr_min = curr_min + (x - curr)
             curr = x
             a.append(curr_min)
             b.append(y)
             c.append(z)
 
-        plt, = ax.plot(a, b, "o")
-        errs.append(ax.errorbar(a, b, yerr=c, fmt=" ", color="#1f77b4", visible=False))
-        box = deviations(_plt, errs, [plt], None)
+        errs.append(ax.errorbar(a, b, yerr=c, fmt="o", visible=True))
+        box = deviations(_plt, errs)
         ax.invert_yaxis()
         return box
 
     def phase_graph(self, moment: float, period: float) -> None:
         """
         Phase graph representation.
 
@@ -220,17 +220,16 @@
         b = []
         c = []
         errs = []
         for x, y, z, _ in self.data_list:
             a.append(((x - moment) / period) % 1)
             b.append(y)
             c.append(z)
-        plt, = ax.plot(a, b, "o")
-        errs.append(ax.errorbar(a, b, yerr=c, fmt=" ", color="#1f77b4", visible=False))
-        box = deviations(_plt, errs, [plt], None)
+        errs.append(ax.errorbar(a, b, yerr=c, fmt="o", visible=True))
+        box = deviations(_plt, errs)
         ax.invert_yaxis()
         return box
 
 
 class DMDU:
     """
     Class for representation of astronomical data.
@@ -332,43 +331,39 @@
 
 
 """
 Graph handling and event handlers for matplotlib graph helper functions.
 """
 
 
-def deviations(plot: _matplotlib.pyplot, errors: List[Any],
-               plts: List[_matplotlib.lines.Line2D],
-               legend: Optional[_matplotlib.legend.Legend]) -> CheckButtons:
+def deviations(plot: _matplotlib.pyplot, errors: List[Any]) -> CheckButtons:
     """
     Serves as checkbutton for graphs (Errorbar for deviations).
 
     Args:
         plot: pyplot from matplotlib
         errors: list of Errorbar containers objects
-        plts: list of Line2D (x-axis and y-axis values)
-        legend: legend of graph [optional]
 
     Returns: Checkbutton for error bar
 
     """
     button = plot.axes([0.01, 0.03, 0.18, 0.05], frameon=False)
     box = CheckButtons(button, ["show with deviations"], [False])
+    for error in errors:
+        for bar in error.lines[2]:
+            bar.set_visible(False)
 
     def set_devs(label: str) -> None:
         """
         Helper function for Checkbutton, logic of togglable errorbar.
         Event handler.
         """
-        for plt in plts:
-            plt.set_visible(True)
-        if legend is not None:
-            for a in legend.get_lines():
-                a.set_visible(True)
         for error in errors:
+            if not error.lines[0].get_visible():
+                continue
             for bar in error.lines[2]:
                 bar.set_visible(box.get_status()[0])
             plot.draw()
 
     box.on_clicked(set_devs)
     return box
 
@@ -396,16 +391,16 @@
             tr = legend.axes.transAxes.inverted()
             legend.set_bbox_to_anchor(bbox.transformed(tr))
             fig.canvas.draw_idle()
 
     fig.canvas.mpl_connect("scroll_event", legend_scroll)
 
 
-def toggle_legend(legend: _matplotlib.legend.Legend, plts: List[_matplotlib.lines.Line2D],
-                  errs: List[Any]) -> None:
+def toggle_legend(legend: _matplotlib.legend.Legend,
+                  errs: List[Any], box: CheckButtons) -> None:
     """
     Serves as creating togglable legend for graph (and event handling).
 
     Args:
         legend: legend of matplotlib.pyplot graph
         plts: list of plots in graph
         errs: list of Errorbar containers objects
@@ -419,22 +414,22 @@
         Event handler for clicking on legend.
 
         Args:
             event: Event
         """
         a = event.artist
         label = a.get_label()
-        visible = False
-        for plt in plts:
-            if plt.get_label() == label:
-                visible = plt.get_visible()
-                plt.set_visible(not visible)
         for err in errs:
             if err.get_label() == label:
+                visible = err.lines[0].get_visible()
+                err.lines[0].set_visible(not visible)
                 for bar in err.lines[2]:
-                    bar.set_visible(False)
+                    if not box.get_status()[0] and not visible:
+                        bar.set_visible(False)
+                        continue
+                    bar.set_visible(not visible)
 
         a.set_visible(not a.get_visible())
 
         _plt.draw()
 
     _plt.connect("pick_event", on_leg_click)
```

### Comparing `aphos_openapi-2.5.0/aphos_openapi/rest.py` & `aphos_openapi-2.5.1/aphos_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/aphos_openapi.egg-info/PKG-INFO` & `aphos_openapi-2.5.1/aphos_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aphos-openapi
-Version: 2.5.0
+Version: 2.5.1
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `aphos_openapi-2.5.0/aphos_openapi.egg-info/SOURCES.txt` & `aphos_openapi-2.5.1/aphos_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.0/setup.py` & `aphos_openapi-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aphos_openapi",
-    version="2.5.0",
+    version="2.5.1",
     author="Pavel Kinc",
     description="APhoS Python library for data representation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license_files=('LICENSE',),
     classifiers=[
```

