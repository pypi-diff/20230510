# Comparing `tmp/volttron_platform_driver-0.2.0rc2.tar.gz` & `tmp/volttron_platform_driver-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_platform_driver-0.2.0rc2.tar", max compression
+gzip compressed data, was "volttron_platform_driver-0.2.0rc3.tar", max compression
```

## Comparing `volttron_platform_driver-0.2.0rc2.tar` & `volttron_platform_driver-0.2.0rc3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10255 2023-05-10 16:34:31.661540 volttron_platform_driver-0.2.0rc2/LICENSE
--rw-r--r--   0        0        0     2777 2023-05-10 16:34:31.661540 volttron_platform_driver-0.2.0rc2/README.md
--rw-r--r--   0        0        0     2111 2023-05-10 16:35:33.458756 volttron_platform_driver-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 16:34:31.665540 volttron_platform_driver-0.2.0rc2/src/platform_driver/__init__.py
--rw-r--r--   0        0        0    34550 2023-05-10 16:34:31.665540 volttron_platform_driver-0.2.0rc2/src/platform_driver/agent.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-05-10 16:36:29.562663 volttron_platform_driver-0.2.0rc3/LICENSE
+-rw-r--r--   0        0        0     2777 2023-05-10 16:36:29.562663 volttron_platform_driver-0.2.0rc3/README.md
+-rw-r--r--   0        0        0     2111 2023-05-10 16:37:33.011334 volttron_platform_driver-0.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 16:36:29.562663 volttron_platform_driver-0.2.0rc3/src/platform_driver/__init__.py
+-rw-r--r--   0        0        0    34550 2023-05-10 16:36:29.562663 volttron_platform_driver-0.2.0rc3/src/platform_driver/agent.py
+-rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 volttron_platform_driver-0.2.0rc3/PKG-INFO
```

### Comparing `volttron_platform_driver-0.2.0rc2/LICENSE` & `volttron_platform_driver-0.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc2/README.md` & `volttron_platform_driver-0.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc2/pyproject.toml` & `volttron_platform_driver-0.2.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-platform-driver"
-version = "0.2.0rc2"
+version = "0.2.0rc3"
 description = "The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/platform-driver-agent"
 homepage = "https://github.com/eclipse-volttron/platform-driver-agent"
 keywords = []
```

### Comparing `volttron_platform_driver-0.2.0rc2/src/platform_driver/agent.py` & `volttron_platform_driver-0.2.0rc3/src/platform_driver/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_platform_driver-0.2.0rc2/PKG-INFO` & `volttron_platform_driver-0.2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-platform-driver
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: The Platform Driver agent is a special purpose agent that manages communication between the Volttron platform and devices. The Platform driver features a number of endpoints for collecting data and sending control signals using the message bus and automatically publishes data to the bus on a specified interval.
 Home-page: https://github.com/eclipse-volttron/platform-driver-agent
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

