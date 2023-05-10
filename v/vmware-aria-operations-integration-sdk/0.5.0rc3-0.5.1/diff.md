# Comparing `tmp/vmware_aria_operations_integration_sdk-0.5.0rc3.tar.gz` & `tmp/vmware_aria_operations_integration_sdk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware_aria_operations_integration_sdk-0.5.0rc3.tar", max compression
+gzip compressed data, was "vmware_aria_operations_integration_sdk-0.5.1.tar", max compression
```

## Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3.tar` & `vmware_aria_operations_integration_sdk-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10449 2022-10-27 15:46:24.345895 vmware_aria_operations_integration_sdk-0.5.0rc3/LICENSE
--rw-r--r--   0        0        0    14832 2023-04-14 19:48:56.128849 vmware_aria_operations_integration_sdk-0.5.0rc3/README.md
--rw-r--r--   0        0        0     1992 2023-04-14 20:07:29.284449 vmware_aria_operations_integration_sdk-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0       70 2022-11-22 16:59:16.872140 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/__init__.py
--rw-r--r--   0        0        0     4039 2023-02-24 14:06:04.218957 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_container.py
--rw-r--r--   0        0        0       70 2022-11-30 20:30:20.187730 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/__init__.py
--rw-r--r--   0        0        0    10899 2023-01-27 15:59:03.422897 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/adapter.py
--rw-r--r--   0        0        0    38857 2023-01-11 16:15:44.602229 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd
--rw-r--r--   0        0        0   115627 2022-11-22 16:59:16.875203 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd
--rw-r--r--   0        0        0      877 2022-11-30 20:30:20.188151 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/java.py
--rw-r--r--   0        0        0      504 2023-02-02 21:38:57.354182 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/powershell.py
--rw-r--r--   0        0        0    12694 2022-11-22 16:59:16.876825 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd
--rw-r--r--   0        0        0       70 2022-11-22 16:59:16.877055 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/__init__.py
--rw-r--r--   0        0        0     8537 2022-11-22 16:59:16.877842 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json
--rw-r--r--   0        0        0    22318 2023-03-31 18:20:30.853497 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json
--rw-r--r--   0        0        0    17880 2023-03-28 19:28:30.435791 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/collection_statistics.py
--rw-r--r--   0        0        0     2864 2023-01-11 16:15:44.604632 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/config.py
--rw-r--r--   0        0        0     1298 2023-04-14 19:48:56.132533 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/constant.py
--rw-r--r--   0        0        0      501 2023-03-31 18:48:42.334870 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/container_versions.json
--rw-r--r--   0        0        0     6522 2023-03-31 18:20:30.854391 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py
--rw-r--r--   0        0        0    18841 2023-03-30 20:55:20.203300 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/describe.py
--rw-r--r--   0        0        0    14164 2023-03-30 20:55:20.204815 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/docker_wrapper.py
--rw-r--r--   0        0        0     2018 2023-03-31 18:20:30.857197 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/filesystem.py
--rw-r--r--   0        0        0     1737 2023-01-11 16:15:44.610687 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/logging_format.py
--rw-r--r--   0        0        0     2194 2023-01-11 16:15:44.611683 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/model.py
--rw-r--r--   0        0        0    22850 2023-04-14 19:48:56.134212 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_build.py
--rw-r--r--   0        0        0    19790 2023-04-14 19:48:56.135094 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_init.py
--rw-r--r--   0        0        0    33436 2023-03-31 18:20:30.859579 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_test.py
--rw-r--r--   0        0        0     6888 2023-03-31 18:20:30.860710 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/project.py
--rw-r--r--   0        0        0      852 2023-04-07 21:23:08.899171 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/propertiesfile.py
--rw-r--r--   0        0        0    13100 2023-03-31 18:20:30.861565 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/serialization.py
--rw-r--r--   0        0        0     2822 2023-01-11 16:15:44.620174 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/stats.py
--rw-r--r--   0        0        0      634 2023-01-11 16:15:44.621124 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/threading.py
--rw-r--r--   0        0        0     1590 2023-01-11 16:15:44.622057 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/timer.py
--rw-r--r--   0        0        0    17620 2023-02-24 14:06:04.222246 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/ui.py
--rw-r--r--   0        0        0      762 2023-01-11 16:15:44.624427 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/util.py
--rw-r--r--   0        0        0       70 2022-11-30 20:30:20.193055 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/__init__.py
--rw-r--r--   0        0        0     2262 2023-03-31 18:20:30.862856 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py
--rw-r--r--   0        0        0     3136 2023-03-31 18:20:30.863841 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/api_response_validation.py
--rw-r--r--   0        0        0    11224 2023-03-31 18:20:30.864980 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/describe_checks.py
--rw-r--r--   0        0        0     1961 2023-03-31 18:20:30.865956 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py
--rw-r--r--   0        0        0     6874 2023-03-31 18:20:30.866991 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/highlights.py
--rw-r--r--   0        0        0     6923 2023-03-31 18:20:30.867726 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/input_validators.py
--rw-r--r--   0        0        0     5191 2023-03-31 18:20:30.868584 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/relationship_validator.py
--rw-r--r--   0        0        0     1311 2023-03-31 18:20:30.869895 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/result.py
--rw-r--r--   0        0        0    16957 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc3/setup.py
--rw-r--r--   0        0        0    16331 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    10449 2022-10-27 15:46:24.345895 vmware_aria_operations_integration_sdk-0.5.1/LICENSE
+-rw-r--r--   0        0        0    10449 2023-05-01 16:50:55.899383 vmware_aria_operations_integration_sdk-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0    76402 2023-05-10 18:37:00.224072 vmware_aria_operations_integration_sdk-0.5.1/README.md
+-rw-r--r--   0        0        0     1989 2023-05-10 18:37:00.229520 vmware_aria_operations_integration_sdk-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-11-22 16:59:16.872140 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/__init__.py
+-rw-r--r--   0        0        0     4039 2023-02-24 14:06:04.218957 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_container.py
+-rw-r--r--   0        0        0       70 2022-11-30 20:30:20.187730 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/__init__.py
+-rw-r--r--   0        0        0    11527 2023-05-10 18:37:00.231033 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/adapter.py
+-rw-r--r--   0        0        0    38857 2023-01-11 16:15:44.602229 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd
+-rw-r--r--   0        0        0   115627 2022-11-22 16:59:16.875203 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd
+-rw-r--r--   0        0        0      877 2022-11-30 20:30:20.188151 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/java.py
+-rw-r--r--   0        0        0      504 2023-02-02 21:38:57.354182 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/powershell.py
+-rw-r--r--   0        0        0    12694 2022-11-22 16:59:16.876825 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd
+-rw-r--r--   0        0        0       70 2022-11-22 16:59:16.877055 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/api/__init__.py
+-rw-r--r--   0        0        0     9427 2023-05-09 21:05:24.499736 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json
+-rw-r--r--   0        0        0    22318 2023-03-31 18:20:30.853497 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json
+-rw-r--r--   0        0        0    17880 2023-03-28 19:28:30.435791 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/collection_statistics.py
+-rw-r--r--   0        0        0     2864 2023-01-11 16:15:44.604632 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/config.py
+-rw-r--r--   0        0        0     1298 2023-04-14 19:48:56.132533 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/constant.py
+-rw-r--r--   0        0        0      501 2023-05-09 21:05:24.502784 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/container_versions.json
+-rw-r--r--   0        0        0     6522 2023-03-31 18:20:30.854391 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py
+-rw-r--r--   0        0        0    19917 2023-05-09 21:05:24.507803 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/describe.py
+-rw-r--r--   0        0        0    14252 2023-05-10 18:37:00.233032 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/docker_wrapper.py
+-rw-r--r--   0        0        0     2018 2023-03-31 18:20:30.857197 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/filesystem.py
+-rw-r--r--   0        0        0     1737 2023-01-11 16:15:44.610687 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/logging_format.py
+-rw-r--r--   0        0        0     2194 2023-01-11 16:15:44.611683 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/model.py
+-rw-r--r--   0        0        0    22850 2023-04-14 19:48:56.134212 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_build.py
+-rw-r--r--   0        0        0    20020 2023-05-10 18:37:00.233985 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_init.py
+-rw-r--r--   0        0        0    33436 2023-03-31 18:20:30.859579 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_test.py
+-rw-r--r--   0        0        0     6888 2023-03-31 18:20:30.860710 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/project.py
+-rw-r--r--   0        0        0      852 2023-04-07 21:23:08.899171 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/propertiesfile.py
+-rw-r--r--   0        0        0    13100 2023-03-31 18:20:30.861565 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/serialization.py
+-rw-r--r--   0        0        0     2822 2023-01-11 16:15:44.620174 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/stats.py
+-rw-r--r--   0        0        0      634 2023-01-11 16:15:44.621124 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/threading.py
+-rw-r--r--   0        0        0     1590 2023-01-11 16:15:44.622057 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/timer.py
+-rw-r--r--   0        0        0    17620 2023-02-24 14:06:04.222246 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/ui.py
+-rw-r--r--   0        0        0      762 2023-01-11 16:15:44.624427 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/util.py
+-rw-r--r--   0        0        0       70 2022-11-30 20:30:20.193055 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/__init__.py
+-rw-r--r--   0        0        0     2262 2023-03-31 18:20:30.862856 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py
+-rw-r--r--   0        0        0     3136 2023-03-31 18:20:30.863841 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/api_response_validation.py
+-rw-r--r--   0        0        0    11224 2023-03-31 18:20:30.864980 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/describe_checks.py
+-rw-r--r--   0        0        0     1961 2023-03-31 18:20:30.865956 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py
+-rw-r--r--   0        0        0     6874 2023-03-31 18:20:30.866991 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/highlights.py
+-rw-r--r--   0        0        0     6923 2023-05-10 18:36:53.458479 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/input_validators.py
+-rw-r--r--   0        0        0     5191 2023-03-31 18:20:30.868584 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/relationship_validator.py
+-rw-r--r--   0        0        0     1311 2023-03-31 18:20:30.869895 vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/result.py
+-rw-r--r--   0        0        0    77898 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.1/PKG-INFO
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/LICENSE` & `vmware_aria_operations_integration_sdk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/pyproject.toml` & `vmware_aria_operations_integration_sdk-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "lib/python/tests"]
 
 [tool.poetry]
 name = "vmware_aria_operations_integration_sdk"
-version = "0.5.0rc3"
+version = "0.5.1"
 description = "A set of tools to help users create, test, and build containerized management packs for VMware Aria Operations"
 authors = ["Kyle Rokos <krokos@vmware.com>", "Santiago Quiroga Cubillos <squirogacubi@vmware.com>"]
 license = "APACHE-2.0"
 readme = "README.md"
 packages = [{include = "vmware_aria_operations_integration_sdk"}]
 include = [
     "vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd",
@@ -27,16 +27,16 @@
 python = "^3.9"
 GitPython = "3.1.30"
 aenum = "3.1.11"
 openapi-schema-validator = "0.2.3"
 openapi-spec-validator = "0.4.0"
 lxml = "4.9.2"
 prompt-toolkit = "3.0.29"
-vmware-aria-operations-integration-sdk-lib = "^0.7.1"
-docker = "6.0.0"
+vmware-aria-operations-integration-sdk-lib = "^0.7.3"
+docker = "6.1.1"
 httpx = "0.23.0"
 xmlschema = "^2.1.1"
 pillow = "^9.3.0"
 importlib-resources = "^5.10.0"
 openapi-core = "0.15.0"
 importlib-metadata = "^5.0.0"
 sen = "^0.6.2"
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_container.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_container.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/adapter.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,221 +9,220 @@
 from aria.ops.data import Metric
 from aria.ops.data import Property
 from aria.ops.definition.adapter_definition import AdapterDefinition
 from aria.ops.definition.units import Units
 from aria.ops.result import CollectResult
 from aria.ops.result import EndpointResult
 from aria.ops.result import TestResult
+from aria.ops.timer import Timer
 from constants import ADAPTER_KIND
 from constants import ADAPTER_NAME
 
 logger = logging.getLogger(__name__)
 
 
-def test(adapter_instance: AdapterInstance) -> TestResult:
-    logger.info("Starting 'Test'")
-    result = TestResult()
-    try:
-        # Sample test connection code follows. Replace with your own test connection code.
-        # A typical test connection will generally consist of:
-        # 1. Read identifier values from adapter_instance that are required to
-        #    connect to the target(s)
-        # 2. Connect to the target(s), and retrieve some sample data
-        # 3. Disconnect cleanly from the target (ensure this happens even if an error occurs)
-        # 4. If any of the above failed, return an error, otherwise pass.
-
-        # Read the 'ID' identifier in the adapter instance and use it for a
-        # connection test.
-        id = adapter_instance.get_identifier_value("ID")
-
-        # In this case the adapter does not need to connect
-        # to anything, as it reads directly from the host it is running on.
-        if id is None:
-            result.with_error("No ID Found")
-        elif id.lower() == "bad":
-            # As there is not an actual failure condition to test for, this
-            # example only shows the mechanics of reading identifiers and
-            # constructing test results. Here we add an error to the result
-            # that is returned.
-            result.with_error("The ID is bad")
-        # otherwise, the test has passed
-        logger.info(f"Finished 'Test'")
-        logger.debug(f"Returning test result: {result.get_json()}")
-        return result
-
-    except Exception as e:
-        # TODO: If any connections are still open, make sure they are closed before returning
-        logger.error("Unexpected connection test error")
-        logger.exception(e)
-        result.with_error("Unexpected connection test error: " + repr(e))
-        return result
-
+def get_adapter_definition() -> AdapterDefinition:
+    """
+    The adapter definition defines the object types and attribute types (metric/property) that are present
+    in a collection. Setting these object types and attribute types helps VMware Aria Operations to
+    validate, process, and display the data correctly.
+    :return: AdapterDefinition
+    """
+    with Timer(logger, "Get Adapter Definition"):
+        definition = AdapterDefinition(ADAPTER_KIND, ADAPTER_NAME)
 
-def get_endpoints(adapter_instance: AdapterInstance) -> EndpointResult:
-    logger.info("Starting 'Get Endpoints'")
-    result = EndpointResult()
-    # In the case that an SSL Certificate is needed to communicate to the target,
-    # add each URL that the adapter uses here. Often this will be derived from a 'host'
-    # parameter in the adapter instance. In this Adapter we don't use any HTTPS
-    # connections, so we won't add any. If we did, we might do something like this:
-    # result.with_endpoint(adapter_instance.get_identifier_value("host"))
-    #
-    # Multiple endpoints can be returned, like this:
-    # result.with_endpoint(adapter_instance.get_identifier_value("primary_host"))
-    # result.with_endpoint(adapter_instance.get_identifier_value("secondary_host"))
-    #
-    # This 'get_endpoints' method will be run before the 'test' method,
-    # and VMware Aria Operations will use the results to extract a certificate from
-    # each URL. If the certificate is not trusted by the VMware Aria Operations Trust
-    # Store, the user will be prompted to either accept or reject the certificate. If
-    # it is accepted, the certificate will be added to the AdapterInstance object that
-    # is passed to the 'test' and 'collect' methods. Any certificate that is
-    # encountered in those methods should then be validated against the certificate(s)
-    # in the AdapterInstance.
-    logger.info(f"Finished 'Get Endpoints'")
-    logger.debug(f"Returning endpoints: {result.get_json()}")
-    return result
+        definition.define_string_parameter(
+            "ID",
+            label="ID",
+            description="Example identifier. Using a value of 'bad' will cause "
+            "test connection to fail; any other value will pass.",
+            required=True,
+        )
+        # The key 'container_memory_limit' is a special key that is read by the VMware Aria Operations collector to
+        # determine how much memory to allocate to the docker container running this adapter. It does not
+        # need to be read inside the adapter code.
+        definition.define_int_parameter(
+            "container_memory_limit",
+            label="Adapter Memory Limit (MB)",
+            description="Sets the maximum amount of memory VMware Aria Operations can "
+            "allocate to the container running this adapter instance.",
+            required=True,
+            advanced=True,
+            default=1024,
+        )
+
+        cpu = definition.define_object_type("cpu", "CPU")
+        cpu.define_numeric_property("cpu_count", "CPU Count", is_discrete=True)
+        cpu.define_metric("user_time", "User Time", Units.TIME.SECONDS)
+        cpu.define_metric(
+            "nice_time", "Nice Time", Units.TIME.SECONDS, is_key_attribute=True
+        )
+        cpu.define_metric("system_time", "System Time", Units.TIME.SECONDS)
+        cpu.define_metric("idle_time", "Idle Time", Units.TIME.SECONDS)
+
+        disk = definition.define_object_type("disk", "Disk")
+        disk.define_string_property("partition", "Partition")
+        disk.define_metric(
+            "total_space", "Total Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
+        )
+        disk.define_metric(
+            "used_space", "Used Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
+        )
+        disk.define_metric(
+            "free_space", "Free Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
+        )
+        disk.define_metric(
+            "percent_used_space",
+            "Disk Utilization",
+            unit=Units.RATIO.PERCENT,
+            is_key_attribute=True,
+        )
 
+        system = definition.define_object_type("system", "System")
 
-def collect(adapter_instance: AdapterInstance) -> CollectResult:
-    result = CollectResult()
-    try:
-        logger.info("Starting 'Collection'")
-        # Sample collection code follows. Replace this with your own collection code.
-        # A typical collection will generally consist of:
-        # 1. Read identifier values from adapter_instance that are required to
-        #    connect to the target(s)
-        # 2. Connect to the target(s), and retrieve data
-        # 3. Add the data into a CollectResult's objects, properties, metrics, etc
-        # 4. Disconnect cleanly from the target (ensure this happens even if an error occurs)
-        # 5. Return the CollectResult.
-
-        # CPU
-        cpu = result.object(ADAPTER_KIND, "CPU", "CPU")
-        # properties
-        cpu_count_property = Property("cpu_count", psutil.cpu_count())
-        cpu.add_property(cpu_count_property)
-
-        # metrics
-        cpu_percent = Metric("cpu_percent", psutil.cpu_percent(1))
-        user, nice, system, idle, *_ = psutil.cpu_times()
-
-        user_time = Metric("user_time", user)
-        nice_time = Metric("nice_time", nice)
-        system_time = Metric("system_time", system)
-        idle_time = Metric("idle_time", idle)
-
-        # adding metrics to CPU
-        cpu.add_metric(user_time)
-        cpu.add_metric(nice_time)
-        cpu.add_metric(system_time)
-        cpu.add_metric(idle_time)
-
-        # Disk
-        disk = result.object(ADAPTER_KIND, "Disk", "Disk")
-        # gathering properties
-        partition, mount_point, *_ = psutil.disk_partitions().pop()
-        partition_property = Property("partition", partition)
-
-        # adding properties
-        disk.add_property(partition_property)
-
-        # gathering metrics
-        total, used, free, percent = psutil.disk_usage(mount_point)
-
-        total_space = Metric("total_space", total)
-        used_space = Metric("used_space", used)
-        free_space = Metric("free_space", free)
-        percent_used_space = Metric("percent_used_space", percent)
-
-        # adding metrics to Disk
-        disk.add_metric(total_space)
-        disk.add_metric(used_space)
-        disk.add_metric(free_space)
-        disk.add_metric(percent_used_space)
+        logger.debug(f"Returning adapter definition: {definition.to_json()}")
+        return definition
 
-        # Add system object to demonstrate relationships
-        system = result.object(ADAPTER_KIND, "System", "System")
 
-        system.add_child(disk)
-        system.add_child(cpu)
+def test(adapter_instance: AdapterInstance) -> TestResult:
+    with Timer(logger, "Test"):
+        result = TestResult()
+        try:
+            # Sample test connection code follows. Replace with your own test connection
+            # code. A typical test connection will generally consist of:
+            # 1. Read identifier values from adapter_instance that are required to
+            #    connect to the target(s)
+            # 2. Connect to the target(s), and retrieve some sample data
+            # 3. Disconnect cleanly from the target (ensure this happens even if an
+            #    error occurs)
+            # 4. If any of the above failed, return an error, otherwise pass.
+
+            # Read the 'ID' identifier in the adapter instance and use it for a
+            # connection test.
+            id = adapter_instance.get_identifier_value("ID")
+
+            # In this case the adapter does not need to connect
+            # to anything, as it reads directly from the host it is running on.
+            if id is None:
+                result.with_error("No ID Found")
+            elif id.lower() == "bad":
+                # As there is not an actual failure condition to test for, this
+                # example only shows the mechanics of reading identifiers and
+                # constructing test results. Here we add an error to the result
+                # that is returned.
+                result.with_error("The ID is bad")
+            # otherwise, the test has passed
+        except Exception as e:
+            # TODO: If any connections are still open, make sure they are closed before
+            #  returning
+            logger.error("Unexpected connection test error")
+            logger.exception(e)
+            result.with_error("Unexpected connection test error: " + repr(e))
+        finally:
+            logger.debug(f"Returning test result: {result.get_json()}")
+            return result
 
-        logger.info(f"Finished 'Collection'")
-        logger.debug(f"Returning collection result {result.get_json()}")
-        return result
-    except Exception as e:
-        # TODO: If any connections are still open, make sure they are closed before returning
-        logger.error("Unexpected collection error")
-        logger.exception(e)
-        result.with_error("Unexpected collection error: " + repr(e))
-        return result
 
+def collect(adapter_instance: AdapterInstance) -> CollectResult:
+    with Timer(logger, "Collection"):
+        result = CollectResult()
+        try:
+            # Sample collection code follows. Replace this with your own collection
+            # code. A typical collection will generally consist of:
+            # 1. Read identifier values from adapter_instance that are required to
+            #    connect to the target(s)
+            # 2. Connect to the target(s), and retrieve data
+            # 3. Add the data into a CollectResult's objects, properties, metrics, etc
+            # 4. Disconnect cleanly from the target (ensure this happens even if an
+            #    error occurs)
+            # 5. Return the CollectResult.
+
+            # CPU
+            cpu = result.object(ADAPTER_KIND, "cpu", "CPU")
+            # properties
+            cpu_count_property = Property("cpu_count", psutil.cpu_count())
+            cpu.add_property(cpu_count_property)
+
+            # metrics
+            cpu_percent = Metric("cpu_percent", psutil.cpu_percent(1))
+            user, nice, system, idle, *_ = psutil.cpu_times()
+
+            user_time = Metric("user_time", user)
+            nice_time = Metric("nice_time", nice)
+            system_time = Metric("system_time", system)
+            idle_time = Metric("idle_time", idle)
+
+            # adding metrics to CPU
+            cpu.add_metric(user_time)
+            cpu.add_metric(nice_time)
+            cpu.add_metric(system_time)
+            cpu.add_metric(idle_time)
+
+            # Disk
+            disk = result.object(ADAPTER_KIND, "disk", "Disk")
+            # gathering properties
+            partition, mount_point, *_ = psutil.disk_partitions().pop()
+            partition_property = Property("partition", partition)
+
+            # adding properties
+            disk.add_property(partition_property)
+
+            # gathering metrics
+            total, used, free, percent = psutil.disk_usage(mount_point)
+
+            total_space = Metric("total_space", total)
+            used_space = Metric("used_space", used)
+            free_space = Metric("free_space", free)
+            percent_used_space = Metric("percent_used_space", percent)
+
+            # adding metrics to Disk
+            disk.add_metric(total_space)
+            disk.add_metric(used_space)
+            disk.add_metric(free_space)
+            disk.add_metric(percent_used_space)
+
+            # Add system object to demonstrate relationships
+            system = result.object(ADAPTER_KIND, "system", "System")
+
+            system.add_child(disk)
+            system.add_child(cpu)
+        except Exception as e:
+            # TODO: If any connections are still open, make sure they are closed before returning
+            logger.error("Unexpected collection error")
+            logger.exception(e)
+            result.with_error("Unexpected collection error: " + repr(e))
+        finally:
+            logger.debug(f"Returning collection result {result.get_json()}")
+            return result
 
-def get_adapter_definition() -> AdapterDefinition:
-    logger.info("Starting 'Get Adapter Definition'")
-    """
-    The adapter definition defines the object types and attribute types (metric/property) that are present
-    in a collection. Setting these object types and attribute types helps VMware Aria Operations to
-    validate, process, and display the data correctly.
-    :return: AdapterDefinition
-    """
-    definition = AdapterDefinition(ADAPTER_KIND, ADAPTER_NAME)
 
-    definition.define_string_parameter(
-        "ID",
-        label="ID",
-        description="Example identifier. Using a value of 'bad' will cause "
-        "test connection to fail; any other value will pass.",
-        required=True,
-    )
-    # The key 'container_memory_limit' is a special key that is read by the VMware Aria Operations collector to
-    # determine how much memory to allocate to the docker container running this adapter. It does not
-    # need to be read inside the adapter code.
-    definition.define_int_parameter(
-        "container_memory_limit",
-        label="Adapter Memory Limit (MB)",
-        description="Sets the maximum amount of memory VMware Aria Operations can "
-        "allocate to the container running this adapter instance.",
-        required=True,
-        advanced=True,
-        default=1024,
-    )
-
-    cpu = definition.define_object_type("cpu", "CPU")
-    cpu.define_numeric_property("cpu_count", "CPU Count", is_discrete=True)
-    cpu.define_metric("user_time", "User Time", Units.TIME.SECONDS)
-    cpu.define_metric(
-        "nice_time", "Nice Time", Units.TIME.SECONDS, is_key_attribute=True
-    )
-    cpu.define_metric("system_time", "System Time", Units.TIME.SECONDS)
-    cpu.define_metric("idle_time", "Idle Time", Units.TIME.SECONDS)
-
-    disk = definition.define_object_type("disk", "Disk")
-    disk.define_string_property("partition", "Partition")
-    disk.define_metric(
-        "total_space", "Total Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
-    )
-    disk.define_metric(
-        "used_space", "Used Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
-    )
-    disk.define_metric(
-        "free_space", "Free Space", is_discrete=True, unit=Units.DATA_SIZE.BIBYTE
-    )
-    disk.define_metric(
-        "percent_used_space",
-        "Disk Utilization",
-        unit=Units.RATIO.PERCENT,
-        is_key_attribute=True,
-    )
-
-    system = definition.define_object_type("system", "System")
-
-    logger.info("Finished 'Get Adapter Definition'")
-    logger.debug(f"Returning adapter definition: {definition.to_json()}")
-    return definition
+def get_endpoints(adapter_instance: AdapterInstance) -> EndpointResult:
+    with Timer(logger, "Get Endpoints"):
+        result = EndpointResult()
+        # In the case that an SSL Certificate is needed to communicate to the target,
+        # add each URL that the adapter uses here. Often this will be derived from a
+        # 'host' parameter in the adapter instance. In this Adapter we don't use any
+        # HTTPS connections, so we won't add any. If we did, we might do something like
+        # this:
+        # result.with_endpoint(adapter_instance.get_identifier_value("host"))
+        #
+        # Multiple endpoints can be returned, like this:
+        # result.with_endpoint(adapter_instance.get_identifier_value("primary_host"))
+        # result.with_endpoint(adapter_instance.get_identifier_value("secondary_host"))
+        #
+        # This 'get_endpoints' method will be run before the 'test' method,
+        # and VMware Aria Operations will use the results to extract a certificate from
+        # each URL. If the certificate is not trusted by the VMware Aria Operations
+        # Trust Store, the user will be prompted to either accept or reject the
+        # certificate. If it is accepted, the certificate will be added to the
+        # AdapterInstance object that is passed to the 'test' and 'collect' methods.
+        # Any certificate that is encountered in those methods should then be validated
+        # against the certificate(s) in the AdapterInstance.
+        logger.debug(f"Returning endpoints: {result.get_json()}")
+        return result
 
 
 # Main entry point of the adapter. You should not need to modify anything below this line.
 def main(argv: List[str]) -> None:
     logging.setup_logging("adapter.log")
     # Start a new log file by calling 'rotate'. By default, the last five calls will be
     # retained. If the logs are not manually rotated, the 'setup_logging' call should be
@@ -234,30 +233,32 @@
     if len(argv) != 3:
         # `inputfile` and `outputfile` are always automatically appended to the
         # argument list by the server
         logger.error("Arguments must be <method> <inputfile> <ouputfile>")
         exit(1)
 
     method = argv[0]
-
-    if method == "test":
-        test(AdapterInstance.from_input()).send_results()
-    elif method == "endpoint_urls":
-        get_endpoints(AdapterInstance.from_input()).send_results()
-    elif method == "collect":
-        collect(AdapterInstance.from_input()).send_results()
-    elif method == "adapter_definition":
-        result = get_adapter_definition()
-        if type(result) is AdapterDefinition:
-            result.send_results()
+    try:
+        if method == "test":
+            test(AdapterInstance.from_input()).send_results()
+        elif method == "endpoint_urls":
+            get_endpoints(AdapterInstance.from_input()).send_results()
+        elif method == "collect":
+            collect(AdapterInstance.from_input()).send_results()
+        elif method == "adapter_definition":
+            result = get_adapter_definition()
+            if type(result) is AdapterDefinition:
+                result.send_results()
+            else:
+                logger.info(
+                    "get_adapter_definition method did not return an AdapterDefinition"
+                )
+                exit(1)
         else:
-            logger.info(
-                "get_adapter_definition method did not return an AdapterDefinition"
-            )
+            logger.error(f"Command {method} not found")
             exit(1)
-    else:
-        logger.error(f"Command {method} not found")
-        exit(1)
+    finally:
+        logger.info(Timer.graph())
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/java.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/java.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999368873780903%*

 * *Differences: {"'components'": "{'schemas': {'CredentialDefinition': {'properties': {'fields': {'items': "*

 * *                 "{'properties': {'enum_values': {'items': {'type': 'object', 'properties': "*

 * *                 "OrderedDict([('key', OrderedDict([('type', 'string')])), ('label', "*

 * *                 "OrderedDict([('type', 'string')])), ('display_order', OrderedDict([('type', "*

 * *                 "'integer'), ('format', 'int32'), ('minimum', 0)]))])}}}}}}}, "*

 * *                 "'IdentifierDefinition': {'properties': {'en […]*

```diff
@@ -24,14 +24,18 @@
                         "type": "integer"
                     },
                     "object_types": {
                         "items": {
                             "$ref": "#/components/schemas/ObjectDefinition"
                         },
                         "type": "array"
+                    },
+                    "schema_version": {
+                        "format": "int32",
+                        "type": "integer"
                     }
                 },
                 "required": [
                     "adapter_key",
                     "adapter_label",
                     "describe_version",
                     "adapter_instance",
@@ -116,15 +120,28 @@
                                 },
                                 "enum": {
                                     "default": false,
                                     "type": "boolean"
                                 },
                                 "enum_values": {
                                     "items": {
-                                        "type": "string"
+                                        "properties": {
+                                            "display_order": {
+                                                "format": "int32",
+                                                "minimum": 0,
+                                                "type": "integer"
+                                            },
+                                            "key": {
+                                                "type": "string"
+                                            },
+                                            "label": {
+                                                "type": "string"
+                                            }
+                                        },
+                                        "type": "object"
                                     },
                                     "type": "array"
                                 },
                                 "key": {
                                     "type": "string"
                                 },
                                 "label": {
@@ -201,15 +218,28 @@
                     },
                     "enum": {
                         "default": false,
                         "type": "boolean"
                     },
                     "enum_values": {
                         "items": {
-                            "type": "string"
+                            "properties": {
+                                "display_order": {
+                                    "format": "int32",
+                                    "minimum": 0,
+                                    "type": "integer"
+                                },
+                                "key": {
+                                    "type": "string"
+                                },
+                                "label": {
+                                    "type": "string"
+                                }
+                            },
+                            "type": "object"
                         },
                         "type": "array"
                     },
                     "ident_type": {
                         "default": 1,
                         "format": "int32",
                         "type": "integer"
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/collection_statistics.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/collection_statistics.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/config.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/config.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/constant.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/constant.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/describe.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/describe.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,43 +234,46 @@
     # The only valid lexical values for boolean are ["true", "false", "1", "0"] (case-sensitive)
     # https://www.w3.org/TR/xmlschema-2/#boolean
     return element.get(attr, default) in ["true", "1"]
 
 
 def json_to_xml(json: Dict) -> Element:
     names = _Names()
+    schema_version = int(json.get("schema_version", 0))
+
     describe = Element(
         "{http://schemas.vmware.com/vcops/schema}AdapterKind",
         attrib={
             "key": json["adapter_key"],
             "nameKey": names.get_key(json["adapter_label"]),
             "version": str(json["describe_version"]),
         },
         nsmap=ns_map,
     )
 
     # CredentialKinds
     credential_kinds = SubElement(describe, "CredentialKinds", nsmap=ns_map)
     for credential_kind in json["credential_types"]:
-        add_credential_kind(credential_kinds, credential_kind, names)
+        add_credential_kind(credential_kinds, credential_kind, names, schema_version)
 
     # ResourceKinds
     resource_kinds = SubElement(describe, "ResourceKinds", nsmap=ns_map)
     credential_types: Iterable[str] = map(
         lambda cred_type: str(cred_type["key"]), json["credential_types"]
     )
     add_resource_kind(
         resource_kinds,
         json["adapter_instance"],
         names,
+        schema_version,
         type=7,
         credential_kinds=credential_types,
     )
     for object_type in json["object_types"]:
-        add_resource_kind(resource_kinds, object_type, names)
+        add_resource_kind(resource_kinds, object_type, names, schema_version)
 
     # CustomGroupMetrics
     # CapacityDefinitions
     # Faults
     # LaunchConfigurations
     # add_launch_configurations(describe, names)
     # BasePolicyAnalysisSettings
@@ -286,15 +289,18 @@
 def write_describe(describe: Element, filename: str) -> None:
     root = ET.ElementTree(describe)
     ET.indent(root)
     root.write(filename, encoding="utf-8", xml_declaration=True)
 
 
 def add_credential_kind(
-    parent: Element, credential_kind_json: Dict, names: _Names
+    parent: Element,
+    credential_kind_json: Dict,
+    names: _Names,
+    schema_version: int,
 ) -> Element:
     xml = SubElement(
         parent,
         "CredentialKind",
         attrib={
             "key": credential_kind_json["key"],
             "nameKey": names.get_key(credential_kind_json["label"]),
@@ -312,22 +318,23 @@
                 "dispOrder": str(field["display_order"]),
                 "password": str(field["password"]).lower(),
                 "enum": str(field["enum"]).lower(),
                 "type": str(field["type"]),
             },
             nsmap=ns_map,
         )
-        add_enum_values(field_xml, field)
+        add_enum_values(field_xml, field, names, schema_version)
     return xml
 
 
 def add_resource_kind(
     parent: Element,
     resource_kind_json: Dict,
     names: _Names,
+    schema_version: int,
     type: int = 1,
     credential_kinds: Optional[Iterable[str]] = None,
 ) -> Element:
     attributes = {
         "key": resource_kind_json["key"],
         "nameKey": names.get_key(resource_kind_json["label"]),
         "type": str(type),
@@ -335,23 +342,28 @@
     if credential_kinds:
         attributes["credentialKind"] = ",".join(credential_kinds)
 
     resourcekind_xml = SubElement(
         parent, "ResourceKind", attrib=attributes, nsmap=ns_map
     )
     for identifier in resource_kind_json["identifiers"]:
-        add_identifier(resourcekind_xml, identifier, names)
+        add_identifier(resourcekind_xml, identifier, names, schema_version)
     for attribute in resource_kind_json["attributes"]:
         add_attribute(resourcekind_xml, attribute, names)
     for group in resource_kind_json["groups"]:
         add_group(resourcekind_xml, group, names)
     return resourcekind_xml
 
 
-def add_identifier(parent: Element, identifier_json: Dict, names: _Names) -> Element:
+def add_identifier(
+    parent: Element,
+    identifier_json: Dict,
+    names: _Names,
+    schema_version: int,
+) -> Element:
     default = identifier_json.get("default")
     if default is None:
         default = ""
     identifier_xml = SubElement(
         parent,
         "ResourceIdentifier",
         attrib={
@@ -364,32 +376,56 @@
             "dispOrder": str(identifier_json["display_order"]),
             "enum": str(identifier_json["enum"]).lower(),
             "type": str(identifier_json["type"]),
             "identType": str(identifier_json["ident_type"]),
         },
         nsmap=ns_map,
     )
-    add_enum_values(identifier_xml, identifier_json)
+    add_enum_values(identifier_xml, identifier_json, names, schema_version)
     return identifier_xml
 
 
-def add_enum_values(parent: Element, identifier_json: Dict) -> None:
+def add_enum_values(
+    parent: Element, identifier_json: Dict, names: _Names, schema_version: int
+) -> None:
     if "enum_values" in identifier_json:
-        for value in identifier_json["enum_values"]:
-            SubElement(
-                parent,
-                "enum",
-                attrib={
-                    "value": str(value),
-                    "default": str(
-                        value == identifier_json.get("default", False)
-                    ).lower(),
-                },
-                nsmap=ns_map,
-            )
+        if schema_version >= 1:
+            _add_enum_values_v1(parent, identifier_json, names)
+        else:
+            _add_enum_values_v0(parent, identifier_json, names)
+
+
+def _add_enum_values_v0(parent: Element, identifier_json: Dict, names: _Names) -> None:
+    for value in identifier_json["enum_values"]:
+        SubElement(
+            parent,
+            "enum",
+            attrib={
+                "value": str(value),
+                "default": str(value == identifier_json.get("default", False)).lower(),
+            },
+            nsmap=ns_map,
+        )
+
+
+def _add_enum_values_v1(parent: Element, identifier_json: Dict, names: _Names) -> None:
+    enum_values: list[dict[str, int]] = sorted(
+        identifier_json["enum_values"], key=lambda value: value["display_order"]
+    )
+    for value in enum_values:
+        SubElement(
+            parent,
+            "enum",
+            attrib={
+                "value": str(value["key"]),
+                "nameKey": names.get_key(str(value["label"])),
+                "default": str(value == identifier_json.get("default", False)).lower(),
+            },
+            nsmap=ns_map,
+        )
 
 
 def add_attribute(parent: Element, attribute_json: Dict, names: _Names) -> Element:
     attribute_xml = SubElement(
         parent,
         "ResourceAttribute",
         attrib={
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/docker_wrapper.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/docker_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,24 @@
     """
     try:
         client = docker.from_env()
 
         return client
     except docker.errors.DockerException as e:
         if "ConnectionRefusedError" or "FileNotFoundError" or "CreateFile" in e.args[0]:
+            logger.debug(e, exc_info=True)
             raise InitError(
                 message="Cannot connect to the Docker daemon",
                 recommendation="Ensure the docker daemon is running",
             )
         elif "PermissionError" in e.args[0]:
+            logger.debug(e, exc_info=True)
             raise InitError(
                 message="Cannot run docker commands.",
-                recommendation=f"Make sure the user {os.getlogin()} has permissions to run docker",
+                recommendation=f"Make sure the user '{os.getlogin()}' has permissions to run docker",
             )
         else:
             raise InitError(e)
 
 
 def push_image(client: DockerClient, image_tag: str) -> str:
     """
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/filesystem.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/filesystem.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/logging_format.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/logging_format.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/model.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/model.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_build.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_build.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_init.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,19 @@
 ) -> None:
     mkdir(path)
 
     project = Project(path)
 
     build_content_directory(path)
     conf_dir = mkdir(path, "conf")
-    conf_resources_dir = mkdir(path, "conf", "resources")
+    conf_resources_dir = mkdir(conf_dir, "resources")
+    conf_images_dir = mkdir(conf_dir, "images")
+    add_git_keep_file(mkdir(conf_images_dir, "AdapterKind"))
+    add_git_keep_file(mkdir(conf_images_dir, "ResourceKind"))
+    add_git_keep_file(mkdir(conf_images_dir, "TraversalSpec"))
 
     create_manifest_localization_file(path, name, vendor, description)
     eula_file = create_eula_file(path, eula_file)
     icon_file = create_icon_file(path, icon_file)
     manifest = create_manifest_file(path, adapter_key, eula_file, icon_file)
 
     # This has to happen after the manifest.txt file is created, because this function only records a project if
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_test.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/mp_test.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/project.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/project.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/propertiesfile.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/propertiesfile.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/serialization.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/serialization.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/stats.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/stats.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/threading.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/threading.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/timer.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/ui.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/ui.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/util.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/util.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/api_response_validation.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/api_response_validation.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/describe_checks.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/describe_checks.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/highlights.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/highlights.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/input_validators.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/input_validators.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/relationship_validator.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/relationship_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/result.py` & `vmware_aria_operations_integration_sdk-0.5.1/vmware_aria_operations_integration_sdk/validation/result.py`

 * *Files identical despite different names*

