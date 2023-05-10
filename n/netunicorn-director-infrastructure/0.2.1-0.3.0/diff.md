# Comparing `tmp/netunicorn-director-infrastructure-0.2.1.tar.gz` & `tmp/netunicorn-director-infrastructure-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-director-infrastructure-0.2.1.tar", last modified: Thu Feb 16 01:28:13 2023, max compression
+gzip compressed data, was "netunicorn-director-infrastructure-0.3.0.tar", last modified: Wed May 10 08:32:56 2023, max compression
```

## Comparing `netunicorn-director-infrastructure-0.2.1.tar` & `netunicorn-director-infrastructure-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/
--rw-rw-r--   0 kell      (1000) kell      (1000)     1067 2023-02-13 02:46:42.000000 netunicorn-director-infrastructure-0.2.1/LICENSE
--rw-rw-r--   0 kell      (1000) kell      (1000)      828 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      486 2023-02-13 02:46:33.000000 netunicorn-director-infrastructure-0.2.1/README.md
--rw-rw-r--   0 kell      (1000) kell      (1000)      627 2023-02-16 01:27:50.000000 netunicorn-director-infrastructure-0.2.1/pyproject.toml
--rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/setup.cfg
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-02-13 02:46:33.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      415 2023-02-14 21:59:55.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/__main__.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-02-13 02:46:33.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     2690 2023-02-15 01:04:23.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/dummy.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     4364 2023-02-15 00:35:59.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/protocol.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/rest/
--rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-02-15 00:45:16.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/rest/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     4450 2023-02-15 02:15:32.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     2938 2023-02-15 02:17:50.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py
--rw-rw-r--   0 kell      (1000) kell      (1000)      109 2023-02-13 02:46:33.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/connectors/types.py
--rw-rw-r--   0 kell      (1000) kell      (1000)    19446 2023-02-15 22:50:02.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/kernel.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     3021 2023-02-15 01:08:37.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/server.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-02-16 01:28:13.356327 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/
--rw-rw-r--   0 kell      (1000) kell      (1000)      828 2023-02-16 01:28:13.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      997 2023-02-16 01:28:13.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-02-16 01:28:13.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       70 2023-02-16 01:28:13.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/requires.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-02-16 01:28:13.000000 netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.010753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-10 08:32:44.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:32:56.014753 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:32:56.000000 netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/top_level.txt
```

### Comparing `netunicorn-director-infrastructure-0.2.1/LICENSE` & `netunicorn-director-infrastructure-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-director-infrastructure-0.2.1/PKG-INFO` & `netunicorn-director-infrastructure-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-director-infrastructure
-Version: 0.2.1
+Version: 0.3.0
 Summary: netunicorn infrastructure module
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-director-infrastructure-0.2.1/pyproject.toml` & `netunicorn-director-infrastructure-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [project]
 name = "netunicorn-director-infrastructure"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn infrastructure module"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "fastapi",
-    "netunicorn-base >= 0.2.0",
+    "netunicorn-base >= 0.3.0",
     "uvicorn",
     "asyncpg",
     "pyyaml",
     "returns",
     "aiohttp",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
 python_version = "3.10"
 ignore_missing_imports = true
-strict = true
+explicit_package_bases = true
+strict = true
+exclude = "tests"
+mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
```

### Comparing `netunicorn-director-infrastructure-0.2.1/src/netunicorn/director/infrastructure/kernel.py` & `netunicorn-director-infrastructure-0.3.0/src/netunicorn/director/infrastructure/kernel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from __future__ import annotations
 
+import asyncio
 import importlib
 import os
 from collections import defaultdict
 from logging import Logger
-from typing import Union, Any, Tuple, Optional
+from typing import Any, NoReturn, Optional, Tuple, Union
 
 import asyncpg
 import yaml
 from asyncpg import Record
 from fastapi import BackgroundTasks
 from netunicorn.base.deployment import Deployment
 from netunicorn.base.experiment import Experiment, ExperimentStatus
 from netunicorn.base.nodes import CountableNodePool, Nodes
+from netunicorn.base.types import ExperimentRepresentation
+from netunicorn.director.base.connectors.protocol import NetunicornConnectorProtocol
+from netunicorn.director.base.connectors.types import StopExecutorRequest
 from netunicorn.director.base.resources import LOGGING_LEVELS, get_logger
+from netunicorn.director.base.types import ConnectorContext
 from netunicorn.director.base.utils import __init_connection
 from returns.result import Failure, Success
 
-from .connectors.protocol import NetunicornConnectorProtocol
-from .connectors.types import StopExecutorRequest
+from .tasks import cleanup_watchdog_task
 
 logger: Logger
 db_connection_pool: asyncpg.pool.Pool
 connectors: dict[str, NetunicornConnectorProtocol] = {}
+tasks: dict[str, asyncio.Task[NoReturn]] = {}  # type: ignore
 
 
 async def initialize_connector(
     connector_name: str, config: dict[str, Any], default_gateway: str
 ) -> None:
     if "enabled" in config and not config["enabled"]:
         logger.info(f"Skipping connector {connector_name} as disabled")
@@ -51,15 +56,15 @@
         connector = cls(
             connector_name, config_file, netunicorn_gateway, connector_logger
         )
         await connector.initialize()
         connectors[connector_name] = connector
         logger.info(f"Connector {connector_name} initialized")
     except Exception as e:
-        logger.error(f"Failed to initialize connector {connector_name}: {e}")
+        logger.exception(f"Failed to initialize connector {connector_name}: {e}")
     return
 
 
 def parse_config(filepath: str) -> dict[str, Any]:
     """
     Parse configuration file
     All parameters are read from the next priority list:
@@ -76,31 +81,32 @@
 
     with open(filepath, "r") as f:
         config = yaml.safe_load(f)
         assert isinstance(config, dict)
 
     # log level
     config["netunicorn.infrastructure.log.level"] = (
-        os.environ.get("NETUNICORN_INFRASTRUCTURE_LOG_LEVEL", False)
-        or config.get("netunicorn.infrastructure.log.level", False)
+        os.environ.get("NETUNICORN_INFRASTRUCTURE_LOG_LEVEL", None)
+        or config.get("netunicorn.infrastructure.log.level", None)
+        or os.environ.get("NETUNICORN_LOG_LEVEL", None)
         or "info"
-    )
+    ).lower()
     logger_level = config["netunicorn.infrastructure.log.level"].upper()
     if logger_level not in LOGGING_LEVELS:
         raise ValueError(f"Invalid log level {logger_level}")
     logger = get_logger(
         "netunicorn.director.infrastructure", LOGGING_LEVELS[logger_level]
     )
     logger.info(f"Logger initialized, level: {logger_level}")
 
     # module host and port
     config["netunicorn.infrastructure.host"] = (
-        os.environ.get("NETUNICORN_INFRASTRUCTURE_HOST", False)
-        or config.get("netunicorn.infrastructure.host", False)
-        or "127.0.0.1"
+        os.environ.get("NETUNICORN_INFRASTRUCTURE_IP", False)
+        or config.get("netunicorn.infrastructure.ip", False)
+        or "0.0.0.0"
     )
     logger.info(f"Host: {config['netunicorn.infrastructure.host']}")
     config["netunicorn.infrastructure.port"] = (
         int(os.environ.get("NETUNICORN_INFRASTRUCTURE_PORT", False))
         or int(config.get("netunicorn.infrastructure.port", False))
         or 26514
     )
@@ -137,15 +143,15 @@
     logger.info(
         f"Database: {config['netunicorn.database.db']}, user: {config['netunicorn.database.user']}, endpoint: {config['netunicorn.database.endpoint']}"
     )
     return config
 
 
 async def initialize(config: dict[str, Any]) -> None:
-    global db_connection_pool, connectors
+    global db_connection_pool
 
     db_connection_pool = await asyncpg.create_pool(
         host=config["netunicorn.database.endpoint"],
         user=config["netunicorn.database.user"],
         password=config["netunicorn.database.password"],
         database=config["netunicorn.database.db"],
         init=__init_connection,
@@ -157,31 +163,40 @@
         logger.warning("No connectors configured")
 
     for connector_name, connector_config in connectors_config.items():
         await initialize_connector(
             connector_name, connector_config, config["netunicorn.gateway.endpoint"]
         )
 
+    tasks["cleanup"] = asyncio.create_task(
+        cleanup_watchdog_task(
+            connectors=connectors, db_conn_pool=db_connection_pool, logger=logger
+        )
+    )
+
     return
 
 
 async def health() -> Tuple[int, str]:
     statuses: list[Tuple[str, bool, str]] = []
     try:
         await db_connection_pool.fetchval("SELECT 1")
         statuses.append(("database", True, "OK"))
     except Exception as e:
         statuses.append(("database", False, str(e)))
 
-    for connector_name, connector in connectors.items():
+    for connector_name in set(connectors.keys()):
+        connector = connectors[connector_name]
         try:
             status, description = await connector.health()
         except Exception as e:
             status, description = False, str(e)
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
             logger.warning(f"Connector {connector_name} moved to unavailable status.")
             connectors.pop(connector_name)
         statuses.append((connector_name, status, description))
 
     global_status = 200 if all([status for _, status, _ in statuses]) else 500
     return global_status, "\n".join(
         [f"{name}: {status} - {description}" for name, status, description in statuses]
@@ -190,95 +205,141 @@
 
 async def shutdown() -> None:
     await db_connection_pool.close()
     for connector_name, connector in connectors.items():
         try:
             await connector.shutdown()
         except Exception as e:
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
 
 
-async def get_nodes(username: str) -> Tuple[int, Union[Nodes, str]]:
+async def get_nodes(
+    username: str,
+    netunicorn_authentication_context: ConnectorContext = None,
+) -> Tuple[int, Union[Nodes, str]]:
     pools = []
-    for connector_name, connector in connectors.items():
+    for connector_name in set(connectors.keys()):
+        connector = connectors[connector_name]
         try:
-            nodes = await connector.get_nodes(username)
+            connector_authentication_context = None
+            if (
+                netunicorn_authentication_context
+                and connector_name in netunicorn_authentication_context
+            ):
+                connector_authentication_context = netunicorn_authentication_context[
+                    connector_name
+                ]
+            nodes = await connector.get_nodes(
+                username, connector_authentication_context
+            )
             nodes.set_property("connector", connector_name)
             pools.append(nodes)
         except Exception as e:
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
             logger.warning(f"Connector {connector_name} moved to unavailable status.")
             connectors.pop(connector_name)
-    pools = CountableNodePool(nodes=pools)
-    return 200, pools
+    return 200, CountableNodePool(nodes=pools)  # type: ignore
 
 
 async def deploy(
-    username: str, experiment_id: str, background_tasks: BackgroundTasks
+    username: str,
+    experiment_id: str,
+    background_tasks: BackgroundTasks,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> Tuple[int, str]:
     # 1. take experiment information from the database
-    experiment_data: Optional[dict[str, Any]] = await db_connection_pool.fetchval(
+    experiment_data: ExperimentRepresentation = await db_connection_pool.fetchval(
         "SELECT data::jsonb FROM experiments WHERE experiment_id = $1",
         experiment_id,
     )
     if experiment_data is None:
         return 404, f"Experiment {experiment_id} not found"
 
     experiment: Experiment = Experiment.from_json(experiment_data)
-    logger.debug(f"Starting deployment of experiment {experiment_id}")
+    logger.info(f"Starting deployment of experiment {experiment_id}")
 
     # 2. find all prepared deployments per each connector
     deployments: dict[str, list[Deployment]] = defaultdict(list)
     for deployment in experiment.deployment_map:
         if not deployment.prepared:
-            logger.debug(
+            logger.info(
                 f"Skipping deployment of not prepared executor {deployment.executor_id}, node {deployment.node}"
             )
             continue
-        deployments[deployment.node["connector"]].append(deployment)
+        deployments[str(deployment.node["connector"])].append(deployment)
 
     # 3. check that all connectors are available
     for connector_name in deployments.keys():
         if connector_name not in connectors:
             return (
                 500,
                 f"Connector {connector_name} participating in the experiment {experiment_id} is not available, cannot proceed",
             )
 
     # 4. start background task to deploy
     background_tasks.add_task(
-        background_deploy_task, username, experiment_id, deployments
+        background_deploy_task,
+        username,
+        experiment_id,
+        deployments,
+        experiment.deployment_context,
+        netunicorn_authentication_context,
     )
     return 200, f"Deployment of experiment {experiment_id} started"
 
 
 async def background_deploy_task(
-    username: str, experiment_id: str, deployments: dict[str, list[Deployment]]
+    username: str,
+    experiment_id: str,
+    deployments: dict[str, list[Deployment]],
+    deployment_context: Optional[dict[str, dict[str, str]]],
+    netunicorn_authentication_context: Optional[dict[str, dict[str, str]]] = None,
 ) -> None:
     # 5. deploy on each connector
     for connector_name, connector_deployments in deployments.items():
         try:
+            connector_deploy_context = None
+            if deployment_context and connector_name in deployment_context:
+                connector_deploy_context = deployment_context[connector_name]
+            connector_auth_context = None
+            if (
+                netunicorn_authentication_context
+                and connector_name in netunicorn_authentication_context
+            ):
+                connector_auth_context = netunicorn_authentication_context[
+                    connector_name
+                ]
             results = await connectors[connector_name].deploy(
-                username, experiment_id, connector_deployments
+                username,
+                experiment_id,
+                connector_deployments,
+                connector_deploy_context,
+                connector_auth_context,
             )
         except Exception as e:
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
             logger.warning(f"Connector {connector_name} moved to unavailable status.")
             connectors.pop(connector_name)
             failure_reason = f"Connector {connector_name} raised an exception and deployment couldn't be completed"
             results = {
                 deployment.executor_id: Failure(failure_reason)
                 for deployment in connector_deployments
             }
 
         # each key in result is an executor id, value is Success or Failure with description
         # noinspection DuplicatedCode
         for executor_id, result in results.items():
             if isinstance(result, Success):
-                logger.debug(
+                logger.info(
                     f"Deployment of executor {executor_id} on connector {connector_name} succeeded"
                 )
                 continue
 
             failure_reason = str(result.failure())
             logger.warning(
                 f"Deployment of executor {executor_id} on connector {connector_name} failed: {failure_reason}"
@@ -286,34 +347,38 @@
             await db_connection_pool.execute(
                 "UPDATE executors SET finished = TRUE, error = $1 WHERE experiment_id = $2 AND executor_id = $3",
                 failure_reason,
                 experiment_id,
                 executor_id,
             )
 
-    logger.debug(f"Experiment {experiment_id} deployment finished")
+    logger.info(f"Experiment {experiment_id} deployment finished")
     await db_connection_pool.execute(
         "UPDATE experiments SET status = $1 WHERE experiment_id = $2",
         ExperimentStatus.READY.value,
         experiment_id,
     )
 
 
 async def execute(
-    username: str, experiment_id: str, background_tasks: BackgroundTasks
+    username: str,
+    experiment_id: str,
+    background_tasks: BackgroundTasks,
+    execution_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> Tuple[int, str]:
     # 1. take experiment information from the database
-    experiment_data: Optional[dict[str, Any]] = await db_connection_pool.fetchval(
+    experiment_data: ExperimentRepresentation = await db_connection_pool.fetchval(
         "SELECT data::jsonb FROM experiments WHERE experiment_id = $1",
         experiment_id,
     )
     if experiment_data is None:
         return 404, f"Experiment {experiment_id} not found"
     experiment: Experiment = Experiment.from_json(experiment_data)
-    logger.debug(f"Starting execution of experiment {experiment_id}")
+    logger.info(f"Starting execution of experiment {experiment_id}")
 
     # There could be unprepared deployments and already finished executors:
     # 1.1. remove from deployment map all which executors already finished
     deployment_map = experiment.deployment_map
     finished_executors: Optional[list[Record]] = await db_connection_pool.fetch(
         "SELECT executor_id FROM executors WHERE experiment_id = $1 AND finished = TRUE",
         experiment_id,
@@ -337,55 +402,81 @@
     deployment_map = [
         deployment for deployment in deployment_map if deployment.prepared
     ]
 
     # 2. find all prepared deployments per each connector
     deployments: dict[str, list[Deployment]] = defaultdict(list)
     for deployment in deployment_map:
-        deployments[deployment.node["connector"]].append(deployment)
+        deployments[str(deployment.node["connector"])].append(deployment)
 
     # 3. check that all connectors are available
     for connector_name in deployments.keys():
         if connector_name not in connectors:
             return (
                 500,
                 f"Connector {connector_name} participating in the experiment {experiment_id} is not available, cannot proceed",
             )
 
     # 4. start background task to execute
     background_tasks.add_task(
-        background_execute_task, username, experiment_id, deployments
+        background_execute_task,
+        username,
+        experiment_id,
+        deployments,
+        execution_context,
+        netunicorn_authentication_context,
     )
     return 200, f"Execution of experiment {experiment_id} started"
 
 
 async def background_execute_task(
-    username: str, experiment_id: str, deployments: dict[str, list[Deployment]]
+    username: str,
+    experiment_id: str,
+    deployments: dict[str, list[Deployment]],
+    execution_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> None:
     # 5. execute on each connector
     for connector_name, connector_deployments in deployments.items():
         try:
+            connector_execution_context = None
+            if execution_context and connector_name in execution_context:
+                connector_execution_context = execution_context[connector_name]
+            connector_auth_context = None
+            if (
+                netunicorn_authentication_context
+                and connector_name in netunicorn_authentication_context
+            ):
+                connector_auth_context = netunicorn_authentication_context[
+                    connector_name
+                ]
             results = await connectors[connector_name].execute(
-                username, experiment_id, connector_deployments
+                username,
+                experiment_id,
+                connector_deployments,
+                connector_execution_context,
+                connector_auth_context,
             )
         except Exception as e:
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
             logger.warning(f"Connector {connector_name} moved to unavailable status.")
             connectors.pop(connector_name)
             failure_reason = f"Connector {connector_name} raised an exception and execution couldn't be completed"
             results = {
                 deployment.executor_id: Failure(failure_reason)
                 for deployment in connector_deployments
             }
 
         # each key in result is an executor id, value is Success or Failure with description
         # noinspection DuplicatedCode
         for executor_id, result in results.items():
             if isinstance(result, Success):
-                logger.debug(
+                logger.info(
                     f"Execution of executor {executor_id} on connector {connector_name} succeeded"
                 )
                 continue
 
             failure_reason = str(result.failure())
             logger.warning(
                 f"Execution of executor {executor_id} on connector {connector_name} failed: {failure_reason}"
@@ -393,26 +484,34 @@
             await db_connection_pool.execute(
                 "UPDATE executors SET finished = TRUE, error = $1 WHERE experiment_id = $2 AND executor_id = $3",
                 failure_reason,
                 experiment_id,
                 executor_id,
             )
 
-    logger.debug(f"Experiment {experiment_id} execution started")
+    logger.info(f"Experiment {experiment_id} execution started")
 
 
 async def stop_execution(
-    username: str, experiment_id: str, background_tasks: BackgroundTasks
+    username: str,
+    experiment_id: str,
+    background_tasks: BackgroundTasks,
+    cancellation_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> Tuple[int, str]:
     # TODO: implement
     return 500, "Not implemented"
 
 
 async def stop_executors(
-    username: str, executors: list[str], background_tasks: BackgroundTasks
+    username: str,
+    executors: list[str],
+    background_tasks: BackgroundTasks,
+    cancellation_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> Tuple[int, str]:
     # find all connectors to ask and give them information about executors to stop
     # 1. find all executors
     executors_data: Optional[list[Record]] = await db_connection_pool.fetch(
         "SELECT executor_id, node_name, connector FROM executors WHERE executor_id = ANY($1)",
         executors,
     )
@@ -431,40 +530,65 @@
         if connector_name not in connectors:
             logger.warning(
                 f"Connector {connector_name} participating in the executors {connector_executors} is not available, cannot proceed"
             )
             return 500, f"Connector {connector_name} is not available, cannot proceed"
 
     # 4. start background task to stop executors
-    background_tasks.add_task(background_stop_executors_task, username, executors_dict)
+    background_tasks.add_task(
+        background_stop_executors_task,
+        username,
+        executors_dict,
+        cancellation_context,
+        netunicorn_authentication_context,
+    )
     return 200, f"Stopping executors {executors_dict} started"
 
 
 async def background_stop_executors_task(
-    username: str, executors: dict[str, list[StopExecutorRequest]]
+    username: str,
+    executors: dict[str, list[StopExecutorRequest]],
+    cancellation_context: Optional[dict[str, dict[str, str]]] = None,
+    netunicorn_authentication_context: ConnectorContext = None,
 ) -> None:
     for connector_name, executors_list in executors.items():
         try:
+            connector_cancellation_context = None
+            if cancellation_context and connector_name in cancellation_context:
+                connector_cancellation_context = cancellation_context[connector_name]
+            connector_auth_context = None
+            if (
+                netunicorn_authentication_context
+                and connector_name in netunicorn_authentication_context
+            ):
+                connector_auth_context = netunicorn_authentication_context[
+                    connector_name
+                ]
             results = await connectors[connector_name].stop_executors(
-                username, executors_list
+                username,
+                executors_list,
+                connector_cancellation_context,
+                connector_auth_context,
             )
         except Exception as e:
-            logger.warning(f"Connector {connector_name} raised an exception: {e}")
+            logger.warning(
+                f"Connector {connector_name} raised an exception: {str(e.with_traceback(e.__traceback__))}"
+            )
             logger.warning(f"Connector {connector_name} moved to unavailable status.")
             connectors.pop(connector_name)
             failure_reason = f"Connector {connector_name} raised an exception and execution couldn't be completed"
             results = {
                 stop_executor_request["executor_id"]: Failure(failure_reason)
                 for stop_executor_request in executors_list
             }
 
         # each key in result is an executor id, value is Success or Failure with description
         for executor_id, result in results.items():
             if isinstance(result, Success):
-                logger.debug(
+                logger.info(
                     f"Stopping of executor {executor_id} on connector {connector_name} succeeded"
                 )
                 await db_connection_pool.execute(
                     "UPDATE executors SET finished = TRUE, error = $1 WHERE executor_id = $2",
                     "Executor was stopped",
                     executor_id,
                 )
```

### Comparing `netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/PKG-INFO` & `netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-director-infrastructure
-Version: 0.2.1
+Version: 0.3.0
 Summary: netunicorn infrastructure module
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-director-infrastructure-0.2.1/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt` & `netunicorn-director-infrastructure-0.3.0/src/netunicorn_director_infrastructure.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 src/netunicorn/director/infrastructure/__init__.py
 src/netunicorn/director/infrastructure/__main__.py
 src/netunicorn/director/infrastructure/kernel.py
 src/netunicorn/director/infrastructure/server.py
+src/netunicorn/director/infrastructure/tasks.py
 src/netunicorn/director/infrastructure/connectors/__init__.py
 src/netunicorn/director/infrastructure/connectors/dummy.py
-src/netunicorn/director/infrastructure/connectors/protocol.py
-src/netunicorn/director/infrastructure/connectors/types.py
 src/netunicorn/director/infrastructure/connectors/rest/__init__.py
 src/netunicorn/director/infrastructure/connectors/rest/simple_rest.py
 src/netunicorn/director/infrastructure/connectors/rest/simple_rest_server.py
 src/netunicorn_director_infrastructure.egg-info/PKG-INFO
 src/netunicorn_director_infrastructure.egg-info/SOURCES.txt
 src/netunicorn_director_infrastructure.egg-info/dependency_links.txt
 src/netunicorn_director_infrastructure.egg-info/requires.txt
```

