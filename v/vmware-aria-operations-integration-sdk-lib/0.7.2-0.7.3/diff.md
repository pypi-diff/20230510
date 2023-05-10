# Comparing `tmp/vmware-aria-operations-integration-sdk-lib-0.7.2.tar.gz` & `tmp/vmware-aria-operations-integration-sdk-lib-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.2.tar", last modified: Wed Apr 19 11:59:02 2023, max compression
+gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.3.tar", last modified: Wed May 10 14:54:52 2023, max compression
```

## Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2.tar` & `vmware-aria-operations-integration-sdk-lib-0.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.313619 vmware-aria-operations-integration-sdk-lib-0.7.2/
--rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/LICENSE
--rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/NOTICE
--rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-04-19 11:59:02.314088 vmware-aria-operations-integration-sdk-lib-0.7.2/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     2038 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/README.md
--rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-01-11 16:15:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/pyproject.toml
--rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-04-19 11:59:02.316345 vmware-aria-operations-integration-sdk-lib-0.7.2/setup.cfg
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:01.948565 vmware-aria-operations-integration-sdk-lib-0.7.2/src/
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:01.956125 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/__init__.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.163673 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/
--rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     3522 2023-02-01 19:20:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_instance.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2948 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_logging.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2910 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/data.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.269973 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    12336 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/adapter_definition.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/assertions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     7217 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/attribute.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     9414 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/credential_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/exceptions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    11446 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/group.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6393 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/object_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6437 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/parameter.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/units.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2449 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17112 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/object.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1183 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/pipe_utils.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    13941 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    13784 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/suite_api_client.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     4259 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/timer.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.291415 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/
--rw-r--r--   0 kylerokos   (501) staff       (20)     2859 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-04-19 11:59:01.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-04-19 11:59:02.312456 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/
--rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_collect_result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_object_key.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_result.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.175380 vmware-aria-operations-integration-sdk-lib-0.7.3/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/LICENSE
+-rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/NOTICE
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-05-10 14:54:52.175682 vmware-aria-operations-integration-sdk-lib-0.7.3/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2199 2023-04-20 17:56:10.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/README.md
+-rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-01-11 16:15:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/pyproject.toml
+-rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-05-10 14:54:52.177217 vmware-aria-operations-integration-sdk-lib-0.7.3/setup.cfg
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.098170 vmware-aria-operations-integration-sdk-lib-0.7.3/src/
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.103989 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/__init__.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.123404 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/
+-rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3522 2023-02-01 19:20:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_instance.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2948 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_logging.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2910 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/data.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.149748 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12374 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/adapter_definition.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/assertions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     7217 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/attribute.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     9884 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/credential_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/exceptions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    11446 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/group.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     6442 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/object_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     6916 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/parameter.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/units.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2449 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17112 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/object.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1183 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/pipe_utils.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    13941 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    13784 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/suite_api_client.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     4259 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/timer.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.158528 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.174455 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_collect_result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_object_key.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_result.py
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/LICENSE` & `vmware-aria-operations-integration-sdk-lib-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
+[![PyPI version](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib.svg)](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib)
+
 Overview
 --------
 The VMware Aria Operations Integration SDK Library is a Python package that streamlines creating adapters using the
 VMware Aria Operations Integration SDK.
 
 Installing
 ---------
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/README.md` & `vmware-aria-operations-integration-sdk-lib-0.7.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib.svg)](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib)
+
 Overview
 --------
 The VMware Aria Operations Integration SDK Library is a Python package that streamlines creating adapters using the
 VMware Aria Operations Integration SDK.
 
 Installing
 ---------
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/setup.cfg` & `vmware-aria-operations-integration-sdk-lib-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vmware-aria-operations-integration-sdk-lib
-version = 0.7.2
+version = 0.7.3
 author = VMware, Inc.
 author_email = krokos@vmware.com
 description = Object model for interacting with the VMware Aria Operations Containerized API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vmware/vmware-aria-operations-integration-sdk
 project_urls =
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_instance.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_instance.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/adapter_logging.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_logging.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/data.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/data.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/adapter_definition.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/adapter_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 VMware, Inc.
+#  Copyright 2022-2023 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import sys
 from collections import OrderedDict
 from typing import Optional
 
@@ -70,14 +70,15 @@
         super().__init__()
 
     def to_json(self) -> dict:
         return {
             "adapter_key": self.key,
             "adapter_label": self.label,
             "describe_version": self.version,
+            "schema_version": 1,
             "adapter_instance": {
                 "key": self.adapter_instance_key,
                 "label": self.adapter_instance_label,
                 "identifiers": [
                     identifier.to_json() for identifier in self.parameters.values()
                 ],
             }
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/assertions.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/assertions.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/attribute.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/attribute.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/credential_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/credential_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  Copyright 2022 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from abc import ABC
 from collections import OrderedDict
 from typing import Optional
+from typing import Union
 
 from aria.ops.definition.assertions import validate_key
 from aria.ops.definition.exceptions import DuplicateKeyException
 
 
 class CredentialParameter(ABC):
     def __init__(
@@ -118,32 +119,43 @@
     :param required: True if user is required to provide this parameter. Defaults to True.
     :param display_order: Determines the order parameters will be displayed in the UI.
     """
 
     def __init__(
         self,
         key: str,
-        values: list[str],
+        values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
         default: Optional[str] = None,
         required: bool = True,
         display_order: int = 0,
     ):
         super().__init__(key, label, required, display_order)
         self.values = values
         self.default = default
-        if default is not None and default not in values:
-            self.values.append(default)
+
+        if (
+            default not in [v[0] if isinstance(v, tuple) else v for v in self.values]
+            and default is not None
+        ):
+            self.values.append((default, default))
 
     def to_json(self) -> dict:
         return super().to_json() | {
             "type": "string",
             "default": self.default,
             "enum": True,
-            "enum_values": [str(value) for value in self.values],
+            "enum_values": [
+                {
+                    "key": str(value[0]) if isinstance(value, tuple) else value,
+                    "label": str(value[1]) if isinstance(value, tuple) else value,
+                    "display_order": display_order,
+                }
+                for display_order, value in enumerate(self.values)
+            ],
         }
 
 
 class CredentialType:
     def __init__(self, key: str, label: Optional[str] = None):
         self.key = validate_key(key, "Credential type")
         self.label = label
@@ -192,15 +204,15 @@
         field = CredentialPasswordParameter(key, label, required)
         self.add_parameter(field)
         return field
 
     def define_enum_parameter(
         self,
         key: str,
-        values: list[str],
+        values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
         default: Optional[str] = None,
         required: bool = True,
     ) -> CredentialEnumParameter:
         """
         Create a new enum credential parameter and apply it to this credential definition.
         :param key: Used to identify the parameter.
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/group.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/group.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/object_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/object_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  Copyright 2022 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from collections import OrderedDict
 from typing import Optional
+from typing import Union
 
 from aria.ops.definition.assertions import validate_key
 from aria.ops.definition.exceptions import DuplicateKeyException
 from aria.ops.definition.group import GroupType
 from aria.ops.definition.parameter import EnumParameter
 from aria.ops.definition.parameter import IntParameter
 from aria.ops.definition.parameter import Parameter
@@ -87,15 +88,15 @@
         )
         self.add_identifier(parameter)
         return self
 
     def define_enum_identifier(
         self,
         key: str,
-        values: list[str],
+        values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
         required: bool = True,
         is_part_of_uniqueness: bool = True,
         default: Optional[str] = None,
     ) -> ObjectType:
         """
         Create a new enum identifier and apply it to this object type definition.
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/parameter.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #  Copyright 2022 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from abc import ABC
 from typing import Optional
+from typing import Union
 
 from aria.ops.definition.assertions import validate_key
 from aria.ops.definition.exceptions import DuplicateKeyException
 
 
 class Parameter(ABC):
     def __init__(
         self,
         key: str,
         label: Optional[str] = None,
         description: Optional[str] = None,
-        default: Optional[str | int] = None,
+        default: Optional[Union[str, int]] = None,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
         """
         :param key: Used to identify the parameter.
         :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
@@ -117,15 +118,15 @@
         }
 
 
 class EnumParameter(Parameter):
     def __init__(
         self,
         key: str,
-        values: list[str],
+        values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
         description: Optional[str] = None,
         default: Optional[str] = None,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
@@ -143,18 +144,31 @@
         super().__init__(
             key, label, description, default, required, advanced, display_order
         )
         if len(values) > len(set(values)):
             raise DuplicateKeyException(
                 f"Duplicate enum value in parameter {key}: {values}."
             )
+
         self.values = values
-        if default not in self.values and default is not None:
-            self.values.append(default)
+        self.default = default
+
+        if (
+            default not in [v[0] if isinstance(v, tuple) else v for v in self.values]
+            and default is not None
+        ):
+            self.values.append((default, default))
 
     def to_json(self) -> dict:
         return super().to_json() | {
             "type": "string",
             "enum": True,
-            "enum_values": [str(value) for value in self.values],
+            "enum_values": [
+                {
+                    "key": str(value[0]) if isinstance(value, tuple) else value,
+                    "label": str(value[1]) if isinstance(value, tuple) else value,
+                    "display_order": display_order,
+                }
+                for display_order, value in enumerate(self.values)
+            ],
             "default": self.default,
         }
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/definition/units.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/units.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/event.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/event.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/object.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/object.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/pipe_utils.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/pipe_utils.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/result.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/suite_api_client.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/suite_api_client.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/aria/ops/timer.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/timer.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.2
+Version: 0.7.3
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
+[![PyPI version](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib.svg)](https://badge.fury.io/py/vmware-aria-operations-integration-sdk-lib)
+
 Overview
 --------
 The VMware Aria Operations Integration SDK Library is a Python package that streamlines creating adapters using the
 VMware Aria Operations Integration SDK.
 
 Installing
 ---------
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt` & `vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_collect_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_collect_result.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_object_key.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_object_key.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.2/tests/test_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_result.py`

 * *Files identical despite different names*

