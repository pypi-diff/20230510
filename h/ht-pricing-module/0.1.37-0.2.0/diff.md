# Comparing `tmp/ht_pricing_module-0.1.37.tar.gz` & `tmp/ht_pricing_module-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.1.37.tar", last modified: Fri Apr 21 01:21:28 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.2.0.tar", last modified: Tue May  9 09:24:24 2023, max compression
```

## Comparing `ht_pricing_module-0.1.37.tar` & `ht_pricing_module-0.2.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.086066 ht_pricing_module-0.1.37/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.1.37/MANIFEST.in
--rw-rw-rw-   0        0        0      264 2023-04-21 01:21:28.086066 ht_pricing_module-0.1.37/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.665064 ht_pricing_module-0.1.37/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.1.37/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.688003 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.696979 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.653097 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.725947 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.744898 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    45824 2023-04-14 09:34:03.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.758886 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.768858 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.781823 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4499 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.793799 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.809749 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.895520 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      506 2023-03-22 14:42:29.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4317 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3485 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4294 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     5195 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4472 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4277 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3539 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4526 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4603 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5270 2023-04-14 09:34:03.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.903498 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     4012 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.925491 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.969377 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.972370 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1131 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.996307 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.006279 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     3714 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.017249 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3452 2023-04-12 02:15:47.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.030215 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     7325 2023-02-23 05:31:40.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.053154 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.074097 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:28.077089 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    43982 2023-04-14 09:45:29.000000 ht_pricing_module-0.1.37/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:21:27.677034 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      264 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4864 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-21 01:21:27.000000 ht_pricing_module-0.1.37/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 01:21:28.087063 ht_pricing_module-0.1.37/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-04-21 01:21:10.000000 ht_pricing_module-0.1.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.257183 ht_pricing_module-0.2.0/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      263 2023-05-09 09:24:24.256187 ht_pricing_module-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.838280 ht_pricing_module-0.2.0/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.0/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.867202 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.876178 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.826311 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.905101 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.924050 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    45824 2023-04-14 09:34:03.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.938013 ht_pricing_module-0.2.0/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.0/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.946989 ht_pricing_module-0.2.0/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.0/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.959954 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4526 2023-05-09 02:19:35.000000 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.961949 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.970925 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.069661 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4091 2023-04-26 06:01:26.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3324 2023-04-26 06:01:26.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4109 2023-04-26 06:05:23.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4851 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4196 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4018 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3372 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4244 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4324 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5008 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     5262 2023-04-26 06:18:03.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.071656 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     3933 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.096589 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.131496 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.134488 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.157450 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.168421 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     4521 2023-05-09 09:23:44.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.187370 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2555 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3452 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.199338 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     7205 2023-05-08 09:57:30.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.215296 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.236240 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:24.242224 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    43982 2023-04-14 09:45:29.000000 ht_pricing_module-0.2.0/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-09 09:24:23.854237 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-05-09 09:24:23.000000 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4957 2023-05-09 09:24:23.000000 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 09:24:23.000000 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-05-09 09:24:23.000000 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-09 09:24:23.000000 ht_pricing_module-0.2.0/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 09:24:24.257183 ht_pricing_module-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1148 2023-05-09 09:24:14.000000 ht_pricing_module-0.2.0/setup.py
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.2.0/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.2.0/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.2.0/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         if hasattr(self.param, 'riskfree_rate'):
             current_up = self.param.riskfree_rate + step
             pricer_up = deepcopy(self)
             pricer_up.param.riskfree_rate = current_up
             return pricer_up.present_value() - self.present_value()
         return 0.0
 
-    def corr_sens(self, step: float = 0.01) -> float:
+    @lru_cache(maxsize=10)
+    def dpvdcorr(self, step: float = 0.01) -> float:
         if hasattr(self.param, 'correlation'):
             corr_up = self.param.correlation + step
             corr_down = self.param.correlation - step
             pricer_up = deepcopy(self)
             pricer_up.param.correlation = corr_up
             pricer_down = deepcopy(self)
             pricer_down.param.correlation = corr_down
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from ..one_asset_option_base import *
 from ..barrier.discrete_barrier_as import DiscreteBarrier
-from ..barrier.discrete_barrier_binary_as import DiscreteBarrierBinary
 
 
-class FixedAccAko(OneAssetOptionBase):
+class LinearAccAko(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_barrier_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        barrier_binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                      OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP,
-                        OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_barrier_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['volatility'] = self.param.volatility
@@ -29,36 +25,36 @@
             param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
-            leveraged_barrier = DiscreteBarrier(param)
+            barrier1 = DiscreteBarrier(param)
 
             param = Struct({})
-            param['option_type'] = barrier_binary_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['volatility'] = self.param.volatility
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
-            param['payoff'] = self.param.payoff
+            param['rebate'] = self.param.payoff
             param['obs_freq'] = self.param.obs_freq
-            barrier_binary = DiscreteBarrierBinary(param)
-            rst = rst + (-self.param.leverage * leveraged_barrier.present_value()
-                         + barrier_binary.present_value())
+            barrier2 = DiscreteBarrier(param)
+
+            rst = rst + (-self.param.leverage * barrier1.present_value() + barrier2.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 
 
 class FixedAcc(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                              OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = binary_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            binary = Binary(param)
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + binary.present_value())
+            binary2 = Binary(param)
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + binary2.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,63 +4,59 @@
 
 
 class FixedAccBarrier(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                               OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                              OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = binary_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            binary1 = Binary(param)
+            binary2 = Binary(param)
 
             param = Struct({})
-            param['option_type'] = binary_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            binary2 = Binary(param)
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + binary1.present_value()
-                         - binary2.present_value())
+            binary3 = Binary(param)
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + binary2.present_value() - binary3.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,65 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
+from ..sharkfin.sharkfin_as import Sharkfin
+from ..vanilla.vanilla_as import Vanilla
 from ..binary import Binary
 
 
-class FixedAccBarrierEnhanced(OneAssetOptionBase):
+class LinearAccFixedEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        non_leveraged_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                     OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = non_leveraged_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
+            param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
-            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            non_leveraged_binary1 = Binary(param)
+            sharkfin2 = Sharkfin(param)
 
             param = Struct({})
-            param['option_type'] = non_leveraged_option_type
+            param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            non_leveraged_binary2 = Binary(param)
-
-            param = Struct({})
-            param['option_type'] = non_leveraged_option_type
-            param['exercise_type'] = self.param.exercise_type
-            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.barrier_price
-            param['expiry_date'] = obs.obs_index
-            param['current_date'] = self.param.current_date
-            param['volatility'] = self.param.volatility
-            param['riskfree_rate'] = self.param.riskfree_rate
-            param['dividend'] = self.param.dividend
-            param['year_base'] = self.param.year_base
-            non_leveraged_vanilla = Vanilla(param)
+            binary3 = Binary(param)
 
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + non_leveraged_binary1.present_value()
-                         - non_leveraged_binary2.present_value()
-                         + non_leveraged_vanilla.present_value())
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + sharkfin2.present_value() + binary3.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 from ..one_asset_option_base import *
-from ..vanilla import Vanilla
-from ..binary import Binary
+from ..sharkfin.sharkfin_as import Sharkfin
+from ..vanilla.vanilla_as import Vanilla
 
 
-class FixedAccEnhanced(OneAssetOptionBase):
+class LinearAccEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                              OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        enhanced_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                        OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = binary_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
+            param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
-            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            binary = Binary(param)
+            sharkfin2 = Sharkfin(param)
 
             param = Struct({})
-            param['option_type'] = enhanced_vanilla_option_type
+            param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            enhanced_vanilla = Vanilla(param)
+            vanilla3 = Vanilla(param)
 
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + binary.present_value()
-                         + enhanced_vanilla.present_value())
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + sharkfin2.present_value() + vanilla3.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,80 @@
 from ..one_asset_option_base import *
-from ..barrier.discrete_barrier_as import DiscreteBarrier
 
 
-class LinearAccAko(OneAssetOptionBase):
+class OneTouch(OneAssetOptionBase):
+    """
+    触碰期权 cash or nothing(连续)
+    American Window
+    reference: The Complete Guide to Option Pricing Formulas, 2nd ed. L177
+    No touch option(NT): 上涨或下跌失效 OUT,触碰障碍期权失效无赔付,不触碰障碍到期赔付rebate
+    One touch option(OT): 上涨或下跌生效 IN, 触碰障碍立即支付或到期支付rebate,不触碰障碍到期无赔付
+
+    OTD + NTD = rebate * exp(-r * t)
+    OTU + NTU = rebate * exp(-r * t)
+    """
 
     def __calculate_present_value__(self) -> float:
         rst = 0
+        time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
 
-        leveraged_barrier_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        non_leveraged_barrier_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                             OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP,
-                        OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
-
-        for obs in self.param.obs_date:
-            param = Struct({})
-            param['option_type'] = leveraged_barrier_option_type
-            param['exercise_type'] = self.param.exercise_type
-            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.strike_price
-            param['barrier_price'] = self.param.barrier_price
-            param['riskfree_rate'] = self.param.riskfree_rate
-            param['dividend'] = self.param.dividend
-            param['volatility'] = self.param.volatility
-            param['expiry_date'] = obs.obs_index
-            param['current_date'] = self.param.current_date
-            param['year_base'] = self.param.year_base
-            param['barrier_type'] = barrier_type
-            param['knock_type'] = KnockType.OUT
-            param['is_knock_in'] = 0
-            param['rebate'] = 0
-            param['obs_freq'] = self.param.obs_freq
-            leveraged_barrier = DiscreteBarrier(param)
-
-            param = Struct({})
-            param['option_type'] = non_leveraged_barrier_option_type
-            param['exercise_type'] = self.param.exercise_type
-            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.strike_price
-            param['barrier_price'] = self.param.barrier_price
-            param['riskfree_rate'] = self.param.riskfree_rate
-            param['dividend'] = self.param.dividend
-            param['volatility'] = self.param.volatility
-            param['expiry_date'] = obs.obs_index
-            param['current_date'] = self.param.current_date
-            param['year_base'] = self.param.year_base
-            param['barrier_type'] = barrier_type
-            param['knock_type'] = KnockType.OUT
-            param['is_knock_in'] = 0
-            param['rebate'] = self.param.payoff
-            param['obs_freq'] = self.param.obs_freq
-            non_leveraged_barrier = DiscreteBarrier(param)
-
-            rst = rst + (-self.param.leverage * leveraged_barrier.present_value()
-                         + non_leveraged_barrier.present_value())
-        return rst
-
-    @lru_cache(maxsize=10)
-    def theta(self, step: float = 1) -> float:
-        if hasattr(self.param, 'current_date'):
-            current_up = self.param.current_date + step
-            pricer_up = deepcopy(self)
-            pricer_up.param.current_date = current_up
-            for obs in pricer_up.param.obs_date:
-                if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
-                    obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.present_value() - self.present_value()
-        return 0.0
-
-    @lru_cache(maxsize=10)
-    def ddeltadt(self, time_step: float = 1, price_step: float = 0.001):
-        if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
-            current_up = self.param.current_date + time_step
-            pricer_up = deepcopy(self)
-            pricer_up.param.current_date = current_up
-            for obs in pricer_up.param.obs_date:
-                if self.param.current_date <= obs.obs_index < pricer_up.param.current_date:
-                    obs.obs_price = pricer_up.param.spot_price
-            return pricer_up.delta(step=price_step) - self.delta(step=price_step)
-        return 0.0
+        u_knock_flag = self.param.barrier_type == BarrierType.UP and self.param.spot_price >= self.param.barrier_price
+        d_knock_flag = self.param.barrier_type == BarrierType.DOWN and self.param.spot_price <= self.param.barrier_price
+
+        if time_to_expiry <= 0:
+            """已到期"""
+            if self.param.knock_type == KnockType.IN:
+                """触碰生效"""
+                if self.param.is_knock_in or u_knock_flag or d_knock_flag:
+                    """敲入"""
+                    return self.param.rebate
+                else:
+                    return 0
+            elif self.param.knock_type == KnockType.OUT:
+                """触碰失效"""
+                if u_knock_flag or d_knock_flag:
+                    """失效"""
+                    return 0
+                else:
+                    return self.param.rebate
+        else:
+            """存续"""
+            if self.param.knock_type == KnockType.IN:
+                if self.param.is_knock_in or u_knock_flag or d_knock_flag:
+                    """生效"""
+                    if self.param.rebate_type == RebateType.PAH:
+                        return self.param.rebate
+                    elif self.param.rebate_type == RebateType.PAE:
+                        return self.param.rebate * np.exp(-self.param.riskfree_rate * time_to_expiry)
+            elif self.param.knock_type == KnockType.OUT:
+                if u_knock_flag or d_knock_flag:
+                    """敲出失效"""
+                    return 0
+
+            """触碰期权(连续)解析解"""
+            du = {BarrierType.DOWN: 1, BarrierType.UP: -1}[self.param.barrier_type]
+            eh = {KnockType.IN: -du, KnockType.OUT: du}[self.param.knock_type]
+
+            t_adj_vol = self.param.volatility * math.sqrt(time_to_expiry)
+            exp_r_t = np.exp(-1 * self.param.riskfree_rate * time_to_expiry)
+            vol_sq = math.pow(self.param.volatility, 2)
+            ba_d_sp = self.param.barrier_price / self.param.spot_price
+
+            mu = (self.param.riskfree_rate - self.param.dividend - vol_sq / 2) / vol_sq
+            lamda = math.sqrt(math.pow(mu, 2) + 2 * self.param.riskfree_rate / vol_sq)
+
+            x2 = np.log(self.param.spot_price / self.param.barrier_price) / t_adj_vol + (1 + mu) * t_adj_vol
+            y2 = np.log(ba_d_sp) / t_adj_vol + (1 + mu) * t_adj_vol
+            z = np.log(ba_d_sp) / t_adj_vol + lamda * t_adj_vol
+
+            B2 = self.param.rebate * exp_r_t * norm.cdf(eh * x2 - eh * t_adj_vol)
+            B4 = self.param.rebate * exp_r_t * math.pow(ba_d_sp, 2 * mu) * norm.cdf(du * y2 - du * t_adj_vol)
+            A5 = self.param.rebate * (math.pow(ba_d_sp, mu + lamda) * norm.cdf(du * z) +
+                                      math.pow(ba_d_sp, mu - lamda) * norm.cdf(du * z - 2 * du * lamda * t_adj_vol))
+
+            if self.param.knock_type == KnockType.IN:
+                # one touch
+                rst = {RebateType.PAE: B2 + B4, RebateType.PAH: A5}[self.param.rebate_type]
+            elif self.param.knock_type == KnockType.OUT:
+                # no touch
+                rst = B2 - B4
+            return rst
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 
 
 class LinearAcc(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        sharkfin_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = sharkfin_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            sharkfin = Sharkfin(param)
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + sharkfin.present_value())
+            sharkfin2 = Sharkfin(param)
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + sharkfin2.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 from ..one_asset_option_base import *
-from ..sharkfin.sharkfin_as import Sharkfin
-from ..vanilla.vanilla_as import Vanilla
+from ..vanilla import Vanilla
+from ..binary import Binary
 
 
-class LinearAccEnhanced(OneAssetOptionBase):
+class FixedAccEnhanced(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        sharkfin_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        enhanced_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                        OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            vanilla1 = Vanilla(param)
 
             param = Struct({})
-            param['option_type'] = sharkfin_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
-            param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
+            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            sharkfin = Sharkfin(param)
+            binary2 = Binary(param)
 
             param = Struct({})
-            param['option_type'] = enhanced_vanilla_option_type
+            param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
-            enhanced_vanilla = Vanilla(param)
+            vanilla3 = Vanilla(param)
 
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + sharkfin.present_value()
-                         + enhanced_vanilla.present_value())
+            rst = rst + (-self.param.leverage * vanilla1.present_value() + binary2.present_value() + vanilla3.present_value())
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,81 @@
 from ..one_asset_option_base import *
-from ..sharkfin.sharkfin_as import Sharkfin
-from ..vanilla.vanilla_as import Vanilla
-from ..binary import Binary
+from ..barrier.discrete_barrier_as import DiscreteBarrier
 
 
-class LinearAccFixedEnhanced(OneAssetOptionBase):
+class LinearAccFusing(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_vanilla_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        sharkfin_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        enhanced_binary_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                       OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
+        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_vanilla_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
-            param['expiry_date'] = obs.obs_index
-            param['current_date'] = self.param.current_date
-            param['volatility'] = self.param.volatility
+            param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
+            param['volatility'] = self.param.volatility
+            param['expiry_date'] = obs.obs_index
+            param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
-            leveraged_vanilla = Vanilla(param)
+            param['barrier_type'] = barrier_type
+            param['knock_type'] = KnockType.OUT
+            param['is_knock_in'] = 0
+            param['rebate'] = 0
+            param['obs_freq'] = self.param.obs_freq
+            barrier1 = DiscreteBarrier(param)
 
             param = Struct({})
-            param['option_type'] = sharkfin_option_type
+            param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
-            param['expiry_date'] = obs.obs_index
-            param['current_date'] = self.param.current_date
-            param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
-            param['year_base'] = self.param.year_base
-            sharkfin = Sharkfin(param)
-
-            param = Struct({})
-            param['option_type'] = enhanced_binary_option_type
-            param['exercise_type'] = self.param.exercise_type
-            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.barrier_price
+            param['volatility'] = self.param.volatility
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
-            param['volatility'] = self.param.volatility
-            param['riskfree_rate'] = self.param.riskfree_rate
-            param['dividend'] = self.param.dividend
-            param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
-            enhanced_binary = Binary(param)
+            param['barrier_type'] = barrier_type
+            param['knock_type'] = KnockType.OUT
+            param['is_knock_in'] = 0
+            param['rebate'] = self.param.payoff
+            param['obs_freq'] = self.param.obs_freq
+            barrier2 = DiscreteBarrier(param)
+
+            rst = rst + self.param.base_quantity * (-self.param.leverage * barrier1.present_value() + barrier2.present_value())
+
+        param = Struct({})
+        param['option_type'] = option_type1
+        param['exercise_type'] = self.param.exercise_type
+        param['spot_price'] = self.param.spot_price
+        param['strike_price'] = self.param.strike_price
+        param['barrier_price'] = self.param.barrier_price
+        param['riskfree_rate'] = self.param.riskfree_rate
+        param['dividend'] = self.param.dividend
+        param['volatility'] = self.param.volatility
+        param['expiry_date'] = self.param.expiry_date
+        param['current_date'] = self.param.current_date
+        param['year_base'] = self.param.year_base
+        param['barrier_type'] = barrier_type
+        param['knock_type'] = KnockType.OUT
+        param['is_knock_in'] = 0
+        param['rebate'] = 0
+        param['obs_freq'] = self.param.obs_freq
+        barrier3 = DiscreteBarrier(param)
 
-            rst = rst + (-self.param.leverage * leveraged_vanilla.present_value()
-                         + sharkfin.present_value()
-                         + enhanced_binary.present_value())
+        rst = rst - self.param.final_position_multiplier * barrier3.present_value()
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from ..one_asset_option_base import *
 from ..barrier.discrete_barrier_as import DiscreteBarrier
+from ..forward import Forward
+from ..touch import DiscreteOneTouch
 
 
-class LinearAccFusing(OneAssetOptionBase):
+class LinearAccFusingTransForward(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
 
-        leveraged_barrier_option_type = {OptionType.ACCUMULATOR: OptionType.PUT,
-                                         OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
-        non_leveraged_barrier_option_type = {OptionType.ACCUMULATOR: OptionType.CALL,
-                                             OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
-        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP,
-                        OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
+        option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
+        barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
+        cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
 
         for obs in self.param.obs_date:
             param = Struct({})
-            param['option_type'] = leveraged_barrier_option_type
+            param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['volatility'] = self.param.volatility
@@ -28,39 +27,42 @@
             param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
-            leveraged_barrier = DiscreteBarrier(param)
+            barrier1 = DiscreteBarrier(param)
 
             param = Struct({})
-            param['option_type'] = non_leveraged_barrier_option_type
-            param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
-            param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['volatility'] = self.param.volatility
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['year_base'] = self.param.year_base
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
-            param['rebate'] = self.param.payoff
+            param['rebate_type'] = RebateType.PAH
+            param['rebate'] = cp * (self.param.entrance_price - self.param.strike_price)
             param['obs_freq'] = self.param.obs_freq
-            non_leveraged_barrier = DiscreteBarrier(param)
+            touch2 = DiscreteOneTouch(param)
+
+            param = Struct({})
+            param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
+            param['strike_price'] = self.param.entrance_price
+            forward3 = Forward(param)
 
-            rst = rst + self.param.base_quantity * (-self.param.leverage * leveraged_barrier.present_value() + non_leveraged_barrier.present_value())
+            rst = rst + self.param.base_quantity * (-(self.param.leverage - 1) * barrier1.present_value() + touch2.present_value() + cp * forward3.present_value())
 
         param = Struct({})
-        param['option_type'] = leveraged_barrier_option_type
+        param['option_type'] = option_type1
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
@@ -68,17 +70,17 @@
         param['current_date'] = self.param.current_date
         param['year_base'] = self.param.year_base
         param['barrier_type'] = barrier_type
         param['knock_type'] = KnockType.OUT
         param['is_knock_in'] = 0
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
-        fusing_barrier = DiscreteBarrier(param)
+        barrier4 = DiscreteBarrier(param)
 
-        rst = rst - fusing_barrier.present_value() * self.param.final_position_multiplier
+        rst = rst - self.param.final_position_multiplier * barrier4.present_value()
         return rst
 
     @lru_cache(maxsize=10)
     def theta(self, step: float = 1) -> float:
         if hasattr(self.param, 'current_date'):
             current_up = self.param.current_date + step
             pricer_up = deepcopy(self)
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,16 @@
                 (self.param.option_type == OptionType.REVERSE and self.param.spot_price >= self.param.barrier_price):
             param = Struct({})
             param['spot_price'] = self.param.spot_price
             param['strike_price'] = self.param.strike_price
             forward = Forward(param=param)
             return phi * forward.present_value()
 
-        barrier_type = {OptionType.STANDARD: BarrierType.DOWN,
-                        OptionType.REVERSE: BarrierType.UP}[self.param.option_type]
-        knock_out_option_type = {OptionType.STANDARD: OptionType.CALL,
-                                 OptionType.REVERSE: OptionType.PUT}[self.param.option_type]
+        barrier_type = {OptionType.STANDARD: BarrierType.DOWN, OptionType.REVERSE: BarrierType.UP}[self.param.option_type]
+        option_type = {OptionType.STANDARD: OptionType.CALL, OptionType.REVERSE: OptionType.PUT}[self.param.option_type]
 
         param = Struct({})
         param['option_type'] = OptionType.CALL
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
@@ -57,15 +55,15 @@
         param['knock_type'] = KnockType.IN
         param['is_knock_in'] = self.param.is_knock_in
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
         barrier2 = DiscreteBarrier(param)
 
         param = Struct({})
-        param['option_type'] = knock_out_option_type
+        param['option_type'] = option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 class BasketVanilla(OneAssetOptionBase):
     """
     篮子期权
     Bachelier model
     """
     def __calculate_present_value__(self) -> float:
 
-        def __norm_pdf(x):
+        def __norm_pdf__(x):
             return 1 / math.sqrt(2 * math.pi) * math.exp(-1 * pow(x, 2) / 2)
 
         rst = 0
         cp = {OptionType.CALL: 1, OptionType.PUT: -1}[self.param.option_type]
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             rst = max(cp * (self.param.spot_price - self.param.strike_price), 0)
         else:
             b = self.param.riskfree_rate - self.param.dividend
             f0 = self.param.spot_price * math.exp(b * time_to_expiry)
             t_adj_vol = self.param.volatility * math.sqrt(time_to_expiry)
             discount_factor = math.exp(-1 * self.param.riskfree_rate * time_to_expiry)
             d = (f0 - self.param.strike_price) / t_adj_vol
-            rst = discount_factor * (t_adj_vol * __norm_pdf(d) + cp * (f0 - self.param.strike_price) * norm.cdf(cp * d))
+            rst = discount_factor * (t_adj_vol * __norm_pdf__(d) + cp * (f0 - self.param.strike_price) * norm.cdf(cp * d))
         return rst
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,29 +19,27 @@
         time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
         if time_to_expiry <= 0:
             return 0.0
 
         if hasattr(self.param, 'spot_price'):
             spot_up = self.param.spot_price * (1 + step)
             spot_down = self.param.spot_price * (1 - step)
-            pricer_up = deepcopy(self)
+            pricer_up, pricer_down = deepcopy(self), deepcopy(self)
             pricer_up.param.spot_price = spot_up
-            pricer_down = deepcopy(self)
             pricer_down.param.spot_price = spot_down
             return (pricer_up.present_value() - pricer_down.present_value()) / (spot_up - spot_down)
         return 0.0
 
     @lru_cache(maxsize=10)
     def gamma(self, step: float = 0.001) -> float:
         if hasattr(self.param, 'spot_price'):
             spot_up = self.param.spot_price * (1 + step)
             spot_down = self.param.spot_price * (1 - step)
-            pricer_up = deepcopy(self)
+            pricer_up, pricer_down = deepcopy(self), deepcopy(self)
             pricer_up.param.spot_price = spot_up
-            pricer_down = deepcopy(self)
             pricer_down.param.spot_price = spot_down
             return (pricer_up.present_value() + pricer_down.present_value() - 2 * self.present_value()) / pow((spot_up - spot_down) / 2, 2) 
         return 0.0
 
     @lru_cache(maxsize=10)
     def vega(self, step: float = 0.01) -> float:
         if hasattr(self.param, 'volatility'):
@@ -75,14 +73,29 @@
             current_up = self.param.current_date + time_step
             pricer_up = deepcopy(self)
             pricer_up.param.current_date = current_up
             return pricer_up.delta(step=price_step) - self.delta(step=price_step)
         return 0.0
 
     @lru_cache(maxsize=10)
+    def modddeltadt(self, time_step: float = 1, price_step: float = 0.001):
+        if hasattr(self.param, 'current_date') and hasattr(self.param, 'spot_price'):
+            time_to_expiry = (self.param.expiry_date - self.param.current_date) / self.param.year_base
+            if time_to_expiry <= 1:
+                current_mod = 0.0001
+                current_up = current_mod + time_step
+                pricer_mod, pricer_up = deepcopy(self), deepcopy(self)
+                pricer_mod.param.current_date = current_mod
+                pricer_up.param.current_date = current_up
+                return pricer_up.delta(step=price_step) - pricer_mod.delta(step=price_step)
+            else:
+                return self.ddeltadt(time_step=time_step, price_step=price_step)
+        return 0.0
+
+    @lru_cache(maxsize=10)
     def ddeltadv(self, vol_step: float = 0.01, price_step: float = 0.001):
         if hasattr(self.param, 'volatility') and hasattr(self.param, 'spot_price'):
             vol_up = self.param.volatility + vol_step
             pricer_up = deepcopy(self)
             pricer_up.param.volatility = vol_up
             return pricer_up.delta(step=price_step) - self.delta(step=price_step)
         return 0.0
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['payoff'] = abs(self.param.strike_price - self.param.barrier_price)
         param['year_base'] = self.param.year_base
-        binary1 = Binary(param)
+        binary3 = Binary(param)
 
-        return vanilla1.present_value() - vanilla2.present_value() - binary1.present_value()
+        return vanilla1.present_value() - vanilla2.present_value() - binary3.present_value()
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['payoff'] = rebate
         param['year_base'] = self.param.year_base
-        binary1 = Binary(param)
+        binary3 = Binary(param)
 
-        return self.param.notional * (self.param.participation_rate * (vanilla1.present_value() - vanilla2.present_value()) - binary1.present_value() + min_yield)
+        return self.param.notional * (self.param.participation_rate * (vanilla1.present_value() - vanilla2.present_value()) - binary3.present_value() + min_yield)
 
 
 if __name__ == '__main__':
     param = Struct({})
     param['option_type'] = OptionType.CALL
     param['exercise_type'] = ExerciseType.EUROPEAN
     param['notional'] = 1
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,24 +103,22 @@
                                              + np.where(ko_idx == 0, 0, phi * ko_obs_price_ret * participation_rate)
                                              - margin_rate * np.where(ko_idx == 0, 0, np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx - 1] / year_base) - 1))
 
         # 敲入未敲出
         comp_factor = np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
         dis_factor = 1 / comp_factor
 
-        ki_no_ko_arr_flag = np.logical_and(np.logical_or(is_knock_in,
-                                                         np.max(ki_mat_flag, axis=1)),
+        ki_no_ko_arr_flag = np.logical_and(np.logical_or(is_knock_in, np.max(ki_mat_flag, axis=1)),
                                            np.logical_not(np.max(ko_mat_flag, axis=1)))
 
         ki_no_ko_payoff = ki_no_ko_arr_flag * dis_factor * notional * (np.maximum((floor_rate - 1), np.minimum(phi * (price[:, -1] / entrance_price - 1), 0))
                                                                        - margin_rate * (comp_factor - 1))
 
         # 未敲入未敲出
-        no_ki_no_ko_arr_flag = np.logical_and(np.logical_and(1 - is_knock_in,
-                                                             np.logical_not(np.max(ki_mat_flag, axis=1))),
+        no_ki_no_ko_arr_flag = np.logical_and(np.logical_and(1 - is_knock_in, np.logical_not(np.max(ki_mat_flag, axis=1))),
                                               np.logical_not(np.max(ko_mat_flag, axis=1)))
 
         no_ki_no_ko_payoff = no_ki_no_ko_arr_flag * dis_factor * notional * (bonus_rate
                                                                              - margin_rate * (comp_factor - 1))
 
         rst = np.round(np.mean(ko_payoff + ki_no_ko_payoff + no_ki_no_ko_payoff), 8)
         return rst
```

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.2.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.2.0/ht_pricing_module/simple_pricer_engine.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.1.37/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.2.0/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
 ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
 ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
 ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
 ht_pricing_module/one_asset_pricing_module/asian/__init__.py
 ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
 ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
```

### Comparing `ht_pricing_module-0.1.37/setup.py` & `ht_pricing_module-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.1.37"
+VERSION = "0.2.0"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

