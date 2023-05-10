# Comparing `tmp/aie-sdk-2.2.1.tar.gz` & `tmp/aie-sdk-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-2.2.1.tar", last modified: Fri Mar 17 10:01:12 2023, max compression
+gzip compressed data, was "aie-sdk-2.2.2.tar", last modified: Wed May 10 08:11:13 2023, max compression
```

## Comparing `aie-sdk-2.2.1.tar` & `aie-sdk-2.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.024569 aie-sdk-2.2.1/
--rw-r--r--   0 songci     (502) staff       (20)     1068 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/LICENSE
--rw-r--r--   0 songci     (502) staff       (20)       21 2022-12-01 11:50:21.000000 aie-sdk-2.2.1/MANIFEST.in
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-03-17 10:01:12.023992 aie-sdk-2.2.1/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:11.991687 aie-sdk-2.2.1/aie/
--rw-r--r--   0 songci     (502) staff       (20)      974 2023-03-17 10:01:10.000000 aie-sdk-2.2.1/aie/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2302 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/aie_env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.001143 aie-sdk-2.2.1/aie/aie_object/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/aie_object/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)    16729 2023-03-17 10:01:08.000000 aie-sdk-2.2.1/aie/aie_object/classifier.py
--rw-r--r--   0 songci     (502) staff       (20)     5225 2023-03-17 10:00:59.000000 aie-sdk-2.2.1/aie/aie_object/collection.py
--rw-r--r--   0 songci     (502) staff       (20)     2996 2023-03-17 10:01:09.000000 aie-sdk-2.2.1/aie/aie_object/confusion_matrix.py
--rw-r--r--   0 songci     (502) staff       (20)    23049 2023-03-17 10:01:02.000000 aie-sdk-2.2.1/aie/aie_object/feature.py
--rw-r--r--   0 songci     (502) staff       (20)    26855 2023-03-17 10:01:03.000000 aie-sdk-2.2.1/aie/aie_object/feature_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    22797 2023-03-17 10:01:05.000000 aie-sdk-2.2.1/aie/aie_object/filter.py
--rw-r--r--   0 songci     (502) staff       (20)    24135 2023-03-17 10:01:01.000000 aie-sdk-2.2.1/aie/aie_object/geometry.py
--rw-r--r--   0 songci     (502) staff       (20)    72624 2023-03-17 10:00:58.000000 aie-sdk-2.2.1/aie/aie_object/image.py
--rw-r--r--   0 songci     (502) staff       (20)    10314 2023-03-17 10:01:00.000000 aie-sdk-2.2.1/aie/aie_object/image_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    29114 2023-03-17 10:01:07.000000 aie-sdk-2.2.1/aie/aie_object/kernel.py
--rw-r--r--   0 songci     (502) staff       (20)     1463 2023-03-17 10:01:09.000000 aie-sdk-2.2.1/aie/aie_object/model.py
--rw-r--r--   0 songci     (502) staff       (20)    11680 2023-03-17 10:01:05.000000 aie-sdk-2.2.1/aie/aie_object/reducer.py
--rw-r--r--   0 songci     (502) staff       (20)     2961 2023-03-17 10:01:06.000000 aie-sdk-2.2.1/aie/aie_object/terrain.py
--rw-r--r--   0 songci     (502) staff       (20)     2570 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/auth.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.010524 aie-sdk-2.2.1/aie/client/
--rw-r--r--   0 songci     (502) staff       (20)      275 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     6490 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/client.py
--rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/constants.py
--rw-r--r--   0 songci     (502) staff       (20)     3278 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/dataset.py
--rw-r--r--   0 songci     (502) staff       (20)     1370 2022-11-21 11:41:47.000000 aie-sdk-2.2.1/aie/client/endpoints.py
--rw-r--r--   0 songci     (502) staff       (20)     7371 2023-03-10 07:28:16.000000 aie-sdk-2.2.1/aie/client/interactive_session.py
--rw-r--r--   0 songci     (502) staff       (20)     1647 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/maps.py
--rw-r--r--   0 songci     (502) staff       (20)    15854 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/mlproxy.py
--rw-r--r--   0 songci     (502) staff       (20)    18381 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/mlproxy_back.py
--rw-r--r--   0 songci     (502) staff       (20)     2542 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/client/task.py
--rw-r--r--   0 songci     (502) staff       (20)      232 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/customfunction_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.012334 aie-sdk-2.2.1/aie/error/
--rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/error/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/error/aie_error.py
--rw-r--r--   0 songci     (502) staff       (20)     4264 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/export.py
--rw-r--r--   0 songci     (502) staff       (20)     1706 2023-03-06 07:01:53.000000 aie-sdk-2.2.1/aie/function_helper.py
--rw-r--r--   0 songci     (502) staff       (20)      500 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/function_node.py
--rw-r--r--   0 songci     (502) staff       (20)      907 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/g_var.py
--rw-r--r--   0 songci     (502) staff       (20)    11531 2022-12-09 06:48:05.000000 aie-sdk-2.2.1/aie/gen_python_functions.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.016672 aie-sdk-2.2.1/aie/map/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/map/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aie-sdk-2.2.1/aie/map/aie_color.py
--rw-r--r--   0 songci     (502) staff       (20)     8578 2022-12-01 11:50:21.000000 aie-sdk-2.2.1/aie/map/aie_layer.py
--rw-r--r--   0 songci     (502) staff       (20)     4947 2022-12-01 11:50:21.000000 aie-sdk-2.2.1/aie/map/aie_map.py
--rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aie-sdk-2.2.1/aie/map/color.csv
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.019704 aie-sdk-2.2.1/aie/serialize/
--rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/serialize/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     4678 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/serialize/gen_visitor.py
--rw-r--r--   0 songci     (502) staff       (20)     3380 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/serialize/optimizer.py
--rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/serialize/serializer_impl.py
--rw-r--r--   0 songci     (502) staff       (20)      269 2022-11-21 06:06:45.000000 aie-sdk-2.2.1/aie/variable_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-03-17 10:01:12.023193 aie-sdk-2.2.1/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-03-17 10:01:11.000000 aie-sdk-2.2.1/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)     1271 2023-03-17 10:01:11.000000 aie-sdk-2.2.1/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-03-17 10:01:11.000000 aie-sdk-2.2.1/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)       79 2023-03-17 10:01:11.000000 aie-sdk-2.2.1/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-03-17 10:01:11.000000 aie-sdk-2.2.1/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-03-17 10:01:12.024711 aie-sdk-2.2.1/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)      891 2023-02-17 02:27:00.000000 aie-sdk-2.2.1/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.761615 aie-sdk-2.2.2/
+-rw-r--r--   0 songci     (502) staff       (20)     1068 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/LICENSE
+-rw-r--r--   0 songci     (502) staff       (20)       21 2023-04-13 02:48:48.000000 aie-sdk-2.2.2/MANIFEST.in
+-rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-10 08:11:13.761139 aie-sdk-2.2.2/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.730507 aie-sdk-2.2.2/aie/
+-rw-r--r--   0 songci     (502) staff       (20)     1128 2023-05-10 08:11:12.000000 aie-sdk-2.2.2/aie/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2302 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/aie_env.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.739431 aie-sdk-2.2.2/aie/aie_object/
+-rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/aie_object/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)    16729 2023-05-10 08:11:11.000000 aie-sdk-2.2.2/aie/aie_object/classifier.py
+-rw-r--r--   0 songci     (502) staff       (20)     5225 2023-05-10 08:11:04.000000 aie-sdk-2.2.2/aie/aie_object/collection.py
+-rw-r--r--   0 songci     (502) staff       (20)     2996 2023-05-10 08:11:11.000000 aie-sdk-2.2.2/aie/aie_object/confusion_matrix.py
+-rw-r--r--   0 songci     (502) staff       (20)    25064 2023-05-10 08:11:06.000000 aie-sdk-2.2.2/aie/aie_object/feature.py
+-rw-r--r--   0 songci     (502) staff       (20)    27878 2023-05-10 08:11:07.000000 aie-sdk-2.2.2/aie/aie_object/feature_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    22797 2023-05-10 08:11:08.000000 aie-sdk-2.2.2/aie/aie_object/filter.py
+-rw-r--r--   0 songci     (502) staff       (20)    24135 2023-05-10 08:11:05.000000 aie-sdk-2.2.2/aie/aie_object/geometry.py
+-rw-r--r--   0 songci     (502) staff       (20)    81753 2023-05-10 08:11:03.000000 aie-sdk-2.2.2/aie/aie_object/image.py
+-rw-r--r--   0 songci     (502) staff       (20)    23330 2023-05-10 08:11:05.000000 aie-sdk-2.2.2/aie/aie_object/image_collection.py
+-rw-r--r--   0 songci     (502) staff       (20)    29114 2023-05-10 08:11:10.000000 aie-sdk-2.2.2/aie/aie_object/kernel.py
+-rw-r--r--   0 songci     (502) staff       (20)     1463 2023-05-10 08:11:12.000000 aie-sdk-2.2.2/aie/aie_object/model.py
+-rw-r--r--   0 songci     (502) staff       (20)    13998 2023-05-10 08:11:09.000000 aie-sdk-2.2.2/aie/aie_object/reducer.py
+-rw-r--r--   0 songci     (502) staff       (20)     2961 2023-05-10 08:11:09.000000 aie-sdk-2.2.2/aie/aie_object/terrain.py
+-rw-r--r--   0 songci     (502) staff       (20)     2570 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/auth.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.747304 aie-sdk-2.2.2/aie/client/
+-rw-r--r--   0 songci     (502) staff       (20)      275 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     6490 2023-05-10 08:10:26.000000 aie-sdk-2.2.2/aie/client/client.py
+-rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/constants.py
+-rw-r--r--   0 songci     (502) staff       (20)     3278 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/dataset.py
+-rw-r--r--   0 songci     (502) staff       (20)     1370 2022-11-21 11:41:47.000000 aie-sdk-2.2.2/aie/client/endpoints.py
+-rw-r--r--   0 songci     (502) staff       (20)     7371 2023-05-10 08:10:26.000000 aie-sdk-2.2.2/aie/client/interactive_session.py
+-rw-r--r--   0 songci     (502) staff       (20)     1647 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/maps.py
+-rw-r--r--   0 songci     (502) staff       (20)    15854 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/mlproxy.py
+-rw-r--r--   0 songci     (502) staff       (20)    18381 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/client/mlproxy_back.py
+-rw-r--r--   0 songci     (502) staff       (20)     2543 2023-05-08 04:13:45.000000 aie-sdk-2.2.2/aie/client/task.py
+-rw-r--r--   0 songci     (502) staff       (20)      232 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/customfunction_node.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.748984 aie-sdk-2.2.2/aie/error/
+-rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/error/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/error/aie_error.py
+-rw-r--r--   0 songci     (502) staff       (20)     4264 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/export.py
+-rw-r--r--   0 songci     (502) staff       (20)     1706 2023-04-10 02:23:35.000000 aie-sdk-2.2.2/aie/function_helper.py
+-rw-r--r--   0 songci     (502) staff       (20)      500 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/function_node.py
+-rw-r--r--   0 songci     (502) staff       (20)      907 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/g_var.py
+-rw-r--r--   0 songci     (502) staff       (20)    11531 2022-12-09 06:48:05.000000 aie-sdk-2.2.2/aie/gen_python_functions.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.753688 aie-sdk-2.2.2/aie/map/
+-rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/map/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_color.py
+-rw-r--r--   0 songci     (502) staff       (20)     8578 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_layer.py
+-rw-r--r--   0 songci     (502) staff       (20)     4947 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/aie_map.py
+-rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aie-sdk-2.2.2/aie/map/color.csv
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.757385 aie-sdk-2.2.2/aie/serialize/
+-rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/__init__.py
+-rw-r--r--   0 songci     (502) staff       (20)     4678 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/gen_visitor.py
+-rw-r--r--   0 songci     (502) staff       (20)     3380 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/optimizer.py
+-rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/serialize/serializer_impl.py
+-rw-r--r--   0 songci     (502) staff       (20)      269 2022-11-21 06:06:45.000000 aie-sdk-2.2.2/aie/variable_node.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-10 08:11:13.760466 aie-sdk-2.2.2/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)     1271 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)       79 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-05-10 08:11:13.000000 aie-sdk-2.2.2/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-05-10 08:11:13.761754 aie-sdk-2.2.2/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)      891 2023-04-13 02:48:49.000000 aie-sdk-2.2.2/setup.py
```

### Comparing `aie-sdk-2.2.1/LICENSE` & `aie-sdk-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/__init__.py` & `aie-sdk-2.2.2/aie/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
+import sys
 import aie
 from .aie_env import AIEEnv
 from aie.map.aie_map import Map
 from aie.export import Export
 import types
 
 
@@ -37,9 +38,15 @@
 from aie.aie_object.model import Model
 
 
 def Authenticate(token=None):
     aie.auth.Authenticate.auth(token)
 
 
-def Initialize(debug_level=aie.g_var.LogLevel.INFO_LEVEL):
+def Initialize(debug_level=aie.g_var.LogLevel.INFO_LEVEL, debug=False):
+    if debug:
+        debug_level = aie.g_var.LogLevel.DEBUG_LEVEL
     AIEEnv.init(debug_level)
+
+
+def se(obj):
+    return aie.serialize.serializer.encode(obj)
```

### Comparing `aie-sdk-2.2.1/aie/aie_env.py` & `aie-sdk-2.2.2/aie/aie_env.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/classifier.py` & `aie-sdk-2.2.2/aie/aie_object/classifier.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/collection.py` & `aie-sdk-2.2.2/aie/aie_object/collection.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/confusion_matrix.py` & `aie-sdk-2.2.2/aie/aie_object/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/feature.py` & `aie-sdk-2.2.2/aie/aie_object/feature.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
-            "dict": self,
+            "input": self,
             "property": property,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
@@ -669,7 +669,66 @@
         if "offset" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数offset不能为空")
 
         if "maxAngle" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数maxAngle不能为空")
 
         return FunctionHelper.apply("Feature.smooth", "aie.Feature", invoke_args)
+
+    def getNumber(self, property: str) -> object:
+
+        if property is not None and not isinstance(property, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "property": property,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "property" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
+
+        return FunctionHelper.apply("Feature.getNumber", "object", invoke_args)
+
+    def getString(self, property: str) -> object:
+
+        if property is not None and not isinstance(property, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "property": property,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "property" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
+
+        return FunctionHelper.apply("Feature.getString", "object", invoke_args)
+
+    def renamePropertyNames(self, var_args: dict) -> aie.Feature:
+
+        if var_args is not None and not isinstance(var_args, dict):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "var_args": var_args,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "var_args" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
+
+        return FunctionHelper.apply(
+            "Feature.renamePropertyNames", "aie.Feature", invoke_args
+        )
```

### Comparing `aie-sdk-2.2.1/aie/aie_object/feature_collection.py` & `aie-sdk-2.2.2/aie/aie_object/feature_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,18 +469,24 @@
         if "properties" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数properties不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.distinct", "aie.FeatureCollection", invoke_args
         )
 
-    def map(self, baseAlgorithm: types.FunctionType) -> aie.FeatureCollection:
+    def map(
+        self, baseAlgorithm: types.FunctionType
+    ) -> Union[aie.ImageCollection, aie.FeatureCollection]:
 
         node = super(FeatureCollection, self).map(baseAlgorithm)
-        return FunctionHelper.cast(node, "aie.FeatureCollection")
+        baseAlgorithm_return_type = type(node.invoke_args["baseAlgorithm"].body)
+        if aie.Image == baseAlgorithm_return_type:
+            return FunctionHelper.cast(node, "aie.ImageCollection")
+        else:
+            return FunctionHelper.cast(node, "aie.FeatureCollection")
 
     def merge(self, collection2: aie.FeatureCollection) -> aie.FeatureCollection:
 
         if collection2 is not None and not isinstance(
             collection2, aie.FeatureCollection
         ):
             raise AIEError(
@@ -764,7 +770,30 @@
 
         if "predicted" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数predicted不能为空")
 
         return FunctionHelper.apply(
             "FeatureCollection.errorMatrix", "aie.ConfusionMatrix", invoke_args
         )
+
+    def renamePropertyNames(self, var_args: dict) -> aie.FeatureCollection:
+
+        if var_args is not None and not isinstance(var_args, dict):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "var_args": var_args,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "var_args" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
+
+        return FunctionHelper.apply(
+            "FeatureCollection.renamePropertyNames",
+            "aie.FeatureCollection",
+            invoke_args,
+        )
```

### Comparing `aie-sdk-2.2.1/aie/aie_object/filter.py` & `aie-sdk-2.2.2/aie/aie_object/filter.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/geometry.py` & `aie-sdk-2.2.2/aie/aie_object/geometry.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/image.py` & `aie-sdk-2.2.2/aie/aie_object/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1400,15 +1400,15 @@
 
         if property is not None and not isinstance(property, str):
             raise AIEError(
                 AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
             )
 
         invoke_args = {
-            "object": self,
+            "input": self,
             "property": property,
         }
 
         invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
 
         if "property" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
@@ -2176,7 +2176,269 @@
 
         if "numPixels" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数numPixels不能为空")
 
         return FunctionHelper.apply(
             "Image.sample", "aie.FeatureCollection", invoke_args
         )
+
+    def mask(self) -> aie.Image:
+
+        invoke_args = {
+            "input": self,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Image.mask", "aie.Image", invoke_args)
+
+    def id(self) -> object:
+
+        invoke_args = {
+            "input": self,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Image.id", "object", invoke_args)
+
+    def getNumber(self, property: str) -> object:
+
+        if property is not None and not isinstance(property, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "property": property,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "property" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
+
+        return FunctionHelper.apply("Image.getNumber", "object", invoke_args)
+
+    def getString(self, property: str) -> object:
+
+        if property is not None and not isinstance(property, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"property 只支持str类型参数, 传入类型为{type(property)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "property": property,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "property" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数property不能为空")
+
+        return FunctionHelper.apply("Image.getString", "object", invoke_args)
+
+    def random(self, seed: int = 0, distribution: str = "uniform") -> aie.Image:
+
+        if seed is not None and not isinstance(seed, int):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"seed 只支持int类型参数, 传入类型为{type(seed)}"
+            )
+
+        if distribution is not None and not isinstance(distribution, str):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"distribution 只支持str类型参数, 传入类型为{type(distribution)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "seed": seed,
+            "distribution": distribution,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Image.random", "aie.Image", invoke_args)
+
+    def sampleRegion(
+        self, region: aie.Geometry, scale: [int, float], geometries: bool = False
+    ) -> aie.FeatureCollection:
+
+        if region is not None and not isinstance(region, aie.Geometry):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"region 只支持aie.Geometry类型参数, 传入类型为{type(region)}",
+            )
+
+        if scale is not None and not isinstance(scale, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"scale 只支持(int,float)类型参数, 传入类型为{type(scale)}"
+            )
+
+        if geometries is not None and not isinstance(geometries, bool):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"geometries 只支持bool类型参数, 传入类型为{type(geometries)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "region": region,
+            "scale": scale,
+            "geometries": geometries,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "region" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数region不能为空")
+
+        if "scale" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数scale不能为空")
+
+        return FunctionHelper.apply(
+            "Image.sampleRegion", "aie.FeatureCollection", invoke_args
+        )
+
+    def sampleRegions(
+        self,
+        collection: aie.FeatureCollection,
+        scale: [int, float],
+        properties: list = None,
+        geometries: bool = False,
+    ) -> aie.FeatureCollection:
+
+        if collection is not None and not isinstance(collection, aie.FeatureCollection):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
+            )
+
+        if scale is not None and not isinstance(scale, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"scale 只支持(int,float)类型参数, 传入类型为{type(scale)}"
+            )
+
+        if properties is not None and not isinstance(properties, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"properties 只支持list类型参数, 传入类型为{type(properties)}",
+            )
+
+        if geometries is not None and not isinstance(geometries, bool):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"geometries 只支持bool类型参数, 传入类型为{type(geometries)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "collection": collection,
+            "scale": scale,
+            "properties": properties,
+            "geometries": geometries,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "collection" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数collection不能为空")
+
+        if "scale" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数scale不能为空")
+
+        return FunctionHelper.apply(
+            "Image.sampleRegions", "aie.FeatureCollection", invoke_args
+        )
+
+    def samplePoints(
+        self,
+        collection: aie.FeatureCollection,
+        scale: [int, float],
+        properties: list = None,
+        geometries: bool = False,
+    ) -> aie.FeatureCollection:
+
+        if collection is not None and not isinstance(collection, aie.FeatureCollection):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"collection 只支持aie.FeatureCollection类型参数, 传入类型为{type(collection)}",
+            )
+
+        if scale is not None and not isinstance(scale, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"scale 只支持(int,float)类型参数, 传入类型为{type(scale)}"
+            )
+
+        if properties is not None and not isinstance(properties, list):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"properties 只支持list类型参数, 传入类型为{type(properties)}",
+            )
+
+        if geometries is not None and not isinstance(geometries, bool):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"geometries 只支持bool类型参数, 传入类型为{type(geometries)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "collection": collection,
+            "scale": scale,
+            "properties": properties,
+            "geometries": geometries,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "collection" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数collection不能为空")
+
+        if "scale" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数scale不能为空")
+
+        return FunctionHelper.apply(
+            "Image.samplePoints", "aie.FeatureCollection", invoke_args
+        )
+
+    def cast(self, bandTypes: dict) -> aie.Image:
+
+        if bandTypes is not None and not isinstance(bandTypes, dict):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"bandTypes 只支持dict类型参数, 传入类型为{type(bandTypes)}",
+            )
+
+        invoke_args = {
+            "input": self,
+            "bandTypes": bandTypes,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "bandTypes" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数bandTypes不能为空")
+
+        return FunctionHelper.apply("Image.cast", "aie.Image", invoke_args)
+
+    def set(self, var_args: dict) -> aie.Image:
+
+        if var_args is not None and not isinstance(var_args, dict):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR, f"var_args 只支持dict类型参数, 传入类型为{type(var_args)}"
+            )
+
+        invoke_args = {
+            "input": self,
+            "var_args": var_args,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        if "var_args" not in invoke_args:
+            raise AIEError(AIEErrorCode.ARGS_ERROR, "参数var_args不能为空")
+
+        return FunctionHelper.apply("Image.set", "aie.Image", invoke_args)
```

### Comparing `aie-sdk-2.2.1/aie/aie_object/kernel.py` & `aie-sdk-2.2.2/aie/aie_object/kernel.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/model.py` & `aie-sdk-2.2.2/aie/aie_object/model.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/aie_object/reducer.py` & `aie-sdk-2.2.2/aie/aie_object/reducer.py`

 * *Files 11% similar despite different names*

```diff
@@ -354,7 +354,87 @@
 
         if "buckets" not in invoke_args:
             raise AIEError(AIEErrorCode.ARGS_ERROR, "参数buckets不能为空")
 
         return FunctionHelper.apply(
             "Reducer.fixedHistogram", "aie.Reducer", invoke_args
         )
+
+    @staticmethod
+    def linearFit() -> aie.Reducer:
+
+        invoke_args = {}
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply("Reducer.linearFit", "aie.Reducer", invoke_args)
+
+    @staticmethod
+    def linearRegression() -> aie.Reducer:
+
+        invoke_args = {}
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply(
+            "Reducer.linearRegression", "aie.Reducer", invoke_args
+        )
+
+    @staticmethod
+    def pearsonsCorrelation() -> aie.Reducer:
+
+        invoke_args = {}
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply(
+            "Reducer.pearsonsCorrelation", "aie.Reducer", invoke_args
+        )
+
+    @staticmethod
+    def spearmansCorrelation() -> aie.Reducer:
+
+        invoke_args = {}
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply(
+            "Reducer.spearmansCorrelation", "aie.Reducer", invoke_args
+        )
+
+    @staticmethod
+    def ridgeRegression(regParam: [int, float] = 0.1) -> aie.Reducer:
+
+        if regParam is not None and not isinstance(regParam, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"regParam 只支持(int,float)类型参数, 传入类型为{type(regParam)}",
+            )
+
+        invoke_args = {
+            "regParam": regParam,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply(
+            "Reducer.ridgeRegression", "aie.Reducer", invoke_args
+        )
+
+    @staticmethod
+    def lassoRegression(regParam: [int, float] = 0.1) -> aie.Reducer:
+
+        if regParam is not None and not isinstance(regParam, (int, float)):
+            raise AIEError(
+                AIEErrorCode.ARGS_ERROR,
+                f"regParam 只支持(int,float)类型参数, 传入类型为{type(regParam)}",
+            )
+
+        invoke_args = {
+            "regParam": regParam,
+        }
+
+        invoke_args = {k: v for k, v in invoke_args.items() if v is not None}
+
+        return FunctionHelper.apply(
+            "Reducer.lassoRegression", "aie.Reducer", invoke_args
+        )
```

### Comparing `aie-sdk-2.2.1/aie/aie_object/terrain.py` & `aie-sdk-2.2.2/aie/aie_object/terrain.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/auth.py` & `aie-sdk-2.2.2/aie/auth.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/client.py` & `aie-sdk-2.2.2/aie/client/client.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/constants.py` & `aie-sdk-2.2.2/aie/client/constants.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/dataset.py` & `aie-sdk-2.2.2/aie/client/dataset.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/endpoints.py` & `aie-sdk-2.2.2/aie/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/interactive_session.py` & `aie-sdk-2.2.2/aie/client/interactive_session.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/maps.py` & `aie-sdk-2.2.2/aie/client/maps.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/mlproxy.py` & `aie-sdk-2.2.2/aie/client/mlproxy.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/mlproxy_back.py` & `aie-sdk-2.2.2/aie/client/mlproxy_back.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/client/task.py` & `aie-sdk-2.2.2/aie/client/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import aie
 from aie.serialize import serializer
 from aie.error import AIEError, AIEErrorCode
 
 
 class Task(object):
     class StatusCode(object):
-        WAITING = "wating"
+        WAITING = "waiting"
         RUNNING = "running"
         COMPLETED = "completed"
         FAILED = "failed"
         CANCEL_REQUEST = "cancel_request"
         CANCELLED = "cancelled"
 
     class Status(object):
```

### Comparing `aie-sdk-2.2.1/aie/error/aie_error.py` & `aie-sdk-2.2.2/aie/error/aie_error.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/export.py` & `aie-sdk-2.2.2/aie/export.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/function_helper.py` & `aie-sdk-2.2.2/aie/function_helper.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/g_var.py` & `aie-sdk-2.2.2/aie/g_var.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/gen_python_functions.py` & `aie-sdk-2.2.2/aie/gen_python_functions.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/map/aie_color.py` & `aie-sdk-2.2.2/aie/map/aie_color.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/map/aie_layer.py` & `aie-sdk-2.2.2/aie/map/aie_layer.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/map/aie_map.py` & `aie-sdk-2.2.2/aie/map/aie_map.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/map/color.csv` & `aie-sdk-2.2.2/aie/map/color.csv`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/serialize/gen_visitor.py` & `aie-sdk-2.2.2/aie/serialize/gen_visitor.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/serialize/optimizer.py` & `aie-sdk-2.2.2/aie/serialize/optimizer.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie/serialize/serializer_impl.py` & `aie-sdk-2.2.2/aie/serialize/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/aie_sdk.egg-info/SOURCES.txt` & `aie-sdk-2.2.2/aie_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aie-sdk-2.2.1/setup.py` & `aie-sdk-2.2.2/setup.py`

 * *Files identical despite different names*

