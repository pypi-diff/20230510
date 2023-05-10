# Comparing `tmp/fabric_fim-1.4.9.tar.gz` & `tmp/fabric_fim-1.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.4.9.tar", last modified: Sat Apr  8 04:38:05 2023, max compression
+gzip compressed data, was "fabric_fim-1.5.0b1.tar", last modified: Wed May 10 17:53:45 2023, max compression
```

## Comparing `fabric_fim-1.4.9.tar` & `fabric_fim-1.5.0b1.tar`

### file list

```diff
@@ -1,99 +1,119 @@
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.352826 fabric_fim-1.4.9/
--rw-r--r--   0 ibaldin    (502) staff       (20)       26 2020-07-24 21:42:44.000000 fabric_fim-1.4.9/AUTHORS
--rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2020-07-14 22:09:49.000000 fabric_fim-1.4.9/LICENSE
--rw-r--r--   0 ibaldin    (502) staff       (20)      146 2022-04-27 22:22:19.000000 fabric_fim-1.4.9/MANIFEST.in
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-08 04:38:05.352150 fabric_fim-1.4.9/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)    10990 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/README.md
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.300879 fabric_fim-1.4.9/fabric_fim.egg-info/
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)     2324 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/SOURCES.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/dependency_links.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/requires.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        4 2023-04-08 04:38:05.000000 fabric_fim-1.4.9/fabric_fim.egg-info/top_level.txt
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.302372 fabric_fim-1.4.9/fim/
--rw-r--r--   0 ibaldin    (502) staff       (20)       22 2023-04-08 04:37:46.000000 fabric_fim-1.4.9/fim/__init__.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.304078 fabric_fim-1.4.9/fim/authz/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2022-04-27 22:22:19.000000 fabric_fim-1.4.9/fim/authz/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    16139 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/authz/attribute_collector.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.311071 fabric_fim-1.4.9/fim/graph/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:31:38.000000 fabric_fim-1.4.9/fim/graph/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    69794 2023-04-08 04:33:53.000000 fabric_fim-1.4.9/fim/graph/abc_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4093 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/graph/abc_property_graph_constants.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.315925 fabric_fim-1.4.9/fim/graph/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-08-18 21:34:07.000000 fabric_fim-1.4.9/fim/graph/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      283 2020-09-03 22:10:53.000000 fabric_fim-1.4.9/fim/graph/data/capacity_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      100 2020-08-27 20:41:23.000000 fabric_fim-1.4.9/fim/graph/data/constraint_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)     3829 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      547 2020-09-03 22:10:39.000000 fabric_fim-1.4.9/fim/graph/data/label_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)       91 2020-08-27 20:40:54.000000 fabric_fim-1.4.9/fim/graph/data/location_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      367 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    43529 2023-04-08 04:34:03.000000 fabric_fim-1.4.9/fim/graph/neo4j_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6160 2022-10-06 17:38:08.000000 fabric_fim-1.4.9/fim/graph/networkx_mixin.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    42098 2023-04-08 04:33:57.000000 fabric_fim-1.4.9/fim/graph/networkx_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8354 2022-10-07 03:05:34.000000 fabric_fim-1.4.9/fim/graph/networkx_property_graph_disjoint.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.326417 fabric_fim-1.4.9/fim/graph/resources/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:04.000000 fabric_fim-1.4.9/fim/graph/resources/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4484 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/abc_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13570 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/resources/abc_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2991 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/resources/abc_bqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4547 2021-03-31 01:14:29.000000 fabric_fim-1.4.9/fim/graph/resources/abc_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2297 2021-03-07 22:42:30.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2106 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    18425 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5017 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2341 2021-03-07 22:42:30.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2122 2021-05-25 21:09:37.000000 fabric_fim-1.4.9/fim/graph/resources/networkx_arm.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.329026 fabric_fim-1.4.9/fim/graph/slices/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:24.000000 fabric_fim-1.4.9/fim/graph/slices/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8223 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/graph/slices/abc_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3713 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4298 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/graph/slices/networkx_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8615 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/graph/typed_tuples.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.329524 fabric_fim-1.4.9/fim/logging/
--rw-r--r--   0 ibaldin    (502) staff       (20)        0 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/logging/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9071 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/logging/log_collector.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9555 2021-03-24 00:18:51.000000 fabric_fim-1.4.9/fim/pluggable.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.340823 fabric_fim-1.4.9/fim/slivers/
--rw-r--r--   0 ibaldin    (502) staff       (20)      217 2021-06-14 18:36:21.000000 fabric_fim-1.4.9/fim/slivers/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3641 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/attached_components.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13021 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/base_sliver.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    24078 2023-04-08 04:20:22.000000 fabric_fim-1.4.9/fim/slivers/capacities_labels.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11269 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/slivers/component_catalog.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.342257 fabric_fim-1.4.9/fim/slivers/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/slivers/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1657 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/fim/slivers/data/component_catalog.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    76943 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/slivers/data/instance_sizes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    23524 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/delegations.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3593 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/gateway.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      919 2021-06-29 20:04:13.000000 fabric_fim-1.4.9/fim/slivers/identifiers.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3444 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/instance_catalog.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3225 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/interface_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2702 2021-09-22 14:46:40.000000 fabric_fim-1.4.9/fim/slivers/json.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3869 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/json_data.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5983 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/maintenance_mode.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1566 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/slivers/network_attached_storage.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3910 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/network_link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    10209 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/network_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    22042 2023-04-05 22:02:35.000000 fabric_fim-1.4.9/fim/slivers/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6795 2021-06-04 19:43:14.000000 fabric_fim-1.4.9/fim/slivers/path_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3024 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/fim/slivers/tags.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2622 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/slivers/topology_diff.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.349853 fabric_fim-1.4.9/fim/user/
--rw-r--r--   0 ibaldin    (502) staff       (20)     1914 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/user/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11730 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/component.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5668 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/composite_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     7660 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/fim/user/interface.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8381 2022-09-10 21:18:41.000000 fabric_fim-1.4.9/fim/user/link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1219 2021-03-03 19:57:54.000000 fabric_fim-1.4.9/fim/user/measurement.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9668 2023-04-05 18:48:29.000000 fabric_fim-1.4.9/fim/user/model_element.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    29219 2023-04-05 22:02:45.000000 fabric_fim-1.4.9/fim/user/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    22636 2023-02-14 21:58:39.000000 fabric_fim-1.4.9/fim/user/node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    58158 2023-02-14 21:58:39.000000 fabric_fim-1.4.9/fim/user/topology.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      595 2021-03-13 20:40:37.000000 fabric_fim-1.4.9/fim/view_only_dict.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/requirements.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-04-08 04:38:05.352946 fabric_fim-1.4.9/setup.cfg
--rw-r--r--   0 ibaldin    (502) staff       (20)      874 2023-02-02 01:41:56.000000 fabric_fim-1.4.9/setup.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.350899 fabric_fim-1.4.9/test/
--rw-r--r--   0 ibaldin    (502) staff       (20)      654 2022-02-18 19:27:15.000000 fabric_fim-1.4.9/test/test_load.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-08 04:38:05.351453 fabric_fim-1.4.9/util/
--rw-r--r--   0 ibaldin    (502) staff       (20)    14115 2023-04-05 20:55:22.000000 fabric_fim-1.4.9/util/fim_util.py
+-rw-r--r--   0        0        0     2179 2023-05-10 17:49:37.304171 fabric_fim-1.5.0b1/.gitignore
+-rw-r--r--   0        0        0       26 2020-07-24 21:42:44.564662 fabric_fim-1.5.0b1/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-07-14 22:09:49.459777 fabric_fim-1.5.0b1/LICENSE
+-rw-r--r--   0        0        0      146 2022-04-27 22:22:19.297089 fabric_fim-1.5.0b1/MANIFEST.in
+-rw-r--r--   0        0        0    10990 2023-05-10 14:54:24.180391 fabric_fim-1.5.0b1/README.md
+-rw-r--r--   0        0        0    18690 2021-05-25 21:09:37.024101 fabric_fim-1.5.0b1/figs/fim-structure.png
+-rw-r--r--   0        0        0      557 2021-03-15 22:13:52.784044 fabric_fim-1.5.0b1/fim/README.md
+-rw-r--r--   0        0        0      105 2023-05-10 17:52:03.586474 fabric_fim-1.5.0b1/fim/__init__.py
+-rw-r--r--   0        0        0        1 2022-04-27 22:22:19.299449 fabric_fim-1.5.0b1/fim/authz/__init__.py
+-rw-r--r--   0        0        0    16139 2023-02-02 01:41:56.403069 fabric_fim-1.5.0b1/fim/authz/attribute_collector.py
+-rw-r--r--   0        0        0      334 2020-09-12 23:24:52.369007 fabric_fim-1.5.0b1/fim/graph/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:31:38.004468 fabric_fim-1.5.0b1/fim/graph/__init__.py
+-rw-r--r--   0        0        0    69843 2023-05-10 14:54:24.395497 fabric_fim-1.5.0b1/fim/graph/abc_property_graph.py
+-rw-r--r--   0        0        0     4093 2023-02-02 01:41:56.406333 fabric_fim-1.5.0b1/fim/graph/abc_property_graph_constants.py
+-rw-r--r--   0        0        0        1 2020-08-18 21:34:07.036009 fabric_fim-1.5.0b1/fim/graph/data/__init__.py
+-rw-r--r--   0        0        0      283 2020-09-03 22:10:53.500264 fabric_fim-1.5.0b1/fim/graph/data/capacity_types.json
+-rw-r--r--   0        0        0      100 2020-08-27 20:41:23.401941 fabric_fim-1.5.0b1/fim/graph/data/constraint_types.json
+-rw-r--r--   0        0        0     3886 2023-05-10 14:54:24.398493 fabric_fim-1.5.0b1/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0        0        0     3845 2023-05-10 14:54:24.398661 fabric_fim-1.5.0b1/fim/graph/data/graph_validation_rules_neo4j_v4.json
+-rw-r--r--   0        0        0      547 2020-09-03 22:10:39.822590 fabric_fim-1.5.0b1/fim/graph/data/label_types.json
+-rw-r--r--   0        0        0       91 2020-08-27 20:40:54.261031 fabric_fim-1.5.0b1/fim/graph/data/location_types.json
+-rw-r--r--   0        0        0      861 2023-05-10 14:54:24.189132 fabric_fim-1.5.0b1/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0        0        0     3320 2023-05-10 14:54:24.398812 fabric_fim-1.5.0b1/fim/graph/graph_util.py
+-rw-r--r--   0        0        0    44293 2023-05-10 14:54:24.429886 fabric_fim-1.5.0b1/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0        0        0     6160 2022-10-06 17:38:08.214224 fabric_fim-1.5.0b1/fim/graph/networkx_mixin.py
+-rw-r--r--   0        0        0    42211 2023-05-10 14:54:24.400876 fabric_fim-1.5.0b1/fim/graph/networkx_property_graph.py
+-rw-r--r--   0        0        0     8354 2022-10-07 03:05:34.849246 fabric_fim-1.5.0b1/fim/graph/networkx_property_graph_disjoint.py
+-rw-r--r--   0        0        0     1501 2021-03-15 22:13:52.788626 fabric_fim-1.5.0b1/fim/graph/resources/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:04.638774 fabric_fim-1.5.0b1/fim/graph/resources/__init__.py
+-rw-r--r--   0        0        0     4484 2021-05-25 21:09:37.029370 fabric_fim-1.5.0b1/fim/graph/resources/abc_adm.py
+-rw-r--r--   0        0        0    13570 2023-05-10 14:54:24.193783 fabric_fim-1.5.0b1/fim/graph/resources/abc_arm.py
+-rw-r--r--   0        0        0     2991 2022-02-18 19:27:15.586527 fabric_fim-1.5.0b1/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0        0        0     4547 2021-03-31 01:14:29.518807 fabric_fim-1.5.0b1/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0        0        0     2297 2021-03-07 22:42:30.018249 fabric_fim-1.5.0b1/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0        0        0     2106 2021-05-25 21:09:37.031668 fabric_fim-1.5.0b1/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0        0        0    18591 2023-05-10 14:57:18.798602 fabric_fim-1.5.0b1/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0        0        0     5017 2022-02-18 19:27:15.587881 fabric_fim-1.5.0b1/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0        0        0     2341 2021-03-07 22:42:30.020154 fabric_fim-1.5.0b1/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0        0        0     2122 2021-05-25 21:09:37.033196 fabric_fim-1.5.0b1/fim/graph/resources/networkx_arm.py
+-rw-r--r--   0        0        0      301 2021-03-15 22:13:52.789768 fabric_fim-1.5.0b1/fim/graph/slices/README.md
+-rw-r--r--   0        0        0        1 2020-09-02 18:32:24.788341 fabric_fim-1.5.0b1/fim/graph/slices/__init__.py
+-rw-r--r--   0        0        0     8223 2022-02-18 19:27:15.588460 fabric_fim-1.5.0b1/fim/graph/slices/abc_asm.py
+-rw-r--r--   0        0        0     3733 2023-05-10 14:54:24.196715 fabric_fim-1.5.0b1/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0        0        0     4298 2021-06-04 19:43:14.989790 fabric_fim-1.5.0b1/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0        0        0     8615 2021-03-03 19:57:54.288231 fabric_fim-1.5.0b1/fim/graph/typed_tuples.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.409002 fabric_fim-1.5.0b1/fim/logging/__init__.py
+-rw-r--r--   0        0        0     9071 2023-02-02 01:41:56.410072 fabric_fim-1.5.0b1/fim/logging/log_collector.py
+-rw-r--r--   0        0        0     9555 2021-03-24 00:18:51.063382 fabric_fim-1.5.0b1/fim/pluggable.py
+-rw-r--r--   0        0        0      189 2021-06-04 19:43:14.990352 fabric_fim-1.5.0b1/fim/slivers/README.md
+-rw-r--r--   0        0        0      217 2021-06-14 18:36:21.931262 fabric_fim-1.5.0b1/fim/slivers/__init__.py
+-rw-r--r--   0        0        0     3641 2023-02-02 01:41:56.410512 fabric_fim-1.5.0b1/fim/slivers/attached_components.py
+-rw-r--r--   0        0        0    13021 2023-02-02 01:41:56.411041 fabric_fim-1.5.0b1/fim/slivers/base_sliver.py
+-rw-r--r--   0        0        0    24182 2023-05-10 14:54:24.198919 fabric_fim-1.5.0b1/fim/slivers/capacities_labels.py
+-rw-r--r--   0        0        0    11537 2023-05-10 14:54:24.200146 fabric_fim-1.5.0b1/fim/slivers/component_catalog.py
+-rw-r--r--   0        0        0        1 2021-03-03 19:57:54.291739 fabric_fim-1.5.0b1/fim/slivers/data/__init__.py
+-rw-r--r--   0        0        0     1691 2023-05-10 14:54:24.202981 fabric_fim-1.5.0b1/fim/slivers/data/component_catalog.json
+-rw-r--r--   0        0        0    76943 2022-09-10 21:18:41.714675 fabric_fim-1.5.0b1/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0        0        0    23524 2022-02-18 19:27:15.591229 fabric_fim-1.5.0b1/fim/slivers/delegations.py
+-rw-r--r--   0        0        0     3593 2022-02-18 19:27:15.591744 fabric_fim-1.5.0b1/fim/slivers/gateway.py
+-rw-r--r--   0        0        0      919 2021-06-29 20:04:13.972162 fabric_fim-1.5.0b1/fim/slivers/identifiers.py
+-rw-r--r--   0        0        0     3444 2022-02-18 19:27:15.592250 fabric_fim-1.5.0b1/fim/slivers/instance_catalog.py
+-rw-r--r--   0        0        0     3225 2023-02-02 01:41:56.413360 fabric_fim-1.5.0b1/fim/slivers/interface_info.py
+-rw-r--r--   0        0        0     2702 2021-09-22 14:46:40.423027 fabric_fim-1.5.0b1/fim/slivers/json.py
+-rw-r--r--   0        0        0     3869 2023-02-02 01:41:56.413720 fabric_fim-1.5.0b1/fim/slivers/json_data.py
+-rw-r--r--   0        0        0     5983 2023-02-02 01:41:56.414203 fabric_fim-1.5.0b1/fim/slivers/maintenance_mode.py
+-rw-r--r--   0        0        0     1566 2021-03-03 19:57:54.294274 fabric_fim-1.5.0b1/fim/slivers/network_attached_storage.py
+-rw-r--r--   0        0        0     3910 2023-02-02 01:41:56.414662 fabric_fim-1.5.0b1/fim/slivers/network_link.py
+-rw-r--r--   0        0        0    10209 2023-02-02 01:41:56.415082 fabric_fim-1.5.0b1/fim/slivers/network_node.py
+-rw-r--r--   0        0        0    22026 2023-05-10 14:54:24.204710 fabric_fim-1.5.0b1/fim/slivers/network_service.py
+-rw-r--r--   0        0        0     6795 2021-06-04 19:43:14.993329 fabric_fim-1.5.0b1/fim/slivers/path_info.py
+-rw-r--r--   0        0        0     3024 2022-02-18 19:27:15.594931 fabric_fim-1.5.0b1/fim/slivers/tags.py
+-rw-r--r--   0        0        0     2622 2023-02-02 01:41:56.416090 fabric_fim-1.5.0b1/fim/slivers/topology_diff.py
+-rw-r--r--   0        0        0     8706 2022-02-18 19:27:15.595505 fabric_fim-1.5.0b1/fim/user/README.md
+-rw-r--r--   0        0        0     1914 2023-02-02 01:41:56.417286 fabric_fim-1.5.0b1/fim/user/__init__.py
+-rw-r--r--   0        0        0    11730 2022-09-10 21:18:41.716394 fabric_fim-1.5.0b1/fim/user/component.py
+-rw-r--r--   0        0        0     5668 2022-09-10 21:18:41.716675 fabric_fim-1.5.0b1/fim/user/composite_node.py
+-rw-r--r--   0        0        0     7660 2023-02-02 01:41:56.418568 fabric_fim-1.5.0b1/fim/user/interface.py
+-rw-r--r--   0        0        0     8381 2022-09-10 21:18:41.717280 fabric_fim-1.5.0b1/fim/user/link.py
+-rw-r--r--   0        0        0     1219 2021-03-03 19:57:54.300001 fabric_fim-1.5.0b1/fim/user/measurement.py
+-rw-r--r--   0        0        0     9668 2023-04-05 18:48:29.319327 fabric_fim-1.5.0b1/fim/user/model_element.py
+-rw-r--r--   0        0        0    29219 2023-05-10 14:54:24.206616 fabric_fim-1.5.0b1/fim/user/network_service.py
+-rw-r--r--   0        0        0    22636 2023-02-14 21:58:39.970039 fabric_fim-1.5.0b1/fim/user/node.py
+-rw-r--r--   0        0        0    58158 2023-02-14 21:58:39.970995 fabric_fim-1.5.0b1/fim/user/topology.py
+-rw-r--r--   0        0        0        2 2023-05-10 15:46:29.821869 fabric_fim-1.5.0b1/fim/util/__init__.py
+-rw-r--r--   0        0        0    14115 2023-05-10 14:54:24.213707 fabric_fim-1.5.0b1/fim/util/fim_util.py
+-rwxr-xr-x   0        0        0      480 2020-10-01 22:44:51.231545 fabric_fim-1.5.0b1/fim/util/load_graphs.sh
+-rwxr-xr-x   0        0        0      316 2023-03-01 03:21:45.408058 fabric_fim-1.5.0b1/fim/util/merge_dev.sh
+-rwxr-xr-x   0        0        0      563 2023-02-10 01:56:08.037222 fabric_fim-1.5.0b1/fim/util/merge_production.sh
+-rwxr-xr-x   0        0        0      258 2020-10-09 19:51:30.191532 fabric_fim-1.5.0b1/fim/util/test_ws.bash
+-rw-r--r--   0        0        0      595 2021-03-13 20:40:37.643107 fabric_fim-1.5.0b1/fim/view_only_dict.py
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421372 fabric_fim-1.5.0b1/neo4j/data/.empty
+-rw-r--r--   0        0        0        0 2023-02-02 01:41:56.421489 fabric_fim-1.5.0b1/neo4j/imports/.empty
+-rw-r--r--   0        0        0      794 2023-05-10 17:46:53.813408 fabric_fim-1.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-02-02 01:41:56.422084 fabric_fim-1.5.0b1/requirements.txt
+-rw-r--r--   0        0        0     4632 2022-03-09 00:58:31.583145 fabric_fim-1.5.0b1/test/ad_topology_test.py
+-rw-r--r--   0        0        0     4834 2022-09-10 21:18:41.719406 fabric_fim-1.5.0b1/test/after.graphml
+-rw-r--r--   0        0        0    17201 2023-02-02 01:41:56.423227 fabric_fim-1.5.0b1/test/attribute_collector_test.py
+-rw-r--r--   0        0        0     4696 2022-09-10 21:18:41.719615 fabric_fim-1.5.0b1/test/before.graphml
+-rw-r--r--   0        0        0     2729 2022-09-10 21:18:41.719876 fabric_fim-1.5.0b1/test/catalog_test.py
+-rw-r--r--   0        0        0     4319 2022-02-18 19:27:15.602412 fabric_fim-1.5.0b1/test/delegation_label_test.py
+-rw-r--r--   0        0        0     1653 2023-02-02 01:41:56.423551 fabric_fim-1.5.0b1/test/maintenance_test.py
+-rw-r--r--   0        0        0    51613 2023-05-10 17:34:04.562843 fabric_fim-1.5.0b1/test/models/advertised_topo.graphml
+-rw-r--r--   0        0        0    49696 2023-05-10 17:34:04.565992 fabric_fim-1.5.0b1/test/models/graph-template.graphml
+-rw-r--r--   0        0        0    82994 2023-05-10 17:34:04.568753 fabric_fim-1.5.0b1/test/models/network-am-ad.graphml
+-rw-r--r--   0        0        0    57411 2023-05-10 17:34:04.571919 fabric_fim-1.5.0b1/test/models/site-2-am-1broker-ad.graphml
+-rw-r--r--   0        0        0    52887 2023-05-10 17:34:04.574274 fabric_fim-1.5.0b1/test/models/site-3-am-1broker-ad.graphml
+-rw-r--r--   0        0        0   131407 2023-05-10 17:34:04.575177 fabric_fim-1.5.0b1/test/models/site-am-2broker-ad.graphml
+-rw-r--r--   0        0        0    17363 2023-05-10 14:57:53.569975 fabric_fim-1.5.0b1/test/modify_test.py
+-rw-r--r--   0        0        0    13135 2021-05-23 19:50:30.753072 fabric_fim-1.5.0b1/test/networkxx_pg_disjoint_test.py
+-rw-r--r--   0        0        0    14091 2021-05-23 19:50:30.753595 fabric_fim-1.5.0b1/test/networkxx_pg_test.py
+-rw-r--r--   0        0        0     2572 2021-03-24 00:18:51.064667 fabric_fim-1.5.0b1/test/pluggable_test.py
+-rw-r--r--   0        0        0    42433 2023-05-10 14:57:53.570145 fabric_fim-1.5.0b1/test/slice_topology_test.py
+-rw-r--r--   0        0        0     1869 2022-04-27 22:22:19.322857 fabric_fim-1.5.0b1/test/sliver_json_test.py
+-rw-r--r--   0        0        0     5604 2023-05-10 14:54:24.209787 fabric_fim-1.5.0b1/test/sliver_test.py
+-rw-r--r--   0        0        0    97162 2023-02-02 01:41:56.427682 fabric_fim-1.5.0b1/test/substrate_topology_test.py
+-rw-r--r--   0        0        0      654 2022-02-18 19:27:15.604787 fabric_fim-1.5.0b1/test/test_load.py
+-rw-r--r--   0        0        0     2362 2022-02-18 19:27:15.605244 fabric_fim-1.5.0b1/test/tuple_test.py
+-rw-r--r--   0        0        0    15663 2023-05-10 14:57:53.570342 fabric_fim-1.5.0b1/test/zz_neo4j_pg_test.py
+-rw-r--r--   0        0        0    11682 1970-01-01 00:00:00.000000 fabric_fim-1.5.0b1/PKG-INFO
```

### Comparing `fabric_fim-1.4.9/LICENSE` & `fabric_fim-1.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/PKG-INFO` & `fabric_fim-1.5.0b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: fabric_fim
-Version: 1.4.9
-Summary: FABRIC Information Model Library
-Home-page: https://github.com/fabric-testbed/InformationModel
-Author: Ilya Baldin, Komal Thareja
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 [![PyPI](https://img.shields.io/pypi/v/fabric-fim?style=plastic)](https://pypi.org/project/fabric-fim/)
 
 # Information Model
 
 ## Basic Graph Abstractions
 
 FABRIC Information Model library, containing class definitions and methods for operating
```

### Comparing `fabric_fim-1.4.9/README.md` & `fabric_fim-1.5.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: fabric_fim
+Version: 1.5.0b1
+Summary: FABRIC Information Model library and utilities
+Keywords: Neo4j
+Author-email: Ilya Baldin <ibaldin@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Dist: matplotlib >= 3.6.0
+Requires-Dist: neo4j >= 5.2.0
+Requires-Dist: networkx >= 2.8.7
+Requires-Dist: networkx_query >= 1.0.1
+Requires-Dist: PyYAML >= 6.0
+Requires-Dist: recordclass >= 0.17.5
+Requires-Dist: requests >= 2.28.1
+Project-URL: Home, https://github.com/fabric-testbed/InformationModel
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-fim?style=plastic)](https://pypi.org/project/fabric-fim/)
 
 # Information Model
 
 ## Basic Graph Abstractions
 
 FABRIC Information Model library, containing class definitions and methods for operating
@@ -231,7 +251,8 @@
 
 An index can be dropped using the following command (substitute appropriate index name):
 ```
 DROP INDEX graphid
 ```
 
 See [additional documentation](https://neo4j.com/docs/cypher-manual/current/administration/indexes-for-search-performance/).
+
```

### Comparing `fabric_fim-1.4.9/fim/authz/attribute_collector.py` & `fabric_fim-1.5.0b1/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/abc_property_graph.py` & `fabric_fim-1.5.0b1/fim/graph/abc_property_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from fim.slivers.path_info import PathInfo, ERO
 from fim.slivers.tags import Tags
 from fim.slivers.json_data import MeasurementData, UserData, LayoutData
 from fim.slivers.network_service import NetworkServiceSliver, NetworkServiceInfo, NSLayer, MirrorDirection
 from fim.graph.abc_property_graph_constants import ABCPropertyGraphConstants
 from fim.slivers.gateway import Gateway
 from fim.slivers.maintenance_mode import MaintenanceInfo
+from fim.graph.graph_util import GraphML
 
 
 class GraphFormat(Enum):
     # default, works in Neo4j and NetworkX
     GRAPHML = 1
     # JSON formats are specific to NetworkX
     JSON_NODELINK = 2
@@ -1409,15 +1410,15 @@
         # read using networkx
         g = nx.read_graphml(graph_file)
         # add node id to every node
         for n in list(g.nodes):
             if (node_id_prop not in g.nodes[n].keys()) or (len(g.nodes[n][node_id_prop]) == 0):
                 g.nodes[n][node_id_prop] = str(uuid.uuid4())
         # save to a new file
-        nx.write_graphml(g, new_graph_file)
+        GraphML.nx_write_graphml(g, new_graph_file)
 
     @staticmethod
     def enumerate_graph_nodes_to_string(*, graph_file: str, node_id_prop: str = "NodeID") -> str:
         """
         Read in a graph and add a NodeId property to every node assigning a unique GUID (unless present).
         Return GraphML string.
         :param graph_file: original graph file name
```

### Comparing `fabric_fim-1.4.9/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.5.0b1/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.5.0b1/fim/graph/data/graph_validation_rules.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {'0': "{'rule': 'MATCH (n:GraphNode {GraphID: $graphId}) RETURN ALL(r IN collect(n) WHERE r.Class "*

 * *      "IS NOT NULL AND r.NodeID IS NOT NULL AND r.Type IS NOT NULL AND r.Name IS NOT NULL)'}",*

 * * '10': '{\'rule\': \'MATCH (n:NetworkService {GraphID: $graphId}) WHERE n.Type = "Patch" or '*

 * *       'n.Type="L2Path" or n.Type="L2PTP" WITH collect(size([(n) -[:connects]- () | n.NodeID ])) '*

 * *       "AS sizes RETURN sizes IS null or all(s in sizes where s=2)'}",*

 * * '11': '{\'rule\': \'MATCH (n:NetworkService {GraphID […]*

```diff
@@ -1,11 +1,11 @@
 [
     {
         "msg": "All nodes must have Class, Type, Name and NodeID properties",
-        "rule": "MATCH (n:GraphNode {GraphID: $graphId}) RETURN ALL(r IN collect(n) WHERE exists(r.Class) AND exists(r.NodeID) AND exists(r.Type) AND exists(r.Name))"
+        "rule": "MATCH (n:GraphNode {GraphID: $graphId}) RETURN ALL(r IN collect(n) WHERE r.Class IS NOT NULL AND r.NodeID IS NOT NULL AND r.Type IS NOT NULL AND r.Name IS NOT NULL)"
     },
     {
         "msg": "All node NodeIDs must be distinct.",
         "rule": "MATCH (n:GraphNode {GraphID: $graphId}), (m {GraphID: $graphId}) WHERE n.NodeID=m.NodeID AND NOT id(n)=id(m) RETURN count(n) = 0"
     },
     {
         "msg": "All nodes must be of class NetworkNode, CompositeNode, Component, ConnectionPoint, NetworkService or Link",
@@ -37,18 +37,18 @@
     },
     {
         "msg": "Links can only connect to ConnectionPoints",
         "rule": "MATCH (o:GraphNode {GraphID: $graphId}) -[:connects]- (n:Link {GraphID: $graphId}) WHERE o.Class <> \"ConnectionPoint\" return count(o)=0"
     },
     {
         "msg": "Patch, L2Path or L2PTP link type can only connect two ConnectionPoints",
-        "rule": "MATCH (n:NetworkService {GraphID: $graphId}) WHERE n.Type = \"Patch\" or n.Type=\"L2Path\" or n.Type=\"L2PTP\" WITH collect(size((n) -[:connects]- ())) AS sizes RETURN sizes IS null or all(s in sizes where s=2)"
+        "rule": "MATCH (n:NetworkService {GraphID: $graphId}) WHERE n.Type = \"Patch\" or n.Type=\"L2Path\" or n.Type=\"L2PTP\" WITH collect(size([(n) -[:connects]- () | n.NodeID ])) AS sizes RETURN sizes IS null or all(s in sizes where s=2)"
     },
     {
         "msg": "PortMirror link type can only connect one ConnectionPoint",
-        "rule": "MATCH (n:NetworkService {GraphID: $graphId}) WHERE n.Type = \"PortMirror\" WITH collect(size((n) -[:connects]- ())) AS sizes RETURN sizes IS null or all(s in sizes where s=1)"
+        "rule": "MATCH (n:NetworkService {GraphID: $graphId}) WHERE n.Type = \"PortMirror\" WITH collect(size([(n) -[:connects]- () | n.NodeID ])) AS sizes RETURN sizes IS null or all(s in sizes where s=1)"
     },
     {
         "msg": "There should always be one peer for each ServicePort",
-        "rule": "MATCH (n:ConnectionPoint {GraphID: $graphId}) where n.Type = \"ServicePort\" WITH collect(size((n) -[:connects]- (:Link) -[:connects]- (:ConnectionPoint))) AS sizes RETURN sizes IS null or all(s in sizes where s=1)"
+        "rule": "MATCH (n:ConnectionPoint {GraphID: $graphId}) where n.Type = \"ServicePort\" WITH collect(size([(n) -[:connects]- (:Link) -[:connects]- (:ConnectionPoint) | n.NodeID])) AS sizes RETURN sizes IS null or all(s in sizes where s=1)"
     }
 ]
```

### Comparing `fabric_fim-1.4.9/fim/graph/data/label_types.json` & `fabric_fim-1.5.0b1/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.5.0b1/fim/graph/neo4j_property_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import time
 import json
 import networkx as nx
 from neo4j import GraphDatabase
 
 from .abc_property_graph import ABCPropertyGraph, PropertyGraphImportException, \
     PropertyGraphQueryException, ABCGraphImporter, GraphFormat
+from .graph_util import GraphML
 
 # to deal with intermittent APOC problems on MAC
 APOC_RETRY_COUNT = 10
 
 
 class Neo4jPropertyGraph(ABCPropertyGraph):
     """
@@ -364,17 +365,17 @@
 
         if graph_string == self.NEO4j_NONE:
             return None
 
         # CAUTION: horrible kludge - APOC exports without indicating 'labels' is a key,
         # even though it is used, and then NetworkX refuses to import. Direct imports to
         # Neo4j work though. So we add a line to XML to declare 'labels' a key. Sigh /ib 09/12/2020
-        graph_lines = graph_string.splitlines()
-        graph_lines.insert(3, '<key id="labels" for="node" attr.name="labels" attr.type="string"/>\n')
-        graph_string = "".join(graph_lines)
+        #graph_lines = graph_string.splitlines()
+        #graph_lines.insert(3, '<key id="labels" for="node" attr.name="labels" attr.type="string"/>\n')
+        #graph_string = "".join(graph_lines)
         return graph_string
 
     def graph_exists(self) -> bool:
         """
         Does the graph with this ID exist?
         :return:
         """
@@ -423,15 +424,15 @@
         :param node_label:
         :return:
         """
         assert node_id is not None
         assert rel is not None
         assert node_label is not None
         query = f"match (a:GraphNode {{GraphID: $graphId, NodeID: $nodeA}}) -[:{rel}]- " \
-                f"(b:{node_label} {{ GraphID: $graphId}}) return b.NodeID"
+                f"(b:GraphNode:{node_label} {{ GraphID: $graphId}}) return b.NodeID"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, nodeA=node_id).value()
             if val is None:
                 return list()
             return val
 
     def get_first_and_second_neighbor(self, *, node_id: str, rel1: str, node1_label: str,
@@ -449,16 +450,16 @@
         assert node_id is not None
         assert rel1 is not None
         assert node1_label is not None
         assert rel2 is not None
         assert node2_label is not None
 
         query = f"match (a:GraphNode {{GraphID: $graphId, NodeID: $nodeA}}) -[:{rel1}]- "\
-                f"(b:{node1_label} {{GraphID: $graphId}}) -[:{rel2}]- "\
-                f"(c:{node2_label} {{GraphID: $graphId}}) WHERE $nodeA <> c.NodeID return b.NodeID, c.NodeID"
+                f"(b:GraphNode:{node1_label} {{GraphID: $graphId}}) -[:{rel2}]- "\
+                f"(c:GraphNode:{node2_label} {{GraphID: $graphId}}) WHERE $nodeA <> c.NodeID return b.NodeID, c.NodeID"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, nodeA=node_id).values()
             if val is None:
                 return list()
             return val
 
     def delete_node(self, *, node_id: str):
@@ -477,50 +478,49 @@
         Check if this node exists
         :param node_id:
         :param label:
         :return:
         """
         assert node_id is not None
         assert label is not None
-        query = f"MATCH (n:{label} {{GraphID: $graphId, NodeID: $nodeId}} RETURN collect(n.NodeID) as nodeids"
+        query = f"MATCH (n:GraphNode:{label} {{GraphID: $graphId, NodeID: $nodeId}} RETURN collect(n.NodeID) as nodeids"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, nodeId=node_id).single()
             if val is None or len(val.data()) == 0 or len(val.data()['nodeids']) == 0:
                 return False
             return True
 
     def add_node(self, *, node_id: str, label: str, props: Dict[str, Any] = None) -> None:
 
         assert node_id is not None
         assert label is not None
 
-        all_props = f"Class: '{label}', GraphID: '{self.graph_id}', NodeID: '{node_id}', "
-        if props is not None:
-            for k, v in props.items():
-                all_props += f"{k}: '{v}', "
-        all_props = all_props[:-2]
+        all_props = {'Class': f'{label}', 'GraphID': f'{self.graph_id}', 'NodeID': f'{node_id}'}
+        if props:
+            all_props.update(props)
+        string_props = ", ".join((f"{k}: '{v}'" for k, v in all_props.items()))
         labels = f"'GraphNode', '{label}'"
-        query = f"CALL apoc.create.node([ {labels} ], {{ {all_props} }});"
+        query = f"CALL apoc.create.node([ {labels} ], {{ {string_props} }});"
         with self.driver.session() as session:
             session.run(query)
 
     def add_link(self, *, node_a: str, rel: str, node_b: str, props: Dict[str, Any] = None) -> None:
 
         assert node_a is not None
         assert rel is not None
         assert node_b is not None
 
-        all_props = ""
-        if props is not None:
-            for k, v in props.items():
-                all_props += f"{k}: '{v}', "
-        all_props = all_props[:-2]
+        # add default Class property that shadows the label so NetworkX can understand
+        all_props = {'Class': f'{rel}'}
+        if props:
+            all_props.update(props)
+        string_props = ", ".join((f"{k}: '{v}'" for k, v in all_props.items()))
         query = f"MATCH (a:GraphNode {{GraphID: $graphId, NodeID: $nodeA}}) " \
                 f"MATCH (b:GraphNode {{GraphID: $graphId, NodeID: $nodeB}}) " \
-                f"CALL apoc.create.relationship(a, \"{rel}\", {{ {all_props} }}, b)" \
+                f"CALL apoc.create.relationship(a, \"{rel}\", {{ {string_props} }}, b)" \
                 f"YIELD rel RETURN rel"
         with self.driver.session() as session:
             session.run(query, graphId=self.graph_id, nodeA=node_a, nodeB=node_b)
 
     def find_matching_nodes(self, *, other_graph) -> Set:
         """
         Return a set of node ids that match between the two graphs
@@ -593,26 +593,26 @@
                                                   node_id=None, msg="Unable to find stitch nodes")
             return val.data()['nodeids']
 
     def check_node_unique(self, *, label: str, name: str) -> bool:
         assert label is not None
         assert name is not None
 
-        query = f"MATCH (n:{label} {{GraphID: $graphId, Name: $name}}) RETURN collect(n.NodeID) as nodeids"
+        query = f"MATCH (n:GraphNode:{label} {{GraphID: $graphId, Name: $name}}) RETURN collect(n.NodeID) as nodeids"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, name=name).single()
             if val is None or len(val.data()) == 0 or len(val.data()['nodeids']) == 0:
                 return True
             return False
 
     def get_graph_diff(self, other_graph, label: str):
         assert other_graph is not None
         assert label is not None
 
-        query = f"MATCH(n:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:{label} {{GraphID: $graphIdB}}) WITH " \
+        query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:GraphNode:{label} {{GraphID: $graphIdB}}) WITH " \
                 f"collect(DISTINCT n) as A, collect(DISTINCT n1) as B, " \
                 f"collect(DISTINCT n.NodeID) as AN, collect(DISTINCT n1.NodeID) as BN " \
                 f"RETURN [x in A WHERE NOT x.NodeID in BN] as AnotB, [x in B WHERE NOT x.NodeID in AN] as BnotA"
         with self.driver.session() as session:
             val = session.run(query, graphIdA=self.graph_id, graphIdB=other_graph.graph_id).single()
             if val is None:
                 raise PropertyGraphQueryException(graph_id=self.graph_id,
@@ -627,47 +627,47 @@
         assert property is not None
 
         # alternative query
         # FIXME: figure out which one is faster
         #query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:GraphNode:{label} {{GraphID: $graphIdB}}) " \
         #        f"WHERE n.NodeID = n1.NodeID AND " \
         #        f"(" \
-        #        f"((exists(n.Labels) AND exists(n1.Labels) AND n.Labels <> n1.Labels) OR " \
-        #       f"(exists(n.Labels) AND NOT exists(n1.Labels)) OR " \
-        #        f"(NOT exists(n.Labels) AND exists(n1.Labels))) " \
+        #        f"((n.Labels IS NOT NULL AND n1.Labels IS NOT NULL AND n.Labels <> n1.Labels) OR " \
+        #        f"(n.Labels IS NOT NULL AND n1.Labels IS NULL) OR " \
+        #        f"(n.Labels IS NULL AND n1.Labels IS NOT NULL)) " \
         #        f"OR " \
-        #        f"((exists(n.Capacities) AND exists(n1.Capacities) AND n.Capacities <> n1.Capacities) OR " \
-        #        f"(exists(n.Capacities) AND NOT exists(n1.Capacities)) OR " \
-        #        f"(NOT exists(n.Capacities) AND exists(n1.Capacities))) " \
+        #        f"((n.Capacities IS NOT NULL AND n1.Capacities IS NOT NULL AND n.Capacities <> n1.Capacities) OR " \
+        #        f"(n.Capacities IS NOT NULL AND n1.Capacities IS NULL) OR " \
+        #        f"(n.Capacities IS NULL AND n1.Capacities IS NOT NULL)) " \
         #        f"OR " \
-        #        f"((exists(n.UserData) AND exists(n1.UserData) AND n.UserData <> n1.UserData) OR " \
-        #        f"(exists(n.UserData) AND NOT exists(n1.UserData)) OR " \
-        #        f"(NOT exists(n.UserData) AND exists(n1.UserData))) " \
+        #        f"((n.UserData IS NOT NULL AND n1.UserData IS NOT NULL AND n.UserData <> n1.UserData) OR " \
+        #        f"(n.UserData IS NOT NULL AND n1.UserData IS NULL) OR " \
+        #        f"(n.UserData IS NULL AND n1.UserData IS NOT NULL)) " \
         #        f") " \
         #        f"RETURN collect(n) as nodes"
 
         query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:GraphNode:{label} {{GraphID: $graphIdB}}) WHERE " \
                 f"n.NodeID = n1.NodeID AND " \
-                f"((exists(n.Labels) AND exists(n1.Labels) AND n.Labels <> n1.Labels) OR " \
-                f"(exists(n.Labels) AND NOT exists(n1.Labels)) OR " \
-                f"(NOT exists(n.Labels) AND exists(n1.Labels))) " \
+                f"((n.Labels IS NOT NULL AND n1.Labels IS NOT NULL AND n.Labels <> n1.Labels) OR " \
+                f"(n.Labels IS NOT NULL AND n1.Labels IS NULL) OR " \
+                f"(n.Labels IS NULL AND n1.Labels IS NOT NULL)) " \
                 f"RETURN collect(n) as nodes, collect(n1) as nodes1 " \
                 f"UNION " \
                 f"MATCH(n:GraphNode:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:GraphNode:{label} {{GraphID: $graphIdB}}) WHERE " \
                 f"n.NodeID = n1.NodeID AND " \
-                f"((exists(n.Capacities) AND exists(n1.Capacities) AND n.Capacities <> n1.Capacities) OR " \
-                f"(exists(n.Capacities) AND NOT exists(n1.Capacities)) OR " \
-                f"(NOT exists(n.Capacities) AND exists(n1.Capacities))) " \
+                f"((n.Capacities IS NOT NULL AND n1.Capacities IS NOT NULL AND n.Capacities <> n1.Capacities) OR " \
+                f"(n.Capacities IS NOT NULL AND n1.Capacities IS NULL) OR " \
+                f"(n.Capacities IS NULL AND n1.Capacities IS NOT NULL)) " \
                 f"RETURN collect(n) as nodes, collect(n1) as nodes1 " \
                 f"UNION " \
                 f"MATCH(n:GraphNode:{label} {{GraphID: $graphIdA}}) WITH n MATCH(n1:GraphNode:{label} {{GraphID: $graphIdB}}) WHERE " \
                 f"n.NodeID = n1.NodeID AND " \
-                f"((exists(n.UserData) AND exists(n1.UserData) AND n.UserData <> n1.UserData) OR " \
-                f"(exists(n.UserData) AND NOT exists(n1.UserData)) OR " \
-                f"(NOT exists(n.UserData) AND exists(n1.UserData))) " \
+                f"((n.UserData IS NOT NULL AND n1.UserData IS NOT NULL AND n.UserData <> n1.UserData) OR " \
+                f"(n.UserData IS NOT NULL AND n1.UserData IS NULL) OR " \
+                f"(n.UserData IS NULL AND n1.UserData IS NOT NULL)) " \
                 f"RETURN collect(n) as nodes, collect(n1) as nodes1 "
 
         with self.driver.session() as session:
             val = session.run(query, graphIdA=self.graph_id, graphIdB=other_graph.graph_id)
             vd = val.data()
             if vd is None:
                 raise PropertyGraphQueryException(graph_id=self.graph_id,
@@ -750,14 +750,17 @@
         :param graph:
         :param graph_id:
         :return:
         """
         if graph_id is None:
             graph_id = str(uuid.uuid4())
 
+        # massage the GraphML in case it came from non-compliant NetworkX or older version
+        graph = GraphML.networkx_to_neo4j(graph)
+
         # save to file
         with tempfile.NamedTemporaryFile(suffix="-graphml", mode='w') as f1:
             f1.write(graph)
             f1.flush()
             # read using networkx
             g = nx.read_graphml(f1.name)
 
@@ -774,15 +777,15 @@
         if dest_dir is None:
             dest_dir = tempfile.gettempdir()
 
         uniq_name = str(uuid.uuid4())
         host_file_name = os.path.join(dest_dir, uniq_name)
         mapped_file_name = os.path.join(self.import_dir, uniq_name)
 
-        nx.write_graphml(g, host_file_name)
+        GraphML.nx_write_graphml(g, host_file_name)
 
         return graph_id, host_file_name, mapped_file_name
 
     def _import_graph(self, graphml_file: str, graph_id: str) -> None:
         """
         import graph into neo4j giving every node a label GraphNode
         and converting Class property into a label
@@ -803,23 +806,23 @@
                     'readLabels: true, storeNodeIds: true } ) ',
                     fileName=graphml_file).single()
                 # force one common label on all imported nodes
                 self.log.debug(f"Adding GraphNode label to graph {graph_id}")
                 query_string = "MATCH (n {GraphID: $graphId }) SET n:GraphNode"
                 session.run(query_string, graphId=graph_id)
                 # convert class property into a label as well
-                self.log.debug(f"Converting Class property into Neo4j label for all nodes")
-                query_string = "MATCH (n {GraphID: $graphId }) " \
-                               "CALL apoc.create.addLabels([ id(n) ], [ n.Class ]) YIELD node RETURN node"
-                session.run(query_string, graphId=graph_id)
+                #self.log.debug(f"Converting Class property into Neo4j label for all nodes")
+                #query_string = "MATCH (n {GraphID: $graphId }) " \
+                #               "CALL apoc.create.addLabels([ id(n) ], [ n.Class ]) YIELD node RETURN node"
+                #session.run(query_string, graphId=graph_id)
                 # push class labels into class property on relationships
-                self.log.debug(f"Pushing label into Class property on all relationships")
-                query_string = "MATCH (n {GraphID: $graphId }) - [r] - (n1 {GraphID: $graphId }) " \
-                               "CALL apoc.create.setRelProperty(r, 'Class', TYPE(r)) yield rel return rel"
-                session.run(query_string, graphId=graph_id)
+                #self.log.debug(f"Pushing label into Class property on all relationships")
+                #query_string = "MATCH (n {GraphID: $graphId }) - [r] - (n1 {GraphID: $graphId }) " \
+                #               "CALL apoc.create.setRelProperty(r, 'Class', TYPE(r)) yield rel return rel"
+                #session.run(query_string, graphId=graph_id)
         except Exception as e:
             msg = f"Neo4j APOC import error {str(e)}"
             raise PropertyGraphImportException(graph_id=graph_id, msg=msg)
 
     def import_graph_from_string(self, *, graph_string: str, graph_id: str = None) -> Neo4jPropertyGraph:
         """
         import graph into Neo4j from a string, assigning it a unique id
@@ -851,14 +854,15 @@
                 retry -= 1
                 self.delete_graph(graph_id=assigned_id)
                 # sleep and try again
                 time.sleep(1.0)
 
         # remove the file
         self.log.debug(f"Unlinking temporary file {host_file_name}")
+        #print(f'LEAVING TEMPORARY FILE {host_file_name}')
         os.unlink(host_file_name)
 
         if retry == 0:
             raise PropertyGraphImportException(graph_id=assigned_id,
                                                msg='Unable to load graph after multiple attempts')
 
         return Neo4jPropertyGraph(graph_id=assigned_id, importer=self, logger=self.log)
@@ -873,14 +877,16 @@
         dest_dir = self.import_host_dir
         assert dest_dir is not None
         uniq_name = str(uuid.uuid4())
         # need both host file name and what is seen from inside Docker
         host_file_name = os.path.join(dest_dir, uniq_name)
         mapped_file_name = os.path.join(self.import_dir, uniq_name)
 
+        graph_string = GraphML.networkx_to_neo4j(graph_string)
+
         with open(host_file_name, 'w') as f:
             f.write(graph_string)
 
         # get graph id
         graph_id = self.get_graph_id(graph_file=host_file_name)
 
         retry = APOC_RETRY_COUNT
@@ -919,15 +925,23 @@
         dest_dir = self.import_host_dir
         assert dest_dir is not None
         uniq_name = str(uuid.uuid4())
         # need both host file name and what is seen from inside Docker
         host_file_name = os.path.join(dest_dir, uniq_name)
         mapped_file_name = os.path.join(self.import_dir, uniq_name)
 
-        shutil.copyfile(graph_file, host_file_name)
+        #shutil.copyfile(graph_file, host_file_name)
+
+        with open(graph_file, 'r') as f:
+            graph_string = f.read()
+
+        graph_string = GraphML.networkx_to_neo4j(graph_string)
+        with open(host_file_name, 'w') as f:
+            f.write(graph_string)
+            f.flush()
 
         # get graph id
         graph_id = self.get_graph_id(graph_file=host_file_name)
 
         # load file
         self._import_graph(mapped_file_name, graph_id)
```

### Comparing `fabric_fim-1.4.9/fim/graph/networkx_mixin.py` & `fabric_fim-1.5.0b1/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/networkx_property_graph.py` & `fabric_fim-1.5.0b1/fim/graph/networkx_property_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 import uuid
 import json
 import tempfile
 import networkx as nx
 import networkx_query as nxq
 from threading import Lock
 
+
+from fim.graph.graph_util import GraphML
 from .abc_property_graph import ABCPropertyGraph, PropertyGraphImportException, \
     PropertyGraphQueryException, ABCGraphImporter, GraphFormat
 from .networkx_mixin import NetworkXMixin
 
 
 class NetworkXPropertyGraph(ABCPropertyGraph, NetworkXMixin):
     """
@@ -367,14 +369,15 @@
         :return:
         """
         graph = self.storage.extract_graph(self.graph_id)
         graph_string = None
         if graph is not None:
             if format == GraphFormat.GRAPHML:
                 graph_string = '\n'.join(nx.generate_graphml(graph))
+                graph_string = GraphML.networkx_to_neo4j(graph_string)
             elif format == GraphFormat.JSON_NODELINK:
                 json_object = nx.readwrite.node_link_data(graph)
                 graph_string = json.dumps(json_object)
             elif format == GraphFormat.CYTOSCAPE:
                 json_object = nx.readwrite.cytoscape_data(graph)
                 graph_string = json.dumps(json_object)
             else:
```

### Comparing `fabric_fim-1.4.9/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.5.0b1/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/abc_adm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/abc_arm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/neo4j_cbm.py`

 * *Files 5% similar despite different names*

```diff
@@ -293,48 +293,49 @@
                 else:
                     component_counts[(comp.resource_type, comp.resource_model)] = 1
         # unroll properties
         node_props = ", ".join([x + ": " + '"' + props[x] + '"' for x in props.keys()])
 
         if len(component_counts.values()) == 0:
             # simple query on the properties of the node (no components)
-            query = f"MATCH(n:{label} {{GraphID: $graphId, {node_props} }}) RETURN collect(n.NodeID) as candidate_ids"
+            query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphId, {node_props} }}) RETURN collect(n.NodeID) as candidate_ids"
         else:
             # build a query list
-            node_query = f"MATCH(n:{label} {{GraphID: $graphId, {node_props} }}) WHERE "
+            node_query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphId, {node_props} }}) WHERE "
             component_clauses = list()
             # add a clause for every tuple
             for k, v in component_counts.items():
                 comp_props_list = list()
                 if k[0] is not None:
                     comp_props_list.append('Type: ' + '"' + str(k[0]) + '"' + ' ')
                 if k[1] is not None:
                     comp_props_list.append('Model: ' + '"' + k[1] + '"' + ' ')
                 comp_props = ", ".join(comp_props_list)
 
-                component_clauses.append(f"size( (n) -[:has]- (:Component {{GraphID: $graphId, "
-                                         f"{comp_props}}}))>={str(v)} ")
+                # uses pattern comprehension rather than pattern matching as per Neo4j v4+
+                component_clauses.append(f"size([(n) -[:has]- (:Component {{GraphID: $graphId, "
+                                         f"{comp_props}}}) | n.NodeID])>={str(v)}")
             query = node_query + " and ".join(component_clauses) + " RETURN collect(n.NodeID) as candidate_ids"
 
-        # print(f'Resulting query {query=}')
+        #print(f'**** Resulting query {query=}')
 
         with self.driver.session() as session:
 
             val = session.run(query, graphId=self.graph_id).single()
             #print(f'VAL= {val}')
         if val is None:
             return list()
         return val.data()['candidate_ids']
 
     def get_intersite_links(self) -> List[Tuple[str, str, str]]:
         # does a lexicographic comparison of Site properties to ensure only unique links are returned
-        query = 'match p= (n:NetworkNode {Type:"Switch", GraphID: $graphId}) -[:has]- (:NetworkService) ' \
+        query = 'match p= (n:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) -[:has]- (:GraphNode:NetworkService) ' \
                 '-[:connects]- (cp1:ConnectionPoint) -[:connects]- (l:Link) ' \
-                '-[:connects]- (cp2:ConnectionPoint) -[:connects]- (:NetworkService) ' \
-                '-[:has]- (m:NetworkNode {Type:"Switch", GraphID: $graphId}) where n.Site > m.Site ' \
+                '-[:connects]- (cp2:ConnectionPoint) -[:connects]- (:GraphNode:NetworkService) ' \
+                '-[:has]- (m:GraphNode:NetworkNode {Type:"Switch", GraphID: $graphId}) where n.Site > m.Site ' \
                 'return n.NodeID as source, l.NodeID as link, m.NodeID as sink, n.Site as source_site, ' \
                 'm.Site as sink_site, cp1.NodeID as source_cp, cp2.NodeID as sink_cp'
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id).values()
         if val is None:
             return list()
         return val
```

### Comparing `fabric_fim-1.4.9/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.5.0b1/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/slices/abc_asm.py` & `fabric_fim-1.5.0b1/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.5.0b1/fim/graph/slices/neo4j_asm.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,27 +36,27 @@
         super().__init__(graph_id=graph_id, importer=importer, logger=logger)
 
     def check_node_name(self, *, node_id: str, label: str, name: str) -> bool:
         assert node_id is not None
         assert label is not None
         assert name is not None
 
-        query = f"MATCH (n:{label} {{GraphID: $graphId, NodeID: $nodeId, Name: $name}}) " \
+        query = f"MATCH (n:GraphNode:{label} {{GraphID: $graphId, NodeID: $nodeId, Name: $name}}) " \
                 f"RETURN collect(n.NodeID) as nodeids"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, nodeId=node_id, name=name).single()
             if val is None or len(val.data()) == 0:
                 return False
             return len(val.data()['nodeids']) > 0
 
     def find_node_by_name(self, *, node_name: str, label: str) -> str:
 
         assert node_name is not None
         assert label is not None
-        query = f"MATCH(n:{label} {{GraphID: $graphId, Name: $name }}) RETURN collect(n.NodeID) as nodeids"
+        query = f"MATCH(n:GraphNode:{label} {{GraphID: $graphId, Name: $name }}) RETURN collect(n.NodeID) as nodeids"
         with self.driver.session() as session:
             val = session.run(query, graphId=self.graph_id, name=node_name).single()
             if val is None or len(val.data()) == 0:
                 raise PropertyGraphQueryException(graph_id=self.graph_id,
                                                   node_id=None,
                                                   msg=f"Unable to find node with name {node_name} class {label}")
             if len(val.data()['nodeids']) > 1:
```

### Comparing `fabric_fim-1.4.9/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.5.0b1/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/graph/typed_tuples.py` & `fabric_fim-1.5.0b1/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/logging/log_collector.py` & `fabric_fim-1.5.0b1/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/pluggable.py` & `fabric_fim-1.5.0b1/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/attached_components.py` & `fabric_fim-1.5.0b1/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/base_sliver.py` & `fabric_fim-1.5.0b1/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/capacities_labels.py` & `fabric_fim-1.5.0b1/fim/slivers/capacities_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,21 +345,22 @@
         # where we require the full 128 even if some of them are just ':::'
         'ipv6_subnet': (r'(?:[a-fA-F0-9]{0,4}:){0,7}[a-fA-F0-9]{0,4}/[\d]{1,2}',
                         "2001:0db8:85a3:0000:0000/48"),
         'asn': (r'[\d]+', "12345"),
         'vlan': (r'[\d]{1,4}', "1234"),
         'vlan_range': (r'[\d]{1,4}-[\d]{1,4}', "100-200"),
         'inner_vlan': (r'[\d]{1,4}', "1234"),
-        'bgp_key': (r'[\w\-+_/\.:]{6,150}', "Amazon or other bgp key"),
+        'bgp_key': (r'[\w\-+_/\.:]{6,150}', "Amazon or other BGP key"),
         # Azure UUID "3e2480b2-b4d5-3456-976a-7b0de65a1b62"
         # GCP <random>/<vlan-attachment-region>/<edge-availability-domain> "7e51371e-1234-40b5-b844-2e3efefaee59/us-central1/2"
         # AWS 12 digits
         # Oracle ocid1.<RESOURCE TYPE>.<REALM>.[REGION][.FUTURE USE].<UNIQUE ID> "ocid1.instance.oc1.phx.abuw4ljrlsfiqw6vzzxb67hyypt4pkodawglp3wqxjqofakrwvou52gb6s5a"
         'account_id': (r'[\w\-/\.]{3,100}', "Azure/GCP/AWS/Oracle account"),
-        'region': (r'[\w\-\.]{3,100}', "Azure/GCP/AWS/Oracle region identifier")
+        'region': (r'[\w\-\.]{3,100}', "Azure/GCP/AWS/Oracle region identifier"),
+        'usb_id': (r'[0-9a-f]{4}:[0-9a-f]{4}', "USB device id '1234:abcd'")
     }
     LAMBDA_VALIDATORS = {
         'vlan': ((lambda v: True if 0 <= int(v) <= 4096 else False), "0-4096"),
         'inner_vlan': ((lambda v: True if 0 <= int(v) <= 4096 else False), "0-4096"),
         'vlan_range': ((lambda v: True if 0 <= int(v.split('-')[0]) <= 4096 and
                                           0 <= int(v.split('-')[1]) <= 4096 and
                                           int(v.split('-')[0]) <= int(v.split('-')[1]) else False),
@@ -384,14 +385,15 @@
         self.instance_parent = None
         self.local_name = None
         self.local_type = None
         self.device_name = None
         self.bgp_key = None
         self.account_id = None
         self.region = None
+        self.usb_id = None
         self._set_fields(**kwargs)
 
     def _set_fields(self, **kwargs):
         """
         Universal setter for all fields. Values should be strings or lists of strings.
         Throws a LabelException if you try to set a non-existent field.
         :param kwargs:
```

### Comparing `fabric_fim-1.4.9/fim/slivers/component_catalog.py` & `fabric_fim-1.5.0b1/fim/slivers/component_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,22 @@
 
         cs = ComponentSliver()
         cs.set_name(name)
         cs.set_model(component_dict['Model'])
         cs.set_type(cs.type_from_str(component_dict['Type']))
         cs.set_details(component_dict['Details'])
         if 'Interfaces' in component_dict.keys():
+            # for components with interfaces
+            if cs.get_type() in [ComponentType.FPGA]:
+                ns_suffix = '-l2p4'
+                ns_type = ServiceType.P4
+            else:
+                ns_suffix = '-l2ovs'
+                ns_type = ServiceType.OVS
+
             interfaces_dict = component_dict['Interfaces']
             if interface_node_ids is not None:
                 if len(interface_node_ids) != len(interfaces_dict.keys()):
                     raise RuntimeError("The number of interface IDs provided is insufficient for this component "
                                        f"(need {len(interfaces_dict.keys())} instead of {len(interface_node_ids)}")
                 if len(interface_labels) != len(interfaces_dict.keys()):
                     raise RuntimeError("The number of PCI labels and MAC addresses provided is insufficient for this"
@@ -165,18 +173,18 @@
                 iinfo.add_interface(isliver)
             ns = NetworkServiceSliver()
             if ns_node_id is None:
                 ns_node_id = str(uuid.uuid4())
             ns.node_id = ns_node_id
             # network service names are supposed to be unique within a graph
             if parent_name is not None:
-                ns.set_name(parent_name + "-" + name + '-l2ovs')
+                ns.set_name(parent_name + "-" + name + ns_suffix)
             else:
-                ns.set_name(name + "-l2ovs")
-            ns.set_type(ServiceType.OVS)
+                ns.set_name(name + ns_suffix)
+            ns.set_type(ns_type)
             # default to L2 for now
             ns.set_layer(NSLayer.L2)
             ns.interface_info = iinfo
             nsinfo = NetworkServiceInfo()
             nsinfo.add_network_service(ns)
             cs.set_network_service_info(nsinfo)
         return cs
```

### Comparing `fabric_fim-1.4.9/fim/slivers/data/component_catalog.json` & `fabric_fim-1.5.0b1/fim/slivers/data/component_catalog.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9818181818181819%*

 * *Differences: {'10': "{'AlsoModels': ['Alveo U280']}"}*

```diff
@@ -67,14 +67,17 @@
     },
     {
         "Details": "Site-local NAS share",
         "Model": "NAS",
         "Type": "Storage"
     },
     {
+        "AlsoModels": [
+            "Alveo U280"
+        ],
         "Details": "Xilinx U280 FPGA Dual 100G port accelerator card",
         "Interfaces": {
             "p1": "100",
             "p2": "100"
         },
         "Model": "Xilinx-U280",
         "Type": "FPGA"
```

### Comparing `fabric_fim-1.4.9/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.5.0b1/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/delegations.py` & `fabric_fim-1.5.0b1/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/gateway.py` & `fabric_fim-1.5.0b1/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/identifiers.py` & `fabric_fim-1.5.0b1/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/instance_catalog.py` & `fabric_fim-1.5.0b1/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/interface_info.py` & `fabric_fim-1.5.0b1/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/json.py` & `fabric_fim-1.5.0b1/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/json_data.py` & `fabric_fim-1.5.0b1/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/maintenance_mode.py` & `fabric_fim-1.5.0b1/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/network_attached_storage.py` & `fabric_fim-1.5.0b1/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/network_link.py` & `fabric_fim-1.5.0b1/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/network_node.py` & `fabric_fim-1.5.0b1/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/network_service.py` & `fabric_fim-1.5.0b1/fim/slivers/network_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     """
     Services can be limited by the number of interfaces/connection points they can connect
     The number of sites they may connect and the number of instances they may have in a slice.
     """
     ServiceConstraints = {
         ServiceType.P4: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
                                                 num_interfaces=NO_LIMIT, num_sites=1,
-                                                num_instances=NO_LIMIT, required_properties=['controller_url'],
+                                                num_instances=NO_LIMIT, required_properties=[],
                                                 forbidden_properties=['mirror_port',
                                                                       'mirror_direction'],
                                                 required_interface_types=[],
                                                 desc='A P4 service.'),
         ServiceType.OVS: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
                                                  num_interfaces=NO_LIMIT, num_sites=1,
                                                  num_instances=NO_LIMIT, required_properties=[],
```

### Comparing `fabric_fim-1.4.9/fim/slivers/path_info.py` & `fabric_fim-1.5.0b1/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/tags.py` & `fabric_fim-1.5.0b1/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/slivers/topology_diff.py` & `fabric_fim-1.5.0b1/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/__init__.py` & `fabric_fim-1.5.0b1/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/component.py` & `fabric_fim-1.5.0b1/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/composite_node.py` & `fabric_fim-1.5.0b1/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/interface.py` & `fabric_fim-1.5.0b1/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/link.py` & `fabric_fim-1.5.0b1/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/measurement.py` & `fabric_fim-1.5.0b1/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/model_element.py` & `fabric_fim-1.5.0b1/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/network_service.py` & `fabric_fim-1.5.0b1/fim/user/network_service.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/node.py` & `fabric_fim-1.5.0b1/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/user/topology.py` & `fabric_fim-1.5.0b1/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/fim/view_only_dict.py` & `fabric_fim-1.5.0b1/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/test/test_load.py` & `fabric_fim-1.5.0b1/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.9/util/fim_util.py` & `fabric_fim-1.5.0b1/fim/util/fim_util.py`

 * *Files identical despite different names*

