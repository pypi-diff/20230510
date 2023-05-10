# Comparing `tmp/caveclient-5.4.2.tar.gz` & `tmp/caveclient-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.4.2.tar", last modified: Wed May 10 02:43:47 2023, max compression
+gzip compressed data, was "caveclient-5.5.0.tar", last modified: Wed May 10 16:29:22 2023, max compression
```

## Comparing `caveclient-5.4.2.tar` & `caveclient-5.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.325954 caveclient-5.4.2/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.4.2/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:43:47.325549 caveclient-5.4.2/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.4.2/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.315594 caveclient-5.4.2/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 02:43:43.000000 caveclient-5.4.2/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.4.2/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.4.2/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    90661 2023-05-10 02:43:35.000000 caveclient-5.4.2/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.4.2/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.319686 caveclient-5.4.2/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.317595 caveclient-5.4.2/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 02:43:35.000000 caveclient-5.4.2/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 02:43:47.326125 caveclient-5.4.2/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.4.2/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.325209 caveclient-5.4.2/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.4.2/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.4.2/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.4.2/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.651450 caveclient-5.5.0/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.5.0/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 16:29:22.651233 caveclient-5.5.0/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.5.0/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.633972 caveclient-5.5.0/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 16:29:17.000000 caveclient-5.5.0/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.5.0/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.5.0/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.5.0/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.5.0/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.5.0/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.5.0/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    90661 2023-05-10 03:33:26.000000 caveclient-5.5.0/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.5.0/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.638002 caveclient-5.5.0/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.637180 caveclient-5.5.0/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.5.0/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 16:29:22.651508 caveclient-5.5.0/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.5.0/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.649782 caveclient-5.5.0/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.5.0/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.5.0/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.5.0/tests/test_materialization.py
```

### Comparing `caveclient-5.4.2/README.rst` & `caveclient-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/annotationengine.py` & `caveclient-5.5.0/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/auth.py` & `caveclient-5.5.0/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/base.py` & `caveclient-5.5.0/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/chunkedgraph.py` & `caveclient-5.5.0/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/datastack_lookup.py` & `caveclient-5.5.0/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/emannotationschemas.py` & `caveclient-5.5.0/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/endpoints.py` & `caveclient-5.5.0/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/format_utils.py` & `caveclient-5.5.0/caveclient/format_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,22 @@
         objurl_out = f"precomputed://{objurl}"
     elif qry.scheme == "http" or qry.scheme == "https":
         objurl_out = f"precomputed://gs://{qry.path[1:]}"
     else:
         objurl_out = None
     return objurl_out
 
+def format_neuroglancer(objurl):
+    qry = urlparse(objurl)
+    if qry.scheme == 'graphene' or 'https':
+        return format_graphene(objurl)
+    elif qry.scheme == 'precomputed':
+        return format_precomputed_neuroglancer(objurl)
+    else:
+        return format_raw(objurl)
 
 def format_precomputed_https(objurl):
     qry = urlparse(objurl)
     if qry.scheme == "gs":
         objurl_out = f"precomputed://https://storage.googleapis.com/{qry.path[1:]}"
     elif qry.scheme == "http" or qry.scheme == "https":
         objurl_out = f"precomputed://{objurl}"
@@ -29,37 +37,45 @@
         objurl_out = f"graphene://{objurl}"
     elif qry.scheme == "graphene":
         objurl_out = objurl
     else:
         objurl_out = None
     return objurl_out
 
+def format_verbose_graphene(objurl):
+    qry = urlparse(objurl)
+    if qry.scheme == "http" or qry.scheme == "https":
+        objurl_out = f"graphene://middleauth+{objurl}"
+    elif qry.scheme == "graphene":
+        objurl_out = f"graphene://middleauth+{qry.netloc}{qry.path}"
+    return objurl_out
+
 def format_cloudvolume(objurl):
     qry = urlparse(objurl)
     if qry.scheme == "graphene":
         return format_graphene(objurl)
     elif qry.scheme == "gs" or qry.scheme == "http" or qry.scheme == "https":
         return format_precomputed_https(objurl)
     else:
         return None
 
-
 def format_raw(objurl):
     return objurl
 
+def format_cave_explorer(objurl):
+    qry = urlparse(objurl)
+    if qry.scheme == "graphene" or qry.scheme == "https":
+        return format_verbose_graphene(objurl)
+    elif qry.scheme == 'precomputed':
+        return format_precomputed_neuroglancer(objurl)
+    else:
+        return None
 
-# No reformatting
-output_map_raw = {}
-
-# Use precomputed://gs:// links for neuroglancer, but use precomputed://https://storage.googleapis.com links in cloudvolume
-output_map_precomputed = {
-    "raw": format_raw,
-    "cloudvolume": format_precomputed_https,
-    "neuroglancer": format_precomputed_neuroglancer,
-}
 
 # Use graphene://https:// links for both neuroglancer and cloudvolume
-output_map_graphene = {
+
+output_map = {
     "raw": format_raw,
-    "cloudvolume": format_graphene,
-    "neuroglancer": format_graphene,
+    "cloudvolume": format_cloudvolume,
+    "neuroglancer": format_neuroglancer,
+    "cave_explorer": format_cave_explorer,
 }
```

### Comparing `caveclient-5.4.2/caveclient/frameworkclient.py` & `caveclient-5.5.0/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/infoservice.py` & `caveclient-5.5.0/caveclient/infoservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from .auth import AuthClient
 from .endpoints import (
     infoservice_common,
     infoservice_api_versions,
     default_global_server_address,
 )
 from .format_utils import (
-    output_map_raw,
-    output_map_precomputed,
+    output_map,
     format_raw,
 )
 
 
 SERVER_KEY = "i_server_address"
 
 
@@ -165,15 +164,15 @@
 
     def _get_property(
         self,
         info_property,
         datastack_name=None,
         use_stored=True,
         format_for="raw",
-        output_map=output_map_raw,
+        output_map=output_map,
     ):
         if datastack_name is None:
             datastack_name = self.datastack_name
         if datastack_name is None:
             raise ValueError("No Dataset set")
 
         self.get_datastack_info(datastack_name=datastack_name, use_stored=use_stored)
@@ -254,15 +253,15 @@
         return handle_response(response)
 
     def local_server(self, datastack_name=None, use_stored=True):
         return self._get_property(
             "local_server",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            output_map=output_map_raw,
+            output_map=output_map,
         )
 
     def annotation_endpoint(self, datastack_name=None, use_stored=True):
         """AnnotationEngine endpoint for a dataset.
 
         Parameters
         ----------
@@ -331,15 +330,15 @@
             Formatted cloud path to the synapse segmentation
         """
         return self._get_property(
             "synapse_segmentation_source",
             datastack_name=datastack_name,
             use_stored=use_stored,
             format_for=format_for,
-            output_map=output_map_precomputed,
+            output_map=output_map,
         )
 
     def segmentation_source(
         self, datastack_name=None, format_for="raw", use_stored=True
     ):
         """Cloud path to the chunkgraph-backed Graphene segmentation for a dataset
 
@@ -360,15 +359,16 @@
         str
             Formatted cloud path to the Graphene segmentation
         """
         return self._get_property(
             "segmentation_source",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            output_map=output_map_raw,
+            output_map=output_map,
+            format_for=format_for,
         )
 
     def refresh_stored_data(self):
         """Reload the stored info values from the server."""
         for ds in self.info_cache.keys():
             self.get_datastack_info(datastack_name=ds, use_stored=False)
 
@@ -383,65 +383,61 @@
         Returns:
             np.array: voxel resolution as a len(3) np.array
         """
         vx = self._get_property(
             "viewer_resolution_x",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            format_for="raw",
         )
         vy = self._get_property(
             "viewer_resolution_y",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            format_for="raw",
         )
         vz = self._get_property(
             "viewer_resolution_z",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            format_for="raw",
         )
         return np.array([vx, vy, vz])
 
     def viewer_site(self, datastack_name=None, use_stored=True):
         """Get the base Neuroglancer URL for the dataset"""
         return self._get_property(
             "viewer_site",
             datastack_name=datastack_name,
             use_stored=use_stored,
-            format_for="raw",
         )
 
     def image_cloudvolume(self, **kwargs):
         """Generate a cloudvolume instance based on the image source, using authentication if needed and
         sensible default values for reading CAVE resources. By default, fill_missing is True and bounded
         is False. All keyword arguments are passed onto the CloudVolume initialization function, and defaults
         can be overridden.
 
         Requires cloudvolume to be installed, which is not included by default.
         """
-        return self._make_cloudvolume(self.image_source(), **kwargs)
+        return self._make_cloudvolume(self.image_source(format_for='cloudvolume'), **kwargs)
 
     def segmentation_cloudvolume(self, use_client_secret=True, **kwargs):
         """Generate a cloudvolume instance based on the segmentation source, using authentication if needed and
         sensible default values for reading CAVE resources. By default, fill_missing is True and bounded
         is False. All keyword arguments are passed onto the CloudVolume initialization function, and defaults
         can be overridden.
 
         Requires cloudvolume to be installed, which is not included by default.
         """
         return self._make_cloudvolume(
-            self.segmentation_source(), use_client_secret=use_client_secret, **kwargs
+            self.segmentation_source(format_for='cloudvolume'), use_client_secret=use_client_secret, **kwargs
         )
 
     def _make_cloudvolume(self, cloudpath, use_client_secret=True, **kwargs):
         try:
             import cloudvolume
-        except:
+        except ImportError:
             raise ImportError(
                 "Could not import cloudvolume. Make sure it is installed. See https://pypi.org/project/cloud-volume for more info."
             )
 
         use_https = kwargs.pop("use_https", True)
         bounded = kwargs.pop("bounded", False)
         fill_missing = kwargs.pop("fill_missing", True)
```

### Comparing `caveclient-5.4.2/caveclient/jsonservice.py` & `caveclient-5.5.0/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/l2cache.py` & `caveclient-5.5.0/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/materializationengine.py` & `caveclient-5.5.0/caveclient/materializationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/session_config.py` & `caveclient-5.5.0/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/timeit.py` & `caveclient-5.5.0/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/tools/caching.py` & `caveclient-5.5.0/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient/tools/stage.py` & `caveclient-5.5.0/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/caveclient.egg-info/SOURCES.txt` & `caveclient-5.5.0/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/setup.py` & `caveclient-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/tests/conftest.py` & `caveclient-5.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/tests/test_annotation.py` & `caveclient-5.5.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/tests/test_chunkedgraph.py` & `caveclient-5.5.0/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/tests/test_infoservice.py` & `caveclient-5.5.0/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.2/tests/test_materialization.py` & `caveclient-5.5.0/tests/test_materialization.py`

 * *Files identical despite different names*

