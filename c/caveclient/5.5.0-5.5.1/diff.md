# Comparing `tmp/caveclient-5.5.0.tar.gz` & `tmp/caveclient-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.5.0.tar", last modified: Wed May 10 16:29:22 2023, max compression
+gzip compressed data, was "caveclient-5.5.1.tar", last modified: Wed May 10 17:18:52 2023, max compression
```

## Comparing `caveclient-5.5.0.tar` & `caveclient-5.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.651450 caveclient-5.5.0/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.5.0/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 16:29:22.651233 caveclient-5.5.0/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.5.0/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.633972 caveclient-5.5.0/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 16:29:17.000000 caveclient-5.5.0/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.5.0/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.5.0/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.5.0/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.5.0/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.5.0/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.5.0/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.5.0/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    90661 2023-05-10 03:33:26.000000 caveclient-5.5.0/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.5.0/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.638002 caveclient-5.5.0/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.5.0/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.637180 caveclient-5.5.0/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 16:29:22.000000 caveclient-5.5.0/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.5.0/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 16:29:22.651508 caveclient-5.5.0/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.5.0/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 16:29:22.649782 caveclient-5.5.0/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.5.0/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.5.0/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.5.0/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.5.0/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 17:18:52.093921 caveclient-5.5.1/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.5.1/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 17:18:52.093682 caveclient-5.5.1/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.5.1/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 17:18:52.084578 caveclient-5.5.1/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-05-10 17:18:47.000000 caveclient-5.5.1/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.5.1/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.5.1/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.5.1/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.5.1/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.5.1/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11066 2023-04-29 14:05:03.000000 caveclient-5.5.1/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2407 2023-05-10 16:28:45.000000 caveclient-5.5.1/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.5.1/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16314 2023-05-10 16:28:45.000000 caveclient-5.5.1/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.5.1/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    90882 2023-05-10 17:18:31.000000 caveclient-5.5.1/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.5.1/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 17:18:52.087202 caveclient-5.5.1/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.5.1/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 17:18:52.086416 caveclient-5.5.1/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-05-10 17:18:51.000000 caveclient-5.5.1/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-05-10 17:18:52.000000 caveclient-5.5.1/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-10 17:18:51.000000 caveclient-5.5.1/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      119 2023-05-10 17:18:51.000000 caveclient-5.5.1/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-05-10 17:18:51.000000 caveclient-5.5.1/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      118 2023-05-10 03:33:26.000000 caveclient-5.5.1/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-05-10 17:18:52.093986 caveclient-5.5.1/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.5.1/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-10 17:18:52.093369 caveclient-5.5.1/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.5.1/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.5.1/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.5.1/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.5.1/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.5.1/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.5.1/tests/test_materialization.py
```

### Comparing `caveclient-5.5.0/README.rst` & `caveclient-5.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/annotationengine.py` & `caveclient-5.5.1/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/auth.py` & `caveclient-5.5.1/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/base.py` & `caveclient-5.5.1/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/chunkedgraph.py` & `caveclient-5.5.1/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/datastack_lookup.py` & `caveclient-5.5.1/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/emannotationschemas.py` & `caveclient-5.5.1/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/endpoints.py` & `caveclient-5.5.1/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/format_utils.py` & `caveclient-5.5.1/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/frameworkclient.py` & `caveclient-5.5.1/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/infoservice.py` & `caveclient-5.5.1/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/jsonservice.py` & `caveclient-5.5.1/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/l2cache.py` & `caveclient-5.5.1/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/materializationengine.py` & `caveclient-5.5.1/caveclient/materializationengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -766,15 +766,17 @@
                  Defaults to None.
              filter_spatial (dict of dicts, optional):
                  outer layer: keys are table names:
                  inner layer: keys are column names, values are bounding boxes
                               as [[min_x, min_y,min_z],[max_x, max_y, max_z]]
                               Expressed in units of the voxel_resolution of this dataset.
                  Defaults to None
-             select_columns (list of str, optional): columns to select. Defaults to None.
+             select_columns (dict of lists of str, optional): keys are table names,values are the list of columns from that table.
+               Defaults to None, which will select all tables.  Will be passed to server as select_column_maps.
+               Passing a list will be passed as select_columns which is deprecated.
              offset (int, optional): result offset to use. Defaults to None.
                  will only return top K results.
              limit (int, optional): maximum results to return (server will set upper limit, see get_server_config)
              suffixes (dict, optional): suffixes to use for duplicate columns, keys are table names, values are the suffix
              datastack_name (str, optional): datastack to query.
                  If None defaults to one specified in client.
              return_df (bool, optional): whether to return as a dataframe
@@ -1614,21 +1616,23 @@
             "datastack_name": self.datastack_name,
         }
         if not join_query:
             attrs["join_query"] = False
 
             if is_view:
                 meta = self.get_view_metadata(
-                    tables[0], log_warning=False, materialization_version=materialization_version
+                    tables[0],
+                    log_warning=False,
+                    materialization_version=materialization_version,
                 )
             else:
                 try:
-                    meta = self.get_table_metadata(tables[0], 
-                                                   log_warning=False,
-                                                   version=materialization_version)
+                    meta = self.get_table_metadata(
+                        tables[0], log_warning=False, version=materialization_version
+                    )
                 except HTTPError:
                     meta = self.fc.annotation.get_table_metadata(tables[0])
 
             for k, v in meta.items():
                 if re.match("^table", k):
                     attrs[k] = v
                 else:
```

### Comparing `caveclient-5.5.0/caveclient/session_config.py` & `caveclient-5.5.1/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/timeit.py` & `caveclient-5.5.1/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/tools/caching.py` & `caveclient-5.5.1/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient/tools/stage.py` & `caveclient-5.5.1/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/caveclient.egg-info/SOURCES.txt` & `caveclient-5.5.1/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/setup.py` & `caveclient-5.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/tests/conftest.py` & `caveclient-5.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/tests/test_annotation.py` & `caveclient-5.5.1/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/tests/test_chunkedgraph.py` & `caveclient-5.5.1/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/tests/test_infoservice.py` & `caveclient-5.5.1/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.5.0/tests/test_materialization.py` & `caveclient-5.5.1/tests/test_materialization.py`

 * *Files identical despite different names*

