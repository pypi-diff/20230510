# Comparing `tmp/gridworks-0.2.2.tar.gz` & `tmp/gridworks-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.2.tar", max compression
+gzip compressed data, was "gridworks-0.2.3.tar", max compression
```

## Comparing `gridworks-0.2.2.tar` & `gridworks-0.2.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     1065 2023-05-09 19:35:56.464290 gridworks-0.2.2/LICENSE
--rw-r--r--   0        0        0     5778 2023-05-09 19:36:13.624409 gridworks-0.2.2/README.md
--rw-r--r--   0        0        0     2358 2023-05-09 19:36:13.624409 gridworks-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      208 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/__main__.py
--rw-r--r--   0        0        0    47777 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6761 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6440 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0      723 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1254 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2246 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     1331 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/errors.py
--rw-r--r--   0        0        0     4187 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/utils.py
--rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 gridworks-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-10 13:23:45.941739 gridworks-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5778 2023-05-10 13:23:45.941739 gridworks-0.2.3/README.md
+-rw-r--r--   0        0        0     2358 2023-05-10 13:24:02.522652 gridworks-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    47777 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6761 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6440 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5013 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      723 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1254 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-05-10 13:24:02.522652 gridworks-0.2.3/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/errors.py
+-rw-r--r--   0        0        0     4187 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-05-10 13:23:46.021743 gridworks-0.2.3/src/gridworks/utils.py
+-rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 gridworks-0.2.3/PKG-INFO
```

### Comparing `gridworks-0.2.2/LICENSE` & `gridworks-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/README.md` & `gridworks-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/pyproject.toml` & `gridworks-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.2"
+version = "0.2.3"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
```

### Comparing `gridworks-0.2.2/src/gridworks/actor_base.py` & `gridworks-0.2.3/src/gridworks/actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/algo_utils.py` & `gridworks-0.2.3/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/api_utils.py` & `gridworks-0.2.3/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/base_api_types.py` & `gridworks-0.2.3/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.3/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.3/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.3/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.3/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.3/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.3/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.3/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/__init__.py` & `gridworks-0.2.3/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.3/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.3/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.3/src/gridworks/enums/g_node_role.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     """
     Categorizes GNodes by their function within GridWorks. [More Info](https://gridworks.readthedocs.io/en/latest/g-node-role.html).
 
     Choices and descriptions:
 
       * GNode: Default value
       * TerminalAsset: An avatar for a real-word Transactive Device. [More Info](https://gridworks.readthedocs.io/en/latest/transactive-device.html).
-      * AtomicTNode: Transacts in markets on behalf of, and controlling the power use of, a TerminalAsset
-      * MarketMaker: Runs energy markets at its Node in the GNodeTree
+      * AtomicTNode: Transacts in markets on behalf of, and controlling the power use of, a TerminalAsset. [More Info](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html).
+      * MarketMaker: Runs energy markets at its Node in the GNodeTree. [More Info](https://gridworks.readthedocs.io/en/latest/market-maker.html).
       * AtomicMeteringNode: Role of a GNode that will become an AtomicTNode, prior to it owning TaTradingRights
       * ConductorTopologyNode: An avatar for a real-world electric grid node - e.g. a substation or transformer
       * InterconnectionComponent: An avatar for a cable or wire on the electric grid
-      * World: Adminstrative GNode responsible for managing and authorizing instances
+      * World: Adminstrative GNode responsible for managing and authorizing instances. [More Info](https://gridworks.readthedocs.io/en/latest/world-role.html).
       * TimeCoordinator: Responsible for managing time in simulations
-      * Supervisor: Responsible for GNode actors running in a container
+      * Supervisor: Responsible for GNode actors running in a container. [More Info](https://gridworks.readthedocs.io/en/latest/supervisor.html).
       * Scada: GNode associated to the device and code that directly monitors and actuates a Transactive Device
       * PriceService: Provides price forecasts for markets run by MarketMakers
       * WeatherService: Provides weather forecasts
       * AggregatedTNode: An aggregation of AtomicTNodes
       * Persister: Responsible for acking events with delivery guarantees
     """
```

### Comparing `gridworks-0.2.2/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.3/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/gni_status.py` & `gridworks-0.2.3/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.3/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.3/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.3/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/message_category.py` & `gridworks-0.2.3/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.3/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.3/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.3/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/enums/universe_type.py` & `gridworks-0.2.3/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/gw_config.py` & `gridworks-0.2.3/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/message.py` & `gridworks-0.2.3/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/property_format.py` & `gridworks-0.2.3/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/rest_api.py` & `gridworks-0.2.3/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/__init__.py` & `gridworks-0.2.3/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.3/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.3/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.3/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.3/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.3/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.3/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/ready.py` & `gridworks-0.2.3/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.3/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/super_starter.py` & `gridworks-0.2.3/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.3/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/src/gridworks/utils.py` & `gridworks-0.2.3/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.2/PKG-INFO` & `gridworks-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.2
+Version: 0.2.3
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

