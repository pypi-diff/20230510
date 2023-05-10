# Comparing `tmp/gridworks-0.2.3.tar.gz` & `tmp/gridworks-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.3.tar", max compression
+gzip compressed data, was "gridworks-0.2.4.tar", max compression
```

## Comparing `gridworks-0.2.3.tar` & `gridworks-0.2.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1065 2023-05-10 13:23:45.941739 gridworks-0.2.3/LICENSE
--rw-r--r--   0        0        0     5778 2023-05-10 13:23:45.941739 gridworks-0.2.3/README.md
--rw-r--r--   0        0        0     2358 2023-05-10 13:24:02.522652 gridworks-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      208 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/__main__.py
--rw-r--r--   0        0        0    47777 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6761 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6440 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0     5013 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/data_classes/g_node_strategy.py
--rw-r--r--   0        0        0      723 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1254 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2547 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     2734 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/errors.py
--rw-r--r--   0        0        0     4187 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/utils.py
--rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 gridworks-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-10 13:57:51.523962 gridworks-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5778 2023-05-10 13:57:51.523962 gridworks-0.2.4/README.md
+-rw-r--r--   0        0        0     2358 2023-05-10 13:58:08.060213 gridworks-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    47777 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-05-10 13:57:51.587962 gridworks-0.2.4/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6726 2023-05-10 13:58:08.060213 gridworks-0.2.4/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6405 2023-05-10 13:58:08.060213 gridworks-0.2.4/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5011 2023-05-10 13:58:08.060213 gridworks-0.2.4/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      694 2023-05-10 13:58:08.060213 gridworks-0.2.4/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1214 2023-05-10 13:58:08.060213 gridworks-0.2.4/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/errors.py
+-rw-r--r--   0        0        0     4187 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-05-10 13:57:51.591963 gridworks-0.2.4/src/gridworks/utils.py
+-rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 gridworks-0.2.4/PKG-INFO
```

### Comparing `gridworks-0.2.3/LICENSE` & `gridworks-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/README.md` & `gridworks-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/pyproject.toml` & `gridworks-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.3"
+version = "0.2.4"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
```

### Comparing `gridworks-0.2.3/src/gridworks/actor_base.py` & `gridworks-0.2.4/src/gridworks/actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/algo_utils.py` & `gridworks-0.2.4/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/api_utils.py` & `gridworks-0.2.4/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/base_api_types.py` & `gridworks-0.2.4/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.4/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.4/src/gridworks/data_classes/g_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-""" GNode DataClass Definition """
 import logging
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gridworks.data_classes.gps_point import GpsPoint
 from gridworks.enums import GNodeRole
```

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.4/src/gridworks/data_classes/g_node_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-""" GNode DataClass Definition """
 import logging
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from gridworks.data_classes.g_node import GNode
 from gridworks.data_classes.gps_point import GpsPoint
```

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/g_node_strategy.py` & `gridworks-0.2.4/src/gridworks/data_classes/g_node_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from gridworks.enums import GNodeRole
 from gridworks.enums import StrategyName
 
 
 class GNodeStrategy:
     by_id: Dict[StrategyName, "GNodeStrategy"] = {}
 
-    def __new__(cls, name: MarketTypeName, *args, **kwargs) -> "GNodeStrategy":  # type: ignore
+    def __new__(cls, name: StrategyName, *args, **kwargs) -> "GNodeStrategy":  # type: ignore
         try:
             return cls.by_id[name]
         except KeyError:
             instance = super().__new__(cls)
             cls.by_id[name] = instance
             return instance
```

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.4/src/gridworks/data_classes/gps_point.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" GpsPoint Definition """
-
 from typing import Dict
 
 
 class GpsPoint:
     by_id: Dict[str, "GpsPoint"] = {}
 
     def __new__(cls, gps_point_id: str, *args, **kwargs):  # type: ignore
```

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.4/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.4/src/gridworks/data_classes/supervisor_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-""" SupervisorContainer  Definition """
 import logging
 from typing import Dict
 
 from gridworks.enums import SupervisorContainerStatus
 
 
 LOG_FORMAT = (
```

### Comparing `gridworks-0.2.3/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.4/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/__init__.py` & `gridworks-0.2.4/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.4/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.4/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.4/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.4/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/gni_status.py` & `gridworks-0.2.4/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.4/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.4/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.4/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/message_category.py` & `gridworks-0.2.4/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.4/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.4/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.4/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.4/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/enums/universe_type.py` & `gridworks-0.2.4/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/gw_config.py` & `gridworks-0.2.4/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/message.py` & `gridworks-0.2.4/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/property_format.py` & `gridworks-0.2.4/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/rest_api.py` & `gridworks-0.2.4/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/__init__.py` & `gridworks-0.2.4/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.4/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.4/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.4/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.4/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.4/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.4/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/ready.py` & `gridworks-0.2.4/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.4/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/super_starter.py` & `gridworks-0.2.4/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.4/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/src/gridworks/utils.py` & `gridworks-0.2.4/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.3/PKG-INFO` & `gridworks-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.3
+Version: 0.2.4
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

