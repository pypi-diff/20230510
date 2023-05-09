# Comparing `tmp/onefuzztypes-8.0.0.tar.gz` & `tmp/onefuzztypes-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onefuzztypes-8.0.0.tar", last modified: Wed Apr 12 01:45:19 2023, max compression
+gzip compressed data, was "dist/onefuzztypes-8.1.0.tar", last modified: Mon May  8 15:53:18 2023, max compression
```

## Comparing `onefuzztypes-8.0.0.tar` & `onefuzztypes-8.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    11453 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     8236 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    25245 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/onefuzztypes/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/onefuzztypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:19.000000 onefuzztypes-8.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_alnum_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_container_def.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_instance_config_update.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2820 2023-04-12 01:45:17.000000 onefuzztypes-8.0.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/consts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11453 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8396 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25305 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5829 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_alnum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_container_def.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_instance_config_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2820 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_models.py
```

### Comparing `onefuzztypes-8.0.0/PKG-INFO` & `onefuzztypes-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.0.0
+Version: 8.1.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.0.0/README.md` & `onefuzztypes-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/_monkeypatch.py` & `onefuzztypes-8.1.0/onefuzztypes/_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/enums.py` & `onefuzztypes-8.1.0/onefuzztypes/enums.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/events.py` & `onefuzztypes-8.1.0/onefuzztypes/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Licensed under the MIT License.
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID, uuid4
 
-from pydantic import BaseModel, Field
+from pydantic import AnyHttpUrl, BaseModel, Field
 
 from ._monkeypatch import _check_hotfix
 from .enums import (
     OS,
     Architecture,
     NodeState,
     ScalesetState,
@@ -316,14 +316,22 @@
     event_id: UUID = Field(default_factory=uuid4)
     event_type: EventType
     event: Event
     instance_id: UUID
     instance_name: str
 
 
+class DownloadableEventMessage(EventMessage):
+    sas_url: AnyHttpUrl
+
+
+class EventGetResponse(BaseResponse):
+    event: DownloadableEventMessage
+
+
 # because Pydantic does not yet have discriminated union types yet, parse events
 # by hand.  https://github.com/samuelcolvin/pydantic/issues/619
 def parse_event_message(data: Dict[str, Any]) -> EventMessage:
     instance_id = UUID(data["instance_id"])
     instance_name = data["instance_name"]
     event_id = UUID(data["event_id"])
     event_type = EventType[data["event_type"]]
```

### Comparing `onefuzztypes-8.0.0/onefuzztypes/job_templates.py` & `onefuzztypes-8.1.0/onefuzztypes/job_templates.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/models.py` & `onefuzztypes-8.1.0/onefuzztypes/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,15 @@
     scariness_description: Optional[str]
     minimized_stack: Optional[List[str]]
     minimized_stack_sha256: Optional[str]
     minimized_stack_function_names: Optional[List[str]]
     minimized_stack_function_names_sha256: Optional[str]
     minimized_stack_function_lines: Optional[List[str]]
     minimized_stack_function_lines_sha256: Optional[str]
+    report_url: Optional[str]
 
 
 class NoReproReport(BaseModel):
     input_sha256: str
     input_blob: Optional[BlobRef]
     executable: str
     task_id: UUID
@@ -648,14 +649,15 @@
     nodes: Optional[List[Node]]
     config: Optional[AgentConfig]
 
     # work_queue is explicitly not saved to Tables (see save_exclude).  This is
     # intended to be used to pass the information to the CLI when the CLI asks
     # for information about what work is in the queue for the pool.
     work_queue: Optional[List[WorkSetSummary]]
+    object_id: Optional[UUID]
 
     # explicitly excluded from Tables
     scaleset_summary: Optional[List[ScalesetSummary]]
 
 
 class ScalesetNodeState(BaseModel):
     machine_id: UUID
```

### Comparing `onefuzztypes-8.0.0/onefuzztypes/primitives.py` & `onefuzztypes-8.1.0/onefuzztypes/primitives.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/requests.py` & `onefuzztypes-8.1.0/onefuzztypes/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Licensed under the MIT License.
 
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
 from pydantic import AnyHttpUrl, BaseModel, Field, root_validator
 
+from onefuzztypes import models
+
 from ._monkeypatch import _check_hotfix
 from .consts import ONE_HOUR, SEVEN_DAYS
 from .enums import (
     OS,
     Architecture,
     JobState,
     NodeState,
@@ -20,14 +22,15 @@
     TaskState,
 )
 from .events import EventType
 from .models import (
     AutoScaleConfig,
     InstanceConfig,
     NotificationConfig,
+    Report,
     TemplateRenderContext,
 )
 from .primitives import Container, PoolName, Region
 from .webhooks import WebhookMessageFormat
 
 
 class BaseRequest(BaseModel):
@@ -98,14 +101,19 @@
     os: OS
     arch: Architecture
     managed: bool
     object_id: Optional[UUID]
     autoscale: Optional[AutoScaleConfig]
 
 
+class PoolUpdate(BaseRequest):
+    name: PoolName
+    object_id: Optional[UUID]
+
+
 class PoolSearch(BaseRequest):
     pool_id: Optional[UUID]
     name: Optional[PoolName]
     state: Optional[List[PoolState]]
 
 
 class PoolStop(BaseRequest):
@@ -263,8 +271,17 @@
     context: Optional[TemplateRenderContext]
 
 
 class JinjaToScribanMigrationPost(BaseModel):
     dry_run: bool = Field(default=False)
 
 
+class EventsGet(BaseModel):
+    event_id: UUID
+
+
+class NotificationTest(BaseModel):
+    report: Report
+    notification: models.Notification
+
+
 _check_hotfix()
```

### Comparing `onefuzztypes-8.0.0/onefuzztypes/responses.py` & `onefuzztypes-8.1.0/onefuzztypes/responses.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,7 +95,12 @@
 class JinjaToScribanMigrationResponse(BaseResponse):
     updated_notification_ids: List[UUID]
     failed_notification_ids: List[UUID]
 
 
 class JinjaToScribanMigrationDryRunResponse(BaseResponse):
     notification_ids_to_update: List[UUID]
+
+
+class NotificationTestResponse(BaseResponse):
+    success: bool
+    error: Optional[str]
```

### Comparing `onefuzztypes-8.0.0/onefuzztypes/validators.py` & `onefuzztypes-8.1.0/onefuzztypes/validators.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes/webhooks.py` & `onefuzztypes-8.1.0/onefuzztypes/webhooks.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/onefuzztypes.egg-info/PKG-INFO` & `onefuzztypes-8.1.0/onefuzztypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.0.0
+Version: 8.1.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.0.0/onefuzztypes.egg-info/SOURCES.txt` & `onefuzztypes-8.1.0/onefuzztypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/setup.py` & `onefuzztypes-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/tests/test_alnum_filter.py` & `onefuzztypes-8.1.0/tests/test_alnum_filter.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/tests/test_container_def.py` & `onefuzztypes-8.1.0/tests/test_container_def.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/tests/test_instance_config_update.py` & `onefuzztypes-8.1.0/tests/test_instance_config_update.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.0.0/tests/test_models.py` & `onefuzztypes-8.1.0/tests/test_models.py`

 * *Files identical despite different names*

