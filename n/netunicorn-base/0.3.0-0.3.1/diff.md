# Comparing `tmp/netunicorn-base-0.3.0.tar.gz` & `tmp/netunicorn-base-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-base-0.3.0.tar", last modified: Mon May  8 20:49:08 2023, max compression
+gzip compressed data, was "netunicorn-base-0.3.1.tar", last modified: Wed May 10 07:50:11 2023, max compression
```

## Comparing `netunicorn-base-0.3.0.tar` & `netunicorn-base-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/
--rw-rw-r--   0 kell      (1000) kell      (1000)      490 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      859 2023-04-30 04:38:09.000000 netunicorn-base-0.3.0/pyproject.toml
--rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/setup.cfg
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/base/
--rw-rw-r--   0 kell      (1000) kell      (1000)      509 2023-04-12 23:52:52.000000 netunicorn-base-0.3.0/src/netunicorn/base/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      138 2023-02-18 01:38:41.000000 netunicorn-base-0.3.0/src/netunicorn/base/architecture.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     3141 2023-04-11 10:37:18.000000 netunicorn-base-0.3.0/src/netunicorn/base/deployment.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     5279 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/environment_definitions.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     6263 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/base/experiment.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     8831 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/base/nodes.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     3448 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/pipeline.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     4794 2023-03-17 07:55:21.000000 netunicorn-base-0.3.0/src/netunicorn/base/task.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     2509 2023-04-12 22:04:55.000000 netunicorn-base-0.3.0/src/netunicorn/base/types.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     3391 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/utils.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/base/
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-02-18 01:38:41.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/__init__.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     7486 2023-04-30 04:12:53.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/protocol.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      109 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/types.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     1907 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/resources.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      373 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/types.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      314 2023-03-23 00:43:02.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/utils.py
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/py.typed
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/
--rw-rw-r--   0 kell      (1000) kell      (1000)      490 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      894 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/SOURCES.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/dependency_links.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       35 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/requires.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.179487 netunicorn-base-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 07:50:11.175487 netunicorn-base-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:50:11.179487 netunicorn-base-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.171487 netunicorn-base-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.171487 netunicorn-base-0.3.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.175487 netunicorn-base-0.3.1/src/netunicorn/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/environment_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.171487 netunicorn-base-0.3.1/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.175487 netunicorn-base-0.3.1/src/netunicorn/director/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.175487 netunicorn-base-0.3.1/src/netunicorn/director/base/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/connectors/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/connectors/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/director/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:49:54.000000 netunicorn-base-0.3.1/src/netunicorn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:11.175487 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 07:50:11.000000 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-10 07:50:11.000000 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:50:11.000000 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 07:50:11.000000 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 07:50:11.000000 netunicorn-base-0.3.1/src/netunicorn_base.egg-info/top_level.txt
```

### Comparing `netunicorn-base-0.3.0/pyproject.toml` & `netunicorn-base-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-base"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn base module"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/deployment.py` & `netunicorn-base-0.3.1/src/netunicorn/base/deployment.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,27 +34,36 @@
         self.executor_id = ""
         self.error: Optional[Exception] = None
         self.pipeline: SerializedPipelineType = b""
         self.environment_definition = deepcopy(pipeline.environment_definition)
         self.keep_alive_timeout_minutes = keep_alive_timeout_minutes
         self.cleanup = cleanup
 
+        self._validate_deployment(node, pipeline)
+
         pipeline = deepcopy(pipeline)
 
         for i, element in enumerate(pipeline.tasks):
             pipeline.tasks[i] = [
                 x.dispatch(node) if isinstance(x, TaskDispatcher) else x
                 for x in element
             ]
             for x in pipeline.tasks[i]:
                 # now it's only Tasks
                 self.environment_definition.commands.extend(x.requirements)  # type: ignore
 
         self.pipeline = cloudpickle.dumps(pipeline)
 
+    @staticmethod
+    def _validate_deployment(node: Node, pipeline: Pipeline) -> None:
+        if type(pipeline.environment_definition) not in node.available_environments:
+            raise ValueError(
+                f"Node {node.name} does not support environment {type(pipeline.environment_definition).__name__}"
+            )
+
     def __str__(self) -> str:
         return f"Deployment: Node={self.node.name}, executor_id={self.executor_id}, prepared={self.prepared}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __json__(self) -> DeploymentRepresentation:
```

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/environment_definitions.py` & `netunicorn-base-0.3.1/src/netunicorn/base/environment_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,7 +157,13 @@
         data: DockerImageRepresentation = _data  # type: ignore
         instance = cls.__new__(cls)
         instance.commands = data["commands"]
         instance.image = data["image"]
         instance.build_context = BuildContext.from_json(data["build_context"])
         instance.runtime_context = RuntimeContext.from_json(data["runtime_context"])
         return instance
+
+
+_available_environment_definitions = {
+    ShellExecution.__name__: ShellExecution,
+    DockerImage.__name__: DockerImage,
+}
```

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/experiment.py` & `netunicorn-base-0.3.1/src/netunicorn/base/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import base64
 import copy
 from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, Iterator, List, Optional, Sequence, Tuple, Union
 
+from returns.pipeline import is_successful
 from returns.result import Result
 
 from .deployment import Deployment
 from .nodes import Node, Nodes
 from .pipeline import Pipeline
 from .types import (
     DeploymentExecutionResultRepresentation,
@@ -77,18 +78,18 @@
     def __iter__(self) -> Iterator[Deployment]:
         return iter(self.deployment_map)
 
     def __len__(self) -> int:
         return len(self.deployment_map)
 
     def __str__(self) -> str:
-        return "; ".join([f"<{x}>" for x in self.deployment_map])
+        return "\n".join([f" - {x}" for x in self.deployment_map])
 
     def __repr__(self) -> str:
-        return str(self)
+        return self.__str__()
 
     def __add__(self, other: Experiment) -> Experiment:
         new_map = copy.deepcopy(self)
         new_map.deployment_map.extend(other.deployment_map)
         if other.deployment_context:
             if new_map.deployment_context is None:
                 new_map.deployment_context = {}
@@ -120,15 +121,30 @@
         self,
     ) -> Optional[Tuple[Result[PipelineResult, PipelineResult], LogType]]:
         import cloudpickle
 
         return cloudpickle.loads(self._result) if self._result else None
 
     def __str__(self) -> str:
-        return f"DeploymentExecutionResult(node={self.node}, result={self.result}, error={self.error})"
+        text = "DeploymentExecutionResult:\n  Node: {self.node}\n"
+        if self._result:
+            result: Tuple[Result[PipelineResult, PipelineResult], LogType] = self.result  # type: ignore
+            text += f"  Result: {type(result[0])}\n"
+            if not is_successful(result[0]):
+                text += f"   {result[0]}\n"
+            else:
+                for task_id, task_result in result[0].unwrap().items():
+                    text += f"    {task_id}: {task_result}\n"
+            text += f"  Logs:\n"
+            for line in result[1]:
+                text += f"    {line}"
+        if self.error:
+            text += f"  Error: {self.error}\n"
+        text += "\n"
+        return text
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __json__(self) -> DeploymentExecutionResultRepresentation:
         return {
             "node": self.node.__json__(),
@@ -153,14 +169,28 @@
 
 @dataclass(frozen=True)
 class ExperimentExecutionInformation:
     status: ExperimentStatus
     experiment: Optional[Experiment]
     execution_result: Union[None, Exception, List[DeploymentExecutionResult]]
 
+    def __str__(self) -> str:
+        text = (
+            f"ExperimentExecutionInformation:\n"
+            f"status: {self.status}\n"
+            f"experiment: \n"
+            f"{self.experiment}\n"
+            f"execution_result:\n"
+            f"{self.execution_result}\n"
+        )
+        return text
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
     def __json__(self) -> ExperimentExecutionInformationRepresentation:
         execution_result: Union[
             None, str, List[DeploymentExecutionResultRepresentation]
         ] = None
         if isinstance(self.execution_result, list):
             execution_result = [x.__json__() for x in self.execution_result]
         elif isinstance(self.execution_result, Exception):
```

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/nodes.py` & `netunicorn-base-0.3.1/src/netunicorn/base/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from itertools import chain, cycle
-from typing import Callable, Dict, Iterator, List, Sequence, Union
+from typing import Callable, Dict, Iterator, List, Sequence, Set, Union
 from uuid import uuid4
 
 import netunicorn
 
 from .architecture import Architecture
+from .environment_definitions import _available_environment_definitions
 from .types import NodeProperty, NodeRepresentation, NodesRepresentation
 
 
 class Node:
     def __init__(
         self,
         name: str,
         properties: Dict[str, NodeProperty],
         architecture: Architecture = Architecture.UNKNOWN,
     ):
         self.name = name
         self.properties = properties
         self.additional_properties: Dict[str, NodeProperty] = {}
         self.architecture = architecture
+        self.available_environments: Set[type] = self._infer_environments()
+
+    def _infer_environments(self) -> Set[type]:
+        result = set()
+        # noinspection PyBroadException
+        try:
+            environments = self.properties.get(
+                "netunicorn-environments", _available_environment_definitions.keys()
+            )
+            if hasattr(environments, "__iter__"):
+                for environment_name in environments:  # type: ignore
+                    if environment_name in _available_environment_definitions:
+                        result.add(_available_environment_definitions[environment_name])
+        except Exception:
+            return set(_available_environment_definitions.values())
+        return result
 
     def __getitem__(self, item: str) -> NodeProperty:
         return self.properties.get(item, None)
 
     def __iter__(self) -> Iterator[NodeProperty]:
         raise TypeError("Node is not iterable")
```

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/pipeline.py` & `netunicorn-base-0.3.1/src/netunicorn/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/task.py` & `netunicorn-base-0.3.1/src/netunicorn/base/task.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/types.py` & `netunicorn-base-0.3.1/src/netunicorn/base/types.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn/base/utils.py` & `netunicorn-base-0.3.1/src/netunicorn/base/utils.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/protocol.py` & `netunicorn-base-0.3.1/src/netunicorn/director/base/connectors/protocol.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn/director/base/resources.py` & `netunicorn-base-0.3.1/src/netunicorn/director/base/resources.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.3.0/src/netunicorn_base.egg-info/SOURCES.txt` & `netunicorn-base-0.3.1/src/netunicorn_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

