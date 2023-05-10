# Comparing `tmp/cognite_transformations_cli-2.3.3.tar.gz` & `tmp/cognite_transformations_cli-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_transformations_cli-2.3.3.tar", max compression
+gzip compressed data, was "cognite_transformations_cli-2.3.4.tar", max compression
```

## Comparing `cognite_transformations_cli-2.3.3.tar` & `cognite_transformations_cli-2.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10172 2023-03-17 10:25:46.444707 cognite_transformations_cli-2.3.3/LICENSE
--rw-r--r--   0        0        0     4288 2023-03-17 10:25:46.444707 cognite_transformations_cli-2.3.3/README.md
--rw-r--r--   0        0        0       22 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/__init__.py
--rw-r--r--   0        0        0      270 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/__main__.py
--rw-r--r--   0        0        0     2933 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/clients.py
--rw-r--r--   0        0        0        0 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/__init__.py
--rw-r--r--   0        0        0     3615 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/base.py
--rw-r--r--   0        0        0     1491 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/delete.py
--rw-r--r--   0        0        0        0 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/__init__.py
--rw-r--r--   0        0        0     6459 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/deploy.py
--rw-r--r--   0        0        0     6754 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/load_yaml.py
--rw-r--r--   0        0        0     5351 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_config.py
--rw-r--r--   0        0        0     3972 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_types.py
--rw-r--r--   0        0        0     4705 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
--rw-r--r--   0        0        0    13957 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformations_api.py
--rw-r--r--   0        0        0     2166 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/jobs.py
--rw-r--r--   0        0        0     2438 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/list.py
--rw-r--r--   0        0        0     1242 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/query.py
--rw-r--r--   0        0        0     3639 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/run.py
--rw-r--r--   0        0        0     2787 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/show.py
--rw-r--r--   0        0        0     5792 2023-03-17 10:25:46.448707 cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/utils.py
--rw-r--r--   0        0        0     1616 2023-03-17 10:25:46.452707 cognite_transformations_cli-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/LICENSE
+-rw-r--r--   0        0        0     4288 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/__main__.py
+-rw-r--r--   0        0        0     2933 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/clients.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/base.py
+-rw-r--r--   0        0        0     1491 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/delete.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/__init__.py
+-rw-r--r--   0        0        0     6459 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/deploy.py
+-rw-r--r--   0        0        0     6754 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/load_yaml.py
+-rw-r--r--   0        0        0     5351 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_config.py
+-rw-r--r--   0        0        0     4342 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types.py
+-rw-r--r--   0        0        0     4705 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
+-rw-r--r--   0        0        0    13811 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformations_api.py
+-rw-r--r--   0        0        0     2166 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/jobs.py
+-rw-r--r--   0        0        0     2438 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/list.py
+-rw-r--r--   0        0        0     1242 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/query.py
+-rw-r--r--   0        0        0     3639 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/run.py
+-rw-r--r--   0        0        0     2787 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/show.py
+-rw-r--r--   0        0        0     5792 2023-05-10 07:21:58.053352 cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/utils.py
+-rw-r--r--   0        0        0     1616 2023-05-10 07:21:58.057352 cognite_transformations_cli-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.4/PKG-INFO
```

### Comparing `cognite_transformations_cli-2.3.3/LICENSE` & `cognite_transformations_cli-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/README.md` & `cognite_transformations_cli-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/clients.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/clients.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/base.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/delete.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/deploy.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/load_yaml.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/load_yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_config.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_config.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_types.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
 
-class DestinationType(Enum):
+class DestinationType(str, Enum):
     assets = "assets"
     timeseries = "timeseries"
     asset_hierarchy = "asset_hierarchy"
     events = "events"
     datapoints = "datapoints"
     string_datapoints = "string_datapoints"
     sequences = "sequences"
@@ -90,15 +90,24 @@
     type: DestinationType = DestinationType.data_model_instances
 
 
 @dataclass
 class ViewInfo:
     space: str
     external_id: str
-    version: str
+    version: Union[int, str]
+
+    """
+    CAST view version int to string
+    """
+
+    def __init__(self, space: str, external_id: str, version: Union[int, str]):
+        self.space = space
+        self.external_id = external_id
+        self.version = str(version)
 
 
 @dataclass
 class EdgeType:
     space: str
     external_id: str
 
@@ -107,27 +116,29 @@
 class InstanceNodesDestinationConfig:
     """
     Valid type values are: nodes
     """
 
     view: Optional[ViewInfo]
     instance_space: Optional[str]
-    type: DestinationType = DestinationType.nodes
+    type: Literal[DestinationType.nodes] = DestinationType.nodes
 
 
 @dataclass
 class InstanceEdgesDestinationConfig:
     """
     Valid type values are: edges
     """
 
     view: Optional[ViewInfo]
     instance_space: Optional[str]
     edge_type: Optional[EdgeType]
-    type: DestinationType = DestinationType.edges
+    type: Literal[
+        DestinationType.edges
+    ] = DestinationType.edges  # DestinationType updated with  Literal[DestinationType.edges]
 
 
 @dataclass
 class SequenceRowsDestinationConfig:
     """
     Valid type values are: sequence_rows
     """
```

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/deploy/transformations_api.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/deploy/transformations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,18 @@
 from cognite.transformations_cli.commands.utils import chunk_items, exit_with_cognite_api_error
 
 TupleResult = List[Tuple[str, str]]
 StandardResult = List[str]
 
 
 def to_transformation(
-    client: CogniteClient, conf_path: str, config: TransformationConfig, cluster: str = "europe-west1-1"
+    client: CogniteClient,
+    conf_path: str,
+    config: TransformationConfig,
+    cluster: str = "europe-west1-1",
 ) -> Transformation:
     return Transformation(
         name=config.name,
         external_id=config.external_id,
         destination=to_destination(config.destination),
         conflict_mode=to_action(config.action),
         is_public=config.shared,
@@ -60,15 +63,17 @@
         destination_oidc_credentials=to_write_oidc(config.authentication, cluster),
         data_set_id=to_data_set_id(client, config.data_set_id, config.data_set_external_id),
         tags=config.tags,
     )
 
 
 def to_data_set_id(
-    client: CogniteClient, data_set_id: Optional[int], data_set_external_id: Optional[str]
+    client: CogniteClient,
+    data_set_id: Optional[int],
+    data_set_external_id: Optional[str],
 ) -> Optional[int]:
     err = ""
     if data_set_external_id:
         try:
             data_set = client.data_sets.retrieve(external_id=data_set_external_id)
         except CogniteAPIError as e:
             err = f" ({e})"
@@ -93,33 +98,42 @@
         return TransformationDestination.raw(destination.raw_database, destination.raw_table)
     elif isinstance(destination, RawDestinationAlternativeConfig):
         return TransformationDestination.raw(destination.database, destination.table)
     elif isinstance(destination, SequenceRowsDestinationConfig):
         return SequenceRows(destination.external_id)
     elif isinstance(destination, DMIDestinationConfig):
         return DataModelInstances(
-            destination.model_external_id, destination.space_external_id, destination.instance_space_external_id
+            destination.model_external_id,
+            destination.space_external_id,
+            destination.instance_space_external_id,
         )
-    elif isinstance(destination, InstanceNodesDestinationConfig) or isinstance(
-        destination, InstanceEdgesDestinationConfig
-    ):
-        if destination.type == InstanceNodesDestinationConfig.type:
-            view = None
-            if destination.view:
-                view = ViewInfo(destination.view.space, destination.view.external_id, destination.view.version)
-            return InstanceNodes(view, destination.instance_space)
-        elif destination.type == InstanceEdgesDestinationConfig.type:
-            view = None
-            if destination.view:
-                view = ViewInfo(destination.view.space, destination.view.external_id, destination.view.version)
-            edge_type = None
-            # This is a hack, we should have better fix since destination is still InstanceNodesDestinationConfig here...
-            if isinstance(destination, InstanceEdgesDestinationConfig) and destination.edge_type:
-                edge_type = EdgeType(destination.edge_type.space, destination.edge_type.external_id)
-            return InstanceEdges(view, destination.instance_space, edge_type)
+
+    elif isinstance(destination, InstanceNodesDestinationConfig):
+        view = None
+        if destination.view:
+            view = ViewInfo(
+                destination.view.space,
+                destination.view.external_id,
+                destination.view.version,
+            )
+        return InstanceNodes(view, destination.instance_space)
+
+    elif isinstance(destination, InstanceEdgesDestinationConfig):
+        view = None
+        if destination.view:
+            view = ViewInfo(
+                destination.view.space,
+                destination.view.external_id,
+                destination.view.version,
+            )
+        edge_type = None
+        if destination.edge_type:
+            edge_type = EdgeType(destination.edge_type.space, destination.edge_type.external_id)
+        return InstanceEdges(view, destination.instance_space, edge_type)
+
     else:
         return TransformationDestination(destination.value)
 
 
 def to_query(conf_path: str, query: Union[str, QueryConfig]) -> str:
     try:
         dir_path = os.path.dirname(conf_path)
@@ -261,15 +275,19 @@
                 for du in u
             ]
             client.transformations.update(dataset_update)
 
         for c in chunk_items(items_to_create):
             client.transformations.create(c)
 
-        return [], [t.external_id for t in items_to_update], [t.external_id for t in items_to_create]
+        return (
+            [],
+            [t.external_id for t in items_to_update],
+            [t.external_id for t in items_to_create],
+        )
     except (CogniteDuplicatedError, CogniteNotFoundError, CogniteAPIError) as e:
         exit_with_cognite_api_error(e)
     return [], [], []
 
 
 def upsert_schedules(
     client: CogniteClient,
```

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/jobs.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/list.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/query.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/run.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/show.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/cognite/transformations_cli/commands/utils.py` & `cognite_transformations_cli-2.3.4/cognite/transformations_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.3/pyproject.toml` & `cognite_transformations_cli-2.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-transformations-cli"
-version = "2.3.3"
+version = "2.3.4"
 description = "A CLI for the Transformations service in CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>", "Emel Varol <emel.varol@cognite.com>", "Einar Marstrander Omang <einar.omang@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/transformations-cli"
 
 packages = [
```

### Comparing `cognite_transformations_cli-2.3.3/PKG-INFO` & `cognite_transformations_cli-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-transformations-cli
-Version: 2.3.3
+Version: 2.3.4
 Summary: A CLI for the Transformations service in CDF
 Home-page: https://github.com/cognitedata/transformations-cli
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

