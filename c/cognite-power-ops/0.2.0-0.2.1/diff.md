# Comparing `tmp/cognite_power_ops-0.2.0.tar.gz` & `tmp/cognite_power_ops-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.2.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.2.1.tar", max compression
```

## Comparing `cognite_power_ops-0.2.0.tar` & `cognite_power_ops-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0    10758 2023-05-09 07:14:44.989373 cognite_power_ops-0.2.0/LICENSE
--rw-r--r--   0        0        0       76 2023-05-09 07:14:44.989373 cognite_power_ops-0.2.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0    24685 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     2686 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0     1390 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16603 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0     5114 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0     1218 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0     2113 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     3165 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/cognite/powerops/version.py
--rw-r--r--   0        0        0     1330 2023-05-09 07:14:44.993373 cognite_power_ops-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-10 11:20:08.335871 cognite_power_ops-0.2.1/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0    24685 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     2686 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0     1390 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16603 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0     5114 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0     1218 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0     2113 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-10 11:20:08.339871 cognite_power_ops-0.2.1/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1330 2023-05-10 11:20:08.343871 cognite_power_ops-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.1/PKG-INFO
```

### Comparing `cognite_power_ops-0.2.0/LICENSE` & `cognite_power_ops-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.2.1/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/config.py` & `cognite_power_ops-0.2.1/cognite/powerops/config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.2.1/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/logger.py` & `cognite_power_ops-0.2.1/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/main.py` & `cognite_power_ops-0.2.1/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/common.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/files.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.2.1/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.0/pyproject.toml` & `cognite_power_ops-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.2.0"
+version = "0.2.1"
 description = "SDK for power markets operations on Cognite Data Fusion"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
 line-length = 120
```

### Comparing `cognite_power_ops-0.2.0/PKG-INFO` & `cognite_power_ops-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

