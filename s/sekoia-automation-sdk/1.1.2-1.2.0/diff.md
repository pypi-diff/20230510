# Comparing `tmp/sekoia_automation_sdk-1.1.2.tar.gz` & `tmp/sekoia_automation_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.1.2.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.2.0.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.1.2.tar` & `sekoia_automation_sdk-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/LICENSE
--rw-r--r--   0        0        0     8422 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/README.md
--rw-r--r--   0        0        0     2114 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11220 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/action.py
--rw-r--r--   0        0        0     3795 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/config.py
--rw-r--r--   0        0        0     6534 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/connector.py
--rw-r--r--   0        0        0      426 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-04-24 10:18:32.617846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15477 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      647 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10005 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/openapi.py
--rw-r--r--   0        0        0     4626 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/storage.py
--rw-r--r--   0        0        0    10724 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-04-24 10:18:32.621846 sekoia_automation_sdk-1.1.2/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-10 09:31:43.661486 sekoia_automation_sdk-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8422 2023-05-10 09:31:43.661486 sekoia_automation_sdk-1.2.0/README.md
+-rw-r--r--   0        0        0     2114 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11220 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/action.py
+-rw-r--r--   0        0        0     3825 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6958 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      647 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10005 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/openapi.py
+-rw-r--r--   0        0        0     4626 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    12410 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-05-10 09:31:43.665486 sekoia_automation_sdk-1.2.0/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.2.0/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.1.2/LICENSE` & `sekoia_automation_sdk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/README.md` & `sekoia_automation_sdk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/pyproject.toml` & `sekoia_automation_sdk-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.1.2"
+version = "1.2.0"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/action.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from sekoia_automation.scripts.files_generator import FilesGenerator
 from sekoia_automation.scripts.openapi import OpenApiToModule
 
 app = typer.Typer(
     help="SEKOIA.IO's automation helper to generate playbook modules",
     rich_markup_mode="markdown",
 )
-OptionalPath = Optional[Path]
-OptionalStr = Optional[str]
+OptionalPath = Optional[Path]  # noqa: UP007
+OptionalStr = Optional[str]  # noqa: UP007
 
 
 @app.command(name="generate-files-from-code")
 def generate_files(
     module: Path = typer.Argument(
         Path("."),
         exists=True,
```

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/config.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/connector.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/connector/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 class Connector(Trigger):
     configuration: DefaultConnectorConfiguration
 
     seconds_without_events = 3600
 
     def __init__(self, *args, **kwargs):
+        executor_max_worker = kwargs.pop("executor_max_worker", 4)
         super().__init__(*args, **kwargs)
-        self._executor = ThreadPoolExecutor(kwargs.pop("executor_max_worker", 4))
+        self._executor = ThreadPoolExecutor(executor_max_worker)
 
     def stop(self, *args, **kwargs):
         """
         Stop the connector
         """
         super().stop(*args, **kwargs)
         self._executor.shutdown(wait=True)
@@ -75,37 +76,45 @@
             if res.status_code > 299:
                 self.log(f"Intake rejected events: {res.text}", level="error")
                 res.raise_for_status()
             collect_ids[chunk_index] = res.json().get("event_ids", [])
         except Exception as ex:
             self.log_exception(ex, message=f"Failed to forward {len(chunk)} events")
 
-    def push_events_to_intakes(self, events: list[str]) -> list:
+    def push_events_to_intakes(self, events: list[str], sync: bool = False) -> list:
         # no event to push
         if not events:
             return []
 
+        # Reset the consecutive error count
+        self._error_count = 0
         self._last_events_time = datetime.utcnow()
         intake_host = self.configuration.intake_server
         batch_api = urljoin(intake_host, "/batch")
 
         # Dict to collect event_ids for the API
         collect_ids: dict[int, list] = {}
 
         # pushing the events
-        if self._stop_event.is_set():
-            return []
         chunks = self._chunk_events(events, self.configuration.chunk_size)
-        futures = [
-            self._executor.submit(
-                self._send_chunk, batch_api, chunk_index, chunk, collect_ids
-            )
-            for chunk_index, chunk in enumerate(chunks)
-        ]
-        wait_futures(futures)
+
+        # if requested, or if the executor is down
+        if sync or not self.running:
+            # forward in sequence
+            for chunk_index, chunk in enumerate(chunks):
+                self._send_chunk(batch_api, chunk_index, chunk, collect_ids)
+        else:
+            # Parallelize the forwarding
+            futures = [
+                self._executor.submit(
+                    self._send_chunk, batch_api, chunk_index, chunk, collect_ids
+                )
+                for chunk_index, chunk in enumerate(chunks)
+            ]
+            wait_futures(futures)
 
         # reorder event_ids according chunk index
         event_ids = [
             event_id
             for chunk_index in sorted(collect_ids.keys())
             for event_id in collect_ids[chunk_index]
         ]
```

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/module.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -305,26 +305,20 @@
         if not self.name:
             self.name = self.__class__.__name__.lower()
         self._data_path = data_path
 
         self._setup_logging()
 
     def _setup_logging(self):
-        self._logger = logging.getLogger(__name__)
-
-        handler = logging.StreamHandler()
-        handler.setLevel(logging.INFO)
-
-        formatter = logging.Formatter(
-            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        logging.basicConfig(
+            format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+            datefmt="%Y-%m-%d %H:%M:%S",
+            level=logging.INFO,
         )
-        handler.setFormatter(formatter)
-
-        self._logger.addHandler(handler)
-
+        self._logger = logging.getLogger(self.name)
         sentry_sdk.set_tag("name", self.name)
 
     @property
     def token(self) -> str:
         if self._token is None:
             self._token = self.module.load_config(self.TOKEN_FILE_NAME)
 
@@ -384,15 +378,22 @@
                 verb, self.callback_url, json=data, headers=self._headers, timeout=30
             )
             response.raise_for_status()
             return response
         except HTTPError as exception:
             self._log_request_error(exception)
             if attempt == 3:
-                raise SendEventError("Impossible to send event to SEKOIA.IO API")
+                status_code = (
+                    exception.response.status_code
+                    if isinstance(exception.response, Response)
+                    else 500
+                )
+                raise SendEventError(
+                    "Impossible to send event to SEKOIA.IO API", status_code=status_code
+                )
             if (
                 isinstance(exception.response, Response)
                 and 400 <= exception.response.status_code < 500
             ):
                 raise SendEventError(
                     "Impossible to send event to SEKOIA.IO API",
                     status_code=exception.response.status_code,
```

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/trigger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
-import logging
 import signal
 from abc import abstractmethod
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from functools import cached_property
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import Path
 from threading import Event, Thread
 from typing import Any
 
 import requests
 import sentry_sdk
+from botocore.exceptions import ClientError, ConnectionError, HTTPClientError
 from pydantic import BaseModel
 from requests import HTTPError
 from tenacity import retry, stop_after_attempt, wait_exponential
 
 from sekoia_automation.exceptions import (
     InvalidDirectoryError,
     ModuleConfigurationError,
+    SendEventError,
     TriggerConfigurationError,
 )
 from sekoia_automation.module import Module, ModuleItem
 from sekoia_automation.utils import (
     capture_retry_error,
     get_annotation_for,
     get_as_model,
@@ -39,15 +40,14 @@
     # the trigger is considered in error.
     # 0 means that the trigger is never considered in error
     seconds_without_events = 0
     LIVENESS_PORT_FILE_NAME = "liveness_port"
 
     def __init__(self, module: Module | None = None, data_path: Path | None = None):
         super().__init__(module, data_path)
-        logging.basicConfig(level=logging.INFO)
         self._configuration: dict | BaseModel | None = None
         self._error_count = 0
         self._last_events_time = datetime.utcnow()
         sentry_sdk.set_tag("item_type", "trigger")
         self._secrets: dict[str, Any] = {}
         self._stop_event = Event()
 
@@ -119,33 +119,30 @@
     def _execute_once(self) -> None:
         try:
             self.run()
         # Configuration errors are considered to be critical
         except (TriggerConfigurationError, ModuleConfigurationError) as e:
             self.log_exception(e)
             self.log(str(e), "critical")
-        except Exception as e:
-            self.log_exception(e)
-            # Increase the consecutive error count
-            self._error_count += 1
-
-            # If there was more than 5 errors without any event being sent,
-            # consider the error to be critical
-            level = "error"
-            if self._error_count >= 5:
-                level = "critical"
-
-            # Make sure the error is recorded and available to the user
-            self.log(str(e), level=level)
+        except (ConnectionError, HTTPClientError) as ex:
+            # Error while communicating with the S3 storage
+            # Don't increment the error count because this is an internal issue
+            self.log_exception(ex)
+        except ClientError as ex:
+            self._handle_s3_exception(ex)
+        except SendEventError as ex:
+            self._handle_send_event_exception(ex)
+        except Exception as ex:
+            self._handle_trigger_exception(ex)
 
     def execute(self) -> None:
         self._ensure_data_path_set()
         # Always restart the trigger, except if the error seems to be unrecoverable
         self._secrets = self._get_secrets_from_server()
-        while self._error_count < 5:
+        while self._error_count < 5 and not self._stop_event.is_set():
             self._execute_once()
 
     def _rm_tree(self, path: Path):
         """Delete a directory and its children.
 
         :param Path path: The directory to delete
         """
@@ -266,14 +263,15 @@
         LivenessHandler.trigger = self
         self._liveness_server = HTTPServer(("", int(port)), LivenessHandler)
         Thread(target=self._liveness_server.serve_forever, daemon=True).start()
 
     def stop_monitoring(self):
         if self._liveness_server:
             self._liveness_server.shutdown()
+            self._liveness_server = None
 
     def is_alive(self) -> bool:
         """
         Return whether the trigger appears to be alive.
 
         This is based on the date of the last sent events
         compared to the `seconds_without_events` threshold.
@@ -297,14 +295,60 @@
         """
         return {
             "last_events_time": self._last_events_time.isoformat(),
             "seconds_without_events_threshold": self.seconds_without_events,
             "error_count": self._error_count,
         }
 
+    def _handle_trigger_exception(self, e: Exception):
+        self.log_exception(e)
+        # Increase the consecutive error count
+        self._error_count += 1
+
+        # If there was more than 5 errors without any event being sent,
+        # consider the error to be critical
+        level = "error"
+        if self._error_count >= 5:
+            level = "critical"
+
+        # Make sure the error is recorded and available to the user
+        self.log(str(e), level=level)
+
+    def _handle_s3_exception(self, ex: ClientError):
+        """
+        Handle errors coming from the S3 storage
+        """
+        error_code = ex.response.get("Error", {}).get("Code", 500)
+        try:
+            status_code = int(error_code)
+        except ValueError:
+            if error_code in [
+                "InternalError",
+                "ServiceUnavailable",
+                "SlowDown",
+                "503 SlowDown",
+                "InsufficientCapacity",
+            ]:
+                status_code = 500
+            else:
+                status_code = 400
+        if status_code < 500:
+            # Let the exception follow the "normal flow"
+            return self._handle_trigger_exception(ex)
+
+        # We don't increment the error count because this is an internal issue
+        self.log_exception(ex)
+
+    def _handle_send_event_exception(self, ex: SendEventError):
+        if ex.status_code >= 500:
+            # We don't increment the error count because this is an internal issue
+            self.log_exception(ex)
+            return
+        return self._handle_trigger_exception(ex)
+
 
 class LivenessHandler(BaseHTTPRequestHandler):
     trigger: Trigger
 
     def do_GET(self):  # noqa: N802
         if self.path == "/health":
             self.send(
```

### Comparing `sekoia_automation_sdk-1.1.2/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.2.0/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.1.2/PKG-INFO` & `sekoia_automation_sdk-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.1.2
+Version: 1.2.0
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

