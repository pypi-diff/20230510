# Comparing `tmp/caveclient-5.4.1.tar.gz` & `tmp/caveclient-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.4.1.tar", last modified: Wed May 10 02:36:25 2023, max compression
+gzip compressed data, was "caveclient-5.4.2.tar", last modified: Wed May 10 02:43:47 2023, max compression
```

## Comparing `caveclient-5.4.1.tar` & `caveclient-5.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:36:25.657257 caveclient-5.4.1/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.4.1/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:36:25.656359 caveclient-5.4.1/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.4.1/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:36:25.628700 caveclient-5.4.1/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 02:36:20.000000 caveclient-5.4.1/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.4.1/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.4.1/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.4.1/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.4.1/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.4.1/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.4.1/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.4.1/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.4.1/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.4.1/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.4.1/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    90350 2023-05-10 02:36:06.000000 caveclient-5.4.1/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.4.1/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:36:25.634384 caveclient-5.4.1/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.4.1/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:36:25.633343 caveclient-5.4.1/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:36:25.000000 caveclient-5.4.1/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 02:36:25.000000 caveclient-5.4.1/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 02:36:25.000000 caveclient-5.4.1/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-05-10 02:36:25.000000 caveclient-5.4.1/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 02:36:25.000000 caveclient-5.4.1/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      114 2023-05-10 02:35:52.000000 caveclient-5.4.1/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 02:36:25.657365 caveclient-5.4.1/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.4.1/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:36:25.654154 caveclient-5.4.1/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.4.1/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.4.1/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.4.1/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.4.1/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.4.1/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.4.1/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.325954 caveclient-5.4.2/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.4.2/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:43:47.325549 caveclient-5.4.2/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.4.2/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.315594 caveclient-5.4.2/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 02:43:43.000000 caveclient-5.4.2/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.4.2/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.4.2/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.4.2/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.4.2/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    90661 2023-05-10 02:43:35.000000 caveclient-5.4.2/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.4.2/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.319686 caveclient-5.4.2/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.4.2/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.317595 caveclient-5.4.2/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 02:43:47.000000 caveclient-5.4.2/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 02:43:35.000000 caveclient-5.4.2/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 02:43:47.326125 caveclient-5.4.2/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.4.2/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 02:43:47.325209 caveclient-5.4.2/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.4.2/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.4.2/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.4.2/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.4.2/tests/test_materialization.py
```

### Comparing `caveclient-5.4.1/README.rst` & `caveclient-5.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/annotationengine.py` & `caveclient-5.4.2/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/auth.py` & `caveclient-5.4.2/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/base.py` & `caveclient-5.4.2/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/chunkedgraph.py` & `caveclient-5.4.2/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/datastack_lookup.py` & `caveclient-5.4.2/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/emannotationschemas.py` & `caveclient-5.4.2/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/endpoints.py` & `caveclient-5.4.2/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/format_utils.py` & `caveclient-5.4.2/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/frameworkclient.py` & `caveclient-5.4.2/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/infoservice.py` & `caveclient-5.4.2/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/jsonservice.py` & `caveclient-5.4.2/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/l2cache.py` & `caveclient-5.4.2/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/materializationengine.py` & `caveclient-5.4.2/caveclient/materializationengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,14 @@
         response = self.session.get(url)
         d = handle_response(response)
         for md in d:
             md["time_stamp"] = convert_timestamp(md["time_stamp"])
             md["expires_on"] = convert_timestamp(md["expires_on"])
         return d
 
-    
     @cached(cache=TTLCache(maxsize=100, ttl=60 * 60 * 12))
     def get_table_metadata(
         self,
         table_name: str,
         datastack_name=None,
         version: int = None,
         log_warning: bool = True,
@@ -1606,27 +1605,31 @@
         if isinstance(tables, str):
             tables = [tables]
         if isinstance(desired_resolution, str):
             desired_resolution = np.array(
                 [float(r) for r in desired_resolution.split(", ")]
             )
         join_query = len(tables) > 1
-
+        materialization_version = kwargs.get("materialization_version", None)
         attrs = {
             "datastack_name": self.datastack_name,
         }
         if not join_query:
             attrs["join_query"] = False
 
             if is_view:
-                meta = self.get_view_metadata(tables[0], log_warning=False)
+                meta = self.get_view_metadata(
+                    tables[0], log_warning=False, materialization_version=materialization_version
+                )
             else:
                 try:
-                    meta = self.get_table_metadata(tables[0], log_warning=False)
-                except:
+                    meta = self.get_table_metadata(tables[0], 
+                                                   log_warning=False,
+                                                   version=materialization_version)
+                except HTTPError:
                     meta = self.fc.annotation.get_table_metadata(tables[0])
 
             for k, v in meta.items():
                 if re.match("^table", k):
                     attrs[k] = v
                 else:
                     attrs[f"table_{k}"] = v
@@ -1640,15 +1643,15 @@
             table_attrs = attrs["tables"]
             if suffixes is None:
                 suffixes = ["_x", "_y"]
             for (tname, jcol), s in zip(tables, suffixes):
                 table_attrs[tname] = {}
                 try:
                     meta = self.get_table_metadata(tname, log_warning=False)
-                except:
+                except HTTPError:
                     meta = self.fc.annotation.get_table_metadata(tname)
                 for k, v in meta.items():
                     if re.match("^table", k):
                         table_attrs[tname][k] = v
                     else:
                         table_attrs[tname][f"table_{k}"] = v
                 table_attrs[tname]["join_column"] = jcol
@@ -1709,15 +1712,15 @@
         all_metadata = handle_response(response, log_warning=log_warning)
         for metadata_d in all_metadata:
             vx = metadata_d.pop("voxel_resolution_x", None)
             vy = metadata_d.pop("voxel_resolution_y", None)
             vz = metadata_d.pop("voxel_resolution_z", None)
             metadata_d["voxel_resolution"] = [vx, vy, vz]
         return all_metadata
-    
+
     def live_live_query(
         self,
         table: str,
         timestamp: datetime,
         joins=None,
         filter_in_dict=None,
         filter_out_dict=None,
```

### Comparing `caveclient-5.4.1/caveclient/session_config.py` & `caveclient-5.4.2/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/timeit.py` & `caveclient-5.4.2/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/tools/caching.py` & `caveclient-5.4.2/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient/tools/stage.py` & `caveclient-5.4.2/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/caveclient.egg-info/SOURCES.txt` & `caveclient-5.4.2/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/setup.py` & `caveclient-5.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/tests/conftest.py` & `caveclient-5.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/tests/test_annotation.py` & `caveclient-5.4.2/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/tests/test_chunkedgraph.py` & `caveclient-5.4.2/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/tests/test_infoservice.py` & `caveclient-5.4.2/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.4.1/tests/test_materialization.py` & `caveclient-5.4.2/tests/test_materialization.py`

 * *Files identical despite different names*

